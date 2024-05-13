# Comparing `tmp/pysql-repo-0.6.2.tar.gz` & `tmp/pysql-repo-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysql-repo-0.6.2.tar", last modified: Fri Apr 26 10:21:27 2024, max compression
+gzip compressed data, was "pysql-repo-0.6.3.tar", last modified: Mon May 13 09:43:10 2024, max compression
```

## Comparing `pysql-repo-0.6.2.tar` & `pysql-repo-0.6.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:27.370859 pysql-repo-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-04-26 10:21:27.370859 pysql-repo-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    40736 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:27.366859 pysql-repo-0.6.2/pysql_repo/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:27.370859 pysql-repo-0.6.2/pysql_repo/_constants/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/_constants/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/_database_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    18597 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:27.370859 pysql-repo-0.6.2/pysql_repo/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/asyncio/async_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/asyncio/async_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/asyncio/async_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/asyncio/async_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:27.370859 pysql-repo-0.6.2/pysql_repo/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-26 10:21:22.000000 pysql-repo-0.6.2/pysql_repo/libs/file_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:27.370859 pysql-repo-0.6.2/pysql_repo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-04-26 10:21:27.000000 pysql-repo-0.6.2/pysql_repo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-26 10:21:27.000000 pysql-repo-0.6.2/pysql_repo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:21:27.000000 pysql-repo-0.6.2/pysql_repo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 10:21:27.000000 pysql-repo-0.6.2/pysql_repo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 10:21:27.000000 pysql-repo-0.6.2/pysql_repo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:21:27.370859 pysql-repo-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-26 10:21:26.000000 pysql-repo-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    40736 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/pysql_repo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/pysql_repo/_constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_constants/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_database_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18596 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22801 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/pysql_repo/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/asyncio/async_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/asyncio/async_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19428 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/asyncio/async_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/asyncio/async_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/pysql_repo/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-13 09:43:06.000000 pysql-repo-0.6.3/pysql_repo/libs/file_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/pysql_repo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41337 2024-05-13 09:43:10.000000 pysql-repo-0.6.3/pysql_repo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-13 09:43:10.000000 pysql-repo-0.6.3/pysql_repo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:43:10.000000 pysql-repo-0.6.3/pysql_repo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 09:43:10.000000 pysql-repo-0.6.3/pysql_repo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 09:43:10.000000 pysql-repo-0.6.3/pysql_repo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:43:10.645035 pysql-repo-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-13 09:43:09.000000 pysql-repo-0.6.3/setup.py
```

### Comparing `pysql-repo-0.6.2/PKG-INFO` & `pysql-repo-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysql-repo
-Version: 0.6.2
+Version: 0.6.3
 Summary: A project to have a base repository class to perform select/insert/update/delete with dynamic syntax
 Home-page: https://github.com/Impro02/pysql-repo
-Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.6.2.tar.gz
+Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.6.3.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysql-repo-0.6.2/README.md` & `pysql-repo-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.2/pysql_repo/__init__.py` & `pysql-repo-0.6.3/pysql_repo/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sqlalchemy import Engine, event
 
 # PYSQL_REPO
 from pysql_repo._database import DataBase
 from pysql_repo._decorators import with_session
 from pysql_repo._repository import Repository
 from pysql_repo._service import Service
-from pysql_repo._utils import RelationshipOption
+from pysql_repo._utils import RelationshipOption, FilterType
 from pysql_repo._constants.enum import Operators, LoadingTechnique
 
 
 logging.basicConfig()
 _logger = logging.getLogger("pysql_repo.cursor")
 _logger.setLevel(logging.INFO)
```

### Comparing `pysql-repo-0.6.2/pysql_repo/_constants/enum.py` & `pysql-repo-0.6.3/pysql_repo/_constants/enum.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.2/pysql_repo/_database.py` & `pysql-repo-0.6.3/pysql_repo/_database.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.2/pysql_repo/_database_base.py` & `pysql-repo-0.6.3/pysql_repo/_database_base.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.2/pysql_repo/_decorators.py` & `pysql-repo-0.6.3/pysql_repo/_decorators.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.2/pysql_repo/_repository.py` & `pysql-repo-0.6.3/pysql_repo/asyncio/async_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,43 +9,45 @@
     Type,
     TypeVar,
     Union,
     Sequence,
 )
 
 # CONTEXTLIB
-from contextlib import AbstractContextManager
+from contextlib import AbstractAsyncContextManager
 
 # SQLALCHEMY
 from sqlalchemy import ColumnExpressionArgument, Select
+from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import Session, InstrumentedAttribute
+from sqlalchemy.orm import InstrumentedAttribute
 
 # DECORATORS
-from pysql_repo._decorators import check_values as _check_values, with_session
+from pysql_repo._decorators import check_values as _check_values
+from pysql_repo.asyncio.async_decorator import with_async_session
 
 # UTILS
 from pysql_repo._utils import (
-    _FilterType,
+    FilterType,
     RelationshipOption,
+    async_apply_pagination as _async_apply_pagination,
     build_delete_stmt as _build_delete_stmt,
     build_insert_stmt as _build_insert_stmt,
     build_select_stmt as _build_select_stmt,
     build_update_stmt as _build_update_stmt,
     select_distinct as _select_distinct,
-    apply_pagination as _apply_pagination,
 )
 
 
 _T = TypeVar("_T", bound=declarative_base())
 
 
-class Repository:
+class AsyncRepository:
     """
-    Represents a repository for database operations.
+    Represents an asynchronous repository for database operations.
 
     Attributes:
         _session_factory: The session factory used for creating sessions.
 
     Methods:
         session_manager: Returns the session factory.
         _select: Selects a single row from the database.
@@ -54,126 +56,130 @@
         _select_all_stmt: Selects all rows from the database using a custom statement.
         _select_paginate: Selects a paginated set of rows from the database.
         _select_paginate_stmt: Selects a paginated set of rows from the database using a custom statement.
     """
 
     def __init__(
         self,
-        session_factory: Callable[..., AbstractContextManager[Session]],
+        session_factory: Callable[..., AbstractAsyncContextManager[AsyncSession]],
     ) -> None:
         """
-        Initializes the Repository.
+        Initializes the AsyncRepository.
 
         Args:
-            session_factory: A callable that returns a context manager
+            session_factory: A callable that returns an asynchronous context manager
                              for creating and managing database sessions.
 
         Returns:
             None
         """
         self._session_factory = session_factory
 
-    def session_manager(self) -> AbstractContextManager[Session]:
+    def session_manager(self) -> AbstractAsyncContextManager[AsyncSession]:
         """
         Get a session manager.
 
         Returns:
-            AbstractContextManager[Session]: An context manager for managing database sessions.
+            AbstractAsyncContextManager[AsyncSession]: An asynchronous context manager for managing database sessions.
         """
         return self._session_factory()
 
-    @with_session()
-    def _select(
+    @with_async_session()
+    async def _select(
         self,
         model: Type[_T],
         distinct: Optional[ColumnExpressionArgument] = None,
-        filters: Optional[_FilterType] = None,
-        optional_filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
+        optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
             Dict[InstrumentedAttribute, RelationshipOption]
         ] = None,
-        session: Optional[Session] = None,
+        session: Optional[AsyncSession] = None,
     ) -> Optional[_T]:
         """
         Selects a single object from the database.
 
         Args:
             model: The model class representing the table.
             distinct: The distinct column expression.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
-            session: The session to use.
+            The selected object or None if not found.
 
         Returns:
-            The selected object or None if not found.
+            The selected row.
+
         """
         stmt = _select_distinct(
             model=model,
             expr=distinct,
         )
 
-        return self._select_stmt(
+        return await self._select_stmt(
             stmt=stmt,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             session=session,
         )
 
-    @with_session()
-    def _select_stmt(
+    @with_async_session()
+    async def _select_stmt(
         self,
         stmt: Select[Tuple[_T]],
-        filters: Optional[_FilterType] = None,
-        optional_filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
+        optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
             Dict[InstrumentedAttribute, RelationshipOption]
         ] = None,
         group_by: Optional[ColumnExpressionArgument] = None,
-        session: Optional[Session] = None,
+        session: Optional[AsyncSession] = None,
     ) -> Optional[_T]:
         """
         Selects a single object from the database using a custom statement.
 
         Args:
             stmt: The custom select statement.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
             group_by: The column expression to group by.
             session: The session to use.
 
         Returns:
             The selected object or None if not found.
+
         """
         stmt = _build_select_stmt(
             stmt=stmt,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             group_by=group_by,
         )
 
-        return session.execute(stmt).unique().scalar_one_or_none()
+        result = await session.execute(stmt)
+
+        return result.unique().scalar_one_or_none()
 
-    @with_session()
-    def _select_all(
+    @with_async_session()
+    async def _select_all(
         self,
         model: Type[_T],
         distinct: Optional[List[ColumnExpressionArgument]] = None,
-        filters: Optional[_FilterType] = None,
-        optional_filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
+        optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
             Dict[InstrumentedAttribute, RelationshipOption]
         ] = None,
         order_by: Optional[Union[List[str], str]] = None,
-        direction: Optional[str] = None,
+        direction: Optional[Union[List[str], str]] = None,
         limit: int = None,
-        session: Optional[Session] = None,
+        session: Optional[AsyncSession] = None,
     ) -> Sequence[_T]:
         """
         Selects all objects from the database.
 
         Args:
             model: The model class representing the table.
             distinct: The distinct column expressions.
@@ -183,47 +189,48 @@
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of objects to return.
             session: The session to use.
 
         Returns:
             A sequence of selected objects.
+
         """
         stmt = _select_distinct(
             model=model,
             expr=distinct,
         )
 
-        return self._select_all_stmt(
+        return await self._select_all_stmt(
             stmt=stmt,
             model=model,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             order_by=order_by,
             direction=direction,
             limit=limit,
             session=session,
         )
 
-    @with_session()
-    def _select_all_stmt(
+    @with_async_session()
+    async def _select_all_stmt(
         self,
         stmt: Select[Tuple[_T]],
         model: Type[_T],
-        filters: Optional[_FilterType] = None,
-        optional_filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
+        optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
             Dict[InstrumentedAttribute, RelationshipOption]
         ] = None,
         group_by: Optional[ColumnExpressionArgument] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[Union[List[str], str]] = None,
         limit: int = None,
-        session: Optional[Session] = None,
+        session: Optional[AsyncSession] = None,
     ) -> Sequence[_T]:
         """
         Selects all objects from the database using a custom statement.
 
         Args:
             stmt: The custom select statement.
             model: The model class representing the table.
@@ -234,45 +241,48 @@
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of rows to return.
             session: The session to use.
 
         Returns:
             A sequence of selected objects.
+
         """
         stmt = _build_select_stmt(
             stmt=stmt,
             model=model,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             group_by=group_by,
             order_by=order_by,
             direction=direction,
             limit=limit,
         )
 
-        return session.execute(stmt).unique().scalars().all()
+        result = await session.execute(stmt)
 
-    @with_session()
-    def _select_paginate(
+        return result.unique().scalars().all()
+
+    @with_async_session()
+    async def _select_paginate(
         self,
         model: Type[_T],
         page: int,
         per_page: int,
         distinct: Optional[ColumnExpressionArgument] = None,
-        filters: Optional[_FilterType] = None,
-        optional_filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
+        optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
             Dict[InstrumentedAttribute, RelationshipOption]
         ] = None,
         order_by: Optional[Union[List[str], str]] = None,
-        direction: Optional[str] = None,
+        direction: Optional[Union[List[str], str]] = None,
         limit: int = None,
-        session: Optional[Session] = None,
+        session: Optional[AsyncSession] = None,
     ) -> Tuple[Sequence[_T], str]:
         """
         Selects a paginated set of objects from the database.
 
         Args:
             model: The model class representing the table.
             page: The page number.
@@ -284,51 +294,52 @@
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of objects to return.
             session: The session to use.
 
         Returns:
             A tuple containing the selected objects and pagination information.
+
         """
         stmt = _select_distinct(
             model=model,
             expr=distinct,
         )
 
-        return self._select_paginate_stmt(
+        return await self._select_paginate_stmt(
             stmt=stmt,
             model=model,
             page=page,
             per_page=per_page,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             order_by=order_by,
             direction=direction,
             limit=limit,
             session=session,
         )
 
-    @with_session()
-    def _select_paginate_stmt(
+    @with_async_session()
+    async def _select_paginate_stmt(
         self,
         stmt: Select[Tuple[_T]],
         model: Type[_T],
         page: int,
         per_page: int,
-        filters: Optional[_FilterType] = None,
-        optional_filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
+        optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
             Dict[InstrumentedAttribute, RelationshipOption]
         ] = None,
         group_by: Optional[ColumnExpressionArgument] = None,
         order_by: Optional[Union[List[str], str]] = None,
-        direction: Optional[str] = None,
+        direction: Optional[Union[List[str], str]] = None,
         limit: int = None,
-        session: Optional[Session] = None,
+        session: Optional[AsyncSession] = None,
     ) -> Tuple[Sequence[_T], str]:
         """
         Selects a paginated set of rows from the database using a custom statement.
 
         Args:
             stmt: The custom select statement.
             model: The model class representing the table.
@@ -341,46 +352,49 @@
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of rows to return.
             session: The session to use.
 
         Returns:
             A tuple containing the selected objects and pagination information.
+
         """
         stmt = _build_select_stmt(
             stmt=stmt,
             model=model,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             group_by=group_by,
             order_by=order_by,
             direction=direction,
             limit=limit,
         )
 
-        stmt, pagination = _apply_pagination(
+        stmt, pagination = await _async_apply_pagination(
             session=session,
             stmt=stmt,
             page=page,
             per_page=per_page,
         )
 
-        return session.execute(stmt).unique().scalars().all(), pagination
+        result = await session.execute(stmt)
+
+        return result.unique().scalars().all(), pagination
 
     @_check_values(as_list=False)
-    @with_session()
-    def _update_all(
+    @with_async_session()
+    async def _update_all(
         self,
         model: Type[_T],
         values: Dict[str, Any],
-        filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
         flush: bool = False,
         commit: bool = False,
-        session: Optional[Session] = None,
+        session: Optional[AsyncSession] = None,
     ) -> Sequence[_T]:
         """
         Updates multiple objects in the database.
 
         Args:
             model: The model class representing the table.
             values: A dictionary of column-value pairs to update.
@@ -394,35 +408,37 @@
         """
         stmt = _build_update_stmt(
             model=model,
             values=values,
             filters=filters,
         )
 
-        sequence = session.execute(stmt).unique().scalars().all()
+        result = await session.execute(stmt)
+
+        sequence = result.unique().scalars().all()
 
         if flush:
-            session.flush()
+            await session.flush()
         if commit:
-            session.commit()
+            await session.commit()
 
-        [session.refresh(item) for item in sequence]
+        [await session.refresh(item) for item in sequence]
 
         return sequence
 
     @_check_values(as_list=False)
-    @with_session()
-    def _update(
+    @with_async_session()
+    async def _update(
         self,
         model: Type[_T],
         values: Dict[str, Any],
-        filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
         flush: bool = False,
         commit: bool = False,
-        session: Optional[Session] = None,
+        session: Optional[AsyncSession] = None,
     ) -> Optional[_T]:
         """
         Updates a single object in the database.
 
         Args:
             model: The model class representing the table.
             values: A dictionary of column-value pairs to update.
@@ -436,37 +452,39 @@
         """
         stmt = _build_update_stmt(
             model=model,
             values=values,
             filters=filters,
         )
 
-        item = session.execute(stmt).unique().scalar_one_or_none()
+        result = await session.execute(stmt)
+
+        item = result.unique().scalar_one_or_none()
 
         if item is None:
             return None
 
         if flush:
-            session.flush()
+            await session.flush()
         if commit:
-            session.commit()
+            await session.commit()
 
-        session.refresh(item)
+        await session.refresh(item)
 
         return item
 
     @_check_values(as_list=True)
-    @with_session()
-    def _add_all(
+    @with_async_session()
+    async def _add_all(
         self,
         model: Type[_T],
         values: List[Dict[str, Any]],
         flush: bool = False,
         commit: bool = False,
-        session: Optional[Session] = None,
+        session: Optional[AsyncSession] = None,
     ) -> Sequence[_T]:
         """
         Adds multiple objects to the database.
 
         Args:
             model: The model class representing the table.
             values: A list of dictionaries containing column-value pairs for each object.
@@ -475,71 +493,76 @@
             session: The session to use.
 
         Returns:
             A sequence of added objects.
         """
         stmt = _build_insert_stmt(model=model)
 
-        sequence = session.execute(stmt, values).unique().scalars().all()
+        result = await session.execute(stmt, values)
+
+        sequence = result.unique().scalars().all()
 
         if flush:
-            session.flush()
+            await session.flush()
         if commit:
-            session.commit()
+            await session.commit()
 
         if flush or commit:
-            [session.refresh(item) for item in sequence]
+            [await session.refresh(item) for item in sequence]
 
         return sequence
 
     @_check_values(as_list=False)
-    @with_session()
-    def _add(
+    @with_async_session()
+    async def _add(
         self,
         model: Type[_T],
         values: Dict[str, Any],
         flush: bool = False,
         commit: bool = False,
-        session: Optional[Session] = None,
+        session: Optional[AsyncSession] = None,
     ) -> _T:
         """
         Adds a single object to the database.
 
         Args:
             model: The model class representing the table.
             values: A dictionary of column-value pairs for the object.
             flush: Whether to flush the session after adding the object.
             commit: Whether to commit the session after adding the object.
             session: The session to use.
 
         Returns:
             The added object.
+
         """
         stmt = _build_insert_stmt(model=model)
 
-        item = session.execute(stmt, values).unique().scalar_one()
+        result = await session.execute(stmt, values)
+
+        item = result.unique().scalar_one()
 
         if flush:
-            session.flush()
+            await session.flush()
         if commit:
-            session.commit()
+            await session.commit()
 
         if flush or commit:
-            session.refresh(item)
+            await session.refresh(item)
 
         return item
 
-    @with_session()
-    def _delete_all(
+    @with_async_session()
+    async def _delete_all(
         self,
         model: Type[_T],
-        filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
         flush: bool = True,
         commit: bool = False,
-        session: Optional[Session] = None,
+        session: Optional[AsyncSession] = None,
     ) -> bool:
         """
         Deletes multiple objects from the database.
 
         Args:
             model: The model class representing the table.
             filters: The filters to apply.
@@ -551,34 +574,36 @@
             True if any objects were deleted, False otherwise.
         """
         stmt = _build_delete_stmt(
             model=model,
             filters=filters,
         )
 
-        sequence = session.execute(stmt).unique().scalars().all()
+        result = await session.execute(stmt)
+
+        sequence = result.unique().scalars().all()
 
         if len(sequence) == 0:
             return False
 
         if flush:
-            session.flush()
+            await session.flush()
         if commit:
-            session.commit()
+            await session.commit()
 
         return True
 
-    @with_session()
-    def _delete(
+    @with_async_session()
+    async def _delete(
         self,
         model: Type[_T],
-        filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
         flush: bool = True,
         commit: bool = False,
-        session: Optional[Session] = None,
+        session: Optional[AsyncSession] = None,
     ) -> bool:
         """
         Deletes a single object from the database.
 
         Args:
             model: The model class representing the table.
             filters: The filters to apply.
@@ -590,18 +615,20 @@
             True if the object was deleted, False otherwise.
         """
         stmt = _build_delete_stmt(
             model=model,
             filters=filters,
         )
 
-        item = session.execute(stmt).unique().scalar_one_or_none()
+        result = await session.execute(stmt)
+
+        item = result.unique().scalar_one_or_none()
 
         if item is None:
             return False
 
         if flush:
-            session.flush()
+            await session.flush()
         if commit:
-            session.commit()
+            await session.commit()
 
         return True
```

### Comparing `pysql-repo-0.6.2/pysql_repo/_service.py` & `pysql-repo-0.6.3/pysql_repo/_service.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.2/pysql_repo/_utils.py` & `pysql-repo-0.6.3/pysql_repo/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     Dict,
     Iterable,
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
+    TypeAlias,
     Union,
 )
 
 # SQLALCHEMY
 from sqlalchemy import (
     ColumnExpressionArgument,
     Select,
@@ -27,35 +28,40 @@
     select,
     distinct,
     tuple_,
     func,
     update,
 )
 from sqlalchemy.ext.asyncio import AsyncSession
-from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import (
     Session,
     noload,
     lazyload,
     joinedload,
     subqueryload,
     selectinload,
     raiseload,
     contains_eager,
+    declarative_base,
 )
 from sqlalchemy.orm.attributes import InstrumentedAttribute
 from sqlalchemy.sql.dml import ReturningDelete, ReturningInsert, ReturningUpdate
 from sqlalchemy.sql.elements import Null, BinaryExpression
 
 # Enum
 from pysql_repo._constants.enum import LoadingTechnique, Operators
 
-_FilterType = Dict[Union[InstrumentedAttribute, Tuple[InstrumentedAttribute]], Any]
+FilterType: TypeAlias = Dict[
+    Union[InstrumentedAttribute, Tuple[InstrumentedAttribute]], Any
+]
 
-_T = TypeVar("_T", bound=declarative_base())
+_Base = declarative_base()
+
+
+_T = TypeVar("_T", bound=_Base)
 
 
 @dataclass
 class RelationshipOption:
     """
     Represents options for a relationship between two entities.
 
@@ -69,23 +75,23 @@
     added_criteria: Optional[BinaryExpression] = field(default=None)
     children: Dict[InstrumentedAttribute, "RelationshipOption"] = field(default=None)
 
 
 def build_select_stmt(
     stmt: Select[Tuple[_T]],
     model: Optional[Type[_T]] = None,
-    filters: Optional[_FilterType] = None,
-    optional_filters: Optional[_FilterType] = None,
+    filters: Optional[FilterType] = None,
+    optional_filters: Optional[FilterType] = None,
     relationship_options: Optional[
         Dict[InstrumentedAttribute, RelationshipOption]
     ] = None,
     group_by: Optional[ColumnExpressionArgument] = None,
     order_by: Optional[Union[List[str], str]] = None,
     direction: Optional[Union[List[str], str]] = None,
-    limit: int = None,
+    limit: Optional[int] = None,
 ) -> Select[Tuple[_T]]:
     """
     Builds and returns a select statement with optional filters, group by, order by, and limit clauses.
 
     Args:
         stmt (Select[Tuple[_T]]): The base SELECT statement.
         model (Optional[Type[_T]]): The model class associated with the SELECT statement.
@@ -132,15 +138,15 @@
         limit=limit,
     )
 
 
 def build_update_stmt(
     model: Type[_T],
     values: Dict,
-    filters: Optional[_FilterType] = None,
+    filters: Optional[FilterType] = None,
 ) -> ReturningUpdate[Tuple[_T]]:
     """
     Build and delete an update statement for the given model, values, and filters.
 
     Args:
         model (Type[_T]): The model class to update.
         values (Dict): A dictionary containing the column-value pairs to update.
@@ -172,15 +178,15 @@
         ReturningInsert[Tuple[_T]]: The insert statement with a returning clause.
     """
     return insert(model).returning(model)
 
 
 def build_delete_stmt(
     model: Type[_T],
-    filters: _FilterType,
+    filters: FilterType,
 ) -> ReturningDelete[Tuple[_T]]:
     """
     Build and return a delete statement for the given model and filters.
 
     Args:
         model (Type[_T]): The model class to delete from.
         filters (_FilterType): The filters to apply to the delete statement.
@@ -228,15 +234,15 @@
     """
     return stmt.group_by(group_by) if group_by is not None else stmt
 
 
 def apply_relationship_options(
     stmt: Union[Select[Tuple[_T]], Update],
     relationship_options: Dict[InstrumentedAttribute, RelationshipOption],
-    parents: List[InstrumentedAttribute] = None,
+    parents: Optional[List[InstrumentedAttribute]] = None,
 ) -> Union[Select[Tuple[_T]], Update]:
     """
     Apply relationship options to a SQLAlchemy statement.
 
     Args:
         stmt (Union[Select[Tuple[_T]], Update]): The SQLAlchemy statement to apply the relationship options to.
         relationship_options (Dict[InstrumentedAttribute, RelationshipOption]): A dictionary of relationship options.
@@ -308,15 +314,15 @@
             )
 
     return stmt
 
 
 def apply_filters(
     stmt: Union[Select[Tuple[_T]], Update],
-    filter_dict: _FilterType,
+    filter_dict: FilterType,
     with_optional: bool = False,
 ) -> Union[Select[Tuple[_T]], Update, Delete]:
     """
     Apply filters to the given statement.
 
     Args:
         stmt (Union[Select[Tuple[_T]], Update]): The statement to apply filters to.
@@ -466,15 +472,15 @@
     Returns:
         Select[Tuple[_T]]: The modified SQL statement with the limit applied.
     """
     return stmt.limit(limit) if limit is not None else stmt
 
 
 def get_conditions_from_dict(
-    values: _FilterType,
+    values: FilterType,
     with_optional: bool = False,
 ) -> List[ColumnExpressionArgument]:
     """
     Convert a dictionary of filter conditions into a list of SQLAlchemy conditions.
 
     Args:
         values (dict): A dictionary containing the filter conditions.
@@ -637,15 +643,15 @@
 
                         conditions.append(key.any(and_(*v)))
 
     return conditions
 
 
 def get_filters(
-    filters: _FilterType,
+    filters: FilterType,
     with_optional: bool = False,
 ) -> List[ColumnExpressionArgument]:
     """
     Get the conditions for filtering data based on the given filters.
 
     Args:
         filters (dict): The filters to apply on the data.
```

### Comparing `pysql-repo-0.6.2/pysql_repo/asyncio/async_database.py` & `pysql-repo-0.6.3/pysql_repo/asyncio/async_database.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.2/pysql_repo/asyncio/async_decorator.py` & `pysql-repo-0.6.3/pysql_repo/asyncio/async_decorator.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.2/pysql_repo/asyncio/async_repository.py` & `pysql-repo-0.6.3/pysql_repo/_repository.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,45 +9,42 @@
     Type,
     TypeVar,
     Union,
     Sequence,
 )
 
 # CONTEXTLIB
-from contextlib import AbstractAsyncContextManager
+from contextlib import AbstractContextManager
 
 # SQLALCHEMY
 from sqlalchemy import ColumnExpressionArgument, Select
-from sqlalchemy.ext.asyncio import AsyncSession
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import InstrumentedAttribute
+from sqlalchemy.orm import Session, InstrumentedAttribute, declarative_base
 
 # DECORATORS
-from pysql_repo._decorators import check_values as _check_values
-from pysql_repo.asyncio.async_decorator import with_async_session
+from pysql_repo._decorators import check_values as _check_values, with_session
 
 # UTILS
 from pysql_repo._utils import (
-    _FilterType,
+    FilterType,
     RelationshipOption,
-    async_apply_pagination as _async_apply_pagination,
     build_delete_stmt as _build_delete_stmt,
     build_insert_stmt as _build_insert_stmt,
     build_select_stmt as _build_select_stmt,
     build_update_stmt as _build_update_stmt,
     select_distinct as _select_distinct,
+    apply_pagination as _apply_pagination,
 )
 
 
 _T = TypeVar("_T", bound=declarative_base())
 
 
-class AsyncRepository:
+class Repository:
     """
-    Represents an asynchronous repository for database operations.
+    Represents a repository for database operations.
 
     Attributes:
         _session_factory: The session factory used for creating sessions.
 
     Methods:
         session_manager: Returns the session factory.
         _select: Selects a single row from the database.
@@ -56,130 +53,126 @@
         _select_all_stmt: Selects all rows from the database using a custom statement.
         _select_paginate: Selects a paginated set of rows from the database.
         _select_paginate_stmt: Selects a paginated set of rows from the database using a custom statement.
     """
 
     def __init__(
         self,
-        session_factory: Callable[..., AbstractAsyncContextManager[AsyncSession]],
+        session_factory: Callable[..., AbstractContextManager[Session]],
     ) -> None:
         """
-        Initializes the AsyncRepository.
+        Initializes the Repository.
 
         Args:
-            session_factory: A callable that returns an asynchronous context manager
+            session_factory: A callable that returns a context manager
                              for creating and managing database sessions.
 
         Returns:
             None
         """
         self._session_factory = session_factory
 
-    def session_manager(self) -> AbstractAsyncContextManager[AsyncSession]:
+    def session_manager(self) -> AbstractContextManager[Session]:
         """
         Get a session manager.
 
         Returns:
-            AbstractAsyncContextManager[AsyncSession]: An asynchronous context manager for managing database sessions.
+            AbstractContextManager[Session]: An context manager for managing database sessions.
         """
         return self._session_factory()
 
-    @with_async_session()
-    async def _select(
+    @with_session()
+    def _select(
         self,
         model: Type[_T],
         distinct: Optional[ColumnExpressionArgument] = None,
-        filters: Optional[_FilterType] = None,
-        optional_filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
+        optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
             Dict[InstrumentedAttribute, RelationshipOption]
         ] = None,
-        session: Optional[AsyncSession] = None,
+        session: Optional[Session] = None,
     ) -> Optional[_T]:
         """
         Selects a single object from the database.
 
         Args:
             model: The model class representing the table.
             distinct: The distinct column expression.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
-            The selected object or None if not found.
+            session: The session to use.
 
         Returns:
-            The selected row.
-
+            The selected object or None if not found.
         """
         stmt = _select_distinct(
             model=model,
             expr=distinct,
         )
 
-        return await self._select_stmt(
+        return self._select_stmt(
             stmt=stmt,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             session=session,
         )
 
-    @with_async_session()
-    async def _select_stmt(
+    @with_session()
+    def _select_stmt(
         self,
         stmt: Select[Tuple[_T]],
-        filters: Optional[_FilterType] = None,
-        optional_filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
+        optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
             Dict[InstrumentedAttribute, RelationshipOption]
         ] = None,
         group_by: Optional[ColumnExpressionArgument] = None,
-        session: Optional[AsyncSession] = None,
+        session: Optional[Session] = None,
     ) -> Optional[_T]:
         """
         Selects a single object from the database using a custom statement.
 
         Args:
             stmt: The custom select statement.
             filters: The filters to apply.
             optional_filters: The optional filters to apply.
             relationship_options: The relationship options.
             group_by: The column expression to group by.
             session: The session to use.
 
         Returns:
             The selected object or None if not found.
-
         """
         stmt = _build_select_stmt(
             stmt=stmt,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             group_by=group_by,
         )
 
-        result = await session.execute(stmt)
-
-        return result.unique().scalar_one_or_none()
+        return session.execute(stmt).unique().scalar_one_or_none()
 
-    @with_async_session()
-    async def _select_all(
+    @with_session()
+    def _select_all(
         self,
         model: Type[_T],
         distinct: Optional[List[ColumnExpressionArgument]] = None,
-        filters: Optional[_FilterType] = None,
-        optional_filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
+        optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
             Dict[InstrumentedAttribute, RelationshipOption]
         ] = None,
         order_by: Optional[Union[List[str], str]] = None,
-        direction: Optional[str] = None,
+        direction: Optional[Union[List[str], str]] = None,
         limit: int = None,
-        session: Optional[AsyncSession] = None,
+        session: Optional[Session] = None,
     ) -> Sequence[_T]:
         """
         Selects all objects from the database.
 
         Args:
             model: The model class representing the table.
             distinct: The distinct column expressions.
@@ -189,48 +182,47 @@
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of objects to return.
             session: The session to use.
 
         Returns:
             A sequence of selected objects.
-
         """
         stmt = _select_distinct(
             model=model,
             expr=distinct,
         )
 
-        return await self._select_all_stmt(
+        return self._select_all_stmt(
             stmt=stmt,
             model=model,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             order_by=order_by,
             direction=direction,
             limit=limit,
             session=session,
         )
 
-    @with_async_session()
-    async def _select_all_stmt(
+    @with_session()
+    def _select_all_stmt(
         self,
         stmt: Select[Tuple[_T]],
         model: Type[_T],
-        filters: Optional[_FilterType] = None,
-        optional_filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
+        optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
             Dict[InstrumentedAttribute, RelationshipOption]
         ] = None,
         group_by: Optional[ColumnExpressionArgument] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[Union[List[str], str]] = None,
         limit: int = None,
-        session: Optional[AsyncSession] = None,
+        session: Optional[Session] = None,
     ) -> Sequence[_T]:
         """
         Selects all objects from the database using a custom statement.
 
         Args:
             stmt: The custom select statement.
             model: The model class representing the table.
@@ -241,48 +233,45 @@
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of rows to return.
             session: The session to use.
 
         Returns:
             A sequence of selected objects.
-
         """
         stmt = _build_select_stmt(
             stmt=stmt,
             model=model,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             group_by=group_by,
             order_by=order_by,
             direction=direction,
             limit=limit,
         )
 
-        result = await session.execute(stmt)
+        return session.execute(stmt).unique().scalars().all()
 
-        return result.unique().scalars().all()
-
-    @with_async_session()
-    async def _select_paginate(
+    @with_session()
+    def _select_paginate(
         self,
         model: Type[_T],
         page: int,
         per_page: int,
         distinct: Optional[ColumnExpressionArgument] = None,
-        filters: Optional[_FilterType] = None,
-        optional_filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
+        optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
             Dict[InstrumentedAttribute, RelationshipOption]
         ] = None,
         order_by: Optional[Union[List[str], str]] = None,
-        direction: Optional[str] = None,
+        direction: Optional[Union[List[str], str]] = None,
         limit: int = None,
-        session: Optional[AsyncSession] = None,
+        session: Optional[Session] = None,
     ) -> Tuple[Sequence[_T], str]:
         """
         Selects a paginated set of objects from the database.
 
         Args:
             model: The model class representing the table.
             page: The page number.
@@ -294,52 +283,51 @@
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of objects to return.
             session: The session to use.
 
         Returns:
             A tuple containing the selected objects and pagination information.
-
         """
         stmt = _select_distinct(
             model=model,
             expr=distinct,
         )
 
-        return await self._select_paginate_stmt(
+        return self._select_paginate_stmt(
             stmt=stmt,
             model=model,
             page=page,
             per_page=per_page,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             order_by=order_by,
             direction=direction,
             limit=limit,
             session=session,
         )
 
-    @with_async_session()
-    async def _select_paginate_stmt(
+    @with_session()
+    def _select_paginate_stmt(
         self,
         stmt: Select[Tuple[_T]],
         model: Type[_T],
         page: int,
         per_page: int,
-        filters: Optional[_FilterType] = None,
-        optional_filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
+        optional_filters: Optional[FilterType] = None,
         relationship_options: Optional[
             Dict[InstrumentedAttribute, RelationshipOption]
         ] = None,
         group_by: Optional[ColumnExpressionArgument] = None,
         order_by: Optional[Union[List[str], str]] = None,
-        direction: Optional[str] = None,
+        direction: Optional[Union[List[str], str]] = None,
         limit: int = None,
-        session: Optional[AsyncSession] = None,
+        session: Optional[Session] = None,
     ) -> Tuple[Sequence[_T], str]:
         """
         Selects a paginated set of rows from the database using a custom statement.
 
         Args:
             stmt: The custom select statement.
             model: The model class representing the table.
@@ -352,49 +340,46 @@
             order_by: The column(s) to order by.
             direction: The direction of the ordering.
             limit: The maximum number of rows to return.
             session: The session to use.
 
         Returns:
             A tuple containing the selected objects and pagination information.
-
         """
         stmt = _build_select_stmt(
             stmt=stmt,
             model=model,
             filters=filters,
             optional_filters=optional_filters,
             relationship_options=relationship_options,
             group_by=group_by,
             order_by=order_by,
             direction=direction,
             limit=limit,
         )
 
-        stmt, pagination = await _async_apply_pagination(
+        stmt, pagination = _apply_pagination(
             session=session,
             stmt=stmt,
             page=page,
             per_page=per_page,
         )
 
-        result = await session.execute(stmt)
-
-        return result.unique().scalars().all(), pagination
+        return session.execute(stmt).unique().scalars().all(), pagination
 
     @_check_values(as_list=False)
-    @with_async_session()
-    async def _update_all(
+    @with_session()
+    def _update_all(
         self,
         model: Type[_T],
         values: Dict[str, Any],
-        filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
         flush: bool = False,
         commit: bool = False,
-        session: Optional[AsyncSession] = None,
+        session: Optional[Session] = None,
     ) -> Sequence[_T]:
         """
         Updates multiple objects in the database.
 
         Args:
             model: The model class representing the table.
             values: A dictionary of column-value pairs to update.
@@ -408,37 +393,35 @@
         """
         stmt = _build_update_stmt(
             model=model,
             values=values,
             filters=filters,
         )
 
-        result = await session.execute(stmt)
-
-        sequence = result.unique().scalars().all()
+        sequence = session.execute(stmt).unique().scalars().all()
 
         if flush:
-            await session.flush()
+            session.flush()
         if commit:
-            await session.commit()
+            session.commit()
 
-        [await session.refresh(item) for item in sequence]
+        [session.refresh(item) for item in sequence]
 
         return sequence
 
     @_check_values(as_list=False)
-    @with_async_session()
-    async def _update(
+    @with_session()
+    def _update(
         self,
         model: Type[_T],
         values: Dict[str, Any],
-        filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
         flush: bool = False,
         commit: bool = False,
-        session: Optional[AsyncSession] = None,
+        session: Optional[Session] = None,
     ) -> Optional[_T]:
         """
         Updates a single object in the database.
 
         Args:
             model: The model class representing the table.
             values: A dictionary of column-value pairs to update.
@@ -452,39 +435,37 @@
         """
         stmt = _build_update_stmt(
             model=model,
             values=values,
             filters=filters,
         )
 
-        result = await session.execute(stmt)
-
-        item = result.unique().scalar_one_or_none()
+        item = session.execute(stmt).unique().scalar_one_or_none()
 
         if item is None:
             return None
 
         if flush:
-            await session.flush()
+            session.flush()
         if commit:
-            await session.commit()
+            session.commit()
 
-        await session.refresh(item)
+        session.refresh(item)
 
         return item
 
     @_check_values(as_list=True)
-    @with_async_session()
-    async def _add_all(
+    @with_session()
+    def _add_all(
         self,
         model: Type[_T],
         values: List[Dict[str, Any]],
         flush: bool = False,
         commit: bool = False,
-        session: Optional[AsyncSession] = None,
+        session: Optional[Session] = None,
     ) -> Sequence[_T]:
         """
         Adds multiple objects to the database.
 
         Args:
             model: The model class representing the table.
             values: A list of dictionaries containing column-value pairs for each object.
@@ -493,76 +474,71 @@
             session: The session to use.
 
         Returns:
             A sequence of added objects.
         """
         stmt = _build_insert_stmt(model=model)
 
-        result = await session.execute(stmt, values)
-
-        sequence = result.unique().scalars().all()
+        sequence = session.execute(stmt, values).unique().scalars().all()
 
         if flush:
-            await session.flush()
+            session.flush()
         if commit:
-            await session.commit()
+            session.commit()
 
         if flush or commit:
-            [await session.refresh(item) for item in sequence]
+            [session.refresh(item) for item in sequence]
 
         return sequence
 
     @_check_values(as_list=False)
-    @with_async_session()
-    async def _add(
+    @with_session()
+    def _add(
         self,
         model: Type[_T],
         values: Dict[str, Any],
         flush: bool = False,
         commit: bool = False,
-        session: Optional[AsyncSession] = None,
+        session: Optional[Session] = None,
     ) -> _T:
         """
         Adds a single object to the database.
 
         Args:
             model: The model class representing the table.
             values: A dictionary of column-value pairs for the object.
             flush: Whether to flush the session after adding the object.
             commit: Whether to commit the session after adding the object.
             session: The session to use.
 
         Returns:
             The added object.
-
         """
         stmt = _build_insert_stmt(model=model)
 
-        result = await session.execute(stmt, values)
-
-        item = result.unique().scalar_one()
+        item = session.execute(stmt, values).unique().scalar_one()
 
         if flush:
-            await session.flush()
+            session.flush()
         if commit:
-            await session.commit()
+            session.commit()
 
         if flush or commit:
-            await session.refresh(item)
+            session.refresh(item)
 
         return item
 
-    @with_async_session()
-    async def _delete_all(
+    @with_session()
+    def _delete_all(
         self,
         model: Type[_T],
-        filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
         flush: bool = True,
         commit: bool = False,
-        session: Optional[AsyncSession] = None,
+        session: Optional[Session] = None,
     ) -> bool:
         """
         Deletes multiple objects from the database.
 
         Args:
             model: The model class representing the table.
             filters: The filters to apply.
@@ -574,36 +550,34 @@
             True if any objects were deleted, False otherwise.
         """
         stmt = _build_delete_stmt(
             model=model,
             filters=filters,
         )
 
-        result = await session.execute(stmt)
-
-        sequence = result.unique().scalars().all()
+        sequence = session.execute(stmt).unique().scalars().all()
 
         if len(sequence) == 0:
             return False
 
         if flush:
-            await session.flush()
+            session.flush()
         if commit:
-            await session.commit()
+            session.commit()
 
         return True
 
-    @with_async_session()
-    async def _delete(
+    @with_session()
+    def _delete(
         self,
         model: Type[_T],
-        filters: Optional[_FilterType] = None,
+        filters: Optional[FilterType] = None,
         flush: bool = True,
         commit: bool = False,
-        session: Optional[AsyncSession] = None,
+        session: Optional[Session] = None,
     ) -> bool:
         """
         Deletes a single object from the database.
 
         Args:
             model: The model class representing the table.
             filters: The filters to apply.
@@ -615,20 +589,18 @@
             True if the object was deleted, False otherwise.
         """
         stmt = _build_delete_stmt(
             model=model,
             filters=filters,
         )
 
-        result = await session.execute(stmt)
-
-        item = result.unique().scalar_one_or_none()
+        item = session.execute(stmt).unique().scalar_one_or_none()
 
         if item is None:
             return False
 
         if flush:
-            await session.flush()
+            session.flush()
         if commit:
-            await session.commit()
+            session.commit()
 
         return True
```

### Comparing `pysql-repo-0.6.2/pysql_repo/asyncio/async_service.py` & `pysql-repo-0.6.3/pysql_repo/asyncio/async_service.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.2/pysql_repo/libs/file_lib.py` & `pysql-repo-0.6.3/pysql_repo/libs/file_lib.py`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.2/pysql_repo.egg-info/PKG-INFO` & `pysql-repo-0.6.3/pysql_repo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysql-repo
-Version: 0.6.2
+Version: 0.6.3
 Summary: A project to have a base repository class to perform select/insert/update/delete with dynamic syntax
 Home-page: https://github.com/Impro02/pysql-repo
-Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.6.2.tar.gz
+Download-URL: https://github.com/Impro02/pysql-repo/archive/refs/tags/0.6.3.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysql-repo-0.6.2/pysql_repo.egg-info/SOURCES.txt` & `pysql-repo-0.6.3/pysql_repo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysql-repo-0.6.2/setup.py` & `pysql-repo-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.6.2"
+version = "0.6.3"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="pysql-repo",
     version=version,
```

