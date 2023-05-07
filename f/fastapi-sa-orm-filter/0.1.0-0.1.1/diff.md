# Comparing `tmp/fastapi-sa-orm-filter-0.1.0.tar.gz` & `tmp/fastapi-sa-orm-filter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-sa-orm-filter-0.1.0.tar", last modified: Sun May  7 18:16:28 2023, max compression
+gzip compressed data, was "fastapi-sa-orm-filter-0.1.1.tar", last modified: Sun May  7 20:03:52 2023, max compression
```

## Comparing `fastapi-sa-orm-filter-0.1.0.tar` & `fastapi-sa-orm-filter-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      813 2023-05-07 17:56:59.474207 fastapi-sa-orm-filter-0.1.0/.github/workflows/ci_filter.yml
--rw-r--r--   0        0        0     1073 2023-05-07 07:37:25.294746 fastapi-sa-orm-filter-0.1.0/LICENSE
--rw-r--r--   0        0        0      271 2023-05-07 14:19:55.337103 fastapi-sa-orm-filter-0.1.0/Pipfile
--rw-r--r--   0        0        0    23646 2023-05-07 14:21:44.504856 fastapi-sa-orm-filter-0.1.0/Pipfile.lock
--rw-r--r--   0        0        0     2258 2023-05-07 18:15:27.331970 fastapi-sa-orm-filter-0.1.0/README.md
--rw-r--r--   0        0        0      111 2023-05-07 17:34:48.448358 fastapi-sa-orm-filter-0.1.0/fastapi_sa_orm_filter/__init__.py
--rw-r--r--   0        0        0      438 2023-05-07 17:35:28.765807 fastapi-sa-orm-filter-0.1.0/fastapi_sa_orm_filter/filters.py
--rw-r--r--   0        0        0     9211 2023-05-07 18:14:47.576231 fastapi-sa-orm-filter-0.1.0/fastapi_sa_orm_filter/main.py
--rw-r--r--   0        0        0      844 2023-05-07 18:13:40.160724 fastapi-sa-orm-filter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      143 2023-05-04 19:03:00.838038 fastapi-sa-orm-filter-0.1.0/pytest.ini
--rw-r--r--   0        0        0     3256 2023-05-07 18:14:47.572231 fastapi-sa-orm-filter-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0    11004 2023-05-07 10:53:36.010316 fastapi-sa-orm-filter-0.1.0/tests/test_filter.py
--rw-r--r--   0        0        0      323 2023-05-05 21:57:39.693231 fastapi-sa-orm-filter-0.1.0/tests/utils.py
--rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 fastapi-sa-orm-filter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-05-07 17:56:59.474207 fastapi-sa-orm-filter-0.1.1/.github/workflows/ci_filter.yml
+-rw-r--r--   0        0        0     1073 2023-05-07 07:37:25.294746 fastapi-sa-orm-filter-0.1.1/LICENSE
+-rw-r--r--   0        0        0      271 2023-05-07 14:19:55.337103 fastapi-sa-orm-filter-0.1.1/Pipfile
+-rw-r--r--   0        0        0    23646 2023-05-07 14:21:44.504856 fastapi-sa-orm-filter-0.1.1/Pipfile.lock
+-rw-r--r--   0        0        0     2254 2023-05-07 18:27:00.869658 fastapi-sa-orm-filter-0.1.1/README.md
+-rw-r--r--   0        0        0      111 2023-05-07 20:03:40.110270 fastapi-sa-orm-filter-0.1.1/fastapi_sa_orm_filter/__init__.py
+-rw-r--r--   0        0        0      436 2023-05-07 19:08:56.172612 fastapi-sa-orm-filter-0.1.1/fastapi_sa_orm_filter/filters.py
+-rw-r--r--   0        0        0     9002 2023-05-07 19:44:59.724445 fastapi-sa-orm-filter-0.1.1/fastapi_sa_orm_filter/main.py
+-rw-r--r--   0        0        0      844 2023-05-07 18:13:40.160724 fastapi-sa-orm-filter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      143 2023-05-04 19:03:00.838038 fastapi-sa-orm-filter-0.1.1/pytest.ini
+-rw-r--r--   0        0        0     3313 2023-05-07 19:52:51.662374 fastapi-sa-orm-filter-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0    14318 2023-05-07 19:52:51.678374 fastapi-sa-orm-filter-0.1.1/tests/test_filter.py
+-rw-r--r--   0        0        0      323 2023-05-05 21:57:39.693231 fastapi-sa-orm-filter-0.1.1/tests/utils.py
+-rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 fastapi-sa-orm-filter-0.1.1/PKG-INFO
```

### Comparing `fastapi-sa-orm-filter-0.1.0/.github/workflows/ci_filter.yml` & `fastapi-sa-orm-filter-0.1.1/.github/workflows/ci_filter.yml`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.0/LICENSE` & `fastapi-sa-orm-filter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.0/Pipfile.lock` & `fastapi-sa-orm-filter-0.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.0/README.md` & `fastapi-sa-orm-filter-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
            
 select(model)
     .where(
         or_(
             and_(
                 model.salary_from.in_(60,70,80),
                 model.created_at.between(2023-05-01, 2023-05-05)
-                ),
+            ),
             model.category == 'Medicine'
         )
 ```
 
 ### Supported query string format
 
 * field_name__eq=value
```

### Comparing `fastapi-sa-orm-filter-0.1.0/fastapi_sa_orm_filter/main.py` & `fastapi-sa-orm-filter-0.1.1/fastapi_sa_orm_filter/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from datetime import datetime
-from typing import Any, Dict, List, Tuple, Optional, Union
+from typing import Any, Dict, List, Tuple, Optional, Union, Type
 
 import pydantic
 from fastapi import HTTPException
 from pydantic import create_model
 from pydantic.main import ModelMetaclass
 from pydantic_sqlalchemy import sqlalchemy_to_pydantic
 from sqlalchemy import select
@@ -21,72 +21,65 @@
 class FilterCore:
     """
     Class serves of SQLAlchemy orm query creation.
     Convert parsed query data to python data types and form SQLAlchemy query.
     """
 
     def __init__(
-        self, model: DeclarativeMeta, allowed_filters: Dict[str, List[fls]]
+        self, model: Type[DeclarativeMeta], allowed_filters: Dict[str, List[fls]]
     ) -> None:
         """
         Produce a class:`FilterCore` object against a function
 
         :param model: declared SQLAlchemy db model
         :param allowed_filters: dict with allowed model fields and operators
             for filter, like:
                 {
                     'field_name': [startswith, eq, in_],
                     'field_name': [contains, like]
                 }
         """
-        self.model = model
-        self.allowed_filters = allowed_filters
-        self.model_serializer = self._create_pydantic_serializer()
+        self._model = model
+        self._allowed_filters = allowed_filters
+        self._model_serializer = self._create_pydantic_serializer()
 
     def get_query(self, custom_filter: str) -> Select:
         """
         Construct the SQLAlchemy orm query from request query string
 
-        >>> get_query(
-        >>>    'salary_from__in_=60,70,80&'
-        >>>    'created_at__between=2023-05-01,2023-05-05|'
-        >>>    'category__eq=Medicine'
-        >>>    )
-
-
         :param custom_filter: request query string with fields and filter conditions
             'salary_from__in_=60,70,80&
              created_at__between=2023-05-01,2023-05-05|
              category__eq=Medicine'
         :return:
             select(model)
                 .where(
                     or_(
                         and_(
                             model.salary_from.in_(60,70,80),
                             model.created_at.between(2023-05-01, 2023-05-05)
-                            ),
+                        ),
                         model.category == 'Medicine'
                     )
         """
         if not custom_filter:
-            query = select(self.model)
+            query = select(self._model)
             return query
         conditions = []
-        query_parser = QueryParser(custom_filter, self.model, self.allowed_filters)
+        query_parser = QueryParser(custom_filter, self._model, self._allowed_filters)
         for and_expressions in query_parser.get_parsed_query():
             and_condition = []
             for expression in and_expressions:
                 column, operator, value = expression
                 serialized_dict = self._format_expression(column, operator, value)
                 value = serialized_dict[column.name]
                 param = self._get_orm_for_field(column, operator, value)
                 and_condition.append(param)
             conditions.append(and_(*and_condition))
-        query = select(self.model).filter(or_(*conditions))
+        query = select(self._model).filter(or_(*conditions))
         return query
 
     def _create_pydantic_serializer(self) -> Dict[str, ModelMetaclass]:
         """
         Create two pydantic models (optional and list field types)
         for value: str serialization
 
@@ -95,24 +88,24 @@
                 class model.__name__(BaseModel):
                     field: Optional[type]
             'list_model':
                 class model.__name__(BaseModel):
                     field: List[type]
         }
         """
-        pydantic_serializer = sqlalchemy_to_pydantic(self.model)
+        pydantic_serializer = sqlalchemy_to_pydantic(self._model)
         fields_to_optional = {
             f.name: (f.type_, None) for f in pydantic_serializer.__fields__.values()
         }
         fields_wrap_to_list = {
             f.name: (List[f.type_], None)
             for f in pydantic_serializer.__fields__.values()
         }
-        optional_model = create_model(self.model.__name__, **fields_to_optional)
-        list_model = create_model(self.model.__name__, **fields_wrap_to_list)
+        optional_model = create_model(self._model.__name__, **fields_to_optional)
+        list_model = create_model(self._model.__name__, **fields_wrap_to_list)
         return {"optional_model": optional_model, "list_model": list_model}
 
     @staticmethod
     def _get_orm_for_field(
         column: InstrumentedAttribute, operator: str, value: Any
     ) -> BinaryExpression:
         """
@@ -137,26 +130,25 @@
         value = value.split(",")
         try:
             if isinstance(column.type, DateTime):
                 value = [
                     datetime.strptime(date_str, "%Y-%m-%d %H:%M:%S")
                     for date_str in value
                 ]
-            elif isinstance(column.type, Date):
+            if isinstance(column.type, Date):
                 value = [
                     datetime.strptime(date_str, "%Y-%m-%d").date() for date_str in value
                 ]
-            else:
-                if operator not in [fls.between, fls.in_]:
-                    value = value[0]
-                    serialized_dict = self.model_serializer["optional_model"](
-                        **{column.name: value}
-                    ).dict(exclude_none=True)
-                    return serialized_dict
-            serialized_dict = self.model_serializer["list_model"](
+            if operator not in [fls.between, fls.in_]:
+                value = value[0]
+                serialized_dict = self._model_serializer["optional_model"](
+                    **{column.name: value}
+                ).dict(exclude_none=True)
+                return serialized_dict
+            serialized_dict = self._model_serializer["list_model"](
                 **{column.name: value}
             ).dict(exclude_none=True)
             return serialized_dict
         except pydantic.ValidationError as e:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST, detail=json.loads(e.json())
             )
```

### Comparing `fastapi-sa-orm-filter-0.1.0/pyproject.toml` & `fastapi-sa-orm-filter-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.0/tests/conftest.py` & `fastapi-sa-orm-filter-0.1.1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,19 +89,20 @@
     session.add_all(vacancy_instances)
     await session.commit()
 
 
 @pytest.fixture
 def get_custom_restriction():
     return {
-        'title': [fls.startswith, fls.eq, fls.in_],
+        'title': [fls.startswith, fls.eq, fls.endswith],
         'category': [fls.startswith, fls.eq, fls.in_],
-        'salary_from': [fls.between, fls.eq, fls.gt, fls.lt, fls.in_],
+        'salary_from': [fls.between, fls.eq, fls.gt, fls.lt, fls.in_, fls.gte],
         'description': [fls.like, fls.not_like, fls.contains, fls.eq, fls.in_],
-        'created_at': [fls.between, fls.in_, fls.eq, fls.gt, fls.lt],
-        'updated_at': [fls.between, fls.in_, fls.eq, fls.gt, fls.lt]
+        'created_at': [fls.between, fls.in_, fls.eq, fls.gt, fls.lt, fls.not_eq],
+        'updated_at': [fls.between, fls.in_, fls.eq, fls.gt, fls.lt],
+        'is_active': [fls.eq]
     }
 
 
 @pytest.fixture
 def get_filter(get_custom_restriction):
     return FilterCore(Vacancy, get_custom_restriction)
```

### Comparing `fastapi-sa-orm-filter-0.1.0/tests/test_filter.py` & `fastapi-sa-orm-filter-0.1.1/tests/test_filter.py`

 * *Files 15% similar despite different names*

```diff
@@ -75,14 +75,35 @@
         'is_active': True,
         'salary_from': 150,
         'salary_up_to': 200,
         'category': JobCategory.miscellaneous
     }
 
 
+async def test_endswith_with_str(session, get_filter, create_vacancies):
+    query = get_filter.get_query("title__endswith=le1")
+    res = await session.execute(query)
+    data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
+    assert len(data['vacancies']) == 1
+    assert isinstance(data['vacancies'][0]["created_at"], date)
+    assert isinstance(data['vacancies'][0]["updated_at"], datetime)
+    check_data = data['vacancies'][0].copy()
+    del check_data['created_at']
+    del check_data['updated_at']
+    assert check_data == {
+        'id': 1,
+        'title': 'title1',
+        'description': 'description1',
+        'is_active': True,
+        'salary_from': 60,
+        'salary_up_to': 110,
+        'category': JobCategory.finance
+    }
+
+
 async def test_in_with_int(session, get_filter, create_vacancies):
     query = get_filter.get_query("salary_from__in_=60,70,80")
     res = await session.execute(query)
     data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
     assert len(data['vacancies']) == 3
     assert isinstance(data['vacancies'][0]["created_at"], date)
     assert isinstance(data['vacancies'][0]["updated_at"], datetime)
@@ -96,14 +117,77 @@
         'is_active': True,
         'salary_from': 60,
         'salary_up_to': 110,
         'category': JobCategory.finance
     }
 
 
+async def test_gte_with_int(session, get_filter, create_vacancies):
+    query = get_filter.get_query("salary_from__gte=120")
+    res = await session.execute(query)
+    data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
+    assert len(data['vacancies']) == 4
+    assert isinstance(data['vacancies'][0]["created_at"], date)
+    assert isinstance(data['vacancies'][0]["updated_at"], datetime)
+    check_data = data['vacancies'][0].copy()
+    del check_data['created_at']
+    del check_data['updated_at']
+    assert check_data == {
+        'id': 7,
+        'title': 'title7',
+        'description': 'description7',
+        'is_active': True,
+        'salary_from': 120,
+        'salary_up_to': 170,
+        'category': JobCategory.construction
+    }
+
+
+async def test_not_eq_with_date(session, get_filter, create_vacancies):
+    query = get_filter.get_query("created_at__not_eq=2023-05-01")
+    res = await session.execute(query)
+    data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
+    assert len(data['vacancies']) == 9
+    assert isinstance(data['vacancies'][0]["created_at"], date)
+    assert isinstance(data['vacancies'][0]["updated_at"], datetime)
+    check_data = data['vacancies'][0].copy()
+    del check_data['created_at']
+    del check_data['updated_at']
+    assert check_data == {
+        'id': 2,
+        'title': 'title2',
+        'description': 'description2',
+        'is_active': True,
+        'salary_from': 70,
+        'salary_up_to': 120,
+        'category': JobCategory.marketing
+    }
+
+
+async def test_eq_with_bool(session, get_filter, create_vacancies):
+    query = get_filter.get_query("is_active__eq=true")
+    res = await session.execute(query)
+    data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
+    assert len(data['vacancies']) == 10
+    assert isinstance(data['vacancies'][0]["created_at"], date)
+    assert isinstance(data['vacancies'][0]["updated_at"], datetime)
+    check_data = data['vacancies'][0].copy()
+    del check_data['created_at']
+    del check_data['updated_at']
+    assert check_data == {
+        'id': 1,
+        'title': 'title1',
+        'description': 'description1',
+        'is_active': True,
+        'salary_from': 60,
+        'salary_up_to': 110,
+        'category': JobCategory.finance
+    }
+
+
 async def test_between_with_int(session, get_filter, create_vacancies):
     query = get_filter.get_query("salary_from__between=50,90")
     res = await session.execute(query)
     data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
     assert len(data['vacancies']) == 4
     assert isinstance(data['vacancies'][0]["created_at"], date)
     assert isinstance(data['vacancies'][0]["updated_at"], datetime)
@@ -159,15 +243,15 @@
         'is_active': True,
         'salary_from': 100,
         'salary_up_to': 150,
         'category': JobCategory.metallurgy
     }
 
 
-async def test_qt_with_int(session, get_filter, create_vacancies):
+async def test_gt_with_int(session, get_filter, create_vacancies):
     query = get_filter.get_query("salary_from__gt=100")
     res = await session.execute(query)
     data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
     assert len(data['vacancies']) == 5
     assert isinstance(data['vacancies'][0]["created_at"], date)
     assert isinstance(data['vacancies'][0]["updated_at"], datetime)
     check_data = data['vacancies'][0].copy()
@@ -295,15 +379,24 @@
         (
             "created_at__between=2023-05-01,2023-05-05"
             "updated_at__in_=2023-01-05 15:15:15,2023-05-05 15:15:15|"
             "salary_from__gt=100",
             HTTP_400_BAD_REQUEST,
             "Incorrect filter request syntax, "
             "please use pattern :'{field_name}__{condition}={value}{conjunction}'"
-        )
+        ),
+        (
+            "is_active__eq=100",
+            HTTP_400_BAD_REQUEST,
+            [
+                {'loc': ['is_active'],
+                 'msg': 'value could not be parsed to a boolean',
+                 'type': 'type_error.bool'}
+            ]
+        ),
     )
 )
 def test_fail_filter(get_filter, bad_filter, expected_status_code, expected_detail):
     with pytest.raises(Exception) as e:
         get_filter.get_query(bad_filter)
     assert e.type == HTTPException
     assert e.value.status_code == expected_status_code
```

### Comparing `fastapi-sa-orm-filter-0.1.0/PKG-INFO` & `fastapi-sa-orm-filter-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sa-orm-filter
-Version: 0.1.0
+Version: 0.1.1
 Summary: FastAPI-SQLAlchemy filter, transform request query string to SQLAlchemy orm query
 Author-email: Oleksandr Zhydyk <zhydykalex@ukr.net>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: fastapi
 Requires-Dist: sqlalchemy
@@ -78,15 +78,15 @@
            
 select(model)
     .where(
         or_(
             and_(
                 model.salary_from.in_(60,70,80),
                 model.created_at.between(2023-05-01, 2023-05-05)
-                ),
+            ),
             model.category == 'Medicine'
         )
 ```
 
 ### Supported query string format
 
 * field_name__eq=value
```

