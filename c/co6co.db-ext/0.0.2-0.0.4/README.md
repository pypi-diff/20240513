# Comparing `tmp/co6co.db_ext-0.0.2.tar.gz` & `tmp/co6co.db_ext-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "co6co.db_ext-0.0.2.tar", last modified: Thu Nov  2 07:56:47 2023, max compression
+gzip compressed data, was "co6co.db_ext-0.0.4.tar", last modified: Sat May 11 06:45:15 2024, max compression
```

## Comparing `co6co.db_ext-0.0.2.tar` & `co6co.db_ext-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-11-02 07:56:47.320042 co6co.db_ext-0.0.2/
--rw-rw-rw-   0        0        0      572 2023-11-02 07:56:47.319043 co6co.db_ext-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-11-02 07:44:13.000000 co6co.db_ext-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-11-02 07:56:47.290053 co6co.db_ext-0.0.2/co6co.db_ext.egg-info/
--rw-rw-rw-   0        0        0      572 2023-11-02 07:56:47.000000 co6co.db_ext-0.0.2/co6co.db_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-11-02 07:56:47.000000 co6co.db_ext-0.0.2/co6co.db_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-02 07:56:47.000000 co6co.db_ext-0.0.2/co6co.db_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-11-02 07:56:47.000000 co6co.db_ext-0.0.2/co6co.db_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-11-02 03:04:33.000000 co6co.db_ext-0.0.2/co6co.db_ext.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-11-02 07:56:47.318043 co6co.db_ext-0.0.2/co6co_db_ext/
--rw-rw-rw-   0        0        0      107 2023-11-02 07:53:20.000000 co6co.db_ext-0.0.2/co6co_db_ext/__init__.py
--rw-rw-rw-   0        0        0     1879 2023-11-02 03:35:15.000000 co6co.db_ext-0.0.2/co6co_db_ext/db_filter.py
--rw-rw-rw-   0        0        0     6824 2023-11-02 03:54:42.000000 co6co.db_ext-0.0.2/co6co_db_ext/db_operations.py
--rw-rw-rw-   0        0        0      286 2023-10-25 06:57:11.000000 co6co.db_ext-0.0.2/co6co_db_ext/page_param.py
--rw-rw-rw-   0        0        0       42 2023-11-02 07:56:47.320042 co6co.db_ext-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1113 2023-11-02 03:03:45.000000 co6co.db_ext-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:45:15.789774 co6co.db_ext-0.0.4/
+-rw-rw-rw-   0        0        0      803 2024-05-11 06:45:15.787774 co6co.db_ext-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2024-01-02 01:24:42.000000 co6co.db_ext-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 06:45:15.651554 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/
+-rw-rw-rw-   0        0        0      803 2024-05-11 06:45:15.000000 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2024-05-11 06:45:15.000000 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 06:45:15.000000 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-11 06:45:15.000000 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-11 06:45:15.000000 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-11-02 03:04:33.000000 co6co.db_ext-0.0.4/co6co.db_ext.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-05-11 06:45:15.741127 co6co.db_ext-0.0.4/co6co_db_ext/
+-rw-rw-rw-   0        0        0      107 2024-05-11 06:45:12.000000 co6co.db_ext-0.0.4/co6co_db_ext/__init__.py
+-rw-rw-rw-   0        0        0     3496 2024-04-18 06:28:14.000000 co6co.db_ext-0.0.4/co6co_db_ext/db_filter.py
+-rw-rw-rw-   0        0        0    10492 2024-04-22 08:45:51.000000 co6co.db_ext-0.0.4/co6co_db_ext/db_operations.py
+-rw-rw-rw-   0        0        0     3531 2024-04-25 07:12:39.000000 co6co.db_ext-0.0.4/co6co_db_ext/db_session.py
+-rw-rw-rw-   0        0        0     8686 2024-05-07 08:54:23.000000 co6co.db_ext-0.0.4/co6co_db_ext/db_utils.py
+-rw-rw-rw-   0        0        0      423 2023-12-19 08:04:36.000000 co6co.db_ext-0.0.4/co6co_db_ext/page_param.py
+-rw-rw-rw-   0        0        0     1648 2024-05-06 02:10:40.000000 co6co.db_ext-0.0.4/co6co_db_ext/po.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:45:15.785775 co6co.db_ext-0.0.4/co6co_db_ext/res/
+-rw-rw-rw-   0        0        0        0 2023-11-27 04:01:15.000000 co6co.db_ext-0.0.4/co6co_db_ext/res/__init__.py
+-rw-rw-rw-   0        0        0     2554 2023-12-15 03:43:22.000000 co6co.db_ext-0.0.4/co6co_db_ext/res/result.py
+-rw-rw-rw-   0        0        0       42 2024-05-11 06:45:15.789774 co6co.db_ext-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1144 2023-11-20 01:33:12.000000 co6co.db_ext-0.0.4/setup.py
```

### Comparing `co6co.db_ext-0.0.2/setup.py` & `co6co.db_ext-0.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     description="db 数据库扩展",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[ "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.6" ],
     include_package_data=True, zip_safe=True,
     #依赖哪些模块
-    install_requires=[ ],
+    install_requires=["co6co","aiomysql","SQLAlchemy" ],
     #package_dir= {'utils':'src/log','main_package':'main'},#告诉Distutils哪些目录下的文件被映射到哪个源码
     author='co6co',
     author_email ='co6co@qq.com',
     url="http://github.com/co6co",
     data_file={
         ('',"*.txt"),
         ('',"*.md"),
```

