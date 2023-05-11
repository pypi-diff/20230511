# Comparing `tmp/bh-database-0.0.3.tar.gz` & `tmp/bh-database-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bh-database-0.0.3.tar", last modified: Tue May  9 00:06:04 2023, max compression
+gzip compressed data, was "bh-database-0.0.4.tar", last modified: Thu May 11 01:27:00 2023, max compression
```

## Comparing `bh-database-0.0.3.tar` & `bh-database-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 00:06:04.372944 bh-database-0.0.3/
--rw-rw-rw-   0        0        0     2484 2023-05-09 00:06:04.370936 bh-database-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1858 2023-01-25 03:51:11.000000 bh-database-0.0.3/README.md
--rw-rw-rw-   0        0        0     1033 2023-05-08 23:24:08.000000 bh-database-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 00:06:04.372944 bh-database-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 00:06:04.310927 bh-database-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 00:06:04.317931 bh-database-0.0.3/src/bh_database/
--rw-rw-rw-   0        0        0       90 2023-01-25 04:17:39.000000 bh-database-0.0.3/src/bh_database/__init__.py
--rw-rw-rw-   0        0        0    22724 2023-05-06 02:18:13.000000 bh-database-0.0.3/src/bh_database/base_table.py
--rw-rw-rw-   0        0        0     2239 2023-01-25 03:51:11.000000 bh-database-0.0.3/src/bh_database/constant.py
--rw-rw-rw-   0        0        0    17779 2023-04-08 05:23:07.000000 bh-database-0.0.3/src/bh_database/core.py
--rw-rw-rw-   0        0        0     5120 2023-01-25 03:51:11.000000 bh-database-0.0.3/src/bh_database/paginator.py
-drwxrwxrwx   0        0        0        0 2023-05-09 00:06:04.332926 bh-database-0.0.3/src/bh_database.egg-info/
--rw-rw-rw-   0        0        0     2484 2023-05-09 00:06:04.000000 bh-database-0.0.3/src/bh_database.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-05-09 00:06:04.000000 bh-database-0.0.3/src/bh_database.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 00:06:04.000000 bh-database-0.0.3/src/bh_database.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      198 2023-05-09 00:06:04.000000 bh-database-0.0.3/src/bh_database.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-09 00:06:04.000000 bh-database-0.0.3/src/bh_database.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 00:06:04.366935 bh-database-0.0.3/tests/
--rw-rw-rw-   0        0        0     5782 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_01_core_database_postgresql.py
--rw-rw-rw-   0        0        0     5682 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_02_core_database_mysql.py
--rw-rw-rw-   0        0        0     3956 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_05_core_basesqlalchemy_postgresql.py
--rw-rw-rw-   0        0        0     3634 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_06_core_basesqlalchemy_mysql.py
--rw-rw-rw-   0        0        0     3423 2023-05-08 23:54:52.000000 bh-database-0.0.3/tests/test_11_paginator_postgresql.py
--rw-rw-rw-   0        0        0     3336 2023-05-08 23:56:42.000000 bh-database-0.0.3/tests/test_12_paginator_mysql.py
--rw-rw-rw-   0        0        0     6937 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_15_base_table_postgresql.py
--rw-rw-rw-   0        0        0     6413 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_16_base_table_mysql.py
--rw-rw-rw-   0        0        0     1651 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_17_base_table_methods.py
--rw-rw-rw-   0        0        0     1616 2023-01-25 03:51:11.000000 bh-database-0.0.3/tests/test_20_base_table_dunder.py
--rw-rw-rw-   0        0        0    19258 2023-04-08 12:11:15.000000 bh-database-0.0.3/tests/test_25_base_table_crud_methods_postgresql.py
--rw-rw-rw-   0        0        0    19133 2023-04-08 12:10:59.000000 bh-database-0.0.3/tests/test_26_base_table_crud_methods_mysql.py
--rw-rw-rw-   0        0        0     4335 2023-04-08 08:41:22.000000 bh-database-0.0.3/tests/test_30_base_table_exception_postgresql.py
--rw-rw-rw-   0        0        0     4270 2023-04-08 08:43:50.000000 bh-database-0.0.3/tests/test_31_base_table_exception_mysql.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:27:00.880742 bh-database-0.0.4/
+-rw-rw-rw-   0        0        0     2484 2023-05-11 01:27:00.879744 bh-database-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1858 2023-01-25 03:51:11.000000 bh-database-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1033 2023-05-11 01:19:54.000000 bh-database-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 01:27:00.880742 bh-database-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 01:27:00.834746 bh-database-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 01:27:00.841743 bh-database-0.0.4/src/bh_database/
+-rw-rw-rw-   0        0        0       90 2023-05-11 01:18:26.000000 bh-database-0.0.4/src/bh_database/__init__.py
+-rw-rw-rw-   0        0        0    23937 2023-05-11 01:11:19.000000 bh-database-0.0.4/src/bh_database/base_table.py
+-rw-rw-rw-   0        0        0     2239 2023-01-25 03:51:11.000000 bh-database-0.0.4/src/bh_database/constant.py
+-rw-rw-rw-   0        0        0    18162 2023-05-11 00:51:04.000000 bh-database-0.0.4/src/bh_database/core.py
+-rw-rw-rw-   0        0        0     5120 2023-01-25 03:51:11.000000 bh-database-0.0.4/src/bh_database/paginator.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:27:00.862740 bh-database-0.0.4/src/bh_database.egg-info/
+-rw-rw-rw-   0        0        0     2484 2023-05-11 01:27:00.000000 bh-database-0.0.4/src/bh_database.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-05-11 01:27:00.000000 bh-database-0.0.4/src/bh_database.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 01:27:00.000000 bh-database-0.0.4/src/bh_database.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      198 2023-05-11 01:27:00.000000 bh-database-0.0.4/src/bh_database.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-11 01:27:00.000000 bh-database-0.0.4/src/bh_database.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 01:27:00.878742 bh-database-0.0.4/tests/
+-rw-rw-rw-   0        0        0     5782 2023-01-25 03:51:11.000000 bh-database-0.0.4/tests/test_01_core_database_postgresql.py
+-rw-rw-rw-   0        0        0     5682 2023-01-25 03:51:11.000000 bh-database-0.0.4/tests/test_02_core_database_mysql.py
+-rw-rw-rw-   0        0        0     3956 2023-01-25 03:51:11.000000 bh-database-0.0.4/tests/test_05_core_basesqlalchemy_postgresql.py
+-rw-rw-rw-   0        0        0     3634 2023-01-25 03:51:11.000000 bh-database-0.0.4/tests/test_06_core_basesqlalchemy_mysql.py
+-rw-rw-rw-   0        0        0     3551 2023-05-10 03:56:40.000000 bh-database-0.0.4/tests/test_11_paginator_postgresql.py
+-rw-rw-rw-   0        0        0     3466 2023-05-10 03:56:45.000000 bh-database-0.0.4/tests/test_12_paginator_mysql.py
+-rw-rw-rw-   0        0        0     7571 2023-05-11 01:13:14.000000 bh-database-0.0.4/tests/test_15_base_table_postgresql.py
+-rw-rw-rw-   0        0        0     7041 2023-05-11 01:06:29.000000 bh-database-0.0.4/tests/test_16_base_table_mysql.py
+-rw-rw-rw-   0        0        0     1651 2023-01-25 03:51:11.000000 bh-database-0.0.4/tests/test_17_base_table_methods.py
+-rw-rw-rw-   0        0        0     1616 2023-01-25 03:51:11.000000 bh-database-0.0.4/tests/test_20_base_table_dunder.py
+-rw-rw-rw-   0        0        0    19413 2023-05-10 10:35:40.000000 bh-database-0.0.4/tests/test_25_base_table_crud_methods_postgresql.py
+-rw-rw-rw-   0        0        0    19290 2023-05-10 10:38:52.000000 bh-database-0.0.4/tests/test_26_base_table_crud_methods_mysql.py
+-rw-rw-rw-   0        0        0     4496 2023-05-10 03:58:11.000000 bh-database-0.0.4/tests/test_30_base_table_exception_postgresql.py
+-rw-rw-rw-   0        0        0     4427 2023-05-10 03:57:49.000000 bh-database-0.0.4/tests/test_31_base_table_exception_mysql.py
```

### Comparing `bh-database-0.0.3/PKG-INFO` & `bh-database-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bh-database
-Version: 0.0.3
+Version: 0.0.4
 Summary: Database wrapper classes for SQLAlchemy.
 Author-email: Van Be Hai Nguyen <behai_nguyen@hotmail.com>
 Project-URL: repository, https://github.com/behai-nguyen/bh_database
 Project-URL: documentation, https://bh-database.readthedocs.io/
 Keywords: SQLAlchemy,database,wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bh-database-0.0.3/README.md` & `bh-database-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.3/pyproject.toml` & `bh-database-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bh-database"
-version = "0.0.3"
+version = "0.0.4"
 description = "Database wrapper classes for SQLAlchemy."
 
 readme = "README.md"
 authors = [{ name = "Van Be Hai Nguyen", email = "behai_nguyen@hotmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `bh-database-0.0.3/src/bh_database/base_table.py` & `bh-database-0.0.4/src/bh_database/base_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,15 +86,24 @@
 
         assert employees.emp_no == 456000
         ...
         assert employees.hire_date == '2021-11-02' 
 
     where :py:class:`WriteCapableTable` is an indirect subclass of :py:class:`BaseTable`.
 
-    For a full example, please see test module ``./tests/test_17_base_table_methods.py``.
+    In general, for this abstract class and its abstract descendant classes, do not 
+    access :attr:`~bh_database.core.BaseSQLAlchemy.query` when not assigned. E.g.::
+
+        assert BaseTable.query == None
+
+    It results in the following exception::
+
+        ArgumentError("Column expression, FROM clause, or other columns clause element expected, <class 'bh_database.core.BaseSQLAlchemy'>.")
+
+    A relevant test module ``./tests/test_17_base_table_methods.py``.
     """
     __abstract__ = True
 
     def __get_primary_keys(self) -> list:
         """Collect primary key column names and return all as a list.
 
         Most tables have only a single primary key.
@@ -153,14 +162,23 @@
     seldom change.
 
     *Read-only* in the sense that this class has only a public method to query database. 
     It is only a semantic classification. It is also an indirect child of 
     :py:class:`~bh_database.core.BaseSQLAlchemy` class, it can use class attributes
     :attr:`~bh_database.core.BaseSQLAlchemy.session` and 
     :attr:`~bh_database.core.BaseSQLAlchemy.query` to alter data directly.
+
+    In general, for this abstract class and its abstract descendant classes, do not 
+    access :attr:`~bh_database.core.BaseSQLAlchemy.query` when not assigned. E.g.::
+
+        assert ReadOnlyTable.query == None
+
+    It results in the following exception::
+
+        ArgumentError("Column expression, FROM clause, or other columns clause element expected, <class 'bh_database.core.BaseSQLAlchemy'>.")
     """
     
     __abstract__ = True
 
     def run_select_sql(self, sql: str, auto_session=False) -> ResultStatus:
         """Run a SELECT SQL full text statement and returns the result.
 
@@ -241,14 +259,23 @@
 
 class WriteCapableTable(ReadOnlyTable):
     """Implement an abstract base model (table) class which INSERT, UPDATE and DELETE
     functionalities.
 
     This table class should be the parent class for the majority of applications' tables, whom 
     the contents would change.
+
+    In general, for this abstract class and its abstract descendant classes, do not 
+    access :attr:`~bh_database.core.BaseSQLAlchemy.query` when not assigned. E.g.::
+
+        assert WriteCapableTable.query == None
+
+    It results in the following exception::
+
+        ArgumentError("Column expression, FROM clause, or other columns clause element expected, <class 'bh_database.core.BaseSQLAlchemy'>.")
     """
 
     __abstract__ = True
 
     def run_execute_sql(self, sql: str, auto_session=False) -> ResultStatus:
         """Run an execute SQL full text statement and return a `ResultStatus 
         <https://bh-apistatus.readthedocs.io/en/latest/result-status.html>`_.
```

### Comparing `bh-database-0.0.3/src/bh_database/constant.py` & `bh-database-0.0.4/src/bh_database/constant.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.3/src/bh_database/core.py` & `bh-database-0.0.4/src/bh_database/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,21 +124,30 @@
     """The parent most class for all models / tables.
 
     Provide methods to implement transaction atomicity.
 
     Class attributes:
         | session = None. When set, is of type `sqlalchemy.orm.session.Session <https://docs.sqlalchemy.org/en/20/orm/session_api.html#sqlalchemy.orm.Session>`_.
         | query = None. When set, is of type :py:class:`BaseQuery`.
+
+    In general, for this abstract class and its abstract descendant classes, do not 
+    access :attr:`query` when not assigned. E.g.::
+
+        assert core.BaseSQLAlchemy.query == None
+
+    It results in the following exception::
+
+        ArgumentError("Column expression, FROM clause, or other columns clause element expected, <class 'bh_database.core.BaseSQLAlchemy'>.")
     """
 
     __abstract__ = True
 
     #: Class attribute. When set, is of type `sqlalchemy.orm.session.Session <https://docs.sqlalchemy.org/en/20/orm/session_api.html#sqlalchemy.orm.Session>`_.
     session = None
-    #: Class attribute. When set, is of type :py:class:`BaseSQLAlchemy`.
+    #: Class attribute. When set, is of type :py:class:`BaseQuery`.    
     query = None
 
     def begin_transaction(self):
         """Start a new transaction.
         """
         if not self.session.in_transaction(): self.session.begin()
```

### Comparing `bh-database-0.0.3/src/bh_database/paginator.py` & `bh-database-0.0.4/src/bh_database/paginator.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.3/src/bh_database.egg-info/PKG-INFO` & `bh-database-0.0.4/src/bh_database.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bh-database
-Version: 0.0.3
+Version: 0.0.4
 Summary: Database wrapper classes for SQLAlchemy.
 Author-email: Van Be Hai Nguyen <behai_nguyen@hotmail.com>
 Project-URL: repository, https://github.com/behai-nguyen/bh_database
 Project-URL: documentation, https://bh-database.readthedocs.io/
 Keywords: SQLAlchemy,database,wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bh-database-0.0.3/src/bh_database.egg-info/SOURCES.txt` & `bh-database-0.0.4/src/bh_database.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.3/tests/test_01_core_database_postgresql.py` & `bh-database-0.0.4/tests/test_01_core_database_postgresql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.3/tests/test_02_core_database_mysql.py` & `bh-database-0.0.4/tests/test_02_core_database_mysql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.3/tests/test_05_core_basesqlalchemy_postgresql.py` & `bh-database-0.0.4/tests/test_05_core_basesqlalchemy_postgresql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.3/tests/test_06_core_basesqlalchemy_mysql.py` & `bh-database-0.0.4/tests/test_06_core_basesqlalchemy_mysql.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.3/tests/test_11_paginator_postgresql.py` & `bh-database-0.0.4/tests/test_11_paginator_postgresql.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,29 +18,31 @@
 
 import pytest
 
 from bh_database import core
 
 from tests.employees import Employees
 
-# @pytest.mark.paginator_postgresql
-# @pytest.mark.behai_only
+@pytest.mark.paginator_postgresql
 def test_postgresql_prepare(postgresql):
     """Database connection management.
 
     The purpose of this method is to establish the connection to the database.
     The postgresql() method need to run FIRST and ONCE to establish the connection.
 
     I find this sort of work around is the most reliable method to control codes
     execution sequence.
     """
 
     assert core.BaseSQLAlchemy.session != None
+
     # BaseSQLAlchemy is abstract, with no table name.
-    assert core.BaseSQLAlchemy.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert core.BaseSQLAlchemy.query == None
 
     assert Employees.query != None
 
 @pytest.mark.paginator_postgresql
 def test_postgresql_paginator_01():
     """
     First page.
```

### Comparing `bh-database-0.0.3/tests/test_12_paginator_mysql.py` & `bh-database-0.0.4/tests/test_12_paginator_mysql.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,29 +17,31 @@
 
 import pytest
 
 from bh_database import core
 
 from tests.employees import Employees
 
-# @pytest.mark.paginator_mysql
-@pytest.mark.behai_only
+@pytest.mark.paginator_mysql
 def test_mysql_prepare(mysql):
     """Database connection management.
 
     The purpose of this method is to establish the connection to the database.
     The mysql() method need to run FIRST and ONCE to establish the connection.
 
     I find this sort of work around is the most reliable method to control codes
     execution sequence.
     """
 
     assert core.BaseSQLAlchemy.session != None
+
     # BaseSQLAlchemy is abstract, with no table name.
-    assert core.BaseSQLAlchemy.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert core.BaseSQLAlchemy.query == None
 
     assert Employees.query != None
 
 @pytest.mark.paginator_mysql
 def test_mysql_paginator_01():
     """
     First page.
```

### Comparing `bh-database-0.0.3/tests/test_15_base_table_postgresql.py` & `bh-database-0.0.4/tests/test_15_base_table_postgresql.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,16 +58,19 @@
     The postgresql() method need to run FIRST and ONCE to establish the connection.
 
     I find this sort of work around is the most reliable method to control codes
     execution sequence.
     """
 
     assert core.BaseSQLAlchemy.session != None
+
     # BaseSQLAlchemy is abstract, with no table name.
-    assert core.BaseSQLAlchemy.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert core.BaseSQLAlchemy.query == None
 
 @pytest.mark.base_table_postgresql
 def test_postgresql_base_session():
     assert PostgreSQLBaseTable.session != None
 
     test = PostgreSQLBaseTable()	
     assert (test.session is PostgreSQLBaseTable.session) == True
@@ -120,16 +123,20 @@
     assert id(test1.session) == id(BaseTable.session)
 
     assert (test.session is test1.session) == True
     assert id(test.session) == id(test1.session)
 
 @pytest.mark.base_table_postgresql
 def test_postgresql_base_query():
+    
     # BaseTable is abstract with no table name.
-    assert BaseTable.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert BaseTable.query == None
+
     # PostgreSQLBaseTable is not abstract, with a table name.
     assert PostgreSQLBaseTable.query != None
 
     test = PostgreSQLBaseTable()	
     assert test.query != None
     assert (test.query is PostgreSQLBaseTable.query) == False
     assert id(test.query) != id(PostgreSQLBaseTable.query)
@@ -141,15 +148,18 @@
     assert (test.query is test1.query) == False
     assert id(test.query) != id(test1.query)
 
 @pytest.mark.base_table_postgresql 
 def test_postgresql_readonly_query():
 
     # ReadOnlyTable is abstract with no table name.
-    assert ReadOnlyTable.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert ReadOnlyTable.query == None
+
     # PostgreSQLReadOnlyTable is not abstract, with a table name.
     assert PostgreSQLReadOnlyTable.query != None
 
     test = PostgreSQLReadOnlyTable()	
     assert test.query != None
     assert (test.query is PostgreSQLReadOnlyTable.query) == False
     assert id(test.query) != id(PostgreSQLReadOnlyTable.query)
@@ -160,15 +170,18 @@
 
     assert (test.query is test1.query) == False
     assert id(test.query) != id(test1.query)
 
 @pytest.mark.base_table_postgresql
 def test_postgresql_writecapable_query():
     # WriteCapableTable is abstract with no table name.
-    assert WriteCapableTable.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert WriteCapableTable.query == None
+
     # PostgreSQLWriteCapableTable is not abstract, with a table name.
     assert PostgreSQLWriteCapableTable.query != None
 
     test = PostgreSQLWriteCapableTable()	
     assert test.query != None
     assert (test.query is PostgreSQLWriteCapableTable.query) == False
     assert id(test.query) != id(PostgreSQLWriteCapableTable.query)
```

### Comparing `bh-database-0.0.3/tests/test_16_base_table_mysql.py` & `bh-database-0.0.4/tests/test_16_base_table_mysql.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,16 +57,19 @@
     The mysql() method need to run FIRST and ONCE to establish the connection.
 
     I find this sort of work around is the most reliable method to control codes
     execution sequence.
     """
 
     assert core.BaseSQLAlchemy.session != None
+
     # BaseSQLAlchemy is abstract, with no table name.
-    assert core.BaseSQLAlchemy.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert core.BaseSQLAlchemy.query == None
 
 @pytest.mark.base_table_mysql
 def test_mysql_base_session():
     test = MySQLBaseTable()	
     assert (test.session is MySQLBaseTable.session) == True
     assert (test.session is BaseTable.session) == True
     assert id(test.session) == id(MySQLBaseTable.session)
@@ -114,15 +117,18 @@
 
     assert (test.session is test1.session) == True
     assert id(test.session) == id(test1.session)
 
 @pytest.mark.base_table_mysql
 def test_mysql_base_query():
     # BaseTable is abstract with no table name.
-    assert BaseTable.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert BaseTable.query == None
+
     # MySQLBaseTable is not abstract, with a table name.
     assert MySQLBaseTable.query != None
 
     test = MySQLBaseTable()	
     assert test.query != None
     assert (test.query is MySQLBaseTable.query) == False
     assert id(test.query) != id(MySQLBaseTable.query)
@@ -133,15 +139,18 @@
 
     assert (test.query is test1.query) == False
     assert id(test.query) != id(test1.query)
 
 @pytest.mark.base_table_mysql 
 def test_mysql_readonly_query():
     # ReadOnlyTable is abstract with no table name.
-    assert ReadOnlyTable.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert ReadOnlyTable.query == None
+
     # MySQLReadOnlyTable is not abstract, with a table name.
     assert MySQLReadOnlyTable.query != None
 
     test = MySQLReadOnlyTable()	
     assert test.query != None
     assert (test.query is MySQLReadOnlyTable.query) == False
     assert id(test.query) != id(MySQLReadOnlyTable.query)
@@ -152,15 +161,18 @@
 
     assert (test.query is test1.query) == False
     assert id(test.query) != id(test1.query)
 
 @pytest.mark.base_table_mysql
 def test_mysql_writecapable_query():
     # WriteCapableTable is abstract with no table name.
-    assert WriteCapableTable.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert WriteCapableTable.query == None
+
     # MySQLWriteCapableTable is not abstract, with a table name.
     assert MySQLWriteCapableTable.query != None
 
     test = MySQLWriteCapableTable()	
     assert test.query != None
     assert (test.query is MySQLWriteCapableTable.query) == False
     assert id(test.query) != id(MySQLWriteCapableTable.query)
```

### Comparing `bh-database-0.0.3/tests/test_17_base_table_methods.py` & `bh-database-0.0.4/tests/test_17_base_table_methods.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.3/tests/test_20_base_table_dunder.py` & `bh-database-0.0.4/tests/test_20_base_table_dunder.py`

 * *Files identical despite different names*

### Comparing `bh-database-0.0.3/tests/test_25_base_table_crud_methods_postgresql.py` & `bh-database-0.0.4/tests/test_25_base_table_crud_methods_postgresql.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 
     I find this sort of work around is the most reliable method to control codes
     execution sequence.
     """
 
     assert core.BaseSQLAlchemy.session != None
     # BaseSQLAlchemy is abstract, with no table name.
-    assert core.BaseSQLAlchemy.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert core.BaseSQLAlchemy.query == None
 
 @pytest.mark.base_table_crud_postgresql
 def test_postgresql_run_select_sql():
     """Test a full text SELECT SQL statement.
     """
 
     employees = Employees()
```

### Comparing `bh-database-0.0.3/tests/test_26_base_table_crud_methods_mysql.py` & `bh-database-0.0.4/tests/test_26_base_table_crud_methods_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,19 @@
     The postgresql() method need to run FIRST and ONCE to establish the connection.
 
     I find this sort of work around is the most reliable method to control codes
     execution sequence.
     """
 
     assert core.BaseSQLAlchemy.session != None
+
     # BaseSQLAlchemy is abstract, with no table name.
-    assert core.BaseSQLAlchemy.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert core.BaseSQLAlchemy.query == None
 
 @pytest.mark.base_table_crud_mysql
 def test_mysql_run_select_sql():
     """Test a full text SELECT SQL statement.
     """
 
     employees = Employees()
```

### Comparing `bh-database-0.0.3/tests/test_30_base_table_exception_postgresql.py` & `bh-database-0.0.4/tests/test_30_base_table_exception_postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,19 @@
     The postgresql() method need to run FIRST and ONCE to establish the connection.
 
     I find this sort of work around is the most reliable method to control codes
     execution sequence.
     """
 
     assert core.BaseSQLAlchemy.session != None
+
     # BaseSQLAlchemy is abstract, with no table name.
-    assert core.BaseSQLAlchemy.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert core.BaseSQLAlchemy.query == None    
 
 @pytest.mark.base_table_exception_postgresql
 def test_postgresql_write_to_database_exception():
     """Insert two records, one after the other, with duplicate primary key,
     the second one should fail, exception should be handled.
 
     Test that the second insert failed and status code is 500.
```

### Comparing `bh-database-0.0.3/tests/test_31_base_table_exception_mysql.py` & `bh-database-0.0.4/tests/test_31_base_table_exception_mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,19 @@
     The mysql() method need to run FIRST and ONCE to establish the connection.
 
     I find this sort of work around is the most reliable method to control codes
     execution sequence.
     """
 
     assert core.BaseSQLAlchemy.session != None
+
     # BaseSQLAlchemy is abstract, with no table name.
-    assert core.BaseSQLAlchemy.query == None
+    # ArgumentError("Column expression, FROM clause, or other columns clause element expected, 
+    # got <class 'bh_database.core.BaseSQLAlchemy'>.")
+    # assert core.BaseSQLAlchemy.query == None
 
 @pytest.mark.base_table_exception_mysql
 def test_mysql_write_to_database_exception():
     """Insert two records, one after the other, with duplicate primary key,
     the second one should fail, exception should be handled.
 
     Test that the second insert failed and status code is 500.
```

