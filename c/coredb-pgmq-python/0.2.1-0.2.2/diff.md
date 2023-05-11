# Comparing `tmp/coredb_pgmq_python-0.2.1.tar.gz` & `tmp/coredb_pgmq_python-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coredb_pgmq_python-0.2.1.tar", max compression
+gzip compressed data, was "coredb_pgmq_python-0.2.2.tar", max compression
```

## Comparing `coredb_pgmq_python-0.2.1.tar` & `coredb_pgmq_python-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1510 2023-05-01 16:40:17.818132 coredb_pgmq_python-0.2.1/README.md
--rw-r--r--   0        0        0      106 2023-05-01 16:40:17.818132 coredb_pgmq_python-0.2.1/coredb_pgmq_python/__init__.py
--rw-r--r--   0        0        0     3532 2023-05-01 16:40:17.818132 coredb_pgmq_python-0.2.1/coredb_pgmq_python/queue.py
--rw-r--r--   0        0        0     1029 2023-05-01 16:40:17.818132 coredb_pgmq_python-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.2.1/setup.py
--rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1510 2023-05-11 20:48:14.409347 coredb_pgmq_python-0.2.2/README.md
+-rw-r--r--   0        0        0      106 2023-05-11 20:48:14.409347 coredb_pgmq_python-0.2.2/coredb_pgmq_python/__init__.py
+-rw-r--r--   0        0        0     4371 2023-05-11 20:48:14.409347 coredb_pgmq_python-0.2.2/coredb_pgmq_python/queue.py
+-rw-r--r--   0        0        0     1121 2023-05-11 20:48:14.409347 coredb_pgmq_python-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.2.2/setup.py
+-rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.2.2/PKG-INFO
```

### Comparing `coredb_pgmq_python-0.2.1/README.md` & `coredb_pgmq_python-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `coredb_pgmq_python-0.2.1/coredb_pgmq_python/queue.py` & `coredb_pgmq_python-0.2.2/coredb_pgmq_python/queue.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass, field
 from datetime import datetime
-from typing import Optional, Union
+from typing import Optional
 
 from psycopg.types.json import Jsonb
 from psycopg_pool import ConnectionPool
 
 
 @dataclass
 class Message:
@@ -43,46 +43,59 @@
         password={self.password}
         """
         self.pool = ConnectionPool(conninfo, **self.kwargs)
 
         with self.pool.connection() as conn:
             conn.execute("create extension if not exists pgmq cascade;")
 
-    def create_queue(self, queue: str) -> None:
-        """Create a queue"""
-        with self.pool.connection() as conn:
-            conn.execute("select pgmq_create(%s);", [queue])
+    def create_queue(self, queue: str, partition_interval: int = 10000, retention_interval: int = 100000) -> None:
+        """Create a new queue
+
+        Note: Partitions are created pg_partman which must be configured in postgresql.conf
+            Set `pg_partman_bgw.interval` to set the interval for partition creation and deletion.
+            A value of 10 will create new/delete partitions every 10 seconds. This value should be tuned
+            according to the volume of messages being sent to the queue.
+
+        Args:
+            queue: The name of the queue.
+            partition_interval: The number of messages per partition. Defaults to 10,000.
+            retention_interval: The number of messages to retain. Messages exceeding this number will be dropped.
+                Defaults to 100,000.
+        """
 
-    def create_(
-        self, queue: str, partition_interval: Optional[str] = "daily", retention_interval: Optional[str] = "5 days"
-    ) -> None:
-        """Create a partitioned queue"""
         with self.pool.connection() as conn:
-            conn.execute("select pgmq_create_non_partitioned(%s, %s);", [queue, partition_interval, retention_interval])
+            conn.execute("select pgmq_create(%s, %s::text, %s::text);", [queue, partition_interval, retention_interval])
 
     def send(self, queue: str, message: dict, delay: Optional[int] = None) -> int:
         """Send a message to a queue"""
 
         with self.pool.connection() as conn:
             if delay is not None:
                 # TODO(chuckend): implement send_delay in pgmq
                 raise NotImplementedError("send_delay is not implemented in pgmq")
             message = conn.execute(
                 "select * from pgmq_send(%s, %s);",
                 [queue, Jsonb(message)],  # type: ignore
             ).fetchall()
         return message[0][0]
 
-    def read(self, queue: str, vt: Optional[int] = None, limit: int = 1) -> Union[Message, list[Message]]:
+    def read(self, queue: str, vt: Optional[int] = None) -> Optional[Message]:
         """Read a message from a queue"""
         with self.pool.connection() as conn:
-            rows = conn.execute("select * from pgmq_read(%s, %s, %s);", [queue, vt or self.vt, limit]).fetchall()
+            rows = conn.execute("select * from pgmq_read(%s, %s, %s);", [queue, vt or self.vt, 1]).fetchall()
 
         messages = [Message(msg_id=x[0], read_ct=x[1], enqueued_at=x[2], vt=x[3], message=x[4]) for x in rows]
-        return messages[0] if len(messages) == 1 else messages
+        return messages[0] if len(messages) == 1 else None
+
+    def read_batch(self, queue: str, vt: Optional[int] = None, batch_size=1) -> Optional[list[Message]]:
+        """Read abatch of messages from a queue"""
+        with self.pool.connection() as conn:
+            rows = conn.execute("select * from pgmq_read(%s, %s, %s);", [queue, vt or self.vt, batch_size]).fetchall()
+
+        return [Message(msg_id=x[0], read_ct=x[1], enqueued_at=x[2], vt=x[3], message=x[4]) for x in rows]
 
     def pop(self, queue: str) -> Message:
         """Read a message from a queue"""
         with self.pool.connection() as conn:
             rows = conn.execute("select * from pgmq_pop(%s);", [queue]).fetchall()
 
         messages = [Message(msg_id=x[0], read_ct=x[1], enqueued_at=x[2], vt=x[3], message=x[4]) for x in rows]
```

### Comparing `coredb_pgmq_python-0.2.1/pyproject.toml` & `coredb_pgmq_python-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coredb-pgmq-python"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python client for the PGMQ Postgres extension."
 authors = ["Adam Hendel <adam@coredb.io>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "coredb_pgmq_python"}]
 
 [tool.poetry.urls]
@@ -23,14 +23,18 @@
 pandas = "^2.0.1"
 pytest = "^7.3.0"
 debugpy = "^1.6.7"
 black = "^23.3.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 numpy = "^1.24.3"
+matplotlib = "^3.7.1"
+jupyter = "^1.0.0"
+notebook = "^6.5.4"
+pandas-stubs = "^2.0.1.230501"
 
 [tool.black]
 line-length = 120
 target-version = ['py311', 'py310', 'py39']
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `coredb_pgmq_python-0.2.1/setup.py` & `coredb_pgmq_python-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['orjson>=3.8.10,<4.0.0',
  'psycopg[binary,pool]>=3.1.8,<4.0.0',
  'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'coredb-pgmq-python',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Python client for the PGMQ Postgres extension.',
     'long_description': '# Coredb\'s Python Client for PGMQ\n\n## Installation\n\nInstall with `pip` from pypi.org\n\n```bash\npip install coredb-pgmq-python\n```\n\nDependencies:\n\nPostgres running the [CoreDB PGMQ extension](https://github.com/CoreDB-io/coredb/tree/main/extensions/pgmq).\n\n## Usage\n\n## Start a Postgres Instance with the CoreDB extension installed\n\n```bash\ndocker run -d --name postgres -e POSTGRES_PASSWORD=postgres -p 5432:5432 quay.io/coredb/pgmq-pg:latest\n```\n\nInitialize a connection to Postgres\n\n```python\n\nfrom coredb_pgmq_python import PGMQueue, Message\n\nqueue = PGMQueue(host="0.0.0.0")\n```\n\nCreate a queue (or a partitioned queue)\n\n```python\nqueue.create_queue("my_queue")\n# queue.create_partitioned_queue("my_partitioned_queue", partition_size=10000)\n```\n\n\nSend a message\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\n```\n\nRead a message, set it invisible for 30 seconds.\n\n```python\nread_message: Message = queue.read("my_queue", vt=10)\nprint(read_message)\n```\n\nArchive the message after we\'re done with it. Archived messages are moved to an archive table.\n\n```python\narchived: bool = queue.archive("my_queue", read_message.msg_id)\n```\n\nDelete a message completely.\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\nread_message: Message = queue.read("my_queue")\ndeleted: bool = queue.delete("my_queue", read_message.msg_id)\n```\n\nPop a message, deleting it and reading it in one transaction.\n\n```python\npopped_message: Message = queue.pop("my_queue")\nprint(popped_message)\n```\n',
     'author': 'Adam Hendel',
     'author_email': 'adam@coredb.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `coredb_pgmq_python-0.2.1/PKG-INFO` & `coredb_pgmq_python-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coredb-pgmq-python
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python client for the PGMQ Postgres extension.
 License: Apache 2.0
 Author: Adam Hendel
 Author-email: adam@coredb.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

