# Comparing `tmp/ardilla-0.0.2a0.tar.gz` & `tmp/ardilla-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardilla-0.0.2a0.tar", last modified: Wed May 10 03:05:52 2023, max compression
+gzip compressed data, was "ardilla-0.0.3a0.tar", last modified: Thu May 11 02:52:21 2023, max compression
```

## Comparing `ardilla-0.0.2a0.tar` & `ardilla-0.0.3a0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 03:05:52.863148 ardilla-0.0.2a0/
--rw-rw-rw-   0        0        0     1084 2023-05-08 03:28:44.000000 ardilla-0.0.2a0/LICENCE
--rw-rw-rw-   0        0        0     2893 2023-05-10 03:05:52.863148 ardilla-0.0.2a0/PKG-INFO
--rw-rw-rw-   0        0        0     2226 2023-05-10 02:41:02.000000 ardilla-0.0.2a0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 03:05:52.755811 ardilla-0.0.2a0/ardilla/
--rw-rw-rw-   0        0        0      106 2023-05-08 02:18:14.000000 ardilla-0.0.2a0/ardilla/__init__.py
--rw-rw-rw-   0        0        0     2212 2023-05-10 02:30:00.000000 ardilla-0.0.2a0/ardilla/abc.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:05:52.845105 ardilla-0.0.2a0/ardilla/asyncio/
--rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.0.2a0/ardilla/asyncio/__init__.py
--rw-rw-rw-   0        0        0     6118 2023-05-10 02:39:24.000000 ardilla-0.0.2a0/ardilla/asyncio/crud.py
--rw-rw-rw-   0        0        0      760 2023-05-10 02:34:10.000000 ardilla-0.0.2a0/ardilla/asyncio/engine.py
--rw-rw-rw-   0        0        0     5958 2023-05-10 02:39:55.000000 ardilla-0.0.2a0/ardilla/crud.py
--rw-rw-rw-   0        0        0     1045 2023-05-09 21:05:12.000000 ardilla-0.0.2a0/ardilla/engine.py
--rw-rw-rw-   0        0        0      212 2023-05-10 02:29:23.000000 ardilla-0.0.2a0/ardilla/errors.py
--rw-rw-rw-   0        0        0     1106 2023-05-09 14:59:59.000000 ardilla-0.0.2a0/ardilla/models.py
--rw-rw-rw-   0        0        0     1327 2023-05-09 20:34:49.000000 ardilla-0.0.2a0/ardilla/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:05:52.804321 ardilla-0.0.2a0/ardilla.egg-info/
--rw-rw-rw-   0        0        0     2893 2023-05-10 03:05:52.000000 ardilla-0.0.2a0/ardilla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-05-10 03:05:52.000000 ardilla-0.0.2a0/ardilla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 03:05:52.000000 ardilla-0.0.2a0/ardilla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-05-10 03:05:52.000000 ardilla-0.0.2a0/ardilla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 03:05:52.000000 ardilla-0.0.2a0/ardilla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      850 2023-05-10 02:49:34.000000 ardilla-0.0.2a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 03:05:52.863148 ardilla-0.0.2a0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 03:05:52.861365 ardilla-0.0.2a0/tests/
--rw-rw-rw-   0        0        0     4121 2023-05-10 02:48:27.000000 ardilla-0.0.2a0/tests/test_async.py
--rw-rw-rw-   0        0        0      454 2023-05-09 18:32:20.000000 ardilla-0.0.2a0/tests/test_models.py
--rw-rw-rw-   0        0        0     3793 2023-05-10 02:47:41.000000 ardilla-0.0.2a0/tests/test_sync.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:21.453472 ardilla-0.0.3a0/
+-rw-rw-rw-   0        0        0     1084 2023-05-08 03:28:44.000000 ardilla-0.0.3a0/LICENCE
+-rw-rw-rw-   0        0        0     3731 2023-05-11 02:52:21.447479 ardilla-0.0.3a0/PKG-INFO
+-rw-rw-rw-   0        0        0     3064 2023-05-10 04:27:22.000000 ardilla-0.0.3a0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:21.174823 ardilla-0.0.3a0/ardilla/
+-rw-rw-rw-   0        0        0      106 2023-05-08 02:18:14.000000 ardilla-0.0.3a0/ardilla/__init__.py
+-rw-rw-rw-   0        0        0     2836 2023-05-11 02:46:45.000000 ardilla-0.0.3a0/ardilla/abc.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:21.410471 ardilla-0.0.3a0/ardilla/asyncio/
+-rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.0.3a0/ardilla/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     6181 2023-05-11 02:46:29.000000 ardilla-0.0.3a0/ardilla/asyncio/crud.py
+-rw-rw-rw-   0        0        0      738 2023-05-11 02:46:33.000000 ardilla-0.0.3a0/ardilla/asyncio/engine.py
+-rw-rw-rw-   0        0        0     5898 2023-05-11 02:46:43.000000 ardilla-0.0.3a0/ardilla/crud.py
+-rw-rw-rw-   0        0        0     1013 2023-05-11 02:46:53.000000 ardilla-0.0.3a0/ardilla/engine.py
+-rw-rw-rw-   0        0        0      216 2023-05-11 02:46:57.000000 ardilla-0.0.3a0/ardilla/errors.py
+-rw-rw-rw-   0        0        0     1166 2023-05-11 02:47:01.000000 ardilla-0.0.3a0/ardilla/models.py
+-rw-rw-rw-   0        0        0     1263 2023-05-11 02:47:06.000000 ardilla-0.0.3a0/ardilla/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:21.364468 ardilla-0.0.3a0/ardilla.egg-info/
+-rw-rw-rw-   0        0        0     3731 2023-05-11 02:52:20.000000 ardilla-0.0.3a0/ardilla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-05-11 02:52:21.000000 ardilla-0.0.3a0/ardilla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 02:52:20.000000 ardilla-0.0.3a0/ardilla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-05-11 02:52:20.000000 ardilla-0.0.3a0/ardilla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-11 02:52:20.000000 ardilla-0.0.3a0/ardilla.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      867 2023-05-11 02:51:34.000000 ardilla-0.0.3a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 02:52:21.454471 ardilla-0.0.3a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 02:52:21.441468 ardilla-0.0.3a0/tests/
+-rw-rw-rw-   0        0        0     4064 2023-05-11 02:47:13.000000 ardilla-0.0.3a0/tests/test_async.py
+-rw-rw-rw-   0        0        0      464 2023-05-11 02:47:16.000000 ardilla-0.0.3a0/tests/test_models.py
+-rw-rw-rw-   0        0        0     3730 2023-05-11 02:47:20.000000 ardilla-0.0.3a0/tests/test_sync.py
```

### Comparing `ardilla-0.0.2a0/LICENCE` & `ardilla-0.0.3a0/LICENCE`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.2a0/PKG-INFO` & `ardilla-0.0.3a0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,43 @@
-Metadata-Version: 2.1
-Name: ardilla
-Version: 0.0.2a0
-Summary: A small package for performing basic CRUD operations with sqlite via aiosqlite and pydantic
-Author-email: ChrisDewa <chrisdewa@duck.com>
-Project-URL: Homepage, https://github.com/chrisdewa/ardilla
-Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: async
-Provides-Extra: dev
-License-File: LICENCE
-
 # ardilla
 
+<div style="text-align:center">
+  <img 
+    src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
+  >  
+</div>
+
 Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
 
 A very simple library to quickly add SQLite to your program.
 It leverages pydantic for data validation and modeling.
 It comes in sync (sqlite3) and async (aiosqlite) flavors.
 
+## Who and what is this for:
+
+The target audience for this library are developers who want to incorporate a SQLite database to their applications in a fast and easy way. 
+
+What this library excels in simplicity it lacks in flexibility so, if you're expecting to use complex queries and intricate relationships, you should should consider other libraries like [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
+
 
 ## install
-Install directly from github
-__**Without asynchronous support**__
+Install lastest release from PyPi
 ```bash
-pip install git+https://github.com/chrisdewa/ardilla.git
+pip install -U ardilla´
+pip install -U ardilla[async]
 ```
-__**With asynchronous support**__
+
+Or install the lastest changes directly from github
 ```bash
+pip install git+https://github.com/chrisdewa/ardilla.git
 pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[async]
 ```
 
-## How to use:
-
-**This section is greatly underdeveloped**
 
+## How to use:
 ```py
 from ardilla import Engine, Model, Crud
 
 engine = Engine('db.sqlite3')
 Crud.engine = engine
 
 class User(Model):
@@ -85,8 +80,8 @@
 - [ ] Docstring everything using Google format
 - [ ] Add testing
 - [ ] Add proper documentation
   - propper as in a site with how to use
 - [x] Add a schema generator 
   - There should be a method to generate a table's schema off the pydantic model. 
 - [ ] Add a method somewhere to fetch relationships. 
-- [ ] Improve this readme
+- [ ] Improve this read
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ardilla-0.0.2a0/ardilla/asyncio/crud.py` & `ardilla-0.0.3a0/ardilla/asyncio/crud.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,80 +1,83 @@
 from typing import Literal, Generic, Self
 
 import aiosqlite
+from aiosqlite import Row
 
 from .engine import AsyncEngine
 
 from ..errors import QueryExecutionError
 from ..models import M
 from ..abc import CrudABC
 
 
 class AsyncCrud(CrudABC, Generic[M]):
     """Abstracts CRUD actions for model associated tables"""
+
     engine: AsyncEngine
-    
-    async def _get_or_none_any(self, many: bool, **kws):
+
+    async def _get_or_none_any(self, many: bool, **kws) -> list[M] | M | None:
         """
         private helper to the get_or_none queries.
         if param "many" is true it will return a list of matches else will return only one record
         """
         keys, vals = zip(*kws.items())
         to_match = f" AND ".join(f"{k} = ?" for k in keys)
 
-        limit = 'LIMIT 1;' if not many else ';'
-        q = f"SELECT * FROM {self.tablename} WHERE ({to_match}) {limit}"
+        limit = "LIMIT 1;" if not many else ";"
+        q = f"SELECT rowid, * FROM {self.tablename} WHERE ({to_match}) {limit}"
 
         async with self.engine as con:
             async with con.execute(q, vals) as cur:
                 if many:
-                    result = await cur.fetchall()
-                    return [self.Model(**entry) for entry in result]
+                    rows: list[Row] = await cur.fetchall()
+                    return [self._row2obj(row) for row in rows]
 
                 else:
-                    result = await cur.fetchone()
-                    if result:
-                        return self.Model(**result)
+                    row: Row | None = await cur.fetchone()
+                    if row:
+                        return self._row2obj(row)
+        return
 
     async def get_or_none(self, **kws) -> M | None:
         """Gets an object from a database or None if not found"""
         return await self._get_or_none_any(many=False, **kws)
 
-    async def _do_insert(self, ignore: bool = False, returning: bool = True, / , **kws):
+    async def _do_insert(self, ignore: bool = False, returning: bool = True, /, **kws):
         keys, vals = zip(*kws.items())
         placeholders = ", ".join("?" * len(keys))
         cols = ", ".join(keys)
-        
+
         q = "INSERT OR IGNORE " if ignore else "INSERT "
         q += f"INTO {self.tablename} ({cols}) VALUES ({placeholders})"
         q += " RETURNING *;" if returning else ";"
-        
+
         async with self.engine as con:
             con = await self.engine.connect()
             cur = None
             try:
                 cur = await con.execute(q, vals)
             except aiosqlite.IntegrityError as e:
                 raise QueryExecutionError(str(e))
             else:
-                result = await cur.fetchone()
+                row = await cur.fetchone()
                 await con.commit()
-                if returning and result:
-                    return self.Model(**result)
+                if returning and row:
+                    return self._row2obj(row, cur.lastrowid)
             finally:
                 if cur is not None:
                     await cur.close()
                 await con.close()
-    
+
     async def insert(self, **kws):
         """
         Inserts a record into the database.
         Returns:
             Model | None: Returns a model only if newly created
-        Rises: 
+        Rises:
             ardilla.error.QueryExecutionError: if there's a conflict when inserting the record
         """
         return await self._do_insert(False, True, **kws)
 
     async def insert_or_ignore(self, **kws) -> M | None:
         """inserts a the object of a row or ignores it if it already exists"""
         return await self._do_insert(True, True, **kws)
```

### Comparing `ardilla-0.0.2a0/ardilla/crud.py` & `ardilla-0.0.3a0/ardilla/crud.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sqlite3
+from sqlite3 import Row
 from typing import Literal, Generic, Self
 
 from .engine import Engine
 from .abc import CrudABC
 from .models import M, Model as BaseModel
 from .errors import QueryExecutionError
 
@@ -14,68 +15,66 @@
         """
         private helper to the get_or_none queries.
         if param "many" is true it will return a list of matches else will return only one record
         """
         keys, vals = zip(*kws.items())
         to_match = f" AND ".join(f"{k} = ?" for k in keys)
 
-        limit = 'LIMIT 1;' if not many else ';'
-        q = f"SELECT * FROM {self.tablename} WHERE ({to_match}) {limit}"
+        limit = "LIMIT 1;" if not many else ";"
+        q = f"SELECT rowid, * FROM {self.tablename} WHERE ({to_match}) {limit}"
         with self.engine as con:
             with self.engine.cursor(con) as cur:
                 cur.execute(q, vals)
                 if many:
-                    results: list[dict] = cur.fetchall()
-                    return [self.Model(**entry) for entry in results]
+                    rows: list[Row] = cur.fetchall()
+                    return [self._row2obj(row) for row in rows]
                 else:
-                    result: dict = cur.fetchone()
-                    if result:
-                        return self.Model(**result)
+                    row: Row | None = cur.fetchone()
+                    if row:
+                        return self._row2obj(row)
         return
 
-
-    def get_or_none(self, **kws) -> M | None:
-        """Gets an object from a database or None if not found"""
-        return self._get_or_none_any(many=False, **kws)
-    
-    def _do_insert(self, ignore: bool = False, returning: bool = True, / , **kws):
+    def _do_insert(self, ignore: bool = False, returning: bool = True, /, **kws):
         keys, vals = zip(*kws.items())
         placeholders = ", ".join("?" * len(keys))
         cols = ", ".join(keys)
-        
+
         q = "INSERT OR IGNORE " if ignore else "INSERT "
         q += f"INTO {self.tablename} ({cols}) VALUES ({placeholders})"
         q += " RETURNING *;" if returning else ";"
-        
+
         with self.engine as con:
             with self.engine.cursor(con) as cur:
                 try:
                     cur.execute(q, vals)
                 except sqlite3.IntegrityError as e:
-                    raise QueryExecutionError(str(e)) 
-                    
-                result = cur.fetchone()
+                    raise QueryExecutionError(str(e))
+
+                row = cur.fetchone()
                 con.commit()
-                if returning and result:
-                    return self.Model(**result)
-    
+                if returning and row:
+                    return self._row2obj(row, cur.lastrowid)
+
+    def get_or_none(self, **kws) -> M | None:
+        """Gets an object from a database or None if not found"""
+        return self._get_or_none_any(many=False, **kws)
+
     def insert(self, **kws):
         """
         Inserts a record into the database.
         Returns:
             Model | None: Returns a model only if newly created
-        Rises: 
+        Rises:
             ardilla.error.QueryExecutionError: if there's a conflict when inserting the record
         """
         return self._do_insert(False, True, **kws)
 
     def insert_or_ignore(self, **kws) -> M | None:
         """inserts a the object of a row or ignores it if it already exists"""
         return self._do_insert(True, True, **kws)
-        
 
     def get_or_create(self, **kws) -> tuple[M, bool]:
         """Returns object and bool indicated if it was created or not"""
         created = False
         result = self.get_or_none(**kws)
         if not result:
             result = self.insert_or_ignore(**kws)
@@ -86,15 +85,15 @@
         """Gets all objects from the database"""
         q = f"SELECT * FROM {self.tablename};"
         with self.engine as con:
             with self.engine.cursor(con) as cur:
                 cur.execute(q)
                 results = cur.fetchall()
                 return [self.Model(**res) for res in results]
-        
+
     def get_many(self, **kws) -> list[M]:
         """Returns a list of objects that have the given conditions"""
         return self._get_or_none_any(many=True, **kws)
 
     def save_one(self, obj: M) -> Literal[True]:
         """Saves one object to the database"""
         cols, vals = zip(*obj.dict().items())
@@ -112,15 +111,15 @@
         """Saves all the given objects to the database"""
         placeholders = ", ".join("?" * len(self.columns))
         q = f'INSERT OR REPLACE INTO {self.tablename} ({", ".join(self.columns)}) VALUES ({placeholders});'
         vals = [tuple(obj.dict().values()) for obj in objs]
         with self.engine as con:
             con.executemany(q, vals)
             con.commit()
-            
+
         return True
 
     def delete_one(self, obj: M) -> Literal[True]:
         """
         Deletes the object from the database (won't delete the actual object)
         queries only by the Model id fields (fields suffixed with 'id')
         """
@@ -130,15 +129,15 @@
         vals = tuple([obj_dict[k] for k in id_cols])
         q = f"""
         DELETE FROM {self.tablename} WHERE ({placeholders});
         """
         with self.engine as con:
             con.execute(q, vals)
             con.commit()
-        
+
         return True
 
     def delete_many(self, *objs: M) -> Literal[True]:
         if not objs:
             raise IndexError('param "objs" is empty, pass at least one object')
 
         prot = objs[0]
```

### Comparing `ardilla-0.0.2a0/ardilla/engine.py` & `ardilla-0.0.3a0/ardilla/engine.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,40 +3,39 @@
 
 from .models import M
 
 
 class ContextCursor:
     def __init__(self, con: sqlite3.Connection):
         self.con = con
-    
+
     def __enter__(self) -> sqlite3.Cursor:
         self.cur = self.con.cursor()
         return self.cur
 
     def __exit__(self, *_) -> None:
         self.cur.close()
 
+
 class Engine:
     def __init__(self, path: str):
         self.path = path
         self.schemas: set[str] = set()
-        
+
     def __enter__(self) -> sqlite3.Connection:
         con = sqlite3.connect(self.path)
         con.row_factory = sqlite3.Row
         self.con = con
         return con
 
     def __exit__(self, *_):
         self.con.close()
 
     def cursor(self, con: sqlite3.Connection) -> ContextCursor:
         return ContextCursor(con)
-        
+
     def setup(self):
         with self as con:
-            con.execute('PRAGMA foreign_keys = ON;')
+            con.execute("PRAGMA foreign_keys = ON;")
             for table in self.schemas:
                 con.execute(table)
             con.commit()
-    
-
```

### Comparing `ardilla-0.0.2a0/ardilla/models.py` & `ardilla-0.0.3a0/ardilla/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from typing import TypeVar
-from pydantic import BaseModel
+from pydantic import BaseModel, PrivateAttr
 
 from .schemas import make_schema, FIELD_MAPPING, get_tablename
 from .errors import ModelIntegrityError
 
 
 class Model(BaseModel):
-    __tablename__: str # will default to the lowercase name of the subclass
-    __schema__: str # best effort will be made if it's missing
-                    # there's no support for constrains or foreign fields
-        
+    __rowid__: int | None = PrivateAttr(default=None)
+    __tablename__: str  # will default to the lowercase name of the subclass
+    __schema__: str  # best effort will be made if it's missing
+    # there's no support for constrains or foreign fields
+
     def __init_subclass__(cls, **kws) -> None:
         for field in cls.__fields__.values():
             if field.type_ not in FIELD_MAPPING:
-                raise ModelIntegrityError(f'Field "{field.name}" of model "{cls.__name__}" is of unsupported type "{field.type_}"')
-            
-        if not hasattr(cls, '__schema__'):
+                raise ModelIntegrityError(
+                    f'Field "{field.name}" of model "{cls.__name__}" is of unsupported type "{field.type_}"'
+                )
+
+        if not hasattr(cls, "__schema__"):
             cls.__schema__ = make_schema(cls)
-        
-        if not hasattr(cls, '__tablename__'):
+
+        if not hasattr(cls, "__tablename__"):
             tablename = get_tablename(cls)
-            setattr(cls, '__tablename__', tablename)
-        
+            setattr(cls, "__tablename__", tablename)
+
         super().__init_subclass__(**kws)
 
     def __str__(self) -> str:
         return f"{self!r}"
 
 
-M = TypeVar('M', bound=Model)
+M = TypeVar("M", bound=Model)
```

### Comparing `ardilla-0.0.2a0/ardilla/schemas.py` & `ardilla-0.0.3a0/ardilla/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-
 from datetime import datetime, date
 from pydantic import BaseModel
 
 
-SCHEMA_TEMPLATE = 'CREATE TABLE IF NOT EXISTS {tablename} (\n{fields}\n);'
+SCHEMA_TEMPLATE = "CREATE TABLE IF NOT EXISTS {tablename} (\n{fields}\n);"
 
 
 FIELD_MAPPING = {
-    int: 'INTEGER',
-    float: 'REAL',
-    str: 'TEXT',
-    bytes: 'BLOB',
-    bool: 'INTEGER',
-    date: 'DATE',
-    datetime: 'TIMESTAMP'
+    int: "INTEGER",
+    float: "REAL",
+    str: "TEXT",
+    bytes: "BLOB",
+    bool: "INTEGER",
+    date: "DATE",
+    datetime: "TIMESTAMP",
 }
 
+
 def get_tablename(model: type[BaseModel]) -> str:
-    return getattr(model, '__tablename__', model.__name__.lower())
+    return getattr(model, "__tablename__", model.__name__.lower())
+
 
 def get_fields(model: type[BaseModel]) -> str:
-    
     fields = []
     for field in model.__fields__.values():
         if field.type_ not in FIELD_MAPPING:
             raise TypeError(f'Unrecognized sqlite type "{field.type_}"')
-        
+
         type_ = FIELD_MAPPING[field.type_]
-        
-        out = f'    {field.name} {type_}'
-        if field.name == 'id' and type_ == 'INTEGER':
-            out += ' PRIMARY KEY AUTOINCREMENT'
-        if field.required and not out.endswith('AUTOINCREMENT'):
-            out += ' NOT NULL'
+
+        out = f"    {field.name} {type_}"
+        if field.name == "id" and type_ == "INTEGER":
+            out += " PRIMARY KEY"
+        if field.required and not out.endswith("KEY"):
+            out += " NOT NULL"
         if field.default is not None:
-            out += f' DEFAULT {field.default!r}'
-        
+            out += f" DEFAULT {field.default!r}"
+
         fields.append(out)
-        
-    return ',\n'.join(fields)
+
+    return ",\n".join(fields)
+
 
 def make_schema(Model: type[BaseModel]) -> str:
     return SCHEMA_TEMPLATE.format(
-        tablename=get_tablename(Model),
-        fields=get_fields(Model)
-    )
+        tablename=get_tablename(Model), fields=get_fields(Model)
+    )
```

### Comparing `ardilla-0.0.2a0/ardilla.egg-info/PKG-INFO` & `ardilla-0.0.3a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.0.2a0
+Version: 0.0.3a0
 Summary: A small package for performing basic CRUD operations with sqlite via aiosqlite and pydantic
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,36 +13,48 @@
 Description-Content-Type: text/markdown
 Provides-Extra: async
 Provides-Extra: dev
 License-File: LICENCE
 
 # ardilla
 
+<div style="text-align:center">
+  <img 
+    src="https://images-ext-2.discordapp.net/external/sxevZWKA4UIZWNyt352zkHLGWrUMw_PV_jGWLXGPh_I/https/repository-images.githubusercontent.com/638528340/a0238c4e-addf-4130-a0fe-9a458be6cdc9?width=200&height=150"
+  >  
+</div>
+
 Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
 
 A very simple library to quickly add SQLite to your program.
 It leverages pydantic for data validation and modeling.
 It comes in sync (sqlite3) and async (aiosqlite) flavors.
 
+## Who and what is this for:
+
+The target audience for this library are developers who want to incorporate a SQLite database to their applications in a fast and easy way. 
+
+What this library excels in simplicity it lacks in flexibility so, if you're expecting to use complex queries and intricate relationships, you should should consider other libraries like [tortoise-orm](https://github.com/tortoise/tortoise-orm), [sqlalchemy](https://github.com/sqlalchemy/sqlalchemy), [pony](https://github.com/ponyorm/pony) or [peewee](https://github.com/coleifer/peewee).
+
 
 ## install
-Install directly from github
-__**Without asynchronous support**__
+Install lastest release from PyPi
 ```bash
-pip install git+https://github.com/chrisdewa/ardilla.git
+pip install -U ardilla´
+pip install -U ardilla[async]
 ```
-__**With asynchronous support**__
+
+Or install the lastest changes directly from github
 ```bash
+pip install git+https://github.com/chrisdewa/ardilla.git
 pip install git+https://github.com/chrisdewa/ardilla.git#egg=ardilla[async]
 ```
 
-## How to use:
-
-**This section is greatly underdeveloped**
 
+## How to use:
 ```py
 from ardilla import Engine, Model, Crud
 
 engine = Engine('db.sqlite3')
 Crud.engine = engine
 
 class User(Model):
@@ -85,8 +97,8 @@
 - [ ] Docstring everything using Google format
 - [ ] Add testing
 - [ ] Add proper documentation
   - propper as in a site with how to use
 - [x] Add a schema generator 
   - There should be a method to generate a table's schema off the pydantic model. 
 - [ ] Add a method somewhere to fetch relationships. 
-- [ ] Improve this readme
+- [ ] Improve this read
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ardilla-0.0.2a0/pyproject.toml` & `ardilla-0.0.3a0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ardilla"
-version = "0.0.2-alpha"
+version = "0.0.3-alpha"
 authors = [
   { name="ChrisDewa", email="chrisdewa@duck.com" },
 ]
 description = "A small package for performing basic CRUD operations with sqlite via aiosqlite and pydantic"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -19,12 +19,12 @@
 ]
 dependencies = [
   "pydantic==1.10.7",
 ]
 
 [project.optional-dependencies]
 async = ["aiosqlite==0.19.0",]
-dev = ["pytest==7.3.1", "pytest-asyncio==0.21.0"]
+dev = ["pytest==7.3.1", "pytest-asyncio==0.21.0", "black==23.3.0"]
 
 [project.urls]
 "Homepage" = "https://github.com/chrisdewa/ardilla"
 "Bug Tracker" = "https://github.com/chrisdewa/ardilla/issues"
```

### Comparing `ardilla-0.0.2a0/tests/test_async.py` & `ardilla-0.0.3a0/tests/test_async.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,123 +1,129 @@
-
 import sqlite3
 from contextlib import contextmanager, asynccontextmanager
 from pathlib import Path
 
 import pytest
 
 from ardilla import Model
 from ardilla.asyncio import Engine, Crud
 from ardilla.errors import QueryExecutionError
 
 
 path = Path(__file__).parent
-db = path / 'testdb.sqlite' 
+db = path / "testdb.sqlite"
+
 
 class User(Model):
     id: int
     name: str
     age: int
 
+
 @asynccontextmanager
 async def cleanup():
     try:
         db.unlink(missing_ok=True)
         engine = Engine(db)
         Crud.engine = engine
         crud: Crud[User] = Crud(User)
         await engine.setup()
         yield crud
     finally:
         db.unlink(missing_ok=True)
 
+
 @contextmanager
 def query():
     try:
         con = sqlite3.connect(db)
         cur = con.cursor()
         yield cur
     finally:
         cur.close()
         con.close()
 
+
 @pytest.mark.asyncio
 async def test_create():
     async with cleanup() as crud:
-        chris = User(id=1, name='chris', age=35)
-        moni = User(id=2, name='moni', age=36)
-        elena = User(id=3, name='elena', age=5)
+        chris = User(id=1, name="chris", age=35)
+        moni = User(id=2, name="moni", age=36)
+        elena = User(id=3, name="elena", age=5)
         await crud.save_many(chris, moni, elena)
-        fran = User(id=4, name='fran', age=1)
+        fran = User(id=4, name="fran", age=1)
         await crud.save_one(fran)
-        
+
         with query() as cur:
-            cur.execute('SELECT * FROM user;')
+            cur.execute("SELECT * FROM user;")
             res = cur.fetchall()
-        
-        assert len(res) == 4, 'Mistmatch created vs found'
-        
+
+        assert len(res) == 4, "Mistmatch created vs found"
+
         try:
-            await crud.insert(id=1, name='john', age=34)
+            await crud.insert(id=1, name="john", age=34)
         except QueryExecutionError:
             pass
         else:
-            raise Exception('QueryExcecutionError should have been rised')
-        
-        u = await crud.insert_or_ignore(id=1, name='john', age=34)
-        assert u is None, 'Record 1 already exists but was somehow re-inserted'
-        
-        u = await crud.insert_or_ignore(name='john', age=34)
-        assert u is not None and u.name == 'john', 'Bad user was created'
-        
+            raise Exception("QueryExcecutionError should have been rised")
+
+        u = await crud.insert_or_ignore(id=1, name="john", age=34)
+        assert u is None, "Record 1 already exists but was somehow re-inserted"
+
+        u = await crud.insert_or_ignore(name="john", age=34)
+        assert u is not None and u.name == "john", "Bad user was created"
+
+
 @pytest.mark.asyncio
 async def test_read():
     async with cleanup() as crud:
-        chris = User(id=1, name='chris', age=35)
-        chris2 = User(id=2, name='chris', age=36)
-        elena = User(id=3, name='elena', age=5)
+        chris = User(id=1, name="chris", age=35)
+        chris2 = User(id=2, name="chris", age=36)
+        elena = User(id=3, name="elena", age=5)
         await crud.save_many(chris, chris2, elena)
-        
+
         users = await crud.get_all()
-        assert len(users) == 3, 'Wrong number of read users from get_all'
-        users = await crud.get_many(name='chris')
-        assert len(users) == 2, 'wrong number of users from get_many'
+        assert len(users) == 3, "Wrong number of read users from get_all"
+        users = await crud.get_many(name="chris")
+        assert len(users) == 2, "wrong number of users from get_many"
         u = await crud.get_or_none(id=1)
-        assert u == chris, 'bad user found'
+        assert u == chris, "bad user found"
         u = await crud.get_or_none(id=5)
-        assert u is None, 'bad user not found'
-        u,c = await crud.get_or_create(name='fran', age=1)
-        assert c is True, 'Bad created value'
-        assert u == User(id=4, name='fran', age=1), 'bad created user'
-        u,c = await crud.get_or_create(id=3)
-        assert u == elena, 'bad user found'
-        assert c is False, 'Bad not created value'
-        
+        assert u is None, "bad user not found"
+        u, c = await crud.get_or_create(name="fran", age=1)
+        assert c is True, "Bad created value"
+        assert u == User(id=4, name="fran", age=1), "bad created user"
+        u, c = await crud.get_or_create(id=3)
+        assert u == elena, "bad user found"
+        assert c is False, "Bad not created value"
+
+
 @pytest.mark.asyncio
 async def test_update():
     async with cleanup() as crud:
-        chris = User(id=1, name='chris', age=35)
-        moni = User(id=2, name='moni', age=36)
+        chris = User(id=1, name="chris", age=35)
+        moni = User(id=2, name="moni", age=36)
         await crud.save_many(chris, moni)
         chris.age = 40
         await crud.save_one(chris)
         u = await crud.get_or_none(**chris.dict())
-        assert u is not None, 'user not updated'
+        assert u is not None, "user not updated"
         chris.age = 45
         moni.age = 50
         await crud.save_many(chris, moni)
         u = await crud.get_or_none(**moni.dict())
-        assert u is not None, 'User not updated on many'
-        
+        assert u is not None, "User not updated on many"
+
+
 @pytest.mark.asyncio
 async def test_delete():
     async with cleanup() as crud:
-        chris = User(id=1, name='chris', age=35)
-        moni = User(id=2, name='moni', age=36)
-        elena = User(id=3, name='elena', age=5)
+        chris = User(id=1, name="chris", age=35)
+        moni = User(id=2, name="moni", age=36)
+        elena = User(id=3, name="elena", age=5)
         await crud.save_many(chris, moni, elena)
         await crud.delete_one(moni)
         users = await crud.get_all()
         assert len(users) == 2, "Delete one missmatch"
         await crud.delete_many(chris, elena)
         users = await crud.get_all()
-        assert len(users) == 0, "Delete many missmatch"
+        assert len(users) == 0, "Delete many missmatch"
```

### Comparing `ardilla-0.0.2a0/tests/test_sync.py` & `ardilla-0.0.3a0/tests/test_sync.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,121 +1,124 @@
-
 import sqlite3
 from contextlib import contextmanager
 from pathlib import Path
 
 import pytest
 
 from ardilla import Engine, Model, Crud
 from ardilla.errors import QueryExecutionError
 
 
 path = Path(__file__).parent
-db = path / 'testdb.sqlite' 
+db = path / "testdb.sqlite"
+
 
 class User(Model):
     id: int
     name: str
     age: int
 
+
 @contextmanager
 def cleanup():
     try:
         db.unlink(missing_ok=True)
         engine = Engine(db)
         Crud.engine = engine
         crud: Crud[User] = Crud(User)
         engine.setup()
         yield crud
     finally:
         db.unlink(missing_ok=True)
 
+
 @contextmanager
 def query():
     try:
         con = sqlite3.connect(db)
         cur = con.cursor()
         yield cur
     finally:
         cur.close()
         con.close()
 
 
 def test_create():
     with cleanup() as crud:
-        chris = User(id=1, name='chris', age=35)
-        moni = User(id=2, name='moni', age=36)
-        elena = User(id=3, name='elena', age=5)
+        chris = User(id=1, name="chris", age=35)
+        moni = User(id=2, name="moni", age=36)
+        elena = User(id=3, name="elena", age=5)
         crud.save_many(chris, moni, elena)
-        fran = User(id=4, name='fran', age=1)
+        fran = User(id=4, name="fran", age=1)
         crud.save_one(fran)
-        
+
         with query() as cur:
-            cur.execute('SELECT * FROM user;')
+            cur.execute("SELECT * FROM user;")
             res = cur.fetchall()
-        
-        assert len(res) == 4, 'Mistmatch created vs found'
-        
+
+        assert len(res) == 4, "Mistmatch created vs found"
+
         try:
-            crud.insert(id=1, name='john', age=34)
+            crud.insert(id=1, name="john", age=34)
         except QueryExecutionError:
             pass
         else:
-            raise Exception('QueryExcecutionError should have been rised')
-        
-        u = crud.insert_or_ignore(id=1, name='john', age=34)
-        assert u is None, 'Record 1 already exists but was somehow re-inserted'
-        
-        u = crud.insert_or_ignore(name='john', age=34)
-        assert u is not None and u.name == 'john', 'Bad user was created'
-            
-            
+            raise Exception("QueryExcecutionError should have been rised")
+
+        u = crud.insert_or_ignore(id=1, name="john", age=34)
+        assert u is None, "Record 1 already exists but was somehow re-inserted"
+
+        u = crud.insert_or_ignore(name="john", age=34)
+        assert u is not None and u.name == "john", "Bad user was created"
+
 
 def test_read():
     with cleanup() as crud:
-        chris = User(id=1, name='chris', age=35)
-        chris2 = User(id=2, name='chris', age=36)
-        elena = User(id=3, name='elena', age=5)
+        chris = User(id=1, name="chris", age=35)
+        chris2 = User(id=2, name="chris", age=36)
+        elena = User(id=3, name="elena", age=5)
         crud.save_many(chris, chris2, elena)
-        
+
         users = crud.get_all()
-        assert len(users) == 3, 'Wrong number of read users from get_all'
-        users = crud.get_many(name='chris')
-        assert len(users) == 2, 'wrong number of users from get_many'
+        assert len(users) == 3, "Wrong number of read users from get_all"
+        users = crud.get_many(name="chris")
+        assert len(users) == 2, "wrong number of users from get_many"
         u = crud.get_or_none(id=1)
-        assert u == chris, 'bad user found'
+        assert u == chris, "bad user found"
         u = crud.get_or_none(id=5)
-        assert u is None, 'bad user not found'
-        u,c = crud.get_or_create(name='fran', age=1)
-        assert c is True, 'Bad created value'
-        assert u == User(id=4, name='fran', age=1), 'bad created user'
-        u,c = crud.get_or_create(id=3)
-        assert u == elena, 'bad user found'
-        assert c is False, 'Bad not created value'
+        assert u is None, "bad user not found"
+        u, c = crud.get_or_create(name="fran", age=1)
+        assert c is True, "Bad created value"
+        assert u == User(id=4, name="fran", age=1), "bad created user"
+        u, c = crud.get_or_create(id=3)
+        assert u == elena, "bad user found"
+        assert c is False, "Bad not created value"
+
 
 def test_update():
     with cleanup() as crud:
-        chris = User(id=1, name='chris', age=35)
-        moni = User(id=2, name='moni', age=36)
+        chris = User(id=1, name="chris", age=35)
+        moni = User(id=2, name="moni", age=36)
         crud.save_many(chris, moni)
         chris.age = 40
         crud.save_one(chris)
         u = crud.get_or_none(**chris.dict())
-        assert u is not None, 'user not updated'
+        assert u is not None, "user not updated"
         chris.age = 45
         moni.age = 50
         crud.save_many(chris, moni)
         u = crud.get_or_none(**moni.dict())
-        assert u is not None, 'User not updated on many'
+        assert u is not None, "User not updated on many"
+
 
 def test_delete():
     with cleanup() as crud:
-        chris = User(id=1, name='chris', age=35)
-        moni = User(id=2, name='moni', age=36)
-        elena = User(id=3, name='elena', age=5)
+        chris = User(id=1, name="chris", age=35)
+        moni = User(id=2, name="moni", age=36)
+        elena = User(id=3, name="elena", age=5)
         crud.save_many(chris, moni, elena)
         crud.delete_one(moni)
         users = crud.get_all()
         assert len(users) == 2, "Delete one missmatch"
         crud.delete_many(chris, elena)
         users = crud.get_all()
-        assert len(users) == 0, "Delete many missmatch"
+        assert len(users) == 0, "Delete many missmatch"
```

