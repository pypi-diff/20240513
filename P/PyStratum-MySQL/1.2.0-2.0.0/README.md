# Comparing `tmp/PyStratum-MySQL-1.2.0.tar.gz` & `tmp/pystratum_mysql-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyStratum-MySQL-1.2.0.tar", last modified: Fri Jul  8 03:47:32 2022, max compression
+gzip compressed data, was "pystratum_mysql-2.0.0.tar", max compression
```

## Comparing `PyStratum-MySQL-1.2.0.tar` & `pystratum_mysql-2.0.0.tar`

### file list

```diff
@@ -1,44 +1,33 @@
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2022-07-08 03:47:32.201991 PyStratum-MySQL-1.2.0/
--rw-rw-r--   0 water     (1000) water     (1000)     5761 2022-07-08 03:47:32.201991 PyStratum-MySQL-1.2.0/PKG-INFO
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2022-07-08 03:47:32.199992 PyStratum-MySQL-1.2.0/PyStratum_MySQL.egg-info/
--rw-rw-r--   0 water     (1000) water     (1000)     5761 2022-07-08 03:47:32.000000 PyStratum-MySQL-1.2.0/PyStratum_MySQL.egg-info/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)     1482 2022-07-08 03:47:32.000000 PyStratum-MySQL-1.2.0/PyStratum_MySQL.egg-info/SOURCES.txt
--rw-rw-r--   0 water     (1000) water     (1000)        1 2022-07-08 03:47:32.000000 PyStratum-MySQL-1.2.0/PyStratum_MySQL.egg-info/dependency_links.txt
--rw-rw-r--   0 water     (1000) water     (1000)      116 2022-07-08 03:47:32.000000 PyStratum-MySQL-1.2.0/PyStratum_MySQL.egg-info/requires.txt
--rw-rw-r--   0 water     (1000) water     (1000)       16 2022-07-08 03:47:32.000000 PyStratum-MySQL-1.2.0/PyStratum_MySQL.egg-info/top_level.txt
--rw-rw-r--   0 water     (1000) water     (1000)     4622 2020-10-17 12:51:04.000000 PyStratum-MySQL-1.2.0/README.rst
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2022-07-08 03:47:32.199992 PyStratum-MySQL-1.2.0/pystratum_mysql/
--rw-rw-r--   0 water     (1000) water     (1000)     1197 2022-07-08 02:12:50.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/MySqlConnector.py
--rw-rw-r--   0 water     (1000) water     (1000)    16185 2022-07-08 03:13:41.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/MySqlDataLayer.py
--rw-rw-r--   0 water     (1000) water     (1000)     2152 2022-07-08 03:38:18.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/MySqlDefaultConnector.py
--rw-rw-r--   0 water     (1000) water     (1000)    11456 2020-10-17 09:46:32.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/MySqlMetadataDataLayer.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:21.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2022-07-08 03:47:32.200991 PyStratum-MySQL-1.2.0/pystratum_mysql/backend/
--rw-rw-r--   0 water     (1000) water     (1000)     2715 2020-10-18 03:50:28.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/backend/MySqlBackend.py
--rw-rw-r--   0 water     (1000) water     (1000)    12123 2022-07-08 03:06:51.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/backend/MySqlConstantWorker.py
--rw-rw-r--   0 water     (1000) water     (1000)     7759 2020-10-28 04:45:56.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/backend/MySqlRoutineLoaderWorker.py
--rw-rw-r--   0 water     (1000) water     (1000)     1587 2020-10-17 12:39:32.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/backend/MySqlRoutineWrapperGeneratorWorker.py
--rw-rw-r--   0 water     (1000) water     (1000)     3745 2020-10-17 09:16:07.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/backend/MySqlWorker.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2020-10-16 08:28:51.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/backend/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2022-07-08 03:47:32.200991 PyStratum-MySQL-1.2.0/pystratum_mysql/helper/
--rw-rw-r--   0 water     (1000) water     (1000)     4743 2020-10-15 21:37:54.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/helper/MySqlDataTypeHelper.py
--rwxrwxr-x   0 water     (1000) water     (1000)    11120 2020-10-17 06:04:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/helper/MySqlRoutineLoaderHelper.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-09-27 15:36:45.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/helper/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2022-07-08 03:47:32.201991 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/
--rw-rw-r--   0 water     (1000) water     (1000)      726 2020-10-16 09:33:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlBulkWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      713 2020-10-16 09:33:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlFunctionsWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      712 2020-10-16 09:33:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlLogWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      724 2020-10-16 09:33:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlMultiWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      714 2020-10-16 09:33:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlNoneWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      721 2020-10-16 09:33:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlRow0Wrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      716 2020-10-16 09:33:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlRow1Wrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      826 2020-10-16 09:33:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlRowsWithIndexWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      814 2020-10-16 09:33:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlRowsWithKeyWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)     1136 2020-10-16 09:33:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlRowsWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      772 2020-10-16 09:33:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlSingleton0Wrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      785 2020-10-16 09:33:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlSingleton1Wrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      741 2020-10-16 09:33:09.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlTableWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)     5064 2020-10-18 03:07:40.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)     3113 2019-07-03 07:43:51.000000 PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/__init__.py
--rw-rw-r--   0 water     (1000) water     (1000)       38 2022-07-08 03:47:32.201991 PyStratum-MySQL-1.2.0/setup.cfg
--rw-rw-r--   0 water     (1000) water     (1000)     1459 2022-07-08 03:46:29.000000 PyStratum-MySQL-1.2.0/setup.py
+-rw-r--r--   0        0        0     1096 2017-03-05 12:20:49.000000 pystratum_mysql-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0     1070 2024-05-13 14:35:57.084474 pystratum_mysql-2.0.0/README.md
+-rw-r--r--   0        0        0     1276 2024-05-13 14:42:09.172681 pystratum_mysql-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1176 2024-05-13 08:39:21.721325 pystratum_mysql-2.0.0/pystratum_mysql/MySqlConnector.py
+-rw-r--r--   0        0        0    15686 2024-05-13 08:39:21.707324 pystratum_mysql-2.0.0/pystratum_mysql/MySqlDataLayer.py
+-rw-r--r--   0        0        0     2130 2024-05-12 12:06:16.302670 pystratum_mysql-2.0.0/pystratum_mysql/MySqlDefaultConnector.py
+-rw-r--r--   0        0        0    11218 2024-05-13 11:48:48.571690 pystratum_mysql-2.0.0/pystratum_mysql/MySqlMetadataDataLayer.py
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:21.000000 pystratum_mysql-2.0.0/pystratum_mysql/__init__.py
+-rw-r--r--   0        0        0     2491 2024-05-13 08:37:57.261490 pystratum_mysql-2.0.0/pystratum_mysql/backend/MySqlBackend.py
+-rw-r--r--   0        0        0    12143 2024-05-13 11:55:44.284795 pystratum_mysql-2.0.0/pystratum_mysql/backend/MySqlConstantWorker.py
+-rw-r--r--   0        0        0     7646 2024-05-13 12:03:22.391801 pystratum_mysql-2.0.0/pystratum_mysql/backend/MySqlRoutineLoaderWorker.py
+-rw-r--r--   0        0        0     1558 2024-05-13 08:39:21.735325 pystratum_mysql-2.0.0/pystratum_mysql/backend/MySqlRoutineWrapperGeneratorWorker.py
+-rw-r--r--   0        0        0     3633 2024-05-13 12:03:22.386801 pystratum_mysql-2.0.0/pystratum_mysql/backend/MySqlWorker.py
+-rw-r--r--   0        0        0        0 2020-10-16 08:28:51.000000 pystratum_mysql-2.0.0/pystratum_mysql/backend/__init__.py
+-rw-r--r--   0        0        0     4689 2024-05-12 12:00:50.484514 pystratum_mysql-2.0.0/pystratum_mysql/helper/MySqlDataTypeHelper.py
+-rwxr-xr-x   0        0        0    10879 2024-05-13 11:07:24.361857 pystratum_mysql-2.0.0/pystratum_mysql/helper/MySqlRoutineLoaderHelper.py
+-rw-r--r--   0        0        0        0 2016-09-27 15:36:45.000000 pystratum_mysql-2.0.0/pystratum_mysql/helper/__init__.py
+-rw-r--r--   0        0        0      727 2024-05-13 08:39:21.745325 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlBulkWrapper.py
+-rw-r--r--   0        0        0      714 2024-05-13 08:39:21.737325 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlFunctionsWrapper.py
+-rw-r--r--   0        0        0      713 2024-05-13 08:39:21.709324 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlLogWrapper.py
+-rw-r--r--   0        0        0      725 2024-05-13 08:39:21.733325 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlMultiWrapper.py
+-rw-r--r--   0        0        0      715 2024-05-13 08:39:21.724325 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlNoneWrapper.py
+-rw-r--r--   0        0        0      722 2024-05-13 08:39:21.711324 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlRow0Wrapper.py
+-rw-r--r--   0        0        0      717 2024-05-13 08:39:21.704324 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlRow1Wrapper.py
+-rw-r--r--   0        0        0      827 2024-05-13 08:39:21.716324 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlRowsWithIndexWrapper.py
+-rw-r--r--   0        0        0      815 2024-05-13 08:39:21.700324 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlRowsWithKeyWrapper.py
+-rw-r--r--   0        0        0     1115 2024-05-13 08:39:21.743325 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlRowsWrapper.py
+-rw-r--r--   0        0        0      773 2024-05-13 08:39:21.741325 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlSingleton0Wrapper.py
+-rw-r--r--   0        0        0      790 2024-05-13 08:39:21.719324 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlSingleton1Wrapper.py
+-rw-r--r--   0        0        0      742 2024-05-13 08:39:21.717324 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlTableWrapper.py
+-rw-r--r--   0        0        0     4970 2024-05-12 12:00:50.466513 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlWrapper.py
+-rw-r--r--   0        0        0     3111 2024-05-13 08:39:21.728325 pystratum_mysql-2.0.0/pystratum_mysql/wrapper/__init__.py
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 pystratum_mysql-2.0.0/PKG-INFO
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/MySqlConnector.py` & `pystratum_mysql-2.0.0/pystratum_mysql/MySqlConnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from mysql.connector import MySQLConnection
 
 
 class MySqlConnector:
     """
     Interface for classes for connecting to a MySql instances.
     """
+
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def connect(self) -> MySQLConnection:
         """
         Connects to the MySql instance.
         """
         raise NotImplementedError()
@@ -24,13 +25,11 @@
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def is_alive(self) -> bool:
         """
         Returns whether Python is (still) connected to a MySQL or MariaDB instance.
-
-        :rtype: bool
         """
         raise NotImplementedError()
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/MySqlDataLayer.py` & `pystratum_mysql-2.0.0/pystratum_mysql/MySqlDataLayer.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,16 @@
         See https://dev.mysql.com/doc/connector-python/en/connector-python-api-mysqlconnection-commit.html
         """
         self._connection.commit()
 
     # ------------------------------------------------------------------------------------------------------------------
     def connect(self) -> None:
         """
-        Connects to a MySQL instance. See https://dev.mysql.com/doc/connector-python/en/connector-python-connectargs.html
+        Connects to a MySQL instance. See https://dev.mysql.com/doc/connector-python/en/connector-python-connectargs
+        .html
         for a complete overview of all possible keys in config.
         """
         self._connection = self.__connector.connect()
 
     # ------------------------------------------------------------------------------------------------------------------
     def connect_if_not_alive(self) -> None:
         """
@@ -80,32 +81,30 @@
         self.__connector.disconnect()
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_multi(self, sql: str) -> None:
         """
         Executes a multi query that does not select any rows.
 
-        :param str sql: The SQL statements.
+        :param sql: The SQL statements.
         """
         self._last_sql = sql
 
         cursor = MySQLCursor(self._connection)
         for _ in cursor.execute(sql, multi=True):
             pass
         cursor.close()
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_none(self, sql: str, *params) -> int:
         """
         Executes a query that does not select any rows. Returns the number of affected rows.
 
-        :param str sql: The SQL statement.
-        :param iterable params: The values for the statement.
-
-        :rtype: int
+        :param sql: The SQL statement.
+        :param params: The values for the statement.
         """
         self._last_sql = sql
 
         cursor = MySQLCursor(self._connection)
         cursor.execute(sql, params)
         rowcount = cursor.rowcount
         cursor.close()
@@ -113,18 +112,16 @@
         return rowcount
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_rows(self, sql: str, *params) -> List[Dict[str, Any]]:
         """
         Executes a query that selects 0 or more rows. Returns the selected rows (an empty list if no rows are selected).
 
-        :param str sql: The SQL statement.
-        :param iterable params: The arguments for the statement.
-
-        :rtype: list[dict[str,*]]
+        :param sql: The SQL statement.
+        :param params: The arguments for the statement.
         """
         self._last_sql = sql
 
         cursor = MySQLCursorBufferedDict(self._connection)
         cursor.execute(sql, *params)
         ret = cursor.fetchall()
         cursor.close()
@@ -132,18 +129,16 @@
         return ret
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_singleton1(self, sql: str, *params) -> Any:
         """
         Executes SQL statement that selects 1 row with 1 column. Returns the value of the selected column.
 
-        :param str sql: The SQL calling the stored procedure.
-        :param iterable params: The arguments for the stored procedure.
-
-        :rtype: *:
+        :param sql: The SQL calling the stored procedure.
+        :param params: The arguments for the stored procedure.
         """
         self._last_sql = sql
 
         cursor = MySQLCursorBuffered(self._connection)
         cursor.execute(sql, params)
         rowcount = cursor.rowcount
         if rowcount == 1:
@@ -158,19 +153,17 @@
         return ret
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_sp_bulk(self, bulk_handler: BulkHandler, sql: str, *params) -> int:
         """
         Executes a stored routine with designation type "bulk". Returns the number of rows processed.
 
-        :param BulkHandler bulk_handler: The bulk handler for processing the selected rows.
-        :param str sql: The SQL statement for calling the stored routine.
-        :param iterable params: The arguments for calling the stored routine.
-
-        :rtype: int
+        :param bulk_handler: The bulk handler for processing the selected rows.
+        :param sql: The SQL statement for calling the stored routine.
+        :param params: The arguments for calling the stored routine.
         """
         self._last_sql = sql
 
         cursor = MySQLCursorDict(self._connection)
         itr = cursor.execute(sql, params, multi=True)
         bulk_handler.start()
 
@@ -186,18 +179,16 @@
         return rowcount
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_sp_log(self, sql: str, *params) -> int:
         """
         Executes a stored routine with designation type "log". Returns the number of log messages.
 
-        :param str sql: The SQL statement for calling the stored routine.
-        :param iterable params: The arguments for calling the stored routine.
-
-        :rtype: int
+        :param sql: The SQL statement for calling the stored routine.
+        :param params: The arguments for calling the stored routine.
         """
         self._last_sql = sql
 
         cursor = MySQLCursorBuffered(self._connection)
         itr = cursor.execute(sql, params, multi=True)
 
         rowcount = 0
@@ -220,18 +211,16 @@
         return rowcount
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_sp_multi(self, sql: str, *params) -> List[List[Dict[str, Any]]]:
         """
         Executes a stored routine with designation type "multi". Returns a list of the result sets.
 
-        :param str sql: The SQL statement for calling the stored routine.
-        :param iterable params: The arguments for calling the stored routine.
-
-        :rtype: list[list[dict[str,*]]]
+        :param sql: The SQL statement for calling the stored routine.
+        :param params: The arguments for calling the stored routine.
         """
         self._last_sql = sql
 
         cursor = MySQLCursorBufferedDict(self._connection)
         itr = cursor.execute(sql, params, multi=True)
 
         results = []
@@ -246,18 +235,16 @@
         return results
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_sp_none(self, sql: str, *params) -> int:
         """
         Executes a stored routine that does not select any rows. Returns the number of affected rows.
 
-        :param str sql: The SQL calling the stored procedure.
-        :param iterable params: The arguments for the stored procedure.
-
-        :rtype: int
+        :param sql: The SQL calling the stored procedure.
+        :param params: The arguments for the stored procedure.
         """
         self._last_sql = sql
 
         cursor = MySQLCursor(self._connection)
         itr = cursor.execute(sql, params, multi=True)
         result = itr.__next__()
         rowcount = result.rowcount
@@ -266,18 +253,16 @@
         return rowcount
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_sp_row0(self, sql: str, *params) -> Optional[Dict[str, Any]]:
         """
         Executes a stored procedure that selects 0 or 1 row. Returns the selected row or None.
 
-        :param str sql: The SQL call the the stored procedure.
-        :param iterable params: The arguments for the stored procedure.
-
-        :rtype: None|dict[str,*]
+        :param sql: The SQL code to execute the stored procedure.
+        :param params: The arguments for the stored procedure.
         """
         self._last_sql = sql
 
         cursor = MySQLCursorBufferedDict(self._connection)
         itr = cursor.execute(sql, params, multi=True)
         result = itr.__next__()
         rowcount = result.rowcount
@@ -294,18 +279,16 @@
         return ret
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_sp_row1(self, sql: str, *params) -> Dict[str, Any]:
         """
         Executes a stored procedure that selects 1 row. Returns the selected row.
 
-        :param str sql: The SQL calling the the stored procedure.
-        :param iterable params: The arguments for the stored procedure.
-
-        :rtype: dict[str,*]
+        :param sql: The SQL code to execute the stored procedure.
+        :param params: The arguments for the stored procedure.
         """
         self._last_sql = sql
 
         cursor = MySQLCursorBufferedDict(self._connection)
         itr = cursor.execute(sql, params, multi=True)
         result = itr.__next__()
         rowcount = result.rowcount
@@ -323,18 +306,16 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_sp_rows(self, sql: str, *params) -> List[Dict[str, Any]]:
         """
         Executes a stored procedure that selects 0 or more rows. Returns the selected rows (an empty list if no rows
         are selected).
 
-        :param str sql: The SQL statement.
-        :param iterable params: The arguments for the statement.
-
-        :rtype: list[dict[str,*]]
+        :param sql: The SQL code to execute the stored procedure.
+        :param params: The arguments for the statement.
         """
         self._last_sql = sql
 
         cursor = MySQLCursorBufferedDict(self._connection)
         itr = cursor.execute(sql, params, multi=True)
         ret = itr.__next__().fetchall()
         itr.__next__()
@@ -343,18 +324,16 @@
         return ret
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_sp_singleton0(self, sql: str, *params) -> Any:
         """
         Executes a stored procedure that selects 0 or 1 row with 1 column. Returns the value of selected column or None.
 
-        :param str sql: The SQL calling the stored procedure.
-        :param iterable params: The arguments for the stored procedure.
-
-        :rtype: *
+        :param sql: The SQL code to execute the stored procedure.
+        :param params: The arguments for the stored procedure.
         """
         self._last_sql = sql
 
         cursor = MySQLCursorBuffered(self._connection)
         itr = cursor.execute(sql, params, multi=True)
         result = itr.__next__()
         rowcount = result.rowcount
@@ -372,18 +351,16 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_sp_singleton1(self, sql: str, *params) -> Any:
         """
         Executes a stored routine with designation type "table", i.e a stored routine that is expected to select 1 row
         with 1 column.
 
-        :param str sql: The SQL calling the the stored procedure.
-        :param iterable params: The arguments for the stored procedure.
-
-        :rtype: * The value of the selected column.
+        :param sql: The SQL code to execute the stored procedure.
+        :param params: The arguments for the stored procedure.
         """
         self._last_sql = sql
 
         cursor = MySQLCursorBuffered(self._connection)
         itr = cursor.execute(sql, params, multi=True)
         result = itr.__next__()
         rowcount = result.rowcount
@@ -399,16 +376,14 @@
 
         return ret
 
     # ------------------------------------------------------------------------------------------------------------------
     def is_alive(self) -> bool:
         """
         Returns whether Python is (still) connected to a MySQL or MariaDB instance.
-
-        :rtype: bool
         """
         return self.__connector.is_alive()
 
     # ------------------------------------------------------------------------------------------------------------------
     def last_sql(self) -> str:
         """
         Returns the last execute SQL statement.
@@ -428,14 +403,14 @@
                           consistent_snapshot: bool = False,
                           isolation_level: str = 'READ-COMMITTED',
                           readonly: Optional[bool] = None) -> None:
         """
         Starts a transaction.
         See https://dev.mysql.com/doc/connector-python/en/connector-python-api-mysqlconnection-start-transaction.html
 
-        :param bool consistent_snapshot:
-        :param str isolation_level:
-        :param bool readonly:
+        :param consistent_snapshot:
+        :param isolation_level:
+        :param readonly:
         """
         self._connection.start_transaction(consistent_snapshot, isolation_level, readonly)
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/MySqlDefaultConnector.py` & `pystratum_mysql-2.0.0/pystratum_mysql/MySqlDefaultConnector.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,14 @@
             self._connection.close()
             self._connection = None
 
     # ------------------------------------------------------------------------------------------------------------------
     def is_alive(self) -> bool:
         """
         Returns whether Python is (still) connected to a MySQL or MariaDB instance.
-
-        :rtype: bool
         """
         is_alive = False
 
         if self._connection:
             try:
                 result = self._connection.cmd_ping()
                 if isinstance(result, dict):
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/MySqlMetadataDataLayer.py` & `pystratum_mysql-2.0.0/pystratum_mysql/MySqlMetadataDataLayer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 from typing import Any, Dict, List, Union
 
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 from pystratum_common.MetadataDataLayer import MetadataDataLayer
 
 from pystratum_mysql.MySqlConnector import MySqlConnector
 from pystratum_mysql.MySqlDataLayer import MySqlDataLayer
 
 
 class MySqlMetadataDataLayer(MetadataDataLayer):
     """
     Data layer for retrieving metadata and loading stored routines.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, io: StratumStyle, connector: MySqlConnector):
+    def __init__(self, io: StratumIO, connector: MySqlConnector):
         """
         Object constructor.
 
-        :param PyStratumStyle io: The output decorator.
+        :param io: The output decorator.
         """
         super().__init__(io)
 
         self.__dl: MySqlDataLayer = MySqlDataLayer(connector)
         """
         The connection to the MySQL instance.
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     def call_stored_routine(self, routine_name: str) -> int:
         """
         Class a stored procedure without arguments.
 
-        :param str routine_name: The name of the procedure.
-
-        :rtype: int
+        :param routine_name: The name of the procedure.
         """
         sql = 'call {0}()'.format(routine_name)
 
         return self.execute_none(sql)
 
     # ------------------------------------------------------------------------------------------------------------------
     def check_table_exists(self, table_name: str) -> int:
         """
         Checks if a table exists in the current schema.
 
-        :param str table_name: The name of the table.
-
-        :rtype: int
+        :param table_name: The name of the table.
         """
         sql = """
 select 1 from
 information_schema.TABLES
 where TABLE_SCHEMA = database()
 and   TABLE_NAME   = '{0}'""".format(table_name)
 
@@ -64,17 +60,15 @@
         self.__dl.connect()
 
     # ------------------------------------------------------------------------------------------------------------------
     def describe_table(self, table_name: str) -> List[Dict[str, Any]]:
         """
         Describes a table.
 
-        :param str table_name: The name of the table.
-
-        :rtype: list[dict[str,*]]
+        :param table_name: The name of the table.
         """
         sql = 'describe `{0}`'.format(table_name)
 
         return self.execute_rows(sql)
 
     # ------------------------------------------------------------------------------------------------------------------
     def disconnect(self) -> None:
@@ -84,141 +78,129 @@
         self.__dl.disconnect()
 
     # ------------------------------------------------------------------------------------------------------------------
     def drop_stored_routine(self, routine_type: str, routine_name: str) -> None:
         """
         Drops a stored routine if it exists.
 
-        :param str routine_type: The type of the routine (i.e. PROCEDURE or FUNCTION).
-        :param str routine_name: The name of the routine.
+        :param routine_type: The type of the routine (i.e. PROCEDURE or FUNCTION).
+        :param routine_name: The name of the routine.
         """
         sql = 'drop {0} if exists `{1}`'.format(routine_type, routine_name)
 
         self.execute_none(sql)
 
     # ------------------------------------------------------------------------------------------------------------------
     def drop_temporary_table(self, table_name: str) -> None:
         """
         Drops a temporary table.
 
-        :param str table_name: The name of the table.
+        :param table_name: The name of the table.
         """
         sql = 'drop temporary table `{0}`'.format(table_name)
 
         self.execute_none(sql)
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_none(self, query: str) -> int:
         """
         Executes a query that does not select any rows.
 
-        :param str query: The query.
-
-        :rtype: int
+        :param query: The query.
         """
         self._log_query(query)
 
         return self.__dl.execute_none(query)
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_rows(self, query: str) -> List[Dict[str, Any]]:
         """
         Executes a query that selects 0 or more rows. Returns the selected rows (an empty list if no rows are selected).
 
-        :param str query: The query.
-
-        :rtype: list[dict[str,*]]
+        :param query: The query.
         """
         self._log_query(query)
 
         return self.__dl.execute_rows(query)
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute_singleton1(self, query: str) -> Any:
         """
         Executes SQL statement that selects 1 row with 1 column. Returns the value of the selected column.
 
-        :param str query: The query.
-
-        :rtype: *
+        :param query: The query.
         """
         self._log_query(query)
 
         return self.__dl.execute_singleton1(query)
 
     # ------------------------------------------------------------------------------------------------------------------
     def get_all_table_columns(self) -> List[Dict[str, Union[str, int, None]]]:
         """
         Selects metadata of all columns of all tables.
-
-        :rtype: list[dict[str,*]]
         """
         sql = """
 (
-  select table_name
-  ,      column_name
-  ,      column_type
-  ,      character_set_name
-  ,      data_type
-  ,      character_maximum_length
-  ,      numeric_precision
-  ,      ordinal_position
+  select TABLE_NAME                as  table_name
+  ,      COLUMN_NAME               as  column_name
+  ,      COLUMN_TYPE               as  column_type
+  ,      CHARACTER_SET_NAME        as  character_set_name
+  ,      DATA_TYPE                 as  data_type
+  ,      CHARACTER_MAXIMUM_LENGTH  as  character_maximum_length
+  ,      NUMERIC_PRECISION         as  numeric_precision
+  ,      ORDINAL_POSITION          as  ordinal_position
   from   information_schema.COLUMNS
-  where  table_schema = database()
-  and    table_name  rlike '^[a-zA-Z0-9_]*$'
-  and    column_name rlike '^[a-zA-Z0-9_]*$'
-  order by table_name
-  ,        ordinal_position
+  where  TABLE_SCHEMA = database()
+  and    TABLE_NAME  rlike '^[a-zA-Z0-9_]*$'
+  and    COLUMN_NAME rlike '^[a-zA-Z0-9_]*$'
+  order by TABLE_NAME
+  ,        ORDINAL_POSITION
 )
 
 union all
 
 (
-  select concat(table_schema,'.',table_name) table_name
-  ,      column_name
-  ,      column_type
-  ,      character_set_name
-  ,      data_type
-  ,      character_maximum_length
-  ,      numeric_precision
-  ,      ordinal_position
+  select concat(TABLE_SCHEMA,'.',TABLE_NAME) 
+  ,      COLUMN_NAME
+  ,      COLUMN_TYPE
+  ,      CHARACTER_SET_NAME
+  ,      DATA_TYPE
+  ,      CHARACTER_MAXIMUM_LENGTH
+  ,      NUMERIC_PRECISION
+  ,      ORDINAL_POSITION
   from   information_schema.COLUMNS
-  where  table_name  rlike '^[a-zA-Z0-9_]*$'
-  and    column_name rlike '^[a-zA-Z0-9_]*$'
-  order by table_schema
-  ,        table_name
-  ,        ordinal_position
+  where  TABLE_NAME  rlike '^[a-zA-Z0-9_]*$'
+  and    COLUMN_NAME rlike '^[a-zA-Z0-9_]*$'
+  order by TABLE_SCHEMA
+  ,        TABLE_NAME
+  ,        ORDINAL_POSITION
 )
 """
 
         return self.execute_rows(sql)
 
     # ------------------------------------------------------------------------------------------------------------------
     def get_correct_sql_mode(self, sql_mode: str) -> str:
         """
         Selects the SQL mode in the order as preferred by MySQL.
 
-        :param str sql_mode: The SQL mode.
-
-        :rtype: str
+        :param sql_mode: The SQL mode.
         """
         self.set_sql_mode(sql_mode)
 
         sql = 'select @@sql_mode'
 
         return self.execute_singleton1(sql)
 
     # ------------------------------------------------------------------------------------------------------------------
     def get_label_tables(self, regex: str) -> List[Dict[str, Any]]:
         """
         Selects metadata of tables with a label column.
 
-        :param str regex: The regular expression for columns which we want to use.
-
-        :rtype: list[dict[str,*]]
+        :param regex: The regular expression for columns which we want to use.
         """
         sql = """
 select t1.TABLE_NAME  table_name
 ,      t1.COLUMN_NAME id
 ,      t2.COLUMN_NAME label
 from       information_schema.COLUMNS t1
 inner join information_schema.COLUMNS t2 on t1.TABLE_NAME = t2.TABLE_NAME
@@ -231,19 +213,17 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     def get_labels_from_table(self, table_name: str, id_column_name: str, label_column_name: str) -> \
             List[Dict[str, Any]]:
         """
         Selects all labels from a table with labels.
 
-        :param str table_name: The name of the table.
-        :param str id_column_name: The name of the auto increment column.
-        :param str label_column_name: The name of the column with labels.
-
-        :rtype: list[dict[str,*]]
+        :param table_name: The name of the table.
+        :param id_column_name: The name of the auto increment column.
+        :param label_column_name: The name of the column with labels.
         """
         sql = """
 select `{0}`  as `id`
 ,      `{1}`  as `label`
 from   `{2}`
 where   nullif(`{1}`,'') is not null""".format(id_column_name,
                                                label_column_name,
@@ -251,27 +231,23 @@
 
         return self.execute_rows(sql)
 
     # ------------------------------------------------------------------------------------------------------------------
     def last_sql(self) -> str:
         """
         The last executed SQL statement.
-
-        :rtype: str
         """
         return self.__dl.last_sql()
 
     # ------------------------------------------------------------------------------------------------------------------
     def get_routine_parameters(self, routine_name: str) -> List[Dict[str, Any]]:
         """
         Selects metadata of the parameters of a stored routine.
 
-        :param str routine_name: The name of the routine.
-
-        :rtype: list[dict[str,*]]
+        :param routine_name: The name of the routine.
         """
         sql = """
 select t2.PARAMETER_NAME      parameter_name
 ,      t2.DATA_TYPE           parameter_type
 ,      t2.NUMERIC_PRECISION   numeric_precision
 ,      t2.NUMERIC_SCALE       numeric_scale
 ,      t2.DTD_IDENTIFIER      column_type
@@ -286,16 +262,14 @@
 
         return self.execute_rows(sql)
 
     # ------------------------------------------------------------------------------------------------------------------
     def get_routines(self) -> List[Dict[str, Any]]:
         """
         Selects metadata of all routines in the current schema.
-
-        :rtype: list[dict[str,*]]
         """
         sql = """
 select ROUTINE_NAME           as routine_name
 ,      ROUTINE_TYPE           as routine_type
 ,      SQL_MODE               as sql_mode
 ,      CHARACTER_SET_CLIENT   as character_set_client
 ,      COLLATION_CONNECTION   as collation_connection
@@ -306,26 +280,26 @@
         return self.execute_rows(sql)
 
     # ------------------------------------------------------------------------------------------------------------------
     def set_character_set(self, character_set: str, collate: str) -> None:
         """
         Sets the default character set and collate.
 
-        :param str character_set: The name of the character set.
-        :param str collate: The name of the collate
+        :param character_set: The name of the character set.
+        :param collate: The name of collate.
         """
         sql = "set names '{0}' collate '{1}'".format(character_set, collate)
 
         self.execute_none(sql)
 
     # ------------------------------------------------------------------------------------------------------------------
     def set_sql_mode(self, sql_mode: str) -> None:
         """
         Sets the SQL mode.
 
-        :param str sql_mode: The SQL mode.
+        :param sql_mode: The SQL mode.
         """
         sql = "set sql_mode = '{0}'".format(sql_mode)
 
         self.execute_none(sql)
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/backend/MySqlBackend.py` & `pystratum_mysql-2.0.0/pystratum_mysql/backend/MySqlBackend.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 from configparser import ConfigParser
 from typing import Optional
 
 from pystratum_backend.Backend import Backend
 from pystratum_backend.ConstantWorker import ConstantWorker
 from pystratum_backend.RoutineLoaderWorker import RoutineLoaderWorker
 from pystratum_backend.RoutineWrapperGeneratorWorker import RoutineWrapperGeneratorWorker
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 
 from pystratum_mysql.backend.MySqlConstantWorker import MySqlConstantWorker
 from pystratum_mysql.backend.MySqlRoutineLoaderWorker import MySqlRoutineLoaderWorker
 from pystratum_mysql.backend.MySqlRoutineWrapperGeneratorWorker import MySqlRoutineWrapperGeneratorWorker
 
 
 class MySqlBackend(Backend):
     """
     PyStratum Backend for MySQL & MariaDB.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def create_constant_worker(self, config: ConfigParser, io: StratumStyle) -> Optional[ConstantWorker]:
+    def create_constant_worker(self, config: ConfigParser, io: StratumIO) -> Optional[ConstantWorker]:
         """
         Creates the object that does the actual execution of the constant command for the backend.
 
-        :param ConfigParser config: The settings from the PyStratum configuration file.
-        :param StratumStyle io: The output object.
-
-        :rtype: ConstantWorker|None
+        :param config: The settings from the PyStratum configuration file.
+        :param io: The output object.
         """
         return MySqlConstantWorker(io, config)
 
     # ------------------------------------------------------------------------------------------------------------------
-    def create_routine_loader_worker(self, config: ConfigParser, io: StratumStyle) -> Optional[RoutineLoaderWorker]:
+    def create_routine_loader_worker(self, config: ConfigParser, io: StratumIO) -> Optional[RoutineLoaderWorker]:
         """
         Creates the object that does the actual execution of the routine loader command for the backend.
 
-        :param ConfigParser config: The settings from the PyStratum configuration file.
-        :param StratumStyle io: The output object.
-
-        :rtype: RoutineLoaderWorker|None
+        :param config: The settings from the PyStratum configuration file.
+        :param io: The output object.
         """
         return MySqlRoutineLoaderWorker(io, config)
 
     # ------------------------------------------------------------------------------------------------------------------
-    def create_routine_wrapper_generator_worker(self, config: ConfigParser, io: StratumStyle) \
+    def create_routine_wrapper_generator_worker(self, config: ConfigParser, io: StratumIO) \
             -> Optional[RoutineWrapperGeneratorWorker]:
         """
         Creates the object that does the actual execution of the routine wrapper generator command for the backend.
 
-        :param ConfigParser config: The settings from the PyStratum configuration file.
-        :param StratumStyle io: The output object.
-
-        :rtype: RoutineWrapperGeneratorWorker|None
+        :param config: The settings from the PyStratum configuration file.
+        :param io: The output object.
         """
         return MySqlRoutineWrapperGeneratorWorker(io, config)
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/backend/MySqlConstantWorker.py` & `pystratum_mysql-2.0.0/pystratum_mysql/backend/MySqlConstantWorker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import os
 import re
 from configparser import ConfigParser
 from typing import Any, Dict, Optional
 
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 from pystratum_common.backend.CommonConstantWorker import CommonConstantWorker
 from pystratum_common.Util import Util
 
 from pystratum_mysql.backend.MySqlWorker import MySqlWorker
 
 
 class MySqlConstantWorker(MySqlWorker, CommonConstantWorker):
     """
     Class for creating constants based on column widths, and auto increment columns and labels for MySQL databases.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, io: StratumStyle, config: ConfigParser):
+    def __init__(self, io: StratumIO, config: ConfigParser):
         """
         Object constructor.
 
-        :param PyStratumStyle io: The output decorator.
+        :param io: The output decorator.
         """
         MySqlWorker.__init__(self, io, config)
         CommonConstantWorker.__init__(self, io, config)
 
         self._columns: Dict[str, Any] = {}
         """
         All columns in the MySQL schema.
@@ -97,16 +97,16 @@
             else:
                 self._columns[row['table_name']] = {row['column_name']: row}
 
     # ------------------------------------------------------------------------------------------------------------------
     def _enhance_columns(self) -> None:
         """
         Enhances old_columns as follows:
-        If the constant name is *, is is replaced with the column name prefixed by prefix in uppercase.
-        Otherwise the constant name is set to uppercase.
+        If the constant name is *, it is replaced with the column name prefixed by prefix in uppercase.
+        Otherwise, the constant name is set to uppercase.
         """
         if self._old_columns:
             for table_name, table in sorted(self._old_columns.items()):
                 for column_name, column in sorted(table.items()):
                     table_name = column['table_name']
                     column_name = column['column_name']
 
@@ -196,17 +196,15 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def derive_field_length(column: Dict[str, Any]) -> Optional[int]:
         """
         Returns the width of a field based on column.
 
-        :param dict column: The column of which the field is based.
-
-        :rtype: int|None
+        :param column: The column of which the field is based.
         """
         types_length = {'tinyint':    column['numeric_precision'],
                         'smallint':   column['numeric_precision'],
                         'mediumint':  column['numeric_precision'],
                         'int':        column['numeric_precision'],
                         'bigint':     column['numeric_precision'],
                         'decimal':    column['numeric_precision'],
@@ -214,14 +212,15 @@
                         'double':     column['numeric_precision'],
                         'char':       column['character_maximum_length'],
                         'varchar':    column['character_maximum_length'],
                         'binary':     column['character_maximum_length'],
                         'varbinary':  column['character_maximum_length'],
                         'tinytext':   column['character_maximum_length'],
                         'text':       column['character_maximum_length'],
+                        'json':       column['character_maximum_length'],
                         'mediumtext': column['character_maximum_length'],
                         'longtext':   column['character_maximum_length'],
                         'tinyblob':   column['character_maximum_length'],
                         'blob':       column['character_maximum_length'],
                         'mediumblob': column['character_maximum_length'],
                         'longblob':   column['character_maximum_length'],
                         'bit':        column['character_maximum_length'],
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/backend/MySqlRoutineLoaderWorker.py` & `pystratum_mysql-2.0.0/pystratum_mysql/backend/MySqlRoutineLoaderWorker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from configparser import ConfigParser
 from typing import Any, Dict, List, Optional
 
-from pystratum_backend.StratumStyle import StratumStyle
-
+from pystratum_backend.StratumIO import StratumIO
 from pystratum_common.backend.CommonRoutineLoaderWorker import CommonRoutineLoaderWorker
+
 from pystratum_mysql.backend.MySqlWorker import MySqlWorker
 from pystratum_mysql.helper.MySqlRoutineLoaderHelper import MySqlRoutineLoaderHelper
 
 
 class MySqlRoutineLoaderWorker(MySqlWorker, CommonRoutineLoaderWorker):
     """
     Class for loading stored routines into a MySQL instance from (pseudo) SQL files.
@@ -29,19 +29,19 @@
 
     MAX_LENGTH_VARBINARY = 4096
     """
     Maximum length of a varbinary.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, io: StratumStyle, config: ConfigParser):
+    def __init__(self, io: StratumIO, config: ConfigParser):
         """
         Object constructor.
 
-        :param PyStratumStyle io: The output decorator.
+        :param io: The output decorator.
         """
         MySqlWorker.__init__(self, io, config)
         CommonRoutineLoaderWorker.__init__(self, io, config)
 
         self._character_set_client: Optional[str] = None
         """
         The default character set under which the stored routine will be loaded and run.
@@ -58,15 +58,15 @@
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     def __save_column_types_exact(self, rows: List[Dict[str, Any]]) -> None:
         """
         Saves the exact column types as replace pairs.
 
-        :param list[dict[str,*]] rows: The columns types.
+        :param rows: The column types.
         """
         for row in rows:
             key = row['table_name'] + '.' + row['column_name'] + '%type'
 
             value = row['column_type']
             if row['character_set_name']:
                 value += ' character set ' + row['character_set_name']
@@ -74,15 +74,15 @@
             self._add_replace_pair(key, value, False)
 
     # ------------------------------------------------------------------------------------------------------------------
     def __save_column_types_max_length(self, rows: List[Dict[str, Any]]) -> None:
         """
         Saves the column types with maximum length as replace pairs.
 
-        :param list[dict[str,*]] rows: The columns types.
+        :param rows: The column types.
         """
         for row in rows:
             key = row['table_name'] + '.' + row['column_name'] + '%max-type'
 
             if row['data_type'] == 'char':
                 value = row['data_type'] + '(' + str(self.MAX_LENGTH_CHAR) + ')'
                 value += ' character set ' + row['character_set_name']
@@ -116,19 +116,17 @@
     def create_routine_loader_helper(self,
                                      routine_name: str,
                                      pystratum_old_metadata: Optional[Dict],
                                      rdbms_old_metadata: Optional[Dict]) -> MySqlRoutineLoaderHelper:
         """
         Creates a Routine Loader Helper object.
 
-        :param str routine_name: The name of the routine.
-        :param dict pystratum_old_metadata: The old metadata of the stored routine from PyStratum.
-        :param dict rdbms_old_metadata:  The old metadata of the stored routine from MySQL.
-
-        :rtype: MySqlRoutineLoaderHelper
+        :param routine_name: The name of the routine.
+        :param pystratum_old_metadata: The old metadata of the stored routine from PyStratum.
+        :param rdbms_old_metadata:  The old metadata of the stored routine from MySQL.
         """
         return MySqlRoutineLoaderHelper(self._io,
                                         self._dl,
                                         self._source_file_names[routine_name],
                                         self._source_file_encoding,
                                         pystratum_old_metadata,
                                         self._replace_pairs,
@@ -168,12 +166,12 @@
     # ------------------------------------------------------------------------------------------------------------------
     def _read_configuration_file(self) -> None:
         """
         Reads parameters from the configuration file.
         """
         CommonRoutineLoaderWorker._read_configuration_file(self)
 
-        self._character_set_client = self._config.get('database', 'character_set_client', fallback='utf-8')
-        self._collation_connection = self._config.get('database', 'collation_connection', fallback='utf8_general_ci')
+        self._character_set_client = self._config.get('database', 'character_set_client', fallback='utf8mb4')
+        self._collation_connection = self._config.get('database', 'collation_connection', fallback='utf8mb4_general_ci')
         self._sql_mode = self._config.get('database', 'sql_mode')
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/backend/MySqlRoutineWrapperGeneratorWorker.py` & `pystratum_mysql-2.0.0/pystratum_mysql/backend/MySqlRoutineWrapperGeneratorWorker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from configparser import ConfigParser
 from typing import Any, Dict
 
-from pystratum_backend.StratumStyle import StratumStyle
-
+from pystratum_backend.StratumIO import StratumIO
 from pystratum_common.backend.CommonRoutineWrapperGeneratorWorker import CommonRoutineWrapperGeneratorWorker
+
 from pystratum_mysql.backend.MySqlWorker import MySqlWorker
 from pystratum_mysql.wrapper import create_routine_wrapper
 
 
 class MySqlRoutineWrapperGeneratorWorker(MySqlWorker, CommonRoutineWrapperGeneratorWorker):
     """
     Class for generating a class with wrapper methods for calling stored routines in a MySQL database.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, io: StratumStyle, config: ConfigParser):
+    def __init__(self, io: StratumIO, config: ConfigParser):
         """
         Object constructor.
 
-        :param PyStratumStyle io: The output decorator.
+        :param io: The output decorator.
         """
         MySqlWorker.__init__(self, io, config)
         CommonRoutineWrapperGeneratorWorker.__init__(self, io, config)
 
     # ------------------------------------------------------------------------------------------------------------------
     def _write_routine_function(self, routine: Dict[str, Any]) -> None:
         """
         Generates a complete wrapper method for a stored routine.
 
-        :param dict routine: The metadata of the stored routine.
+        :param routine: The metadata of the stored routine.
         """
         wrapper = create_routine_wrapper(routine, self._lob_as_string_flag)
         self._code += wrapper.write_routine_method(routine)
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/backend/MySqlWorker.py` & `pystratum_mysql-2.0.0/pystratum_mysql/backend/MySqlWorker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from configparser import ConfigParser
 from typing import Dict, Optional, Union
 
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 
 from pystratum_mysql.MySqlDefaultConnector import MySqlDefaultConnector
 from pystratum_mysql.MySqlMetadataDataLayer import MySqlMetadataDataLayer
 
 
 class MySqlWorker:
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, io: StratumStyle, config: ConfigParser):
+    def __init__(self, io: StratumIO, config: ConfigParser):
         """
         Object constructor.
 
-        :param PyStratumStyle io: The output decorator.
+        :param io: The output decorator.
         """
 
-        self._io: StratumStyle = io
+        self._io: StratumIO = io
         """
         The output decorator.
         """
 
         self._config: ConfigParser = config
         """
         The configuration object.
@@ -51,39 +51,35 @@
         Reads connections parameters from the configuration file.
         """
         params = {'host':      self.__get_option(self._config, 'database', 'host_name', fallback='localhost'),
                   'user':      self.__get_option(self._config, 'database', 'user'),
                   'password':  self.__get_option(self._config, 'database', 'password'),
                   'database':  self.__get_option(self._config, 'database', 'database'),
                   'port':      int(self.__get_option(self._config, 'database', 'port', fallback='3306')),
-                  'charset':   self.__get_option(self._config, 'database', 'character_set_client', fallback='utf-8'),
+                  'charset':   self.__get_option(self._config, 'database', 'character_set_client', fallback='utf8mb4'),
                   'collation': self.__get_option(self._config, 'database', 'collation_connection',
-                                                 fallback='utf8_general_ci'),
+                                                 fallback='utf8mb4_general_ci'),
                   'sql_mode':  self.__get_option(self._config, 'database', 'sql_mode')
                   }
 
         return params
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def __get_option(config: ConfigParser,
                      section: str,
                      option: str,
                      fallback: Optional[str] = None) -> str:
         """
         Reads an option for a configuration file.
 
-        :param configparser.ConfigParser config: The main config file.
-        :param str section: The name of the section op the option.
-        :param str option: The name of the option.
-        :param str|None fallback: The fallback value of the option if it is not set in either configuration files.
-
-        :rtype: str
-
-        :raise KeyError:
+        :param config: The main config file.
+        :param section: The name of the section op the option.
+        :param option: The name of the option.
+        :param fallback: The fallback value of the option if it is not set in either configuration files.
         """
         return_value = config.get(section, option, fallback=fallback)
 
         if fallback is None and return_value is None:
             raise KeyError("Option '{0!s}' is not found in section '{1!s}'.".format(option, section))
 
         return return_value
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/helper/MySqlDataTypeHelper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/helper/MySqlDataTypeHelper.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,17 @@
     """
     Utility class for deriving information based on a MySQL data type.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def column_type_to_python_type(self, data_type_info: Dict[str, Any]) -> str:
         """
-        Returns the corresponding Python data type of a MySQL data type.
+        Returns the corresponding Python data type of MySQL data type.
 
-        :param dict data_type_info: The MySQL data type metadata.
-
-        :rtype: str
+        :param data_type_info: The MySQL data type metadata.
         """
         if data_type_info['data_type'] in ['tinyint',
                                            'smallint',
                                            'mediumint',
                                            'int',
                                            'bigint',
                                            'year',
@@ -58,17 +56,15 @@
         raise RuntimeError('Unknown data type {0}'.format(data_type_info['data_type']))
 
     # ------------------------------------------------------------------------------------------------------------------
     def column_type_to_python_type_hint(self, data_type_info: Dict[str, Any]) -> str:
         """
         Returns the corresponding Python data type hinting of a MySQL data type.
 
-        :param dict data_type_info: The MySQL data type metadata.
-
-        :rtype: str
+        :param data_type_info: The MySQL data type metadata.
         """
         if data_type_info['data_type'] in ['tinyint',
                                            'smallint',
                                            'mediumint',
                                            'int',
                                            'bigint',
                                            'year',
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/helper/MySqlRoutineLoaderHelper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/helper/MySqlRoutineLoaderHelper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 import re
-from typing import Dict, Optional, Any
+from typing import Any, Dict, Optional
 
 from mysql import connector
-from pystratum_backend.StratumStyle import StratumStyle
-
+from pystratum_backend.StratumIO import StratumIO
 from pystratum_common.exception.LoaderException import LoaderException
 from pystratum_common.helper.DataTypeHelper import DataTypeHelper
 from pystratum_common.helper.RoutineLoaderHelper import RoutineLoaderHelper
+
 from pystratum_mysql.helper.MySqlDataTypeHelper import MySqlDataTypeHelper
 from pystratum_mysql.MySqlMetadataDataLayer import MySqlMetadataDataLayer
 
 
 class MySqlRoutineLoaderHelper(RoutineLoaderHelper):
     """
     Class for loading a single stored routine into a MySQL instance from a (pseudo) SQL file.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def __init__(self,
-                 io: StratumStyle,
+                 io: StratumIO,
                  dl: MySqlMetadataDataLayer,
                  routine_filename: str,
                  routine_file_encoding: str,
                  pystratum_old_metadata: Optional[Dict],
                  replace_pairs: Dict[str, Any],
                  rdbms_old_metadata: Optional[Dict],
                  sql_mode: str,
                  character_set: str,
                  collate: str):
         """
         Object constructor.
                                 
-        :param PyStratumStyle io: The output decorator.
-        :param MySqlMetadataDataLayer dl: The metadata layer.
-        :param str routine_filename: The filename of the source of the stored routine.
-        :param str routine_file_encoding: The encoding of the source file.
-        :param dict pystratum_old_metadata: The metadata of the stored routine from PyStratum.
-        :param dict[str,str] replace_pairs: A map from placeholders to their actual values.
-        :param dict rdbms_old_metadata: The old metadata of the stored routine from MS SQL Server.
-        :param str sql_mode: The SQL mode under which the stored routine must be loaded and run.
-        :param str character_set: The default character set under which the stored routine must be loaded and run.
-        :param str collate: The default collate under which the stored routine must be loaded and run.
+        :param io: The output decorator.
+        :param dl: The metadata layer.
+        :param routine_filename: The filename of the source of the stored routine.
+        :param routine_file_encoding: The encoding of the source file.
+        :param pystratum_old_metadata: The metadata of the stored routine from PyStratum.
+        :param replace_pairs: A map from placeholders to their actual values.
+        :param rdbms_old_metadata: The old metadata of the stored routine from MS SQL Server.
+        :param sql_mode: The SQL mode under which the stored routine must be loaded and run.
+        :param character_set: The default character set under which the stored routine must be loaded and run.
+        :param collate: The default collate under which the stored routine must be loaded and run.
         """
         RoutineLoaderHelper.__init__(self,
                                      io,
                                      routine_filename,
                                      routine_file_encoding,
                                      pystratum_old_metadata,
                                      replace_pairs,
@@ -60,15 +60,15 @@
         The default collate under which the stored routine will be loaded and run.
         """
 
         self._sql_mode: str = sql_mode
         """
         The SQL-mode under which the stored routine will be loaded and run.
         """
-        
+
         self._dl: MySqlMetadataDataLayer = dl
         """
         The metadata layer.
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_bulk_insert_table_columns_info(self) -> None:
@@ -104,16 +104,14 @@
         self._columns_types = tmp_column_types
         self._fields = tmp_fields
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_data_type_helper(self) -> DataTypeHelper:
         """
         Returns a data type helper object for MySQL.
-
-        :rtype: DataTypeHelper
         """
         return MySqlDataTypeHelper()
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_name(self) -> None:
         """
         Extracts the name of the stored routine and the stored routine type (i.e. procedure or function) source.
@@ -131,15 +129,15 @@
         if not self._routine_type:
             raise LoaderException('Unable to find the stored routine name and type in file {0}'.
                                   format(self._source_filename))
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_routine_parameters_info(self) -> None:
         """
-        Retrieves information about the stored routine parameters from the meta data of MySQL.
+        Retrieves information about the stored routine parameters from the metadata of MySQL.
         """
         routine_parameters = self._dl.get_routine_parameters(self._routine_name)
         for routine_parameter in routine_parameters:
             if routine_parameter['parameter_name']:
                 value = routine_parameter['column_type']
                 if 'character_set_name' in routine_parameter:
                     if routine_parameter['character_set_name']:
@@ -155,28 +153,24 @@
                                          'data_type_descriptor': value})
 
     # ------------------------------------------------------------------------------------------------------------------
     def _is_start_of_stored_routine(self, line: str) -> bool:
         """
         Returns True if a line is the start of the code of the stored routine.
 
-        :param str line: The line with source code of the stored routine.
-
-        :rtype: bool
+        :param line: The line with source code of the stored routine.
         """
         return re.match(r'^\s*create\s+(procedure|function)', line, re.IGNORECASE) is not None
 
     # ------------------------------------------------------------------------------------------------------------------
     def _is_start_of_stored_routine_body(self, line: str) -> bool:
         """
         Returns True if a line is the start of the body of the stored routine.
 
-        :param str line: The line with source code of the stored routine.
-
-        :rtype: bool
+        :param line: The line with source code of the stored routine.
         """
         return re.match(r'^\s*begin', line, re.IGNORECASE) is not None
 
     # ------------------------------------------------------------------------------------------------------------------
     def _load_routine_file(self) -> None:
         """
         Loads the stored routine into the MySQL instance.
@@ -193,15 +187,15 @@
         self._dl.execute_none(self._routine_source_code)
 
     # ------------------------------------------------------------------------------------------------------------------
     def _log_exception(self, exception: Exception) -> None:
         """
         Logs an exception.
 
-        :param Exception exception: The exception.
+        :param exception: The exception.
         """
         RoutineLoaderHelper._log_exception(self, exception)
 
         if isinstance(exception, connector.errors.Error):
             if exception.errno == 1064:
                 # Exception is caused by an invalid SQL statement.
                 sql = self._dl.last_sql()
@@ -215,17 +209,15 @@
                         error_line = 0
 
                     self._print_sql_with_error(sql, error_line)
 
     # ------------------------------------------------------------------------------------------------------------------
     def _must_reload(self) -> bool:
         """
-        Returns True if the source file must be load or reloaded. Otherwise returns False.
-
-        :rtype: bool
+        Returns whether the source file must be load or reloaded.
         """
         if not self._pystratum_old_metadata:
             return True
 
         if self._pystratum_old_metadata['timestamp'] != self._m_time:
             return True
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlBulkWrapper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlBulkWrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict
 
 from pystratum_common.wrapper.BulkWrapper import BulkWrapper
+
 from pystratum_mysql.wrapper.MySqlWrapper import MySqlWrapper
 
 
 class MySqlBulkWrapper(MySqlWrapper, BulkWrapper):
     """
     Wrapper method generator for stored procedures with large result sets.
     """
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlFunctionsWrapper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlRow0Wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from typing import Dict, Any
+from typing import Any, Dict
+
+from pystratum_common.wrapper.Row0Wrapper import Row0Wrapper
 
-from pystratum_common.wrapper.FunctionsWrapper import FunctionsWrapper
 from pystratum_mysql.wrapper.MySqlWrapper import MySqlWrapper
 
 
-class MySqlFunctionsWrapper(MySqlWrapper, FunctionsWrapper):
+class MySqlRow0Wrapper(MySqlWrapper, Row0Wrapper):
     """
-    Wrapper method generator for stored functions.
+    Wrapper method generator for stored procedures that are selecting 0 or 1 row.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _write_result_handler(self, routine: Dict[str, Any]) -> None:
-        self._write_line('return self.execute_singleton1({0!s})'.format(self._generate_command(routine)))
+        self._write_line('return self.execute_sp_row0({0!s})'.format(self._generate_command(routine)))
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlLogWrapper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlLogWrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict
 
 from pystratum_common.wrapper.LogWrapper import LogWrapper
+
 from pystratum_mysql.wrapper.MySqlWrapper import MySqlWrapper
 
 
 class MySqlLogWrapper(MySqlWrapper, LogWrapper):
     """
     Wrapper method generator for stored procedures with designation type log.
     """
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlMultiWrapper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlMultiWrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Dict, Any
+from typing import Any, Dict
 
 from pystratum_common.wrapper.MultiWrapper import MultiWrapper
+
 from pystratum_mysql.wrapper.MySqlWrapper import MySqlWrapper
 
 
 class MySqlMultiWrapper(MySqlWrapper, MultiWrapper):
     """
     Wrapper method generator for stored procedures with designation type multi.
     """
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlNoneWrapper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlNoneWrapper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Dict, Any
+from typing import Any, Dict
 
 from pystratum_common.wrapper.NoneWrapper import NoneWrapper
+
 from pystratum_mysql.wrapper.MySqlWrapper import MySqlWrapper
 
 
 class MySqlNoneWrapper(MySqlWrapper, NoneWrapper):
     """
     Wrapper method generator for stored procedures without any result set.
     """
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlRow0Wrapper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlSingleton0Wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from typing import Dict, Any
+from typing import Any, Dict
+
+from pystratum_common.wrapper.Singleton0Wrapper import Singleton0Wrapper
 
-from pystratum_common.wrapper.Row0Wrapper import Row0Wrapper
 from pystratum_mysql.wrapper.MySqlWrapper import MySqlWrapper
 
 
-class MySqlRow0Wrapper(MySqlWrapper, Row0Wrapper):
+class MySqlSingleton0Wrapper(MySqlWrapper, Singleton0Wrapper):
     """
-    Wrapper method generator for stored procedures that are selecting 0 or 1 row.
+    Wrapper method generator for stored procedures that are selecting 0 or 1 row with one column only.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _write_result_handler(self, routine: Dict[str, Any]) -> None:
-        self._write_line('return self.execute_sp_row0({0!s})'.format(self._generate_command(routine)))
+        self._write_line('return self.execute_sp_singleton0({0!s})'.format(self._generate_command(routine)))
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlRow1Wrapper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlRow1Wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict
 
 from pystratum_common.wrapper.Row1Wrapper import Row1Wrapper
+
 from pystratum_mysql.wrapper.MySqlWrapper import MySqlWrapper
 
 
 class MySqlRow1Wrapper(MySqlWrapper, Row1Wrapper):
     """
     Wrapper method generator for stored procedures that are selecting 1 row.
     """
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlRowsWithIndexWrapper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlRowsWithIndexWrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Dict, Any
+from typing import Any, Dict
 
 from pystratum_common.wrapper.RowsWithIndexWrapper import RowsWithIndexWrapper
+
 from pystratum_mysql.wrapper.MySqlWrapper import MySqlWrapper
 
 
 class MySqlRowsWithIndexWrapper(RowsWithIndexWrapper, MySqlWrapper):
     """
     Wrapper method generator for stored procedures whose result set must be returned using tree structure using a
     combination of non-unique columns.
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlRowsWithKeyWrapper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlRowsWithKeyWrapper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Dict, Any
+from typing import Any, Dict
 
 from pystratum_common.wrapper.RowsWithKeyWrapper import RowsWithKeyWrapper
+
 from pystratum_mysql.wrapper.MySqlWrapper import MySqlWrapper
 
 
 class MySqlRowsWithKeyWrapper(RowsWithKeyWrapper, MySqlWrapper):
     """
     Wrapper method generator for stored procedures whose result set must be returned using tree structure using a
     combination of unique columns.
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlRowsWrapper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlRowsWrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-from typing import Dict, Any
+from typing import Any, Dict
 
 from pystratum_common.wrapper.RowsWrapper import RowsWrapper
+
 from pystratum_mysql.wrapper.MySqlWrapper import MySqlWrapper
 
 
 class MySqlRowsWrapper(MySqlWrapper, RowsWrapper):
     """
     Wrapper method generator for stored procedures that are selecting 0, 1, or more rows.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
         return 'List[Dict[str, Any]]'
 
     # ------------------------------------------------------------------------------------------------------------------
     def _write_result_handler(self, routine: Dict[str, Any]) -> None:
         """
         Generates code for calling the stored routine in the wrapper method.
         """
         self._write_line('return self.execute_sp_rows({0!s})'.format(self._generate_command(routine)))
 
-
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlSingleton0Wrapper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlTableWrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from typing import Dict, Any
+from typing import Any, Dict
+
+from pystratum_common.wrapper.TableWrapper import TableWrapper
 
-from pystratum_common.wrapper.Singleton0Wrapper import Singleton0Wrapper
 from pystratum_mysql.wrapper.MySqlWrapper import MySqlWrapper
 
 
-class MySqlSingleton0Wrapper(MySqlWrapper, Singleton0Wrapper):
+class MySqlTableWrapper(MySqlWrapper, TableWrapper):
     """
-    Wrapper method generator for stored procedures that are selecting 0 or 1 row with one column only.
+    Wrapper method generator for printing the result set of stored procedures in a table format.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _write_result_handler(self, routine: Dict[str, Any]) -> None:
-        self._write_line('return self.execute_sp_singleton0({0!s})'.format(self._generate_command(routine)))
+        self._write_line('return self.execute_sp_table({0!s})'.format(self._generate_command(routine)))
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlSingleton1Wrapper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlSingleton1Wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import Dict, Any
+from typing import Any, Dict
 
 from pystratum_common.wrapper.Singleton1Wrapper import Singleton1Wrapper
+
 from pystratum_mysql.wrapper.MySqlWrapper import MySqlWrapper
 
 
 class MySqlSingleton1Wrapper(Singleton1Wrapper, MySqlWrapper):
     """
     Wrapper method generator for stored procedures that are selecting 1 row with one column only.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _write_result_handler(self, routine: Dict[str, Any]) -> None:
         self._write_line(
-            'return self.execute_sp_singleton1({0!s})'.format(str(self._generate_command(routine))))
+                'return self.execute_sp_singleton1({0!s})'.format(str(self._generate_command(routine))))
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/MySqlWrapper.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/MySqlWrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     def is_lob_parameter(self, parameters: List[Dict[str, Any]]) -> bool:
         """
         Returns True of one of the parameters is a BLOB or CLOB. Otherwise, returns False.
 
         :param parameters: The parameters of a stored routine.
-
-        :rtype: bool:
         """
         has_lob = False
 
         lookup = {'bigint':     False,
                   'binary':     False,
                   'bit':        False,
                   'char':       False,
@@ -61,15 +59,14 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     def _generate_command(self, routine: Dict[str, Any]) -> str:
         """
         Generates SQL statement for calling a stored routine.
 
         :param routine: Metadata of the stored routine.
-        :return: The generated SQL statement.
         """
         parameters = ''
         placeholders = ''
 
         execute = 'call'
         if routine['designation'] == 'function':
             execute = 'select'
@@ -98,17 +95,15 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def _get_parameter_format_specifier(data_type: str) -> str:
         """
         Returns the appropriate format specifier for a parameter type.
 
-        :param str data_type: The parameter type.
-
-        :rtype: str
+        :param data_type: The parameter type.
         """
         lookup = {'bigint':     '%s',
                   'binary':     '%s',
                   'bit':        '%s',
                   'blob':       '%s',
                   'char':       '%s',
                   'date':       '%s',
```

### Comparing `PyStratum-MySQL-1.2.0/pystratum_mysql/wrapper/__init__.py` & `pystratum_mysql-2.0.0/pystratum_mysql/wrapper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from pystratum_mysql.wrapper.MySqlRow0Wrapper import MySqlRow0Wrapper
 from pystratum_mysql.wrapper.MySqlRow1Wrapper import MySqlRow1Wrapper
 from pystratum_mysql.wrapper.MySqlRowsWithIndexWrapper import MySqlRowsWithIndexWrapper
 from pystratum_mysql.wrapper.MySqlRowsWithKeyWrapper import MySqlRowsWithKeyWrapper
 from pystratum_mysql.wrapper.MySqlRowsWrapper import MySqlRowsWrapper
 from pystratum_mysql.wrapper.MySqlSingleton0Wrapper import MySqlSingleton0Wrapper
 from pystratum_mysql.wrapper.MySqlSingleton1Wrapper import MySqlSingleton1Wrapper
-
-
 # ----------------------------------------------------------------------------------------------------------------------
 from pystratum_mysql.wrapper.MySqlWrapper import MySqlWrapper
 
 
 def create_routine_wrapper(routine: Dict[str, Any], lob_as_string_flag: bool) -> MySqlWrapper:
     """
     A factory for creating the appropriate object for generating a wrapper method for a stored routine.
```

