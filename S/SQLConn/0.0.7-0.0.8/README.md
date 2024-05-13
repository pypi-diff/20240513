# Comparing `tmp/SQLConn-0.0.7.tar.gz` & `tmp/SQLConn-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLConn-0.0.7.tar", last modified: Fri May 10 05:38:09 2024, max compression
+gzip compressed data, was "SQLConn-0.0.8.tar", last modified: Mon May 13 02:14:36 2024, max compression
```

## Comparing `SQLConn-0.0.7.tar` & `SQLConn-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 05:38:09.232230 SQLConn-0.0.7/
--rw-rw-rw-   0        0        0    10415 2024-05-10 05:38:09.231228 SQLConn-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     9975 2024-05-10 05:36:53.000000 SQLConn-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 05:38:09.226233 SQLConn-0.0.7/SQLConn/
--rw-rw-rw-   0        0        0     5583 2024-05-06 10:21:39.000000 SQLConn-0.0.7/SQLConn/SQLConn.py
--rw-rw-rw-   0        0        0      293 2024-05-06 09:40:40.000000 SQLConn-0.0.7/SQLConn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:38:09.230234 SQLConn-0.0.7/SQLConn.egg-info/
--rw-rw-rw-   0        0        0    10415 2024-05-10 05:38:09.000000 SQLConn-0.0.7/SQLConn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2024-05-10 05:38:09.000000 SQLConn-0.0.7/SQLConn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 05:38:09.000000 SQLConn-0.0.7/SQLConn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-10 05:38:09.000000 SQLConn-0.0.7/SQLConn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-10 05:38:09.000000 SQLConn-0.0.7/SQLConn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 05:38:09.232230 SQLConn-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      650 2024-05-10 04:21:28.000000 SQLConn-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:14:36.890690 SQLConn-0.0.8/
+-rw-rw-rw-   0        0        0    10743 2024-05-13 02:14:36.889696 SQLConn-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    10235 2024-05-13 02:11:10.000000 SQLConn-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 02:14:36.882692 SQLConn-0.0.8/SQLConn/
+-rw-rw-rw-   0        0        0     5583 2024-05-06 10:21:39.000000 SQLConn-0.0.8/SQLConn/SQLConn.py
+-rw-rw-rw-   0        0        0      293 2024-05-06 09:40:40.000000 SQLConn-0.0.8/SQLConn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:14:36.888691 SQLConn-0.0.8/SQLConn.egg-info/
+-rw-rw-rw-   0        0        0    10743 2024-05-13 02:14:36.000000 SQLConn-0.0.8/SQLConn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2024-05-13 02:14:36.000000 SQLConn-0.0.8/SQLConn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:14:36.000000 SQLConn-0.0.8/SQLConn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-13 02:14:36.000000 SQLConn-0.0.8/SQLConn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 02:14:36.000000 SQLConn-0.0.8/SQLConn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:14:36.890690 SQLConn-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      774 2024-05-13 02:14:28.000000 SQLConn-0.0.8/setup.py
```

### Comparing `SQLConn-0.0.7/PKG-INFO` & `SQLConn-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: SQLConn
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package facilitates easy SQL database integration.
 Home-page: https://github.com/janyoungjin/SQLConn
 Author: janyoungjin
 Keywords: mysql,postgresql,sqlite,mssql,oracle,sql
 Description-Content-Type: text/markdown
-Requires-Dist: mysqlclient
 Requires-Dist: pandas
-Requires-Dist: cx_oracle
-Requires-Dist: psycopg2
-Requires-Dist: pymssql
 Requires-Dist: sqlalchemy
+Requires-Dist: MySQL-python
+Requires-Dist: pymssql
+Requires-Dist: psycopg2
+Requires-Dist: sqlite3
+Provides-Extra: oracle
+Requires-Dist: cx_Oracle; extra == "oracle"
 
 # SQLConn
 
 ## 한국어 버전(Korean Version)
 
 SQLConn은 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하여 데이터를 쉽게 조작하고 관리할 수 있는 Python 패키지입니다. 이 패키지는 MySQL, PostgreSQL, Microsoft SQL Server, Oracle 및 SQLite 데이터베이스에 대한 지원을 포함합니다.
 
@@ -39,14 +41,20 @@
 
 파이썬과 pip가 설치된 환경에서 다음 명령어를 통해 `SQLConn` 패키지를 설치할 수 있습니다:
 
 ```bash
 pip install SQLConn
 ```
 
+만약 OracleConn클래스를 쓰고 싶다면 아래와 같이 설치해야합니다:
+
+```bash
+pip install SQLConn['oracle']
+```
+
 ### 클래스 소개
 
 | 클래스명           | 소개                                                                    | 특이 사항                   |
 | ------------------ | ----------------------------------------------------------------------- | --------------------------- |
 | `SQLConn`        | 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하기 위한 클래스입니다. | 추상 클래스입니다.          |
 | `MYSQLConn`      | MySQL 데이터베이스와의 연결을 관리합니다.                               | SQLConn에게 상속 받았습니다 |
 | `MSSQLConn`      | Microsoft SQL Server 데이터베이스와의 연결을 관리합니다.                | SQLConn에게 상속 받았습니다 |
@@ -141,14 +149,20 @@
 
 In an environment where Python and pip are installed, you can install the `SQLConn` package using the following command:
 
 ```bash
 pip install SQLConn
 ```
 
+If you want to use the OracleConn class, you must install it as follows:
+
+```bash
+pip install SQLConn['oracle']
+```
+
 ### class info
 
 | class name         | info                                                                    | significant              |
 | ------------------ | ----------------------------------------------------------------------- | ------------------------ |
 | `SQLConn`        | Class for connecting to various SQL database management systems (DBMS). | It is an abstract class. |
 | `MYSQLConn`      | Manages MySQL database relationships.                                   | protected  SQLConn       |
 | `MSSQLConn`      | Manages connections to Microsoft SQL Server databases.                  | protected  SQLConn       |
```

### Comparing `SQLConn-0.0.7/README.md` & `SQLConn-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
 파이썬과 pip가 설치된 환경에서 다음 명령어를 통해 `SQLConn` 패키지를 설치할 수 있습니다:
 
 ```bash
 pip install SQLConn
 ```
 
+만약 OracleConn클래스를 쓰고 싶다면 아래와 같이 설치해야합니다:
+
+```bash
+pip install SQLConn['oracle']
+```
+
 ### 클래스 소개
 
 | 클래스명           | 소개                                                                    | 특이 사항                   |
 | ------------------ | ----------------------------------------------------------------------- | --------------------------- |
 | `SQLConn`        | 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하기 위한 클래스입니다. | 추상 클래스입니다.          |
 | `MYSQLConn`      | MySQL 데이터베이스와의 연결을 관리합니다.                               | SQLConn에게 상속 받았습니다 |
 | `MSSQLConn`      | Microsoft SQL Server 데이터베이스와의 연결을 관리합니다.                | SQLConn에게 상속 받았습니다 |
@@ -126,14 +132,20 @@
 
 In an environment where Python and pip are installed, you can install the `SQLConn` package using the following command:
 
 ```bash
 pip install SQLConn
 ```
 
+If you want to use the OracleConn class, you must install it as follows:
+
+```bash
+pip install SQLConn['oracle']
+```
+
 ### class info
 
 | class name         | info                                                                    | significant              |
 | ------------------ | ----------------------------------------------------------------------- | ------------------------ |
 | `SQLConn`        | Class for connecting to various SQL database management systems (DBMS). | It is an abstract class. |
 | `MYSQLConn`      | Manages MySQL database relationships.                                   | protected  SQLConn       |
 | `MSSQLConn`      | Manages connections to Microsoft SQL Server databases.                  | protected  SQLConn       |
```

### Comparing `SQLConn-0.0.7/SQLConn/SQLConn.py` & `SQLConn-0.0.8/SQLConn/SQLConn.py`

 * *Files identical despite different names*

### Comparing `SQLConn-0.0.7/SQLConn.egg-info/PKG-INFO` & `SQLConn-0.0.8/SQLConn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: SQLConn
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package facilitates easy SQL database integration.
 Home-page: https://github.com/janyoungjin/SQLConn
 Author: janyoungjin
 Keywords: mysql,postgresql,sqlite,mssql,oracle,sql
 Description-Content-Type: text/markdown
-Requires-Dist: mysqlclient
 Requires-Dist: pandas
-Requires-Dist: cx_oracle
-Requires-Dist: psycopg2
-Requires-Dist: pymssql
 Requires-Dist: sqlalchemy
+Requires-Dist: MySQL-python
+Requires-Dist: pymssql
+Requires-Dist: psycopg2
+Requires-Dist: sqlite3
+Provides-Extra: oracle
+Requires-Dist: cx_Oracle; extra == "oracle"
 
 # SQLConn
 
 ## 한국어 버전(Korean Version)
 
 SQLConn은 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하여 데이터를 쉽게 조작하고 관리할 수 있는 Python 패키지입니다. 이 패키지는 MySQL, PostgreSQL, Microsoft SQL Server, Oracle 및 SQLite 데이터베이스에 대한 지원을 포함합니다.
 
@@ -39,14 +41,20 @@
 
 파이썬과 pip가 설치된 환경에서 다음 명령어를 통해 `SQLConn` 패키지를 설치할 수 있습니다:
 
 ```bash
 pip install SQLConn
 ```
 
+만약 OracleConn클래스를 쓰고 싶다면 아래와 같이 설치해야합니다:
+
+```bash
+pip install SQLConn['oracle']
+```
+
 ### 클래스 소개
 
 | 클래스명           | 소개                                                                    | 특이 사항                   |
 | ------------------ | ----------------------------------------------------------------------- | --------------------------- |
 | `SQLConn`        | 다양한 SQL 데이터베이스 관리 시스템(DBMS)에 연결하기 위한 클래스입니다. | 추상 클래스입니다.          |
 | `MYSQLConn`      | MySQL 데이터베이스와의 연결을 관리합니다.                               | SQLConn에게 상속 받았습니다 |
 | `MSSQLConn`      | Microsoft SQL Server 데이터베이스와의 연결을 관리합니다.                | SQLConn에게 상속 받았습니다 |
@@ -141,14 +149,20 @@
 
 In an environment where Python and pip are installed, you can install the `SQLConn` package using the following command:
 
 ```bash
 pip install SQLConn
 ```
 
+If you want to use the OracleConn class, you must install it as follows:
+
+```bash
+pip install SQLConn['oracle']
+```
+
 ### class info
 
 | class name         | info                                                                    | significant              |
 | ------------------ | ----------------------------------------------------------------------- | ------------------------ |
 | `SQLConn`        | Class for connecting to various SQL database management systems (DBMS). | It is an abstract class. |
 | `MYSQLConn`      | Manages MySQL database relationships.                                   | protected  SQLConn       |
 | `MSSQLConn`      | Manages connections to Microsoft SQL Server databases.                  | protected  SQLConn       |
```

