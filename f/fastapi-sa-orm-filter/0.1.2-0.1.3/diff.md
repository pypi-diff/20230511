# Comparing `tmp/fastapi-sa-orm-filter-0.1.2.tar.gz` & `tmp/fastapi-sa-orm-filter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-sa-orm-filter-0.1.2.tar", last modified: Tue May  9 21:00:40 2023, max compression
+gzip compressed data, was "fastapi-sa-orm-filter-0.1.3.tar", last modified: Thu May 11 06:49:19 2023, max compression
```

## Comparing `fastapi-sa-orm-filter-0.1.2.tar` & `fastapi-sa-orm-filter-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      813 2023-05-07 17:56:59.474207 fastapi-sa-orm-filter-0.1.2/.github/workflows/ci_filter.yml
--rw-r--r--   0        0        0     1073 2023-05-07 07:37:25.294746 fastapi-sa-orm-filter-0.1.2/LICENSE
--rw-r--r--   0        0        0      271 2023-05-07 14:19:55.337103 fastapi-sa-orm-filter-0.1.2/Pipfile
--rw-r--r--   0        0        0    23646 2023-05-07 14:21:44.504856 fastapi-sa-orm-filter-0.1.2/Pipfile.lock
--rw-r--r--   0        0        0     2262 2023-05-09 20:58:55.302181 fastapi-sa-orm-filter-0.1.2/README.md
--rw-r--r--   0        0        0      111 2023-05-09 21:00:38.156799 fastapi-sa-orm-filter-0.1.2/fastapi_sa_orm_filter/__init__.py
--rw-r--r--   0        0        0     8558 2023-05-09 20:19:47.476212 fastapi-sa-orm-filter-0.1.2/fastapi_sa_orm_filter/main.py
--rw-r--r--   0        0        0      434 2023-05-09 20:13:04.305063 fastapi-sa-orm-filter-0.1.2/fastapi_sa_orm_filter/operators.py
--rw-r--r--   0        0        0      844 2023-05-07 18:13:40.160724 fastapi-sa-orm-filter-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      143 2023-05-04 19:03:00.838038 fastapi-sa-orm-filter-0.1.2/pytest.ini
--rw-r--r--   0        0        0     3364 2023-05-09 20:41:44.249744 fastapi-sa-orm-filter-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0    15503 2023-05-09 20:55:09.225275 fastapi-sa-orm-filter-0.1.2/tests/test_filter.py
--rw-r--r--   0        0        0      323 2023-05-05 21:57:39.693231 fastapi-sa-orm-filter-0.1.2/tests/utils.py
--rw-r--r--   0        0        0     3021 1970-01-01 00:00:00.000000 fastapi-sa-orm-filter-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-05-07 17:56:59.474207 fastapi-sa-orm-filter-0.1.3/.github/workflows/ci_filter.yml
+-rw-r--r--   0        0        0     1073 2023-05-07 07:37:25.294746 fastapi-sa-orm-filter-0.1.3/LICENSE
+-rw-r--r--   0        0        0      271 2023-05-07 14:19:55.337103 fastapi-sa-orm-filter-0.1.3/Pipfile
+-rw-r--r--   0        0        0    23646 2023-05-07 14:21:44.504856 fastapi-sa-orm-filter-0.1.3/Pipfile.lock
+-rw-r--r--   0        0        0     2529 2023-05-11 06:46:05.227485 fastapi-sa-orm-filter-0.1.3/README.md
+-rw-r--r--   0        0        0      111 2023-05-11 06:49:13.039045 fastapi-sa-orm-filter-0.1.3/fastapi_sa_orm_filter/__init__.py
+-rw-r--r--   0        0        0     6617 2023-05-11 06:36:12.456633 fastapi-sa-orm-filter-0.1.3/fastapi_sa_orm_filter/main.py
+-rw-r--r--   0        0        0      497 2023-05-10 20:18:36.372884 fastapi-sa-orm-filter-0.1.3/fastapi_sa_orm_filter/operators.py
+-rw-r--r--   0        0        0     4936 2023-05-11 06:30:01.548954 fastapi-sa-orm-filter-0.1.3/fastapi_sa_orm_filter/parsers.py
+-rw-r--r--   0        0        0      844 2023-05-07 18:13:40.160724 fastapi-sa-orm-filter-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      143 2023-05-04 19:03:00.838038 fastapi-sa-orm-filter-0.1.3/pytest.ini
+-rw-r--r--   0        0        0     3364 2023-05-09 20:41:44.249744 fastapi-sa-orm-filter-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0    17207 2023-05-11 06:40:39.744176 fastapi-sa-orm-filter-0.1.3/tests/test_filter.py
+-rw-r--r--   0        0        0      323 2023-05-05 21:57:39.693231 fastapi-sa-orm-filter-0.1.3/tests/utils.py
+-rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 fastapi-sa-orm-filter-0.1.3/PKG-INFO
```

### Comparing `fastapi-sa-orm-filter-0.1.2/.github/workflows/ci_filter.yml` & `fastapi-sa-orm-filter-0.1.3/.github/workflows/ci_filter.yml`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.2/LICENSE` & `fastapi-sa-orm-filter-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.2/Pipfile.lock` & `fastapi-sa-orm-filter-0.1.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.2/README.md` & `fastapi-sa-orm-filter-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ## FastAPI SQLAlchemy Filter 
-Package that helps to implement easy objects filter for applications
+Package that helps to implement easy objects filtering and sorting for applications
 build on FastAPI and SQLAlchemy.
 For using you just need to define your custom filter with filtered fields and applied operators.
 Supported operators, datatypes and example of work you can find below.
 
 ### Installation
 ```shell
 pip install fastapi-sa-orm-filter
@@ -20,62 +20,64 @@
 from db.base import get_session
 from db.models import MyModel
 
 
 app = FastAPI()
 
 # Define fields and operators for filter
-my_item_filter = {
-    'my_model_field_name': [fls.eq, fls.in_],
-    'my_model_field_name': [fls.between, fls.eq, fls.gt, fls.lt, fls.in_],
-    'my_model_field_name': [fls.like, fls.startswith, fls.contains, fls.in_],
-    'my_model_field_name': [fls.between, fls.not_eq, fls.gte, fls.lte]
+my_objects_filter = {
+    'my_model_field_name': [ops.eq, ops.in_],
+    'my_model_field_name': [ops.between, ops.eq, ops.gt, ops.lt, ops.in_],
+    'my_model_field_name': [ops.like, ops.startswith, ops.contains, ops.in_],
+    'my_model_field_name': [ops.between, ops.not_eq, ops.gte, ops.lte]
 }
 
 @app.get("/")
-async def get_filtered_items(
+async def get_filtered_objects(
     filter_query: str = Query(default=''),
     db: AsyncSession = Depends(get_session)
  ) -> List[MyModel]:
-    my_filter = FilterCore(MyModel, my_item_filter)
+    my_filter = FilterCore(MyModel, my_objects_filter)
     query = my_filter.get_query(filter_query)
     res = await db.execute(query)
     return res.scalars().all()
 ```
 
 ### Example of work
 
 ```shell
 
 # Input query string
 '''
 salary_from__in_=60,70,80&
 created_at__between=2023-05-01,2023-05-05|
-category__eq=Medicine"
+category__eq=Medicine&
+order_by=-id,category
 '''
 
    
 # Returned SQLAlchemy orm query exact as:
            
 select(model)
     .where(
         or_(
             and_(
                 model.salary_from.in_(60,70,80),
                 model.created_at.between(2023-05-01, 2023-05-05)
             ),
             model.category == 'Medicine'
-        )
+        ).order_by(model.id.desc(), model.category.asc())
 ```
 
 ### Supported query string format
 
 * field_name__eq=value
 * field_name__in_=value1,value2
 * field_name__eq=value&field_name__in_=value1,value2
+* field_name__eq=value&field_name__in_=value1,value2&order_by=-field_name
 
 ### Supported SQLAlchemy datatypes:
 * DATETIME
 * DATE
 * INTEGER
 * FLOAT
 * TEXT
@@ -97,7 +99,11 @@
 * __ilike__
 * __contains__
 * __icontains__
 * __not_eq__
 * __not_in__
 * __not_like__
 * __not_between__
+
+#### For suggestions and questions, feel free to contact me through email 
+__zhydykalex@ukr.net__
+
```

### Comparing `fastapi-sa-orm-filter-0.1.2/fastapi_sa_orm_filter/main.py` & `fastapi-sa-orm-filter-0.1.3/fastapi_sa_orm_filter/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
-from typing import Any, Dict, List, Tuple, Optional, Union, Type
+from typing import Any, Dict, List, Type
 
 import pydantic
-from fastapi import HTTPException, Query
+from fastapi import HTTPException
 from pydantic import create_model
 from pydantic.main import ModelMetaclass
 from pydantic_sqlalchemy import sqlalchemy_to_pydantic
 from sqlalchemy import select
 from sqlalchemy.orm import InstrumentedAttribute, DeclarativeMeta
 from sqlalchemy.sql.elements import BinaryExpression
 from sqlalchemy.sql.expression import and_, or_
 from starlette import status
 from sqlalchemy.sql import Select
 
 from fastapi_sa_orm_filter.operators import Operators as ops
+from fastapi_sa_orm_filter.parsers import _FilterQueryParser, _OrderByQueryParser
 
 
 class FilterCore:
     """
     Class serves of SQLAlchemy orm query creation.
     Convert parsed query data to python data types and form SQLAlchemy query.
     """
@@ -43,32 +44,44 @@
     def get_query(self, custom_filter: str) -> Select:
         """
         Construct the SQLAlchemy orm query from request query string
 
         :param custom_filter: request query string with fields and filter conditions
             salary_from__in_=60,70,80&
             created_at__between=2023-05-01,2023-05-05|
-            category__eq=Medicine
+            category__eq=Medicine&
+            order_by=-id
 
         :return:
             select(model)
                 .where(
                     or_(
                         and_(
                             model.salary_from.in_(60,70,80),
                             model.created_at.between(2023-05-01, 2023-05-05)
                         ),
                         model.category == 'Medicine'
-                    )
+                    ).order_by(model.id.desc())
         """
+        split_query = self.split_by_order_by(custom_filter)
+        if len(split_query) == 1:
+            filter_query = self._get_filter_query(split_query[0])
+            return filter_query
+        filter_query_str, order_by_query_str = split_query
+        filter_query = self._get_filter_query(filter_query_str)
+        order_by_query = _OrderByQueryParser(self._model).get_order_by_query(order_by_query_str)
+        query = filter_query.order_by(*order_by_query)
+        return query
+
+    def _get_filter_query(self, custom_filter):
         if not custom_filter:
             query = select(self._model)
             return query
         conditions = []
-        query_parser = QueryParser(custom_filter, self._model, self._allowed_filters)
+        query_parser = _FilterQueryParser(custom_filter, self._model, self._allowed_filters)
         for and_expressions in query_parser.get_parsed_query():
             and_condition = []
             for expression in and_expressions:
                 column, operator, value = expression
                 serialized_dict = self._format_expression(column, operator, value)
                 value = serialized_dict[column.name]
                 param = self._get_orm_for_field(column, operator, value)
@@ -84,28 +97,28 @@
 
         :return: {
             'optional_model':
                 class model.__name__(BaseModel):
                     field: Optional[type]
             'list_model':
                 class model.__name__(BaseModel):
-                    field: List[type]
+                    field: Optional[List[type]]
         }
         """
         pydantic_serializer = sqlalchemy_to_pydantic(self._model)
         fields_to_optional = {
             f.name: (f.type_, None) for f in pydantic_serializer.__fields__.values()
         }
-        fields_wrap_to_list = {
+        fields_wrap_to_optional_list = {
             f.name: (List[f.type_], None)
             for f in pydantic_serializer.__fields__.values()
         }
         optional_model = create_model(self._model.__name__, **fields_to_optional)
-        list_model = create_model(self._model.__name__, **fields_wrap_to_list)
-        return {"optional_model": optional_model, "list_model": list_model}
+        optional_list_model = create_model(self._model.__name__, **fields_wrap_to_optional_list)
+        return {"optional_model": optional_model, "list_model": optional_list_model}
 
     @staticmethod
     def _get_orm_for_field(
         column: InstrumentedAttribute, operator: str, value: Any
     ) -> BinaryExpression:
         """
         Create SQLAlchemy orm expression for the field
@@ -143,92 +156,16 @@
             )
         except ValueError:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
                 detail=f"Incorrect filter value '{value}'",
             )
 
-
-class QueryParser:
-    """
-    Class parse request query string.
-    """
-
-    def __init__(self, query, model, allowed_filters):
-        self.query = query
-        self.model = model
-        self.allowed_filters = allowed_filters
-
-    def get_parsed_query(self):
-        """
-        :return:
-            [
-                [[column, operator, value], [column, operator, value]],
-                [[column, operator, value]]
-            ]
-        """
-        and_blocks = self._parse_by_conjunctions()
-        par = []
-        for and_block in and_blocks:
-            parsed_and_blocks = []
-            for expression in and_block:
-                column, operator, value = self._parse_expression(expression)
-                self._validate_query_params(column.name, operator)
-                parsed_and_blocks.append([column, operator, value])
-            par.append(parsed_and_blocks)
-        return par
-
-    def _parse_by_conjunctions(self) -> List[List[str]]:
-        """
-        Split request query string by 'OR' and 'AND' conjunctions
-        to divide query string to field's conditions
-
-        :return: [
-                    ['field_name__operator=value', 'field_name__operator=value'],
-                    ['field_name__operator=value']
-                ]
-        """
-        and_blocks = [block.split("&") for block in self.query.split("|")]
-        return and_blocks
-
-    def _parse_expression(
-        self, expression: str
-    ) -> Union[Tuple[InstrumentedAttribute, str, str], HTTPException]:
-        try:
-            field_name, condition = expression.split("__")
-            operator, value = condition.split("=")
-        except Exception:
-            raise HTTPException(
-                status_code=status.HTTP_400_BAD_REQUEST,
-                detail="Incorrect filter request syntax,"
-                " please use pattern :"
-                "'{field_name}__{condition}={value}{conjunction}'",
-            )
-        if not hasattr(self.model, field_name):
-            raise HTTPException(
-                status_code=status.HTTP_400_BAD_REQUEST,
-                detail=f"DB model {self.model} doesn't have field '{field_name}'",
-            )
-        else:
-            column = getattr(self.model, field_name)
-        return column, operator, value
-
-    def _validate_query_params(
-        self, field_name: str, operator: str
-    ) -> Optional[HTTPException]:
-        """
-        Check expression on valid and allowed field_name and operator
-        """
-        if field_name not in self.allowed_filters:
+    @staticmethod
+    def split_by_order_by(query):
+        split_query = [query_part.strip("&") for query_part in query.split("order_by=")]
+        if len(split_query) > 2:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail=f"Forbidden filter field '{field_name}'",
+                detail="Use only one order_by directive",
             )
-        for allow_filter in self.allowed_filters[field_name]:
-            if operator == allow_filter.name:
-                return
-        raise HTTPException(
-            status_code=status.HTTP_400_BAD_REQUEST,
-            detail=f"Forbidden filter '{operator}' for '{field_name}'",
-        )
-
-    Query
+        return split_query
```

### Comparing `fastapi-sa-orm-filter-0.1.2/pyproject.toml` & `fastapi-sa-orm-filter-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.2/tests/conftest.py` & `fastapi-sa-orm-filter-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.2/tests/test_filter.py` & `fastapi-sa-orm-filter-0.1.3/tests/test_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,14 +332,61 @@
         'is_active': True,
         'salary_from': 100,
         'salary_up_to': 150.725,
         'category': JobCategory.metallurgy
     }
 
 
+async def test_complex_query_with_order_by(session, get_filter, create_vacancies):
+    query = get_filter.get_query(
+        "created_at__between=2023-05-01,2023-05-05&"
+        "updated_at__in_=2023-01-05 15:15:15,2023-05-05 15:15:15|"
+        "salary_from__gt=100&"
+        "order_by=-id"
+    )
+    res = await session.execute(query)
+    data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
+    assert len(data['vacancies']) == 7
+    assert isinstance(data['vacancies'][0]["created_at"], date)
+    assert isinstance(data['vacancies'][0]["updated_at"], datetime)
+    check_data = data['vacancies'][0].copy()
+    del check_data['created_at']
+    del check_data['updated_at']
+    assert check_data == {
+        'id': 10,
+        'title': 'title10',
+        'description': 'description10',
+        'is_active': True,
+        'salary_from': 150,
+        'salary_up_to': 200.725,
+        'category': JobCategory.miscellaneous
+    }
+
+
+async def test_order_by_id(session, get_filter, create_vacancies):
+    query = get_filter.get_query("order_by=-id")
+    res = await session.execute(query)
+    data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
+    assert len(data['vacancies']) == 10
+    assert isinstance(data['vacancies'][0]["created_at"], date)
+    assert isinstance(data['vacancies'][0]["updated_at"], datetime)
+    check_data = data['vacancies'][0].copy()
+    del check_data["created_at"]
+    del check_data["updated_at"]
+    assert check_data == {
+        'id': 10,
+        'title': 'title10',
+        'description': 'description10',
+        'is_active': True,
+        'salary_from': 150,
+        'salary_up_to': 200.725,
+        'category': JobCategory.miscellaneous
+    }
+
+
 @pytest.mark.parametrize(
     "bad_filter, expected_status_code, expected_detail",
     (
         (
             "salary_from__qt=100",
             HTTP_400_BAD_REQUEST,
             "Forbidden filter 'qt' for 'salary_from'"
```

### Comparing `fastapi-sa-orm-filter-0.1.2/PKG-INFO` & `fastapi-sa-orm-filter-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sa-orm-filter
-Version: 0.1.2
+Version: 0.1.3
 Summary: FastAPI-SQLAlchemy filter, transform request query string to SQLAlchemy orm query
 Author-email: Oleksandr Zhydyk <zhydykalex@ukr.net>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: fastapi
 Requires-Dist: sqlalchemy
@@ -15,15 +15,15 @@
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: aiosqlite ; extra == "test"
 Project-URL: Home, https://github.com/OleksandrZhydyk/FastAPI-SQLAlchemy-Filters
 Provides-Extra: formatting
 Provides-Extra: test
 
 ## FastAPI SQLAlchemy Filter 
-Package that helps to implement easy objects filter for applications
+Package that helps to implement easy objects filtering and sorting for applications
 build on FastAPI and SQLAlchemy.
 For using you just need to define your custom filter with filtered fields and applied operators.
 Supported operators, datatypes and example of work you can find below.
 
 ### Installation
 ```shell
 pip install fastapi-sa-orm-filter
@@ -40,62 +40,64 @@
 from db.base import get_session
 from db.models import MyModel
 
 
 app = FastAPI()
 
 # Define fields and operators for filter
-my_item_filter = {
-    'my_model_field_name': [fls.eq, fls.in_],
-    'my_model_field_name': [fls.between, fls.eq, fls.gt, fls.lt, fls.in_],
-    'my_model_field_name': [fls.like, fls.startswith, fls.contains, fls.in_],
-    'my_model_field_name': [fls.between, fls.not_eq, fls.gte, fls.lte]
+my_objects_filter = {
+    'my_model_field_name': [ops.eq, ops.in_],
+    'my_model_field_name': [ops.between, ops.eq, ops.gt, ops.lt, ops.in_],
+    'my_model_field_name': [ops.like, ops.startswith, ops.contains, ops.in_],
+    'my_model_field_name': [ops.between, ops.not_eq, ops.gte, ops.lte]
 }
 
 @app.get("/")
-async def get_filtered_items(
+async def get_filtered_objects(
     filter_query: str = Query(default=''),
     db: AsyncSession = Depends(get_session)
  ) -> List[MyModel]:
-    my_filter = FilterCore(MyModel, my_item_filter)
+    my_filter = FilterCore(MyModel, my_objects_filter)
     query = my_filter.get_query(filter_query)
     res = await db.execute(query)
     return res.scalars().all()
 ```
 
 ### Example of work
 
 ```shell
 
 # Input query string
 '''
 salary_from__in_=60,70,80&
 created_at__between=2023-05-01,2023-05-05|
-category__eq=Medicine"
+category__eq=Medicine&
+order_by=-id,category
 '''
 
    
 # Returned SQLAlchemy orm query exact as:
            
 select(model)
     .where(
         or_(
             and_(
                 model.salary_from.in_(60,70,80),
                 model.created_at.between(2023-05-01, 2023-05-05)
             ),
             model.category == 'Medicine'
-        )
+        ).order_by(model.id.desc(), model.category.asc())
 ```
 
 ### Supported query string format
 
 * field_name__eq=value
 * field_name__in_=value1,value2
 * field_name__eq=value&field_name__in_=value1,value2
+* field_name__eq=value&field_name__in_=value1,value2&order_by=-field_name
 
 ### Supported SQLAlchemy datatypes:
 * DATETIME
 * DATE
 * INTEGER
 * FLOAT
 * TEXT
@@ -118,7 +120,11 @@
 * __contains__
 * __icontains__
 * __not_eq__
 * __not_in__
 * __not_like__
 * __not_between__
 
+#### For suggestions and questions, feel free to contact me through email 
+__zhydykalex@ukr.net__
+
+
```

