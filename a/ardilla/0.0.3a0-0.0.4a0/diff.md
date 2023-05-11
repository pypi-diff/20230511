# Comparing `tmp/ardilla-0.0.3a0.tar.gz` & `tmp/ardilla-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardilla-0.0.3a0.tar", last modified: Thu May 11 02:52:21 2023, max compression
+gzip compressed data, was "ardilla-0.0.4a0.tar", last modified: Thu May 11 19:22:41 2023, max compression
```

## Comparing `ardilla-0.0.3a0.tar` & `ardilla-0.0.4a0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 02:52:21.453472 ardilla-0.0.3a0/
--rw-rw-rw-   0        0        0     1084 2023-05-08 03:28:44.000000 ardilla-0.0.3a0/LICENCE
--rw-rw-rw-   0        0        0     3731 2023-05-11 02:52:21.447479 ardilla-0.0.3a0/PKG-INFO
--rw-rw-rw-   0        0        0     3064 2023-05-10 04:27:22.000000 ardilla-0.0.3a0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 02:52:21.174823 ardilla-0.0.3a0/ardilla/
--rw-rw-rw-   0        0        0      106 2023-05-08 02:18:14.000000 ardilla-0.0.3a0/ardilla/__init__.py
--rw-rw-rw-   0        0        0     2836 2023-05-11 02:46:45.000000 ardilla-0.0.3a0/ardilla/abc.py
-drwxrwxrwx   0        0        0        0 2023-05-11 02:52:21.410471 ardilla-0.0.3a0/ardilla/asyncio/
--rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.0.3a0/ardilla/asyncio/__init__.py
--rw-rw-rw-   0        0        0     6181 2023-05-11 02:46:29.000000 ardilla-0.0.3a0/ardilla/asyncio/crud.py
--rw-rw-rw-   0        0        0      738 2023-05-11 02:46:33.000000 ardilla-0.0.3a0/ardilla/asyncio/engine.py
--rw-rw-rw-   0        0        0     5898 2023-05-11 02:46:43.000000 ardilla-0.0.3a0/ardilla/crud.py
--rw-rw-rw-   0        0        0     1013 2023-05-11 02:46:53.000000 ardilla-0.0.3a0/ardilla/engine.py
--rw-rw-rw-   0        0        0      216 2023-05-11 02:46:57.000000 ardilla-0.0.3a0/ardilla/errors.py
--rw-rw-rw-   0        0        0     1166 2023-05-11 02:47:01.000000 ardilla-0.0.3a0/ardilla/models.py
--rw-rw-rw-   0        0        0     1263 2023-05-11 02:47:06.000000 ardilla-0.0.3a0/ardilla/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-11 02:52:21.364468 ardilla-0.0.3a0/ardilla.egg-info/
--rw-rw-rw-   0        0        0     3731 2023-05-11 02:52:20.000000 ardilla-0.0.3a0/ardilla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-05-11 02:52:21.000000 ardilla-0.0.3a0/ardilla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 02:52:20.000000 ardilla-0.0.3a0/ardilla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-05-11 02:52:20.000000 ardilla-0.0.3a0/ardilla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-11 02:52:20.000000 ardilla-0.0.3a0/ardilla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      867 2023-05-11 02:51:34.000000 ardilla-0.0.3a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 02:52:21.454471 ardilla-0.0.3a0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 02:52:21.441468 ardilla-0.0.3a0/tests/
--rw-rw-rw-   0        0        0     4064 2023-05-11 02:47:13.000000 ardilla-0.0.3a0/tests/test_async.py
--rw-rw-rw-   0        0        0      464 2023-05-11 02:47:16.000000 ardilla-0.0.3a0/tests/test_models.py
--rw-rw-rw-   0        0        0     3730 2023-05-11 02:47:20.000000 ardilla-0.0.3a0/tests/test_sync.py
+drwxrwxrwx   0        0        0        0 2023-05-11 19:22:41.539482 ardilla-0.0.4a0/
+-rw-rw-rw-   0        0        0     1084 2023-05-08 03:28:44.000000 ardilla-0.0.4a0/LICENCE
+-rw-rw-rw-   0        0        0     4011 2023-05-11 19:22:41.537480 ardilla-0.0.4a0/PKG-INFO
+-rw-rw-rw-   0        0        0     3318 2023-05-11 19:20:12.000000 ardilla-0.0.4a0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 19:22:41.462477 ardilla-0.0.4a0/ardilla/
+-rw-rw-rw-   0        0        0      106 2023-05-08 02:18:14.000000 ardilla-0.0.4a0/ardilla/__init__.py
+-rw-rw-rw-   0        0        0     2836 2023-05-11 02:46:45.000000 ardilla-0.0.4a0/ardilla/abc.py
+drwxrwxrwx   0        0        0        0 2023-05-11 19:22:41.520482 ardilla-0.0.4a0/ardilla/asyncio/
+-rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.0.4a0/ardilla/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     6181 2023-05-11 02:46:29.000000 ardilla-0.0.4a0/ardilla/asyncio/crud.py
+-rw-rw-rw-   0        0        0      738 2023-05-11 02:46:33.000000 ardilla-0.0.4a0/ardilla/asyncio/engine.py
+-rw-rw-rw-   0        0        0     6155 2023-05-11 16:51:13.000000 ardilla-0.0.4a0/ardilla/crud.py
+-rw-rw-rw-   0        0        0     1013 2023-05-11 02:46:53.000000 ardilla-0.0.4a0/ardilla/engine.py
+-rw-rw-rw-   0        0        0      216 2023-05-11 02:46:57.000000 ardilla-0.0.4a0/ardilla/errors.py
+-rw-rw-rw-   0        0        0     1482 2023-05-11 17:41:49.000000 ardilla-0.0.4a0/ardilla/models.py
+-rw-rw-rw-   0        0        0     2070 2023-05-11 19:10:57.000000 ardilla-0.0.4a0/ardilla/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-11 19:22:41.510480 ardilla-0.0.4a0/ardilla.egg-info/
+-rw-rw-rw-   0        0        0     4011 2023-05-11 19:22:41.000000 ardilla-0.0.4a0/ardilla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-05-11 19:22:41.000000 ardilla-0.0.4a0/ardilla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 19:22:41.000000 ardilla-0.0.4a0/ardilla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-05-11 19:22:41.000000 ardilla-0.0.4a0/ardilla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-11 19:22:41.000000 ardilla-0.0.4a0/ardilla.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      916 2023-05-11 19:21:43.000000 ardilla-0.0.4a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 19:22:41.540494 ardilla-0.0.4a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 19:22:41.532479 ardilla-0.0.4a0/tests/
+-rw-rw-rw-   0        0        0     4116 2023-05-11 19:14:31.000000 ardilla-0.0.4a0/tests/test_async.py
+-rw-rw-rw-   0        0        0      515 2023-05-11 19:13:13.000000 ardilla-0.0.4a0/tests/test_models.py
+-rw-rw-rw-   0        0        0     3780 2023-05-11 19:14:07.000000 ardilla-0.0.4a0/tests/test_sync.py
```

### Comparing `ardilla-0.0.3a0/LICENCE` & `ardilla-0.0.4a0/LICENCE`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.3a0/PKG-INFO` & `ardilla-0.0.4a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.0.3a0
+Version: 0.0.4a0
 Summary: A small package for performing basic CRUD operations with sqlite via aiosqlite and pydantic
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: async
+Provides-Extra: examples
 Provides-Extra: dev
 License-File: LICENCE
 
 # ardilla
 
 <div style="text-align:center">
   <img 
@@ -35,34 +36,39 @@
 
 What this library excels in simplicity it lacks in flexibility so, if you're expecting to use complex queries and intricate relationships, you should should consider other libraries like [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
 
 
 ## install
 Install lastest release from PyPi
 ```bash
-pip install -U ardilla´
+pip install -U ardilla
 pip install -U ardilla[async]
+pip install -U ardilla[dev]
 ```
+- async instaslls aiosqlite
+- dev installs formatting and testing dependencies
 
 Or install the lastest changes directly from github
 ```bash
 pip install git+https://github.com/chrisdewa/ardilla.git
 pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[async]
+pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[dev]
 ```
 
 
 ## How to use:
 ```py
 from ardilla import Engine, Model, Crud
+from pydantic import Field
 
 engine = Engine('db.sqlite3')
 Crud.engine = engine
 
 class User(Model):
-    id: int
+    id: int = Field(primary=True, autoincrement=True) 
     name: str
     age: int
 
 user_crud: Crud[User] = Crud(User)
 
 def main():
     engine.setup() # creates tables
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ardilla-0.0.3a0/README.md` & `ardilla-0.0.4a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,34 +18,39 @@
 
 What this library excels in simplicity it lacks in flexibility so, if you're expecting to use complex queries and intricate relationships, you should should consider other libraries like [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
 
 
 ## install
 Install lastest release from PyPi
 ```bash
-pip install -U ardilla´
+pip install -U ardilla
 pip install -U ardilla[async]
+pip install -U ardilla[dev]
 ```
+- async instaslls aiosqlite
+- dev installs formatting and testing dependencies
 
 Or install the lastest changes directly from github
 ```bash
 pip install git+https://github.com/chrisdewa/ardilla.git
 pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[async]
+pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[dev]
 ```
 
 
 ## How to use:
 ```py
 from ardilla import Engine, Model, Crud
+from pydantic import Field
 
 engine = Engine('db.sqlite3')
 Crud.engine = engine
 
 class User(Model):
-    id: int
+    id: int = Field(primary=True, autoincrement=True) 
     name: str
     age: int
 
 user_crud: Crud[User] = Crud(User)
 
 def main():
     engine.setup() # creates tables
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ardilla-0.0.3a0/ardilla/abc.py` & `ardilla-0.0.4a0/ardilla/abc.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.3a0/ardilla/asyncio/crud.py` & `ardilla-0.0.4a0/ardilla/asyncio/crud.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.3a0/ardilla/asyncio/engine.py` & `ardilla-0.0.4a0/ardilla/asyncio/engine.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.3a0/ardilla/crud.py` & `ardilla-0.0.4a0/ardilla/crud.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,19 +93,27 @@
     def get_many(self, **kws) -> list[M]:
         """Returns a list of objects that have the given conditions"""
         return self._get_or_none_any(many=True, **kws)
 
     def save_one(self, obj: M) -> Literal[True]:
         """Saves one object to the database"""
         cols, vals = zip(*obj.dict().items())
-        placeholders = ", ".join("?" * len(cols))
 
-        upsert_query = f"""
-        INSERT OR REPLACE INTO {self.tablename} ({', '.join(cols)}) VALUES ({placeholders});
-        """
+        if obj.__rowid__ is not None:
+            upsert_query = f"""
+            UPDATE {self.tablename} SET ({', '.join(f'{k} = ?' for k in cols)}) WHERE rowid = ?;
+            """
+            vals += obj.__rowid__
+
+        else:
+            placeholders = ", ".join("?" * len(cols))
+            upsert_query = f"""
+            INSERT OR REPLACE INTO {self.tablename} ({', '.join(cols)}) VALUES ({placeholders});
+            """
+
         with self.engine as con:
             con.execute(upsert_query, vals)
             con.commit()
         return True
 
     def save_many(self, *objs: M) -> Literal[True]:
         """Saves all the given objects to the database"""
```

### Comparing `ardilla-0.0.3a0/ardilla/engine.py` & `ardilla-0.0.4a0/ardilla/engine.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.3a0/ardilla/models.py` & `ardilla-0.0.4a0/ardilla/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,42 @@
-from typing import TypeVar
+from typing import TypeVar, Annotated
 from pydantic import BaseModel, PrivateAttr
 
-from .schemas import make_schema, FIELD_MAPPING, get_tablename
+from .schemas import make_schema, FIELD_MAPPING, get_tablename, get_pk
 from .errors import ModelIntegrityError
 
 
 class Model(BaseModel):
     __rowid__: int | None = PrivateAttr(default=None)
+    __pk__: str | None # tells the model which key to idenfity as primary
     __tablename__: str  # will default to the lowercase name of the subclass
     __schema__: str  # best effort will be made if it's missing
-    # there's no support for constrains or foreign fields
+    # there's no support for constrains or foreign fields yet but you can
+    # define your own schema to support them
 
     def __init_subclass__(cls, **kws) -> None:
         for field in cls.__fields__.values():
             if field.type_ not in FIELD_MAPPING:
                 raise ModelIntegrityError(
                     f'Field "{field.name}" of model "{cls.__name__}" is of unsupported type "{field.type_}"'
                 )
 
+
         if not hasattr(cls, "__schema__"):
             cls.__schema__ = make_schema(cls)
+        
+        cls.__pk__ = get_pk(cls.__schema__)
 
         if not hasattr(cls, "__tablename__"):
             tablename = get_tablename(cls)
             setattr(cls, "__tablename__", tablename)
 
         super().__init_subclass__(**kws)
 
     def __str__(self) -> str:
         return f"{self!r}"
 
+    @property
+    def has_pk(self) -> bool:
+        return 'primary key' in self.__schema__.lower()
 
 M = TypeVar("M", bound=Model)
```

### Comparing `ardilla-0.0.3a0/ardilla.egg-info/PKG-INFO` & `ardilla-0.0.4a0/ardilla.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.0.3a0
+Version: 0.0.4a0
 Summary: A small package for performing basic CRUD operations with sqlite via aiosqlite and pydantic
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: async
+Provides-Extra: examples
 Provides-Extra: dev
 License-File: LICENCE
 
 # ardilla
 
 <div style="text-align:center">
   <img 
@@ -35,34 +36,39 @@
 
 What this library excels in simplicity it lacks in flexibility so, if you're expecting to use complex queries and intricate relationships, you should should consider other libraries like [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
 
 
 ## install
 Install lastest release from PyPi
 ```bash
-pip install -U ardilla´
+pip install -U ardilla
 pip install -U ardilla[async]
+pip install -U ardilla[dev]
 ```
+- async instaslls aiosqlite
+- dev installs formatting and testing dependencies
 
 Or install the lastest changes directly from github
 ```bash
 pip install git+https://github.com/chrisdewa/ardilla.git
 pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[async]
+pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[dev]
 ```
 
 
 ## How to use:
 ```py
 from ardilla import Engine, Model, Crud
+from pydantic import Field
 
 engine = Engine('db.sqlite3')
 Crud.engine = engine
 
 class User(Model):
-    id: int
+    id: int = Field(primary=True, autoincrement=True) 
     name: str
     age: int
 
 user_crud: Crud[User] = Crud(User)
 
 def main():
     engine.setup() # creates tables
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ardilla-0.0.3a0/pyproject.toml` & `ardilla-0.0.4a0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ardilla"
-version = "0.0.3-alpha"
+version = "0.0.4-alpha"
 authors = [
   { name="ChrisDewa", email="chrisdewa@duck.com" },
 ]
 description = "A small package for performing basic CRUD operations with sqlite via aiosqlite and pydantic"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -19,12 +19,13 @@
 ]
 dependencies = [
   "pydantic==1.10.7",
 ]
 
 [project.optional-dependencies]
 async = ["aiosqlite==0.19.0",]
+examples = ["fastapi-0.95.1", "uvicorn-0.22.0"]
 dev = ["pytest==7.3.1", "pytest-asyncio==0.21.0", "black==23.3.0"]
 
 [project.urls]
 "Homepage" = "https://github.com/chrisdewa/ardilla"
 "Bug Tracker" = "https://github.com/chrisdewa/ardilla/issues"
```

### Comparing `ardilla-0.0.3a0/tests/test_async.py` & `ardilla-0.0.4a0/tests/test_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import sqlite3
 from contextlib import contextmanager, asynccontextmanager
 from pathlib import Path
 
 import pytest
 
+from pydantic import Field
+
 from ardilla import Model
 from ardilla.asyncio import Engine, Crud
 from ardilla.errors import QueryExecutionError
 
 
 path = Path(__file__).parent
 db = path / "testdb.sqlite"
 
 
 class User(Model):
-    id: int
+    id: int = Field(primary=True)
     name: str
     age: int
 
 
 @asynccontextmanager
 async def cleanup():
     try:
```

### Comparing `ardilla-0.0.3a0/tests/test_sync.py` & `ardilla-0.0.4a0/tests/test_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 from contextlib import contextmanager
 from pathlib import Path
 
 import pytest
 
 from ardilla import Engine, Model, Crud
 from ardilla.errors import QueryExecutionError
+from pydantic import Field
 
 
 path = Path(__file__).parent
 db = path / "testdb.sqlite"
 
 
 class User(Model):
-    id: int
+    id: int = Field(primary=True)
     name: str
     age: int
 
 
 @contextmanager
 def cleanup():
     try:
```

