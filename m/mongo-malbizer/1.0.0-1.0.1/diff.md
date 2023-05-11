# Comparing `tmp/mongo_malbizer-1.0.0.tar.gz` & `tmp/mongo_malbizer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mongo_malbizer-1.0.0.tar", last modified: Wed Apr 26 17:58:01 2023, max compression
+gzip compressed data, was "dist\mongo_malbizer-1.0.1.tar", last modified: Thu May 11 19:44:49 2023, max compression
```

## Comparing `mongo_malbizer-1.0.0.tar` & `mongo_malbizer-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 17:58:01.900920 mongo_malbizer-1.0.0/
--rw-rw-rw-   0        0        0     4677 2023-04-26 17:58:01.900920 mongo_malbizer-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3344 2023-04-26 17:57:34.000000 mongo_malbizer-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 17:58:01.896387 mongo_malbizer-1.0.0/mongo_malbizer.egg-info/
--rw-rw-rw-   0        0        0     4677 2023-04-26 17:58:01.000000 mongo_malbizer-1.0.0/mongo_malbizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-04-26 17:58:01.000000 mongo_malbizer-1.0.0/mongo_malbizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 17:58:01.000000 mongo_malbizer-1.0.0/mongo_malbizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-26 17:58:01.000000 mongo_malbizer-1.0.0/mongo_malbizer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-04-26 17:58:01.000000 mongo_malbizer-1.0.0/mongo_malbizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-26 17:58:01.000000 mongo_malbizer-1.0.0/mongo_malbizer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 17:58:01.899902 mongo_malbizer-1.0.0/mongocrud/
--rw-rw-rw-   0        0        0       28 2023-04-26 16:45:44.000000 mongo_malbizer-1.0.0/mongocrud/__init__.py
--rw-rw-rw-   0        0        0     3602 2023-04-26 17:56:53.000000 mongo_malbizer-1.0.0/mongocrud/mongomalbizer.py
--rw-rw-rw-   0        0        0       42 2023-04-26 17:58:01.901903 mongo_malbizer-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1021 2023-04-26 17:57:49.000000 mongo_malbizer-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 19:44:49.858678 mongo_malbizer-1.0.1/
+-rw-rw-rw-   0        0        0     4410 2023-05-11 19:44:49.858678 mongo_malbizer-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3077 2023-04-26 18:13:21.000000 mongo_malbizer-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 19:44:49.853723 mongo_malbizer-1.0.1/mongo_malbizer.egg-info/
+-rw-rw-rw-   0        0        0     4410 2023-05-11 19:44:48.000000 mongo_malbizer-1.0.1/mongo_malbizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-11 19:44:49.000000 mongo_malbizer-1.0.1/mongo_malbizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 19:44:48.000000 mongo_malbizer-1.0.1/mongo_malbizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-26 17:58:01.000000 mongo_malbizer-1.0.1/mongo_malbizer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-05-11 19:44:48.000000 mongo_malbizer-1.0.1/mongo_malbizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 19:44:48.000000 mongo_malbizer-1.0.1/mongo_malbizer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 19:44:49.857717 mongo_malbizer-1.0.1/mongocrud/
+-rw-rw-rw-   0        0        0       28 2023-04-26 16:45:44.000000 mongo_malbizer-1.0.1/mongocrud/__init__.py
+-rw-rw-rw-   0        0        0     3635 2023-05-11 19:44:05.000000 mongo_malbizer-1.0.1/mongocrud/mongomalbizer.py
+-rw-rw-rw-   0        0        0       42 2023-05-11 19:44:49.858678 mongo_malbizer-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1021 2023-05-11 19:44:23.000000 mongo_malbizer-1.0.1/setup.py
```

### Comparing `mongo_malbizer-1.0.0/PKG-INFO` & `mongo_malbizer-1.0.1/mongo_malbizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,111 +1,111 @@
 Metadata-Version: 2.1
-Name: mongo_malbizer
-Version: 1.0.0
+Name: mongo-malbizer
+Version: 1.0.1
 Summary: Python MongoDB CRUD
 Home-page: UNKNOWN
 Author: Anderson Souza
 Author-email: anderson@malbizer.com.br
 License: UNKNOWN
-Description: ## Python Package for MongoDB CRUD
+Description: # Python Package for MongoDB CRUD
         
-        # For use:
-            - Install package with PIP;
-            - Import from mongocrud Mongocrud;
-            - Configure database settings (location, collection, port...);
-            - Call object CRUD operations;
-        
-        # Example:
-        
-            - For INSERT operation in database:
-        
-            ```python
-            from mongocrud import MongoCRUD
-            from datetime import datetime
-        
-            dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
-            
-            dbclients.insert("clients", {"_id": "12345", "name":"Anderson 1", "dtupdate": datetime.now()})
-            dbclients.insert("clients", {"_id": 15 , "name":"Anderson 2", "dtupdate": datetime.now()})
-            dbclients.insert("clients", {"name":"Anderson 3", "dtupdate": datetime.now()})
-            dbclients.insert("clients", {"name":"Anderson 4", "dtupdate": datetime.now()})
-            dbclients.insert("clients", {"name":"Anderson 5", "dtupdate": datetime.now()})
-            #12 bits/24 bits info as _id
-            dbclients.insert("clients", {"_id": ObjectId(b'000000000001'), "name":"Anderson 6", "dtupdate": datetime.now()})
-            ```
-        
-            - For SELECT operation on database (using orderby and direction for sort information):
-        
-            ```python
-            from mongocrud import MongoCRUD
-            from datetime import datetime
-        
-            dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
-            clients_ordered = dbclients.select("clients", orderby="dtupdate", direction=1)
-            
-            for client in clients_ordered: print(client)
-            ```
-        
-            - For SELECT BY _id (select if using ObjectId on _id):
-        
-            ```python
-            from mongocrud import MongoCRUD
-            from datetime import datetime
-        
-            dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
-            
-            clients = dbclients.select_by_id("clients", "12345", is_objectid=False)
-            print(clients)
-            clients = dbclients.select_by_id("clients", 15, is_objectid=False)
-            print(clients)
-            clients = dbclients.select_by_id("clients", "64495d9c140992e498f5fcb2", is_objectid=True)
-            print(clients)
-            ```
-        
-            - For DELETE query in database:
-        
-            ```python
-            from mongocrud import MongoCRUD
-            from datetime import datetime
-        
-            dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
-        
-            items = dbclients.delete("clients", {"name": "Anderson 2"})
-            print("QTD items deleted => ", items)
-            ```
-        
-            - For DELETE BY _id:
-        
-            ```python
-            from mongocrud import MongoCRUD
-            from datetime import datetime
-        
-            dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
-            
-            items = dbclients.delete_by_id("clients", "12345", is_objectid=False)
-            print("QTD items deleted => ", items)
-            
-            items = dbclients.delete_by_id("clients", "64495d9c140992e498f5fcb1", is_objectid=True)
-            print("QTD items deleted => ", items)
-            
-            items = dbclients.delete_by_id("clients", ObjectId(b"000000000001"), is_objectid=False)
-            print("QTD items deleted => ", items)
-            ```
-        
-            - for UPDATE row:
-        
-            ```python
-            from mongocrud import MongoCRUD
-            from datetime import datetime
-        
-            dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
-            
-            dbclients.update_one("clients", "12345", {"name": "teste1", "dtupdate": datetime.now()}, is_objectid=False)
-            dbclients.update_one("clients", "64496373fe1ef021a556b446", {"name": "teste2", "dtupdate": datetime.now()}, is_objectid=True)
-            ```
+        ## For use:
+        - Install package with PIP;
+        - Import from mongocrud Mongocrud;
+        - Configure database settings (location, collection, port...);
+        - Call object CRUD operations;
+        
+        ## Example:
+        
+        * For INSERT operation in database:
+        
+        ```python
+        from mongocrud import MongoCRUD, ObjectId
+        from datetime import datetime
+        
+        dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
+        
+        dbclients.insert("clients", {"_id": "12345", "name":"Anderson 1", "dtupdate": datetime.now()})
+        dbclients.insert("clients", {"_id": 15 , "name":"Anderson 2", "dtupdate": datetime.now()})
+        dbclients.insert("clients", {"name":"Anderson 3", "dtupdate": datetime.now()})
+        dbclients.insert("clients", {"name":"Anderson 4", "dtupdate": datetime.now()})
+        dbclients.insert("clients", {"name":"Anderson 5", "dtupdate": datetime.now()})
+        #12 bits/24 bits info as _id
+        dbclients.insert("clients", {"_id": ObjectId(b'000000000001'), "name":"Anderson 6", "dtupdate": datetime.now()})
+        ```
+        
+        * For SELECT operation on database (using orderby and direction for sort information):
+        
+        ```python
+        from mongocrud import MongoCRUD
+        from datetime import datetime
+        
+        dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
+        clients_ordered = dbclients.select("clients", orderby="dtupdate", direction=1)
+        
+        for client in clients_ordered: print(client)
+        ```
+        
+        * For SELECT BY _id (select if using ObjectId on _id):
+        
+        ```python
+        from mongocrud import MongoCRUD
+        from datetime import datetime
+        
+        dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
+        
+        clients = dbclients.select_by_id("clients", "12345", is_objectid=False)
+        print(clients)
+        clients = dbclients.select_by_id("clients", 15, is_objectid=False)
+        print(clients)
+        clients = dbclients.select_by_id("clients", "64495d9c140992e498f5fcb2", is_objectid=True)
+        print(clients)
+        ```
+        
+        * For DELETE query in database:
+        
+        ```python
+        from mongocrud import MongoCRUD
+        from datetime import datetime
+        
+        dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
+        
+        items = dbclients.delete("clients", {"name": "Anderson 2"})
+        print("QTD items deleted => ", items)
+        ```
+        
+        * For DELETE BY _id:
+        
+        ```python
+        from mongocrud import MongoCRUD, ObjectId
+        from datetime import datetime
+        
+        dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
+        
+        items = dbclients.delete_by_id("clients", "12345", is_objectid=False)
+        print("QTD items deleted => ", items)
+        
+        items = dbclients.delete_by_id("clients", "64495d9c140992e498f5fcb1", is_objectid=True)
+        print("QTD items deleted => ", items)
+        
+        items = dbclients.delete_by_id("clients", ObjectId(b"000000000001"), is_objectid=False)
+        print("QTD items deleted => ", items)
+        ```
+        
+        * for UPDATE row:
+        
+        ```python
+        from mongocrud import MongoCRUD
+        from datetime import datetime
+        
+        dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
+        
+        dbclients.update_one("clients", "12345", {"name": "teste1", "dtupdate": datetime.now()}, is_objectid=False)
+        dbclients.update_one("clients", "64496373fe1ef021a556b446", {"name": "teste2", "dtupdate": datetime.now()}, is_objectid=True)
+        ```
         
         
         
 Keywords: python,mongobd,crud
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mongo_malbizer-1.0.0/README.md` & `mongo_malbizer-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,115 @@
-## Python Package for MongoDB CRUD
-
-# For use:
-    - Install package with PIP;
-    - Import from mongocrud Mongocrud;
-    - Configure database settings (location, collection, port...);
-    - Call object CRUD operations;
-
-# Example:
-
-    - For INSERT operation in database:
-
-    ```python
-    from mongocrud import MongoCRUD
-    from datetime import datetime
-
-    dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
-    
-    dbclients.insert("clients", {"_id": "12345", "name":"Anderson 1", "dtupdate": datetime.now()})
-    dbclients.insert("clients", {"_id": 15 , "name":"Anderson 2", "dtupdate": datetime.now()})
-    dbclients.insert("clients", {"name":"Anderson 3", "dtupdate": datetime.now()})
-    dbclients.insert("clients", {"name":"Anderson 4", "dtupdate": datetime.now()})
-    dbclients.insert("clients", {"name":"Anderson 5", "dtupdate": datetime.now()})
-    #12 bits/24 bits info as _id
-    dbclients.insert("clients", {"_id": ObjectId(b'000000000001'), "name":"Anderson 6", "dtupdate": datetime.now()})
-    ```
-
-    - For SELECT operation on database (using orderby and direction for sort information):
-
-    ```python
-    from mongocrud import MongoCRUD
-    from datetime import datetime
-
-    dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
-    clients_ordered = dbclients.select("clients", orderby="dtupdate", direction=1)
-    
-    for client in clients_ordered: print(client)
-    ```
-
-    - For SELECT BY _id (select if using ObjectId on _id):
-
-    ```python
-    from mongocrud import MongoCRUD
-    from datetime import datetime
-
-    dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
-    
-    clients = dbclients.select_by_id("clients", "12345", is_objectid=False)
-    print(clients)
-    clients = dbclients.select_by_id("clients", 15, is_objectid=False)
-    print(clients)
-    clients = dbclients.select_by_id("clients", "64495d9c140992e498f5fcb2", is_objectid=True)
-    print(clients)
-    ```
-
-    - For DELETE query in database:
-
-    ```python
-    from mongocrud import MongoCRUD
-    from datetime import datetime
-
-    dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
-
-    items = dbclients.delete("clients", {"name": "Anderson 2"})
-    print("QTD items deleted => ", items)
-    ```
-
-    - For DELETE BY _id:
-
-    ```python
-    from mongocrud import MongoCRUD
-    from datetime import datetime
-
-    dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
-    
-    items = dbclients.delete_by_id("clients", "12345", is_objectid=False)
-    print("QTD items deleted => ", items)
-    
-    items = dbclients.delete_by_id("clients", "64495d9c140992e498f5fcb1", is_objectid=True)
-    print("QTD items deleted => ", items)
-    
-    items = dbclients.delete_by_id("clients", ObjectId(b"000000000001"), is_objectid=False)
-    print("QTD items deleted => ", items)
-    ```
-
-    - for UPDATE row:
-
-    ```python
-    from mongocrud import MongoCRUD
-    from datetime import datetime
-
-    dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
-    
-    dbclients.update_one("clients", "12345", {"name": "teste1", "dtupdate": datetime.now()}, is_objectid=False)
-    dbclients.update_one("clients", "64496373fe1ef021a556b446", {"name": "teste2", "dtupdate": datetime.now()}, is_objectid=True)
-    ```
-
-
+Metadata-Version: 2.1
+Name: mongo_malbizer
+Version: 1.0.1
+Summary: Python MongoDB CRUD
+Home-page: UNKNOWN
+Author: Anderson Souza
+Author-email: anderson@malbizer.com.br
+License: UNKNOWN
+Description: # Python Package for MongoDB CRUD
+        
+        ## For use:
+        - Install package with PIP;
+        - Import from mongocrud Mongocrud;
+        - Configure database settings (location, collection, port...);
+        - Call object CRUD operations;
+        
+        ## Example:
+        
+        * For INSERT operation in database:
+        
+        ```python
+        from mongocrud import MongoCRUD, ObjectId
+        from datetime import datetime
+        
+        dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
+        
+        dbclients.insert("clients", {"_id": "12345", "name":"Anderson 1", "dtupdate": datetime.now()})
+        dbclients.insert("clients", {"_id": 15 , "name":"Anderson 2", "dtupdate": datetime.now()})
+        dbclients.insert("clients", {"name":"Anderson 3", "dtupdate": datetime.now()})
+        dbclients.insert("clients", {"name":"Anderson 4", "dtupdate": datetime.now()})
+        dbclients.insert("clients", {"name":"Anderson 5", "dtupdate": datetime.now()})
+        #12 bits/24 bits info as _id
+        dbclients.insert("clients", {"_id": ObjectId(b'000000000001'), "name":"Anderson 6", "dtupdate": datetime.now()})
+        ```
+        
+        * For SELECT operation on database (using orderby and direction for sort information):
+        
+        ```python
+        from mongocrud import MongoCRUD
+        from datetime import datetime
+        
+        dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
+        clients_ordered = dbclients.select("clients", orderby="dtupdate", direction=1)
+        
+        for client in clients_ordered: print(client)
+        ```
+        
+        * For SELECT BY _id (select if using ObjectId on _id):
+        
+        ```python
+        from mongocrud import MongoCRUD
+        from datetime import datetime
+        
+        dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
+        
+        clients = dbclients.select_by_id("clients", "12345", is_objectid=False)
+        print(clients)
+        clients = dbclients.select_by_id("clients", 15, is_objectid=False)
+        print(clients)
+        clients = dbclients.select_by_id("clients", "64495d9c140992e498f5fcb2", is_objectid=True)
+        print(clients)
+        ```
+        
+        * For DELETE query in database:
+        
+        ```python
+        from mongocrud import MongoCRUD
+        from datetime import datetime
+        
+        dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
+        
+        items = dbclients.delete("clients", {"name": "Anderson 2"})
+        print("QTD items deleted => ", items)
+        ```
+        
+        * For DELETE BY _id:
+        
+        ```python
+        from mongocrud import MongoCRUD, ObjectId
+        from datetime import datetime
+        
+        dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
+        
+        items = dbclients.delete_by_id("clients", "12345", is_objectid=False)
+        print("QTD items deleted => ", items)
+        
+        items = dbclients.delete_by_id("clients", "64495d9c140992e498f5fcb1", is_objectid=True)
+        print("QTD items deleted => ", items)
+        
+        items = dbclients.delete_by_id("clients", ObjectId(b"000000000001"), is_objectid=False)
+        print("QTD items deleted => ", items)
+        ```
+        
+        * for UPDATE row:
+        
+        ```python
+        from mongocrud import MongoCRUD
+        from datetime import datetime
+        
+        dbclients = MongoCRUD("mongodb://localhost","mongoteste1")
+        
+        dbclients.update_one("clients", "12345", {"name": "teste1", "dtupdate": datetime.now()}, is_objectid=False)
+        dbclients.update_one("clients", "64496373fe1ef021a556b446", {"name": "teste2", "dtupdate": datetime.now()}, is_objectid=True)
+        ```
+        
+        
+        
+Keywords: python,mongobd,crud
+Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Description-Content-Type: text/markdown
```

### Comparing `mongo_malbizer-1.0.0/mongocrud/mongomalbizer.py` & `mongo_malbizer-1.0.1/mongocrud/mongomalbizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
         try:
             collection = self.db[table]
             _id = collection.insert_one(value).inserted_id
             return _id
         except Exception as e:
             return None
         
-    def insert_or_update(self,table, idvalue, value):
+    def insert_or_update(self,table, idvalue, value, is_objectid = True):
         try:
-            _id = self.update_one(table, idvalue, value)
+            _id = self.update_one(table, idvalue, value, is_objectid)
             if _id == None:
                 value['_id'] = idvalue
                 _id = self.insert(table, value)
             return _id
         except Exception as e:
             print(e)
             return None
```

### Comparing `mongo_malbizer-1.0.0/setup.py` & `mongo_malbizer-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '1.0.0' 
+VERSION = '1.0.1' 
 DESCRIPTION = 'Python MongoDB CRUD'
 LONG_DESCRIPTION = open("README.md",'r').read()
 
 
 # Setting up
 setup(
         name="mongo_malbizer",
```

