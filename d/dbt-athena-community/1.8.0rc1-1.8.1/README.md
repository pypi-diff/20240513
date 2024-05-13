# Comparing `tmp/dbt_athena_community-1.8.0rc1.tar.gz` & `tmp/dbt_athena_community-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_athena_community-1.8.0rc1.tar", last modified: Tue May  7 07:24:18 2024, max compression
+gzip compressed data, was "dbt_athena_community-1.8.1.tar", last modified: Mon May 13 10:49:12 2024, max compression
```

## Comparing `dbt_athena_community-1.8.0rc1.tar` & `dbt_athena_community-1.8.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.745608 dbt_athena_community-1.8.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    33196 2024-05-07 07:24:18.745608 dbt_athena_community-1.8.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32051 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.733608 dbt_athena_community-1.8.0rc1/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.733608 dbt_athena_community-1.8.0rc1/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.737608 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57310 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/lakeformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.733608 dbt_athena_community-1.8.0rc1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.737608 dbt_athena_community-1.8.0rc1/dbt/include/athena/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.733608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.737608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/python_submissions.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.737608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.733608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.741608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.741608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.741608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.741608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.741608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.741608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.745608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/ddl_dml_data_type.sql
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/profile_template.yml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.745608 dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    33196 2024-05-07 07:24:18.000000 dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-07 07:24:18.000000 dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:24:18.000000 dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 07:24:18.000000 dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 07:24:18.000000 dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:24:18.745608 dbt_athena_community-1.8.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.955687 dbt_athena_community-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    34898 2024-05-13 10:49:12.955687 dbt_athena_community-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33725 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.943687 dbt_athena_community-1.8.1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.943687 dbt_athena_community-1.8.1/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.943687 dbt_athena_community-1.8.1/dbt/adapters/athena/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    58912 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/lakeformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.939687 dbt_athena_community-1.8.1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.947687 dbt_athena_community-1.8.1/dbt/include/athena/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.939687 dbt_athena_community-1.8.1/dbt/include/athena/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.947687 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/python_submissions.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.947687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.939687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.947687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.947687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.947687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.951687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.951687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.951687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.951687 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/ddl_dml_data_type.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/profile_template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.955687 dbt_athena_community-1.8.1/dbt_athena_community.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34898 2024-05-13 10:49:12.000000 dbt_athena_community-1.8.1/dbt_athena_community.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-13 10:49:12.000000 dbt_athena_community-1.8.1/dbt_athena_community.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:49:12.000000 dbt_athena_community-1.8.1/dbt_athena_community.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-13 10:49:12.000000 dbt_athena_community-1.8.1/dbt_athena_community.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-13 10:49:12.000000 dbt_athena_community-1.8.1/dbt_athena_community.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:49:12.955687 dbt_athena_community-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/setup.py
```

### Comparing `dbt_athena_community-1.8.0rc1/LICENSE.txt` & `dbt_athena_community-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/PKG-INFO` & `dbt_athena_community-1.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-athena-community
-Version: 1.8.0rc1
+Version: 1.8.1
 Summary: The athena adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-athena/dbt-athena
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: dbt-common<2.0,>=1.0.0b2
 Requires-Dist: dbt-adapters<2.0,>=1.0.0b2
+Requires-Dist: dbt-core>=1.8.0
 Requires-Dist: boto3>=1.28
 Requires-Dist: boto3-stubs[athena,glue,lakeformation,sts]>=1.28
 Requires-Dist: pyathena<4.0,>=2.25
 Requires-Dist: mmh3<4.2.0,>=4.0.1
 Requires-Dist: pydantic<3.0,>=1.10
 Requires-Dist: tenacity~=8.2
 
@@ -58,21 +59,23 @@
     - [Table Configuration](#table-configuration)
     - [Table location](#table-location)
     - [Incremental models](#incremental-models)
     - [On schema change](#on-schema-change)
     - [Iceberg](#iceberg)
     - [Highly available table (HA)](#highly-available-table-ha)
       - [HA Known issues](#ha-known-issues)
+    - [Update glue data catalog](#update-glue-data-catalog)
   - [Snapshots](#snapshots)
     - [Timestamp strategy](#timestamp-strategy)
     - [Check strategy](#check-strategy)
     - [Hard-deletes](#hard-deletes)
-    - [AWS Lakeformation integration](#aws-lakeformation-integration)
     - [Working example](#working-example)
     - [Snapshots Known issues](#snapshots-known-issues)
+  - [AWS Lakeformation integration](#aws-lakeformation-integration)
+  - [Python Models](#python-models)
   - [Contracts](#contracts)
   - [Contributing](#contributing)
   - [Contributors ✨](#contributors-)
 <!-- TOC -->
 
 # Features
 
@@ -302,15 +305,15 @@
                       'principals': ['principal_arn1', 'principal_arn2']
                   }
               }
           }
       }
   ```
 
-> Notes:  
+> Notes:
 >
 > - `lf_tags` and `lf_tags_columns` configs support only attaching lf tags to corresponding resources.
 > We recommend managing LF Tags permissions somewhere outside dbt. For example, you may use
 > [terraform](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions) or
 > [aws cdk](https://docs.aws.amazon.com/cdk/api/v1/docs/aws-lakeformation-readme.html) for such purpose.
 > - `data_cell_filters` management can't be automated outside dbt because the filter can't be attached to the table
 > which doesn't exist. Once you `enable` this config, dbt will set all filters and their permissions during every
@@ -530,14 +533,42 @@
 
 - When swapping from a table with partitions to a table without (and the other way around), there could be a little
   downtime.
   In case high performances are needed consider bucketing instead of partitions
 - By default, Glue "duplicates" the versions internally, so the last two versions of a table point to the same location
 - It's recommended to have `versions_to_keep` >= 4, as this will avoid having the older location removed
 
+### Update glue data catalog
+
+Optionally persist resource descriptions as column and relation comments to the glue data catalog, and meta as
+[glue table properties](https://docs.aws.amazon.com/glue/latest/dg/tables-described.html#table-properties)
+and [column parameters](https://docs.aws.amazon.com/glue/latest/webapi/API_Column.html).
+By default, documentation persistence is disabled, but it can be enabled for specific resources or
+groups of resources as needed.
+
+For example:
+
+```yaml
+models:
+  - name: test_deduplicate
+    description: another value
+    config:
+      persist_docs:
+        relation: true
+        columns: true
+      meta:
+        test: value
+    columns:
+      - name: id
+        meta:
+          primary_key: true
+```
+
+See [persist docs](https://docs.getdbt.com/reference/resource-configs/persist_docs) for more details.
+
 ## Snapshots
 
 The adapter supports snapshot materialization. It supports both timestamp and check strategy. To create a snapshot
 create a snapshot file in the snapshots directory. If the directory does not exist create one.
 
 ### Timestamp strategy
 
@@ -549,74 +580,181 @@
 To use the check strategy refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy)
 
 ### Hard-deletes
 
 The materialization also supports invalidating hard deletes. Check
 the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to understand usage.
 
-### AWS Lakeformation integration
+### Working example
+
+seed file - employent_indicators_november_2022_csv_tables.csv
+
+```csv
+Series_reference,Period,Data_value,Suppressed
+MEIM.S1WA,1999.04,80267,
+MEIM.S1WA,1999.05,70803,
+MEIM.S1WA,1999.06,65792,
+MEIM.S1WA,1999.07,66194,
+MEIM.S1WA,1999.08,67259,
+MEIM.S1WA,1999.09,69691,
+MEIM.S1WA,1999.1,72475,
+MEIM.S1WA,1999.11,79263,
+MEIM.S1WA,1999.12,86540,
+MEIM.S1WA,2000.01,82552,
+MEIM.S1WA,2000.02,81709,
+MEIM.S1WA,2000.03,84126,
+MEIM.S1WA,2000.04,77089,
+MEIM.S1WA,2000.05,73811,
+MEIM.S1WA,2000.06,70070,
+MEIM.S1WA,2000.07,69873,
+MEIM.S1WA,2000.08,71468,
+MEIM.S1WA,2000.09,72462,
+MEIM.S1WA,2000.1,74897,
+```
+
+model.sql
+
+```sql
+{{ config(
+    materialized='table'
+) }}
+
+select row_number() over() as id
+       , *
+       , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) as refresh_timestamp
+from {{ ref('employment_indicators_november_2022_csv_tables') }}
+```
+
+timestamp strategy - model_snapshot_1
+
+```sql
+{% snapshot model_snapshot_1 %}
+
+{{
+    config(
+      strategy='timestamp',
+      updated_at='refresh_timestamp',
+      unique_key='id'
+    )
+}}
+
+select *
+from {{ ref('model') }} {% endsnapshot %}
+```
+
+invalidate hard deletes - model_snapshot_2
+
+```sql
+{% snapshot model_snapshot_2 %}
+
+{{
+    config
+    (
+        unique_key='id',
+        strategy='timestamp',
+        updated_at='refresh_timestamp',
+        invalidate_hard_deletes=True,
+    )
+}}
+select *
+from {{ ref('model') }} {% endsnapshot %}
+```
+
+check strategy - model_snapshot_3
+
+```sql
+{% snapshot model_snapshot_3 %}
+
+{{
+    config
+    (
+        unique_key='id',
+        strategy='check',
+        check_cols=['series_reference','data_value']
+    )
+}}
+select *
+from {{ ref('model') }} {% endsnapshot %}
+```
+
+### Snapshots Known issues
+
+- Incremental Iceberg models - Sync all columns on schema change can't remove columns used as partitioning.
+  The only way, from a dbt perspective, is to do a full-refresh of the incremental model.
+
+- Tables, schemas and database should only be lowercase
+
+- In order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/dbt-athena) is not
+  installed in the target environment.
+  See <https://github.com/dbt-athena/dbt-athena/issues/103> for more details.
+
+- Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column
+  from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
+
+## AWS Lakeformation integration
 
 The adapter implements AWS Lakeformation tags management in the following way:
 
 - you can enable or disable lf-tags management via [config](#table-configuration) (disabled by default)
 - once you enable the feature, lf-tags will be updated on every dbt run
 - first, all lf-tags for columns are removed to avoid inheritance issues
 - then all redundant lf-tags are removed from table and actual tags from config are applied
 - finally, lf-tags for columns are applied
 
 It's important to understand the following points:
 
 - dbt does not manage lf-tags for database
 - dbt does not manage lakeformation permissions
 
-That's why you should handle this by yourself manually or using some automation tools like terraform, AWS CDK etc.  
+That's why you should handle this by yourself manually or using some automation tools like terraform, AWS CDK etc.
 You may find the following links useful to manage that:
 
 <!-- markdownlint-disable -->
 * [terraform aws_lakeformation_permissions](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions)
 * [terraform aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags)
 <!-- markdownlint-restore -->
 
 ## Python Models
 
 The adapter supports python models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
 
 ### Setup
 
-- A spark enabled work group created in athena
+- A Spark-enabled workgroup created in Athena
 - Spark execution role granted access to Athena, Glue and S3
-- The spark work group is added to the ~/.dbt/profiles.yml file and the profile is referenced in dbt_project.yml
-  that will be created. It is recommended to keep this same as threads.
+- The Spark workgroup is added to the `~/.dbt/profiles.yml` file and the profile
+ is referenced in `dbt_project.yml` that will be created. It is recommended to keep this same as threads.
 
-### Spark specific table configuration
+### Spark-specific table configuration
 
 - `timeout` (`default=43200`)
-  - Time out in seconds for each python model execution. Defaults to 12 hours/43200 seconds.
+  - Time out in seconds for each Python model execution. Defaults to 12 hours/43200 seconds.
 - `spark_encryption` (`default=false`)
   - If this flag is set to true, encrypts data in transit between Spark nodes and also encrypts data at rest stored
    locally by Spark.
 - `spark_cross_account_catalog` (`default=false`)
-  - In spark, you can query the external account catalog and for that the consumer account has to be configured to
+  - In Spark, you can query the external account catalog and for that the consumer account has to be configured to
    access the producer catalog.
   - If this flag is set to true, "/" can be used as the glue catalog separator.
-   Ex: 999999999999/mydatabase.cloudfront_logs (*where *999999999999* is the external catalog id*)
+   Ex: 999999999999/mydatabase.cloudfront_logs (*where *999999999999* is the external catalog ID*)
 - `spark_requester_pays` (`default=false`)
   - When an Amazon S3 bucket is configured as requester pays, the account of the user running the query is charged for
    data access and data transfer fees associated with the query.
   - If this flag is set to true, requester pays S3 buckets are enabled in Athena for Spark.
 
 ### Spark notes
 
 - A session is created for each unique engine configuration defined in the models that are part of the invocation.
 - A session's idle timeout is set to 10 minutes. Within the timeout period, if there is a new calculation
- (spark python model) ready for execution and the engine configuration matches, the process will reuse the same session.
-- Number of python models running at a time depends on the `threads`.  Number of sessions created for the entire run
- depends on number of unique engine configurations and availability of session to maintain threads concurrency.
-- For iceberg table, it is recommended to use table_properties configuration to set the format_version to 2. This is to
- maintain compatability between iceberg tables created by Trino with those created by Spark.
+ (Spark Python model) ready for execution and the engine configuration matches, the process will reuse the same session.
+- The number of Python models running at a time depends on the `threads`. The number of sessions created for the
+ entire run depends on the number of unique engine configurations and the availability of sessions to maintain
+ thread concurrency.
+- For Iceberg tables, it is recommended to use `table_properties` configuration to set the `format_version` to 2.
+ This is to maintain compatibility between Iceberg tables created by Trino with those created by Spark.
 
 ### Example models
 
 #### Simple pandas model
 
 ```python
 import pandas as pd
@@ -710,126 +848,30 @@
     data = [(1, "a"), (2, "b"), (3, "c")]
     cols = ["num", "alpha"]
     df = spark_session.createDataFrame(data, cols)
 
     return df.withColumn("udf_test_col", udf_with_import(col("alpha")))
 ```
 
-#### Known issues in python models
+### Known issues in Python models
 
-- Incremental models do not fully utilize spark capabilities. They depend partially on existing sql based logic which
- runs on trino.
-- Snapshots materializations are not supported.
+- Python models cannot
+ [reference Athena SQL views](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
+- Third-party Python libraries can be used, but they must be [included in the pre-installed list]([pre-installed list])
+ or [imported manually]([imported manually]).
+- Python models can only reference or write to tables with names meeting the
+ regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special characters are not
+ supported by Spark, even though Athena supports them.
+- Incremental models do not fully utilize Spark capabilities. They depend partially on existing SQL-based logic which
+ runs on Trino.
+- Snapshot materializations are not supported.
 - Spark can only reference tables within the same catalog.
 
-### Working example
-
-seed file - employent_indicators_november_2022_csv_tables.csv
-
-```csv
-Series_reference,Period,Data_value,Suppressed
-MEIM.S1WA,1999.04,80267,
-MEIM.S1WA,1999.05,70803,
-MEIM.S1WA,1999.06,65792,
-MEIM.S1WA,1999.07,66194,
-MEIM.S1WA,1999.08,67259,
-MEIM.S1WA,1999.09,69691,
-MEIM.S1WA,1999.1,72475,
-MEIM.S1WA,1999.11,79263,
-MEIM.S1WA,1999.12,86540,
-MEIM.S1WA,2000.01,82552,
-MEIM.S1WA,2000.02,81709,
-MEIM.S1WA,2000.03,84126,
-MEIM.S1WA,2000.04,77089,
-MEIM.S1WA,2000.05,73811,
-MEIM.S1WA,2000.06,70070,
-MEIM.S1WA,2000.07,69873,
-MEIM.S1WA,2000.08,71468,
-MEIM.S1WA,2000.09,72462,
-MEIM.S1WA,2000.1,74897,
-```
-
-model.sql
-
-```sql
-{{ config(
-    materialized='table'
-) }}
-
-select row_number() over() as id
-       , *
-       , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) as refresh_timestamp
-from {{ ref('employment_indicators_november_2022_csv_tables') }}
-```
-
-timestamp strategy - model_snapshot_1
-
-```sql
-{% snapshot model_snapshot_1 %}
-
-{{
-    config(
-      strategy='timestamp',
-      updated_at='refresh_timestamp',
-      unique_key='id'
-    )
-}}
-
-select *
-from {{ ref('model') }} {% endsnapshot %}
-```
-
-invalidate hard deletes - model_snapshot_2
-
-```sql
-{% snapshot model_snapshot_2 %}
-
-{{
-    config
-    (
-        unique_key='id',
-        strategy='timestamp',
-        updated_at='refresh_timestamp',
-        invalidate_hard_deletes=True,
-    )
-}}
-select *
-from {{ ref('model') }} {% endsnapshot %}
-```
-
-check strategy - model_snapshot_3
-
-```sql
-{% snapshot model_snapshot_3 %}
-
-{{
-    config
-    (
-        unique_key='id',
-        strategy='check',
-        check_cols=['series_reference','data_value']
-    )
-}}
-select *
-from {{ ref('model') }} {% endsnapshot %}
-```
-
-### Snapshots Known issues
-
-- Incremental Iceberg models - Sync all columns on schema change can't remove columns used as partitioning.
-  The only way, from a dbt perspective, is to do a full-refresh of the incremental model.
-
-- Tables, schemas and database should only be lowercase
-
-- In order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/dbt-athena) is not
-  installed in the target environment.
-  See <https://github.com/dbt-athena/dbt-athena/issues/103> for more details.
-
-- Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column
-  from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
+[pre-installed list]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark-preinstalled-python-libraries.html
+[imported manually]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-libraries.html
 
 ## Contracts
 
 The adapter partly supports contract definition.
 
 - Concerning the `data_type`, it is supported but needs to be adjusted for complex types. They must be specified
   entirely (for instance `array<int>`) even though they won't be checked. Indeed, as dbt recommends, we only compare
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.0rc1 Summary: The
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.1 Summary: The
 athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
 dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Python: >=3.8,<3.13
 Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
 Dist: dbt-common<2.0,>=1.0.0b2 Requires-Dist: dbt-adapters<2.0,>=1.0.0b2
-Requires-Dist: boto3>=1.28 Requires-Dist: boto3-stubs
-[athena,glue,lakeformation,sts]>=1.28 Requires-Dist: pyathena<4.0,>=2.25
+Requires-Dist: dbt-core>=1.8.0 Requires-Dist: boto3>=1.28 Requires-Dist: boto3-
+stubs[athena,glue,lakeformation,sts]>=1.28 Requires-Dist: pyathena<4.0,>=2.25
 Requires-Dist: mmh3<4.2.0,>=4.0.1 Requires-Dist: pydantic<3.0,>=1.10 Requires-
 Dist: tenacity~=8.2
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
 dbt-athena-long.png]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_._s_v_g_]_[_h_t_t_p_s_:_/
  _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
     _b_a_d_g_e_/_%_2_0_i_m_p_o_r_t_s_-_i_s_o_r_t_-_%_2_3_1_6_7_4_b_1_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_e_f_8_3_3_6_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]_[_h_t_t_p_s_:_/_/_w_w_w_._m_y_p_y_-_l_a_n_g_._o_r_g_/
@@ -24,19 +24,20 @@
 - [Features](#features) - [Quick Start](#quick-start) - [Installation]
 (#installation) - [Prerequisites](#prerequisites) - [Credentials](#credentials)
 - [Configuring your profile](#configuring-your-profile) - [Additional
 information](#additional-information) - [Models](#models) - [Table
 Configuration](#table-configuration) - [Table location](#table-location) -
 [Incremental models](#incremental-models) - [On schema change](#on-schema-
 change) - [Iceberg](#iceberg) - [Highly available table (HA)](#highly-
-available-table-ha) - [HA Known issues](#ha-known-issues) - [Snapshots]
-(#snapshots) - [Timestamp strategy](#timestamp-strategy) - [Check strategy]
-(#check-strategy) - [Hard-deletes](#hard-deletes) - [AWS Lakeformation
-integration](#aws-lakeformation-integration) - [Working example](#working-
-example) - [Snapshots Known issues](#snapshots-known-issues) - [Contracts]
+available-table-ha) - [HA Known issues](#ha-known-issues) - [Update glue data
+catalog](#update-glue-data-catalog) - [Snapshots](#snapshots) - [Timestamp
+strategy](#timestamp-strategy) - [Check strategy](#check-strategy) - [Hard-
+deletes](#hard-deletes) - [Working example](#working-example) - [Snapshots
+Known issues](#snapshots-known-issues) - [AWS Lakeformation integration](#aws-
+lakeformation-integration) - [Python Models](#python-models) - [Contracts]
 (#contracts) - [Contributing](#contributing) - [Contributors â¨]
 (#contributors-) # Features - Supports dbt version `1.7.*` - Support for Python
 - Supports [seeds][seeds] - Correctly detects views and their columns -
 Supports [table materialization][table] - [Iceberg tables][athena-iceberg] are
 supported **only with Athena Engine v3** and **a unique table location** (see
 table location section below) - Hive tables are supported by both Athena
 engines. - Supports [incremental models][incremental] - On Iceberg tables : -
@@ -262,98 +263,35 @@
 the materialization keeps the last 4 table versions, you can change it by
 setting `versions_to_keep`. #### HA Known issues - When swapping from a table
 with partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
 instead of partitions - By default, Glue "duplicates" the versions internally,
 so the last two versions of a table point to the same location - It's
 recommended to have `versions_to_keep` >= 4, as this will avoid having the
-older location removed ## Snapshots The adapter supports snapshot
-materialization. It supports both timestamp and check strategy. To create a
-snapshot create a snapshot file in the snapshots directory. If the directory
-does not exist create one. ### Timestamp strategy To use the timestamp strategy
-refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
-strategy-recommended) ### Check strategy To use the check strategy refer to the
-[dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
-Hard-deletes The materialization also supports invalidating hard deletes. Check
-the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
-understand usage. ### AWS Lakeformation integration The adapter implements AWS
-Lakeformation tags management in the following way: - you can enable or disable
-lf-tags management via [config](#table-configuration) (disabled by default) -
-once you enable the feature, lf-tags will be updated on every dbt run - first,
-all lf-tags for columns are removed to avoid inheritance issues - then all
-redundant lf-tags are removed from table and actual tags from config are
-applied - finally, lf-tags for columns are applied It's important to understand
-the following points: - dbt does not manage lf-tags for database - dbt does not
-manage lakeformation permissions That's why you should handle this by yourself
-manually or using some automation tools like terraform, AWS CDK etc. You may
-find the following links useful to manage that: * [terraform
-aws_lakeformation_permissions](https://registry.terraform.io/providers/
-hashicorp/aws/latest/docs/resources/lakeformation_permissions) * [terraform
-aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/
-hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags) ## Python
-Models The adapter supports python models using [`spark`](https://
-docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html). ### Setup - A spark
-enabled work group created in athena - Spark execution role granted access to
-Athena, Glue and S3 - The spark work group is added to the ~/.dbt/profiles.yml
-file and the profile is referenced in dbt_project.yml that will be created. It
-is recommended to keep this same as threads. ### Spark specific table
-configuration - `timeout` (`default=43200`) - Time out in seconds for each
-python model execution. Defaults to 12 hours/43200 seconds. -
-`spark_encryption` (`default=false`) - If this flag is set to true, encrypts
-data in transit between Spark nodes and also encrypts data at rest stored
-locally by Spark. - `spark_cross_account_catalog` (`default=false`) - In spark,
-you can query the external account catalog and for that the consumer account
-has to be configured to access the producer catalog. - If this flag is set to
-true, "/" can be used as the glue catalog separator. Ex: 999999999999/
-mydatabase.cloudfront_logs (*where *999999999999* is the external catalog id*)
-- `spark_requester_pays` (`default=false`) - When an Amazon S3 bucket is
-configured as requester pays, the account of the user running the query is
-charged for data access and data transfer fees associated with the query. - If
-this flag is set to true, requester pays S3 buckets are enabled in Athena for
-Spark. ### Spark notes - A session is created for each unique engine
-configuration defined in the models that are part of the invocation. - A
-session's idle timeout is set to 10 minutes. Within the timeout period, if
-there is a new calculation (spark python model) ready for execution and the
-engine configuration matches, the process will reuse the same session. - Number
-of python models running at a time depends on the `threads`. Number of sessions
-created for the entire run depends on number of unique engine configurations
-and availability of session to maintain threads concurrency. - For iceberg
-table, it is recommended to use table_properties configuration to set the
-format_version to 2. This is to maintain compatability between iceberg tables
-created by Trino with those created by Spark. ### Example models #### Simple
-pandas model ```python import pandas as pd def model(dbt, session): dbt.config
-(materialized="table") model_df = pd.DataFrame({"A": [1, 2, 3, 4]}) return
-model_df ``` #### Simple spark ```python def model(dbt, spark_session):
-dbt.config(materialized="table") data = [(1,), (2,), (3,), (4,)] df =
-spark_session.createDataFrame(data, ["A"]) return df ``` #### Spark incremental
-```python def model(dbt, spark_session): dbt.config(materialized="incremental")
-df = dbt.ref("model") if dbt.is_incremental: max_from_this = ( f"select max
-(run_date) from {dbt.this.schema}.{dbt.this.identifier}" ) df = df.filter
-(df.run_date >= spark_session.sql(max_from_this).collect()[0][0]) return df ```
-#### Config spark model ```python def model(dbt, spark_session): dbt.config
-( materialized="table", engine_config={ "CoordinatorDpuSize": 1,
-"MaxConcurrentDpus": 3, "DefaultExecutorDpuSize": 1 }, spark_encryption=True,
-spark_cross_account_catalog=True, spark_requester_pays=True
-polling_interval=15, timeout=120, ) data = [(1,), (2,), (3,), (4,)] df =
-spark_session.createDataFrame(data, ["A"]) return df ``` #### Create pySpark
-udf using imported external python files ```python def model(dbt,
-spark_session): dbt.config( materialized="incremental",
-incremental_strategy="merge", unique_key="num", ) sc =
-spark_session.sparkContext sc.addPyFile("s3://athena-dbt/test/file1.py")
-sc.addPyFile("s3://athena-dbt/test/file2.py") def func(iterator): from file2
-import transform return [transform(i) for i in iterator] from
-pyspark.sql.functions import udf from pyspark.sql.functions import col
-udf_with_import = udf(func) data = [(1, "a"), (2, "b"), (3, "c")] cols =
-["num", "alpha"] df = spark_session.createDataFrame(data, cols) return
-df.withColumn("udf_test_col", udf_with_import(col("alpha"))) ``` #### Known
-issues in python models - Incremental models do not fully utilize spark
-capabilities. They depend partially on existing sql based logic which runs on
-trino. - Snapshots materializations are not supported. - Spark can only
-reference tables within the same catalog. ### Working example seed file -
-employent_indicators_november_2022_csv_tables.csv ```csv
+older location removed ### Update glue data catalog Optionally persist resource
+descriptions as column and relation comments to the glue data catalog, and meta
+as [glue table properties](https://docs.aws.amazon.com/glue/latest/dg/tables-
+described.html#table-properties) and [column parameters](https://
+docs.aws.amazon.com/glue/latest/webapi/API_Column.html). By default,
+documentation persistence is disabled, but it can be enabled for specific
+resources or groups of resources as needed. For example: ```yaml models: -
+name: test_deduplicate description: another value config: persist_docs:
+relation: true columns: true meta: test: value columns: - name: id meta:
+primary_key: true ``` See [persist docs](https://docs.getdbt.com/reference/
+resource-configs/persist_docs) for more details. ## Snapshots The adapter
+supports snapshot materialization. It supports both timestamp and check
+strategy. To create a snapshot create a snapshot file in the snapshots
+directory. If the directory does not exist create one. ### Timestamp strategy
+To use the timestamp strategy refer to the [dbt docs](https://docs.getdbt.com/
+docs/build/snapshots#timestamp-strategy-recommended) ### Check strategy To use
+the check strategy refer to the [dbt docs](https://docs.getdbt.com/docs/build/
+snapshots#check-strategy) ### Hard-deletes The materialization also supports
+invalidating hard deletes. Check the [docs](https://docs.getdbt.com/docs/build/
+snapshots#hard-deletes-opt-in) to understand usage. ### Working example seed
+file - employent_indicators_november_2022_csv_tables.csv ```csv
 Series_reference,Period,Data_value,Suppressed MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803, MEIM.S1WA,1999.06,65792, MEIM.S1WA,1999.07,66194,
 MEIM.S1WA,1999.08,67259, MEIM.S1WA,1999.09,69691, MEIM.S1WA,1999.1,72475,
 MEIM.S1WA,1999.11,79263, MEIM.S1WA,1999.12,86540, MEIM.S1WA,2000.01,82552,
 MEIM.S1WA,2000.02,81709, MEIM.S1WA,2000.03,84126, MEIM.S1WA,2000.04,77089,
 MEIM.S1WA,2000.05,73811, MEIM.S1WA,2000.06,70070, MEIM.S1WA,2000.07,69873,
 MEIM.S1WA,2000.08,71468, MEIM.S1WA,2000.09,72462, MEIM.S1WA,2000.1,74897, ```
@@ -375,19 +313,102 @@
 The only way, from a dbt perspective, is to do a full-refresh of the
 incremental model. - Tables, schemas and database should only be lowercase - In
 order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://
 github.com/Tomme/dbt-athena) is not installed in the target environment. See
 github.com/dbt-athena/dbt-athena/issues/103> for more details. - Snapshot does
 not support dropping columns from the source table. If you drop a column make
 sure to drop the column from the snapshot as well. Another workaround is to
-NULL the column in the snapshot definition to preserve history ## Contracts The
-adapter partly supports contract definition. - Concerning the `data_type`, it
-is supported but needs to be adjusted for complex types. They must be specified
-entirely (for instance `array`) even though they won't be checked. Indeed, as
-dbt recommends, we only compare the broader type (array, map, int, varchar).
-The complete definition is used in order to check that the data types defined
-in athena are ok (pre-flight check). - the adapter does not support the
-constraints since no constraints don't exist in Athena. ## Contributing See
-[CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
-this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
-_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-_a_t_h_e_n_a_]Contributions of any kind welcome!
+NULL the column in the snapshot definition to preserve history ## AWS
+Lakeformation integration The adapter implements AWS Lakeformation tags
+management in the following way: - you can enable or disable lf-tags management
+via [config](#table-configuration) (disabled by default) - once you enable the
+feature, lf-tags will be updated on every dbt run - first, all lf-tags for
+columns are removed to avoid inheritance issues - then all redundant lf-tags
+are removed from table and actual tags from config are applied - finally, lf-
+tags for columns are applied It's important to understand the following points:
+- dbt does not manage lf-tags for database - dbt does not manage lakeformation
+permissions That's why you should handle this by yourself manually or using
+some automation tools like terraform, AWS CDK etc. You may find the following
+links useful to manage that: * [terraform aws_lakeformation_permissions](https:
+//registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/
+lakeformation_permissions) * [terraform aws_lakeformation_resource_lf_tags]
+(https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/
+lakeformation_resource_lf_tags) ## Python Models The adapter supports python
+models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-
+spark.html). ### Setup - A Spark-enabled workgroup created in Athena - Spark
+execution role granted access to Athena, Glue and S3 - The Spark workgroup is
+added to the `~/.dbt/profiles.yml` file and the profile is referenced in
+`dbt_project.yml` that will be created. It is recommended to keep this same as
+threads. ### Spark-specific table configuration - `timeout` (`default=43200`) -
+Time out in seconds for each Python model execution. Defaults to 12 hours/43200
+seconds. - `spark_encryption` (`default=false`) - If this flag is set to true,
+encrypts data in transit between Spark nodes and also encrypts data at rest
+stored locally by Spark. - `spark_cross_account_catalog` (`default=false`) - In
+Spark, you can query the external account catalog and for that the consumer
+account has to be configured to access the producer catalog. - If this flag is
+set to true, "/" can be used as the glue catalog separator. Ex: 999999999999/
+mydatabase.cloudfront_logs (*where *999999999999* is the external catalog ID*)
+- `spark_requester_pays` (`default=false`) - When an Amazon S3 bucket is
+configured as requester pays, the account of the user running the query is
+charged for data access and data transfer fees associated with the query. - If
+this flag is set to true, requester pays S3 buckets are enabled in Athena for
+Spark. ### Spark notes - A session is created for each unique engine
+configuration defined in the models that are part of the invocation. - A
+session's idle timeout is set to 10 minutes. Within the timeout period, if
+there is a new calculation (Spark Python model) ready for execution and the
+engine configuration matches, the process will reuse the same session. - The
+number of Python models running at a time depends on the `threads`. The number
+of sessions created for the entire run depends on the number of unique engine
+configurations and the availability of sessions to maintain thread concurrency.
+- For Iceberg tables, it is recommended to use `table_properties` configuration
+to set the `format_version` to 2. This is to maintain compatibility between
+Iceberg tables created by Trino with those created by Spark. ### Example models
+#### Simple pandas model ```python import pandas as pd def model(dbt, session):
+dbt.config(materialized="table") model_df = pd.DataFrame({"A": [1, 2, 3, 4]})
+return model_df ``` #### Simple spark ```python def model(dbt, spark_session):
+dbt.config(materialized="table") data = [(1,), (2,), (3,), (4,)] df =
+spark_session.createDataFrame(data, ["A"]) return df ``` #### Spark incremental
+```python def model(dbt, spark_session): dbt.config(materialized="incremental")
+df = dbt.ref("model") if dbt.is_incremental: max_from_this = ( f"select max
+(run_date) from {dbt.this.schema}.{dbt.this.identifier}" ) df = df.filter
+(df.run_date >= spark_session.sql(max_from_this).collect()[0][0]) return df ```
+#### Config spark model ```python def model(dbt, spark_session): dbt.config
+( materialized="table", engine_config={ "CoordinatorDpuSize": 1,
+"MaxConcurrentDpus": 3, "DefaultExecutorDpuSize": 1 }, spark_encryption=True,
+spark_cross_account_catalog=True, spark_requester_pays=True
+polling_interval=15, timeout=120, ) data = [(1,), (2,), (3,), (4,)] df =
+spark_session.createDataFrame(data, ["A"]) return df ``` #### Create pySpark
+udf using imported external python files ```python def model(dbt,
+spark_session): dbt.config( materialized="incremental",
+incremental_strategy="merge", unique_key="num", ) sc =
+spark_session.sparkContext sc.addPyFile("s3://athena-dbt/test/file1.py")
+sc.addPyFile("s3://athena-dbt/test/file2.py") def func(iterator): from file2
+import transform return [transform(i) for i in iterator] from
+pyspark.sql.functions import udf from pyspark.sql.functions import col
+udf_with_import = udf(func) data = [(1, "a"), (2, "b"), (3, "c")] cols =
+["num", "alpha"] df = spark_session.createDataFrame(data, cols) return
+df.withColumn("udf_test_col", udf_with_import(col("alpha"))) ``` ### Known
+issues in Python models - Python models cannot [reference Athena SQL views]
+(https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html). - Third-
+party Python libraries can be used, but they must be [included in the pre-
+installed list]([pre-installed list]) or [imported manually]([imported
+manually]). - Python models can only reference or write to tables with names
+meeting the regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special
+characters are not supported by Spark, even though Athena supports them. -
+Incremental models do not fully utilize Spark capabilities. They depend
+partially on existing SQL-based logic which runs on Trino. - Snapshot
+materializations are not supported. - Spark can only reference tables within
+the same catalog. [pre-installed list]: https://docs.aws.amazon.com/athena/
+latest/ug/notebooks-spark-preinstalled-python-libraries.html [imported
+manually]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-
+libraries.html ## Contracts The adapter partly supports contract definition. -
+Concerning the `data_type`, it is supported but needs to be adjusted for
+complex types. They must be specified entirely (for instance `array`) even
+though they won't be checked. Indeed, as dbt recommends, we only compare the
+broader type (array, map, int, varchar). The complete definition is used in
+order to check that the data types defined in athena are ok (pre-flight check).
+- the adapter does not support the constraints since no constraints don't exist
+in Athena. ## Contributing See [CONTRIBUTING](CONTRIBUTING.md) for more
+information on how to contribute to this project. ## Contributors â¨ Thanks
+goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
+en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-
+_a_t_h_e_n_a_]Contributions of any kind welcome!
```

### Comparing `dbt_athena_community-1.8.0rc1/README.md` & `dbt_athena_community-1.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,23 @@
     - [Table Configuration](#table-configuration)
     - [Table location](#table-location)
     - [Incremental models](#incremental-models)
     - [On schema change](#on-schema-change)
     - [Iceberg](#iceberg)
     - [Highly available table (HA)](#highly-available-table-ha)
       - [HA Known issues](#ha-known-issues)
+    - [Update glue data catalog](#update-glue-data-catalog)
   - [Snapshots](#snapshots)
     - [Timestamp strategy](#timestamp-strategy)
     - [Check strategy](#check-strategy)
     - [Hard-deletes](#hard-deletes)
-    - [AWS Lakeformation integration](#aws-lakeformation-integration)
     - [Working example](#working-example)
     - [Snapshots Known issues](#snapshots-known-issues)
+  - [AWS Lakeformation integration](#aws-lakeformation-integration)
+  - [Python Models](#python-models)
   - [Contracts](#contracts)
   - [Contributing](#contributing)
   - [Contributors ✨](#contributors-)
 <!-- TOC -->
 
 # Features
 
@@ -273,15 +275,15 @@
                       'principals': ['principal_arn1', 'principal_arn2']
                   }
               }
           }
       }
   ```
 
-> Notes:  
+> Notes:
 >
 > - `lf_tags` and `lf_tags_columns` configs support only attaching lf tags to corresponding resources.
 > We recommend managing LF Tags permissions somewhere outside dbt. For example, you may use
 > [terraform](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions) or
 > [aws cdk](https://docs.aws.amazon.com/cdk/api/v1/docs/aws-lakeformation-readme.html) for such purpose.
 > - `data_cell_filters` management can't be automated outside dbt because the filter can't be attached to the table
 > which doesn't exist. Once you `enable` this config, dbt will set all filters and their permissions during every
@@ -501,14 +503,42 @@
 
 - When swapping from a table with partitions to a table without (and the other way around), there could be a little
   downtime.
   In case high performances are needed consider bucketing instead of partitions
 - By default, Glue "duplicates" the versions internally, so the last two versions of a table point to the same location
 - It's recommended to have `versions_to_keep` >= 4, as this will avoid having the older location removed
 
+### Update glue data catalog
+
+Optionally persist resource descriptions as column and relation comments to the glue data catalog, and meta as
+[glue table properties](https://docs.aws.amazon.com/glue/latest/dg/tables-described.html#table-properties)
+and [column parameters](https://docs.aws.amazon.com/glue/latest/webapi/API_Column.html).
+By default, documentation persistence is disabled, but it can be enabled for specific resources or
+groups of resources as needed.
+
+For example:
+
+```yaml
+models:
+  - name: test_deduplicate
+    description: another value
+    config:
+      persist_docs:
+        relation: true
+        columns: true
+      meta:
+        test: value
+    columns:
+      - name: id
+        meta:
+          primary_key: true
+```
+
+See [persist docs](https://docs.getdbt.com/reference/resource-configs/persist_docs) for more details.
+
 ## Snapshots
 
 The adapter supports snapshot materialization. It supports both timestamp and check strategy. To create a snapshot
 create a snapshot file in the snapshots directory. If the directory does not exist create one.
 
 ### Timestamp strategy
 
@@ -520,74 +550,181 @@
 To use the check strategy refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy)
 
 ### Hard-deletes
 
 The materialization also supports invalidating hard deletes. Check
 the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to understand usage.
 
-### AWS Lakeformation integration
+### Working example
+
+seed file - employent_indicators_november_2022_csv_tables.csv
+
+```csv
+Series_reference,Period,Data_value,Suppressed
+MEIM.S1WA,1999.04,80267,
+MEIM.S1WA,1999.05,70803,
+MEIM.S1WA,1999.06,65792,
+MEIM.S1WA,1999.07,66194,
+MEIM.S1WA,1999.08,67259,
+MEIM.S1WA,1999.09,69691,
+MEIM.S1WA,1999.1,72475,
+MEIM.S1WA,1999.11,79263,
+MEIM.S1WA,1999.12,86540,
+MEIM.S1WA,2000.01,82552,
+MEIM.S1WA,2000.02,81709,
+MEIM.S1WA,2000.03,84126,
+MEIM.S1WA,2000.04,77089,
+MEIM.S1WA,2000.05,73811,
+MEIM.S1WA,2000.06,70070,
+MEIM.S1WA,2000.07,69873,
+MEIM.S1WA,2000.08,71468,
+MEIM.S1WA,2000.09,72462,
+MEIM.S1WA,2000.1,74897,
+```
+
+model.sql
+
+```sql
+{{ config(
+    materialized='table'
+) }}
+
+select row_number() over() as id
+       , *
+       , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) as refresh_timestamp
+from {{ ref('employment_indicators_november_2022_csv_tables') }}
+```
+
+timestamp strategy - model_snapshot_1
+
+```sql
+{% snapshot model_snapshot_1 %}
+
+{{
+    config(
+      strategy='timestamp',
+      updated_at='refresh_timestamp',
+      unique_key='id'
+    )
+}}
+
+select *
+from {{ ref('model') }} {% endsnapshot %}
+```
+
+invalidate hard deletes - model_snapshot_2
+
+```sql
+{% snapshot model_snapshot_2 %}
+
+{{
+    config
+    (
+        unique_key='id',
+        strategy='timestamp',
+        updated_at='refresh_timestamp',
+        invalidate_hard_deletes=True,
+    )
+}}
+select *
+from {{ ref('model') }} {% endsnapshot %}
+```
+
+check strategy - model_snapshot_3
+
+```sql
+{% snapshot model_snapshot_3 %}
+
+{{
+    config
+    (
+        unique_key='id',
+        strategy='check',
+        check_cols=['series_reference','data_value']
+    )
+}}
+select *
+from {{ ref('model') }} {% endsnapshot %}
+```
+
+### Snapshots Known issues
+
+- Incremental Iceberg models - Sync all columns on schema change can't remove columns used as partitioning.
+  The only way, from a dbt perspective, is to do a full-refresh of the incremental model.
+
+- Tables, schemas and database should only be lowercase
+
+- In order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/dbt-athena) is not
+  installed in the target environment.
+  See <https://github.com/dbt-athena/dbt-athena/issues/103> for more details.
+
+- Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column
+  from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
+
+## AWS Lakeformation integration
 
 The adapter implements AWS Lakeformation tags management in the following way:
 
 - you can enable or disable lf-tags management via [config](#table-configuration) (disabled by default)
 - once you enable the feature, lf-tags will be updated on every dbt run
 - first, all lf-tags for columns are removed to avoid inheritance issues
 - then all redundant lf-tags are removed from table and actual tags from config are applied
 - finally, lf-tags for columns are applied
 
 It's important to understand the following points:
 
 - dbt does not manage lf-tags for database
 - dbt does not manage lakeformation permissions
 
-That's why you should handle this by yourself manually or using some automation tools like terraform, AWS CDK etc.  
+That's why you should handle this by yourself manually or using some automation tools like terraform, AWS CDK etc.
 You may find the following links useful to manage that:
 
 <!-- markdownlint-disable -->
 * [terraform aws_lakeformation_permissions](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions)
 * [terraform aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags)
 <!-- markdownlint-restore -->
 
 ## Python Models
 
 The adapter supports python models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
 
 ### Setup
 
-- A spark enabled work group created in athena
+- A Spark-enabled workgroup created in Athena
 - Spark execution role granted access to Athena, Glue and S3
-- The spark work group is added to the ~/.dbt/profiles.yml file and the profile is referenced in dbt_project.yml
-  that will be created. It is recommended to keep this same as threads.
+- The Spark workgroup is added to the `~/.dbt/profiles.yml` file and the profile
+ is referenced in `dbt_project.yml` that will be created. It is recommended to keep this same as threads.
 
-### Spark specific table configuration
+### Spark-specific table configuration
 
 - `timeout` (`default=43200`)
-  - Time out in seconds for each python model execution. Defaults to 12 hours/43200 seconds.
+  - Time out in seconds for each Python model execution. Defaults to 12 hours/43200 seconds.
 - `spark_encryption` (`default=false`)
   - If this flag is set to true, encrypts data in transit between Spark nodes and also encrypts data at rest stored
    locally by Spark.
 - `spark_cross_account_catalog` (`default=false`)
-  - In spark, you can query the external account catalog and for that the consumer account has to be configured to
+  - In Spark, you can query the external account catalog and for that the consumer account has to be configured to
    access the producer catalog.
   - If this flag is set to true, "/" can be used as the glue catalog separator.
-   Ex: 999999999999/mydatabase.cloudfront_logs (*where *999999999999* is the external catalog id*)
+   Ex: 999999999999/mydatabase.cloudfront_logs (*where *999999999999* is the external catalog ID*)
 - `spark_requester_pays` (`default=false`)
   - When an Amazon S3 bucket is configured as requester pays, the account of the user running the query is charged for
    data access and data transfer fees associated with the query.
   - If this flag is set to true, requester pays S3 buckets are enabled in Athena for Spark.
 
 ### Spark notes
 
 - A session is created for each unique engine configuration defined in the models that are part of the invocation.
 - A session's idle timeout is set to 10 minutes. Within the timeout period, if there is a new calculation
- (spark python model) ready for execution and the engine configuration matches, the process will reuse the same session.
-- Number of python models running at a time depends on the `threads`.  Number of sessions created for the entire run
- depends on number of unique engine configurations and availability of session to maintain threads concurrency.
-- For iceberg table, it is recommended to use table_properties configuration to set the format_version to 2. This is to
- maintain compatability between iceberg tables created by Trino with those created by Spark.
+ (Spark Python model) ready for execution and the engine configuration matches, the process will reuse the same session.
+- The number of Python models running at a time depends on the `threads`. The number of sessions created for the
+ entire run depends on the number of unique engine configurations and the availability of sessions to maintain
+ thread concurrency.
+- For Iceberg tables, it is recommended to use `table_properties` configuration to set the `format_version` to 2.
+ This is to maintain compatibility between Iceberg tables created by Trino with those created by Spark.
 
 ### Example models
 
 #### Simple pandas model
 
 ```python
 import pandas as pd
@@ -681,126 +818,30 @@
     data = [(1, "a"), (2, "b"), (3, "c")]
     cols = ["num", "alpha"]
     df = spark_session.createDataFrame(data, cols)
 
     return df.withColumn("udf_test_col", udf_with_import(col("alpha")))
 ```
 
-#### Known issues in python models
+### Known issues in Python models
 
-- Incremental models do not fully utilize spark capabilities. They depend partially on existing sql based logic which
- runs on trino.
-- Snapshots materializations are not supported.
+- Python models cannot
+ [reference Athena SQL views](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
+- Third-party Python libraries can be used, but they must be [included in the pre-installed list]([pre-installed list])
+ or [imported manually]([imported manually]).
+- Python models can only reference or write to tables with names meeting the
+ regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special characters are not
+ supported by Spark, even though Athena supports them.
+- Incremental models do not fully utilize Spark capabilities. They depend partially on existing SQL-based logic which
+ runs on Trino.
+- Snapshot materializations are not supported.
 - Spark can only reference tables within the same catalog.
 
-### Working example
-
-seed file - employent_indicators_november_2022_csv_tables.csv
-
-```csv
-Series_reference,Period,Data_value,Suppressed
-MEIM.S1WA,1999.04,80267,
-MEIM.S1WA,1999.05,70803,
-MEIM.S1WA,1999.06,65792,
-MEIM.S1WA,1999.07,66194,
-MEIM.S1WA,1999.08,67259,
-MEIM.S1WA,1999.09,69691,
-MEIM.S1WA,1999.1,72475,
-MEIM.S1WA,1999.11,79263,
-MEIM.S1WA,1999.12,86540,
-MEIM.S1WA,2000.01,82552,
-MEIM.S1WA,2000.02,81709,
-MEIM.S1WA,2000.03,84126,
-MEIM.S1WA,2000.04,77089,
-MEIM.S1WA,2000.05,73811,
-MEIM.S1WA,2000.06,70070,
-MEIM.S1WA,2000.07,69873,
-MEIM.S1WA,2000.08,71468,
-MEIM.S1WA,2000.09,72462,
-MEIM.S1WA,2000.1,74897,
-```
-
-model.sql
-
-```sql
-{{ config(
-    materialized='table'
-) }}
-
-select row_number() over() as id
-       , *
-       , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) as refresh_timestamp
-from {{ ref('employment_indicators_november_2022_csv_tables') }}
-```
-
-timestamp strategy - model_snapshot_1
-
-```sql
-{% snapshot model_snapshot_1 %}
-
-{{
-    config(
-      strategy='timestamp',
-      updated_at='refresh_timestamp',
-      unique_key='id'
-    )
-}}
-
-select *
-from {{ ref('model') }} {% endsnapshot %}
-```
-
-invalidate hard deletes - model_snapshot_2
-
-```sql
-{% snapshot model_snapshot_2 %}
-
-{{
-    config
-    (
-        unique_key='id',
-        strategy='timestamp',
-        updated_at='refresh_timestamp',
-        invalidate_hard_deletes=True,
-    )
-}}
-select *
-from {{ ref('model') }} {% endsnapshot %}
-```
-
-check strategy - model_snapshot_3
-
-```sql
-{% snapshot model_snapshot_3 %}
-
-{{
-    config
-    (
-        unique_key='id',
-        strategy='check',
-        check_cols=['series_reference','data_value']
-    )
-}}
-select *
-from {{ ref('model') }} {% endsnapshot %}
-```
-
-### Snapshots Known issues
-
-- Incremental Iceberg models - Sync all columns on schema change can't remove columns used as partitioning.
-  The only way, from a dbt perspective, is to do a full-refresh of the incremental model.
-
-- Tables, schemas and database should only be lowercase
-
-- In order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/dbt-athena) is not
-  installed in the target environment.
-  See <https://github.com/dbt-athena/dbt-athena/issues/103> for more details.
-
-- Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column
-  from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
+[pre-installed list]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark-preinstalled-python-libraries.html
+[imported manually]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-libraries.html
 
 ## Contracts
 
 The adapter partly supports contract definition.
 
 - Concerning the `data_type`, it is supported but needs to be adjusted for complex types. They must be specified
   entirely (for instance `array<int>`) even though they won't be checked. Indeed, as dbt recommends, we only compare
```

#### html2text {}

```diff
@@ -8,19 +8,20 @@
 - [Features](#features) - [Quick Start](#quick-start) - [Installation]
 (#installation) - [Prerequisites](#prerequisites) - [Credentials](#credentials)
 - [Configuring your profile](#configuring-your-profile) - [Additional
 information](#additional-information) - [Models](#models) - [Table
 Configuration](#table-configuration) - [Table location](#table-location) -
 [Incremental models](#incremental-models) - [On schema change](#on-schema-
 change) - [Iceberg](#iceberg) - [Highly available table (HA)](#highly-
-available-table-ha) - [HA Known issues](#ha-known-issues) - [Snapshots]
-(#snapshots) - [Timestamp strategy](#timestamp-strategy) - [Check strategy]
-(#check-strategy) - [Hard-deletes](#hard-deletes) - [AWS Lakeformation
-integration](#aws-lakeformation-integration) - [Working example](#working-
-example) - [Snapshots Known issues](#snapshots-known-issues) - [Contracts]
+available-table-ha) - [HA Known issues](#ha-known-issues) - [Update glue data
+catalog](#update-glue-data-catalog) - [Snapshots](#snapshots) - [Timestamp
+strategy](#timestamp-strategy) - [Check strategy](#check-strategy) - [Hard-
+deletes](#hard-deletes) - [Working example](#working-example) - [Snapshots
+Known issues](#snapshots-known-issues) - [AWS Lakeformation integration](#aws-
+lakeformation-integration) - [Python Models](#python-models) - [Contracts]
 (#contracts) - [Contributing](#contributing) - [Contributors â¨]
 (#contributors-) # Features - Supports dbt version `1.7.*` - Support for Python
 - Supports [seeds][seeds] - Correctly detects views and their columns -
 Supports [table materialization][table] - [Iceberg tables][athena-iceberg] are
 supported **only with Athena Engine v3** and **a unique table location** (see
 table location section below) - Hive tables are supported by both Athena
 engines. - Supports [incremental models][incremental] - On Iceberg tables : -
@@ -246,98 +247,35 @@
 the materialization keeps the last 4 table versions, you can change it by
 setting `versions_to_keep`. #### HA Known issues - When swapping from a table
 with partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
 instead of partitions - By default, Glue "duplicates" the versions internally,
 so the last two versions of a table point to the same location - It's
 recommended to have `versions_to_keep` >= 4, as this will avoid having the
-older location removed ## Snapshots The adapter supports snapshot
-materialization. It supports both timestamp and check strategy. To create a
-snapshot create a snapshot file in the snapshots directory. If the directory
-does not exist create one. ### Timestamp strategy To use the timestamp strategy
-refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
-strategy-recommended) ### Check strategy To use the check strategy refer to the
-[dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
-Hard-deletes The materialization also supports invalidating hard deletes. Check
-the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
-understand usage. ### AWS Lakeformation integration The adapter implements AWS
-Lakeformation tags management in the following way: - you can enable or disable
-lf-tags management via [config](#table-configuration) (disabled by default) -
-once you enable the feature, lf-tags will be updated on every dbt run - first,
-all lf-tags for columns are removed to avoid inheritance issues - then all
-redundant lf-tags are removed from table and actual tags from config are
-applied - finally, lf-tags for columns are applied It's important to understand
-the following points: - dbt does not manage lf-tags for database - dbt does not
-manage lakeformation permissions That's why you should handle this by yourself
-manually or using some automation tools like terraform, AWS CDK etc. You may
-find the following links useful to manage that: * [terraform
-aws_lakeformation_permissions](https://registry.terraform.io/providers/
-hashicorp/aws/latest/docs/resources/lakeformation_permissions) * [terraform
-aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/
-hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags) ## Python
-Models The adapter supports python models using [`spark`](https://
-docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html). ### Setup - A spark
-enabled work group created in athena - Spark execution role granted access to
-Athena, Glue and S3 - The spark work group is added to the ~/.dbt/profiles.yml
-file and the profile is referenced in dbt_project.yml that will be created. It
-is recommended to keep this same as threads. ### Spark specific table
-configuration - `timeout` (`default=43200`) - Time out in seconds for each
-python model execution. Defaults to 12 hours/43200 seconds. -
-`spark_encryption` (`default=false`) - If this flag is set to true, encrypts
-data in transit between Spark nodes and also encrypts data at rest stored
-locally by Spark. - `spark_cross_account_catalog` (`default=false`) - In spark,
-you can query the external account catalog and for that the consumer account
-has to be configured to access the producer catalog. - If this flag is set to
-true, "/" can be used as the glue catalog separator. Ex: 999999999999/
-mydatabase.cloudfront_logs (*where *999999999999* is the external catalog id*)
-- `spark_requester_pays` (`default=false`) - When an Amazon S3 bucket is
-configured as requester pays, the account of the user running the query is
-charged for data access and data transfer fees associated with the query. - If
-this flag is set to true, requester pays S3 buckets are enabled in Athena for
-Spark. ### Spark notes - A session is created for each unique engine
-configuration defined in the models that are part of the invocation. - A
-session's idle timeout is set to 10 minutes. Within the timeout period, if
-there is a new calculation (spark python model) ready for execution and the
-engine configuration matches, the process will reuse the same session. - Number
-of python models running at a time depends on the `threads`. Number of sessions
-created for the entire run depends on number of unique engine configurations
-and availability of session to maintain threads concurrency. - For iceberg
-table, it is recommended to use table_properties configuration to set the
-format_version to 2. This is to maintain compatability between iceberg tables
-created by Trino with those created by Spark. ### Example models #### Simple
-pandas model ```python import pandas as pd def model(dbt, session): dbt.config
-(materialized="table") model_df = pd.DataFrame({"A": [1, 2, 3, 4]}) return
-model_df ``` #### Simple spark ```python def model(dbt, spark_session):
-dbt.config(materialized="table") data = [(1,), (2,), (3,), (4,)] df =
-spark_session.createDataFrame(data, ["A"]) return df ``` #### Spark incremental
-```python def model(dbt, spark_session): dbt.config(materialized="incremental")
-df = dbt.ref("model") if dbt.is_incremental: max_from_this = ( f"select max
-(run_date) from {dbt.this.schema}.{dbt.this.identifier}" ) df = df.filter
-(df.run_date >= spark_session.sql(max_from_this).collect()[0][0]) return df ```
-#### Config spark model ```python def model(dbt, spark_session): dbt.config
-( materialized="table", engine_config={ "CoordinatorDpuSize": 1,
-"MaxConcurrentDpus": 3, "DefaultExecutorDpuSize": 1 }, spark_encryption=True,
-spark_cross_account_catalog=True, spark_requester_pays=True
-polling_interval=15, timeout=120, ) data = [(1,), (2,), (3,), (4,)] df =
-spark_session.createDataFrame(data, ["A"]) return df ``` #### Create pySpark
-udf using imported external python files ```python def model(dbt,
-spark_session): dbt.config( materialized="incremental",
-incremental_strategy="merge", unique_key="num", ) sc =
-spark_session.sparkContext sc.addPyFile("s3://athena-dbt/test/file1.py")
-sc.addPyFile("s3://athena-dbt/test/file2.py") def func(iterator): from file2
-import transform return [transform(i) for i in iterator] from
-pyspark.sql.functions import udf from pyspark.sql.functions import col
-udf_with_import = udf(func) data = [(1, "a"), (2, "b"), (3, "c")] cols =
-["num", "alpha"] df = spark_session.createDataFrame(data, cols) return
-df.withColumn("udf_test_col", udf_with_import(col("alpha"))) ``` #### Known
-issues in python models - Incremental models do not fully utilize spark
-capabilities. They depend partially on existing sql based logic which runs on
-trino. - Snapshots materializations are not supported. - Spark can only
-reference tables within the same catalog. ### Working example seed file -
-employent_indicators_november_2022_csv_tables.csv ```csv
+older location removed ### Update glue data catalog Optionally persist resource
+descriptions as column and relation comments to the glue data catalog, and meta
+as [glue table properties](https://docs.aws.amazon.com/glue/latest/dg/tables-
+described.html#table-properties) and [column parameters](https://
+docs.aws.amazon.com/glue/latest/webapi/API_Column.html). By default,
+documentation persistence is disabled, but it can be enabled for specific
+resources or groups of resources as needed. For example: ```yaml models: -
+name: test_deduplicate description: another value config: persist_docs:
+relation: true columns: true meta: test: value columns: - name: id meta:
+primary_key: true ``` See [persist docs](https://docs.getdbt.com/reference/
+resource-configs/persist_docs) for more details. ## Snapshots The adapter
+supports snapshot materialization. It supports both timestamp and check
+strategy. To create a snapshot create a snapshot file in the snapshots
+directory. If the directory does not exist create one. ### Timestamp strategy
+To use the timestamp strategy refer to the [dbt docs](https://docs.getdbt.com/
+docs/build/snapshots#timestamp-strategy-recommended) ### Check strategy To use
+the check strategy refer to the [dbt docs](https://docs.getdbt.com/docs/build/
+snapshots#check-strategy) ### Hard-deletes The materialization also supports
+invalidating hard deletes. Check the [docs](https://docs.getdbt.com/docs/build/
+snapshots#hard-deletes-opt-in) to understand usage. ### Working example seed
+file - employent_indicators_november_2022_csv_tables.csv ```csv
 Series_reference,Period,Data_value,Suppressed MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803, MEIM.S1WA,1999.06,65792, MEIM.S1WA,1999.07,66194,
 MEIM.S1WA,1999.08,67259, MEIM.S1WA,1999.09,69691, MEIM.S1WA,1999.1,72475,
 MEIM.S1WA,1999.11,79263, MEIM.S1WA,1999.12,86540, MEIM.S1WA,2000.01,82552,
 MEIM.S1WA,2000.02,81709, MEIM.S1WA,2000.03,84126, MEIM.S1WA,2000.04,77089,
 MEIM.S1WA,2000.05,73811, MEIM.S1WA,2000.06,70070, MEIM.S1WA,2000.07,69873,
 MEIM.S1WA,2000.08,71468, MEIM.S1WA,2000.09,72462, MEIM.S1WA,2000.1,74897, ```
@@ -359,19 +297,102 @@
 The only way, from a dbt perspective, is to do a full-refresh of the
 incremental model. - Tables, schemas and database should only be lowercase - In
 order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://
 github.com/Tomme/dbt-athena) is not installed in the target environment. See
 github.com/dbt-athena/dbt-athena/issues/103> for more details. - Snapshot does
 not support dropping columns from the source table. If you drop a column make
 sure to drop the column from the snapshot as well. Another workaround is to
-NULL the column in the snapshot definition to preserve history ## Contracts The
-adapter partly supports contract definition. - Concerning the `data_type`, it
-is supported but needs to be adjusted for complex types. They must be specified
-entirely (for instance `array`) even though they won't be checked. Indeed, as
-dbt recommends, we only compare the broader type (array, map, int, varchar).
-The complete definition is used in order to check that the data types defined
-in athena are ok (pre-flight check). - the adapter does not support the
-constraints since no constraints don't exist in Athena. ## Contributing See
-[CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
-this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
-_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-_a_t_h_e_n_a_]Contributions of any kind welcome!
+NULL the column in the snapshot definition to preserve history ## AWS
+Lakeformation integration The adapter implements AWS Lakeformation tags
+management in the following way: - you can enable or disable lf-tags management
+via [config](#table-configuration) (disabled by default) - once you enable the
+feature, lf-tags will be updated on every dbt run - first, all lf-tags for
+columns are removed to avoid inheritance issues - then all redundant lf-tags
+are removed from table and actual tags from config are applied - finally, lf-
+tags for columns are applied It's important to understand the following points:
+- dbt does not manage lf-tags for database - dbt does not manage lakeformation
+permissions That's why you should handle this by yourself manually or using
+some automation tools like terraform, AWS CDK etc. You may find the following
+links useful to manage that: * [terraform aws_lakeformation_permissions](https:
+//registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/
+lakeformation_permissions) * [terraform aws_lakeformation_resource_lf_tags]
+(https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/
+lakeformation_resource_lf_tags) ## Python Models The adapter supports python
+models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-
+spark.html). ### Setup - A Spark-enabled workgroup created in Athena - Spark
+execution role granted access to Athena, Glue and S3 - The Spark workgroup is
+added to the `~/.dbt/profiles.yml` file and the profile is referenced in
+`dbt_project.yml` that will be created. It is recommended to keep this same as
+threads. ### Spark-specific table configuration - `timeout` (`default=43200`) -
+Time out in seconds for each Python model execution. Defaults to 12 hours/43200
+seconds. - `spark_encryption` (`default=false`) - If this flag is set to true,
+encrypts data in transit between Spark nodes and also encrypts data at rest
+stored locally by Spark. - `spark_cross_account_catalog` (`default=false`) - In
+Spark, you can query the external account catalog and for that the consumer
+account has to be configured to access the producer catalog. - If this flag is
+set to true, "/" can be used as the glue catalog separator. Ex: 999999999999/
+mydatabase.cloudfront_logs (*where *999999999999* is the external catalog ID*)
+- `spark_requester_pays` (`default=false`) - When an Amazon S3 bucket is
+configured as requester pays, the account of the user running the query is
+charged for data access and data transfer fees associated with the query. - If
+this flag is set to true, requester pays S3 buckets are enabled in Athena for
+Spark. ### Spark notes - A session is created for each unique engine
+configuration defined in the models that are part of the invocation. - A
+session's idle timeout is set to 10 minutes. Within the timeout period, if
+there is a new calculation (Spark Python model) ready for execution and the
+engine configuration matches, the process will reuse the same session. - The
+number of Python models running at a time depends on the `threads`. The number
+of sessions created for the entire run depends on the number of unique engine
+configurations and the availability of sessions to maintain thread concurrency.
+- For Iceberg tables, it is recommended to use `table_properties` configuration
+to set the `format_version` to 2. This is to maintain compatibility between
+Iceberg tables created by Trino with those created by Spark. ### Example models
+#### Simple pandas model ```python import pandas as pd def model(dbt, session):
+dbt.config(materialized="table") model_df = pd.DataFrame({"A": [1, 2, 3, 4]})
+return model_df ``` #### Simple spark ```python def model(dbt, spark_session):
+dbt.config(materialized="table") data = [(1,), (2,), (3,), (4,)] df =
+spark_session.createDataFrame(data, ["A"]) return df ``` #### Spark incremental
+```python def model(dbt, spark_session): dbt.config(materialized="incremental")
+df = dbt.ref("model") if dbt.is_incremental: max_from_this = ( f"select max
+(run_date) from {dbt.this.schema}.{dbt.this.identifier}" ) df = df.filter
+(df.run_date >= spark_session.sql(max_from_this).collect()[0][0]) return df ```
+#### Config spark model ```python def model(dbt, spark_session): dbt.config
+( materialized="table", engine_config={ "CoordinatorDpuSize": 1,
+"MaxConcurrentDpus": 3, "DefaultExecutorDpuSize": 1 }, spark_encryption=True,
+spark_cross_account_catalog=True, spark_requester_pays=True
+polling_interval=15, timeout=120, ) data = [(1,), (2,), (3,), (4,)] df =
+spark_session.createDataFrame(data, ["A"]) return df ``` #### Create pySpark
+udf using imported external python files ```python def model(dbt,
+spark_session): dbt.config( materialized="incremental",
+incremental_strategy="merge", unique_key="num", ) sc =
+spark_session.sparkContext sc.addPyFile("s3://athena-dbt/test/file1.py")
+sc.addPyFile("s3://athena-dbt/test/file2.py") def func(iterator): from file2
+import transform return [transform(i) for i in iterator] from
+pyspark.sql.functions import udf from pyspark.sql.functions import col
+udf_with_import = udf(func) data = [(1, "a"), (2, "b"), (3, "c")] cols =
+["num", "alpha"] df = spark_session.createDataFrame(data, cols) return
+df.withColumn("udf_test_col", udf_with_import(col("alpha"))) ``` ### Known
+issues in Python models - Python models cannot [reference Athena SQL views]
+(https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html). - Third-
+party Python libraries can be used, but they must be [included in the pre-
+installed list]([pre-installed list]) or [imported manually]([imported
+manually]). - Python models can only reference or write to tables with names
+meeting the regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special
+characters are not supported by Spark, even though Athena supports them. -
+Incremental models do not fully utilize Spark capabilities. They depend
+partially on existing SQL-based logic which runs on Trino. - Snapshot
+materializations are not supported. - Spark can only reference tables within
+the same catalog. [pre-installed list]: https://docs.aws.amazon.com/athena/
+latest/ug/notebooks-spark-preinstalled-python-libraries.html [imported
+manually]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-
+libraries.html ## Contracts The adapter partly supports contract definition. -
+Concerning the `data_type`, it is supported but needs to be adjusted for
+complex types. They must be specified entirely (for instance `array`) even
+though they won't be checked. Indeed, as dbt recommends, we only compare the
+broader type (array, map, int, varchar). The complete definition is used in
+order to check that the data types defined in athena are ok (pre-flight check).
+- the adapter does not support the constraints since no constraints don't exist
+in Athena. ## Contributing See [CONTRIBUTING](CONTRIBUTING.md) for more
+information on how to contribute to this project. ## Contributors â¨ Thanks
+goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
+en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-
+_a_t_h_e_n_a_]Contributions of any kind welcome!
```

### Comparing `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/column.py` & `dbt_athena_community-1.8.1/dbt/adapters/athena/column.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/config.py` & `dbt_athena_community-1.8.1/dbt/adapters/athena/config.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/connections.py` & `dbt_athena_community-1.8.1/dbt/adapters/athena/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/constants.py` & `dbt_athena_community-1.8.1/dbt/adapters/athena/constants.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/impl.py` & `dbt_athena_community-1.8.1/dbt/adapters/athena/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -708,15 +708,15 @@
             # this allows dbt to create and manage schemas/databases
             if e.response["Error"]["Code"] == "EntityNotFoundException":
                 LOGGER.debug(f"Schema '{schema_relation.schema}' does not exist - Ignoring: {e}")
                 return []
             else:
                 raise e
 
-        relations: list[BaseRelation] = []
+        relations: List[BaseRelation] = []
         quote_policy = {"database": True, "schema": True, "identifier": True}
         for table in tables:
             if "TableType" not in table:
                 LOGGER.info(f"Table '{table['Name']}' has no TableType attribute - Ignoring")
                 continue
             _type = table["TableType"]
             _detailed_table_type = table.get("Parameters", {}).get("table_type", "")
@@ -952,14 +952,15 @@
         # By default, there is no need to update Glue Table
         need_to_update_table = False
         # Get Table from Glue
         table = glue_client.get_table(CatalogId=catalog_id, DatabaseName=relation.schema, Name=relation.name)["Table"]
         # Prepare new version of Glue Table picking up significant fields
         table_input = self._get_table_input(table)
         table_parameters = table_input["Parameters"]
+
         # Update table description
         if persist_relation_docs:
             # Prepare dbt description
             clean_table_description = ellipsis_comment(clean_sql_comment(model["description"]))
             # Get current description from Glue
             glue_table_description = table.get("Description", "")
             # Get current description parameter from Glue
@@ -1009,14 +1010,37 @@
                     glue_col_comment = col_obj.get("Comment", "")
                     # Check that column description is already attached to Glue table
                     if glue_col_comment != clean_col_comment:
                         need_to_update_table = True
                     # Save column description from dbt
                     col_obj["Comment"] = clean_col_comment
 
+                    # Get dbt model column meta if available
+                    col_meta: Dict[str, Any] = model["columns"][col_name].get("meta", {})
+                    # Add empty Parameters dictionary if not present
+                    if col_meta and "Parameters" not in col_obj.keys():
+                        col_obj["Parameters"] = {}
+                    # Prepare meta values for column properties and check if update is required
+                    for meta_key, meta_value_raw in col_meta.items():
+                        if is_valid_table_parameter_key(meta_key):
+                            meta_value = stringify_table_parameter_value(meta_value_raw)
+                            if meta_value is not None:
+                                # Check if meta value is already attached to Glue column
+                                col_current_meta_value: Optional[str] = col_obj["Parameters"].get(meta_key)
+                                if col_current_meta_value is None or col_current_meta_value != meta_value:
+                                    need_to_update_table = True
+                                # Save Glue column parameter
+                                col_obj["Parameters"][meta_key] = meta_value
+                            else:
+                                LOGGER.warning(
+                                    f"Column meta value for key '{meta_key}' is not supported and will be ignored"
+                                )
+                        else:
+                            LOGGER.warning(f"Column meta key '{meta_key}' is not supported and will be ignored")
+
         # Update Glue Table only if table/column description is modified.
         # It prevents redundant schema version creating after incremental runs.
         if need_to_update_table:
             table_input["Parameters"] = table_parameters
             glue_client.update_table(
                 CatalogId=catalog_id,
                 DatabaseName=relation.schema,
```

### Comparing `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/lakeformation.py` & `dbt_athena_community-1.8.1/dbt/adapters/athena/lakeformation.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/python_submissions.py` & `dbt_athena_community-1.8.1/dbt/adapters/athena/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/query_headers.py` & `dbt_athena_community-1.8.1/dbt/adapters/athena/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/relation.py` & `dbt_athena_community-1.8.1/dbt/adapters/athena/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/session.py` & `dbt_athena_community-1.8.1/dbt/adapters/athena/session.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/utils.py` & `dbt_athena_community-1.8.1/dbt/adapters/athena/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/columns.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/metadata.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/persist_docs.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/persist_docs.sql`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% macro athena__persist_docs(relation, model, for_relation=true, for_columns=true) -%}
-  {% set persist_relation_docs = for_relation and config.persist_relation_docs() and model.description %}
+  {% set persist_relation_docs = for_relation and config.persist_relation_docs()%}
   {% set persist_column_docs = for_columns and config.persist_column_docs() and model.columns %}
   {% if persist_relation_docs or persist_column_docs %}
     {% do adapter.persist_docs_to_glue(
             relation=relation,
             model=model,
             persist_relation_docs=persist_relation_docs,
             persist_column_docs=persist_column_docs,
```

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/python_submissions.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/python_submissions.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/relation.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/hooks.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/helpers.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/incremental.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/merge.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/table/create_table_as.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/table/table.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/view/view.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/seeds/helpers.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/snapshots/snapshot.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/datediff.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/ddl_dml_data_type.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/ddl_dml_data_type.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/timestamps.sql` & `dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt/include/athena/profile_template.yml` & `dbt_athena_community-1.8.1/dbt/include/athena/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/PKG-INFO` & `dbt_athena_community-1.8.1/dbt_athena_community.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-athena-community
-Version: 1.8.0rc1
+Version: 1.8.1
 Summary: The athena adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-athena/dbt-athena
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: dbt-common<2.0,>=1.0.0b2
 Requires-Dist: dbt-adapters<2.0,>=1.0.0b2
+Requires-Dist: dbt-core>=1.8.0
 Requires-Dist: boto3>=1.28
 Requires-Dist: boto3-stubs[athena,glue,lakeformation,sts]>=1.28
 Requires-Dist: pyathena<4.0,>=2.25
 Requires-Dist: mmh3<4.2.0,>=4.0.1
 Requires-Dist: pydantic<3.0,>=1.10
 Requires-Dist: tenacity~=8.2
 
@@ -58,21 +59,23 @@
     - [Table Configuration](#table-configuration)
     - [Table location](#table-location)
     - [Incremental models](#incremental-models)
     - [On schema change](#on-schema-change)
     - [Iceberg](#iceberg)
     - [Highly available table (HA)](#highly-available-table-ha)
       - [HA Known issues](#ha-known-issues)
+    - [Update glue data catalog](#update-glue-data-catalog)
   - [Snapshots](#snapshots)
     - [Timestamp strategy](#timestamp-strategy)
     - [Check strategy](#check-strategy)
     - [Hard-deletes](#hard-deletes)
-    - [AWS Lakeformation integration](#aws-lakeformation-integration)
     - [Working example](#working-example)
     - [Snapshots Known issues](#snapshots-known-issues)
+  - [AWS Lakeformation integration](#aws-lakeformation-integration)
+  - [Python Models](#python-models)
   - [Contracts](#contracts)
   - [Contributing](#contributing)
   - [Contributors ✨](#contributors-)
 <!-- TOC -->
 
 # Features
 
@@ -302,15 +305,15 @@
                       'principals': ['principal_arn1', 'principal_arn2']
                   }
               }
           }
       }
   ```
 
-> Notes:  
+> Notes:
 >
 > - `lf_tags` and `lf_tags_columns` configs support only attaching lf tags to corresponding resources.
 > We recommend managing LF Tags permissions somewhere outside dbt. For example, you may use
 > [terraform](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions) or
 > [aws cdk](https://docs.aws.amazon.com/cdk/api/v1/docs/aws-lakeformation-readme.html) for such purpose.
 > - `data_cell_filters` management can't be automated outside dbt because the filter can't be attached to the table
 > which doesn't exist. Once you `enable` this config, dbt will set all filters and their permissions during every
@@ -530,14 +533,42 @@
 
 - When swapping from a table with partitions to a table without (and the other way around), there could be a little
   downtime.
   In case high performances are needed consider bucketing instead of partitions
 - By default, Glue "duplicates" the versions internally, so the last two versions of a table point to the same location
 - It's recommended to have `versions_to_keep` >= 4, as this will avoid having the older location removed
 
+### Update glue data catalog
+
+Optionally persist resource descriptions as column and relation comments to the glue data catalog, and meta as
+[glue table properties](https://docs.aws.amazon.com/glue/latest/dg/tables-described.html#table-properties)
+and [column parameters](https://docs.aws.amazon.com/glue/latest/webapi/API_Column.html).
+By default, documentation persistence is disabled, but it can be enabled for specific resources or
+groups of resources as needed.
+
+For example:
+
+```yaml
+models:
+  - name: test_deduplicate
+    description: another value
+    config:
+      persist_docs:
+        relation: true
+        columns: true
+      meta:
+        test: value
+    columns:
+      - name: id
+        meta:
+          primary_key: true
+```
+
+See [persist docs](https://docs.getdbt.com/reference/resource-configs/persist_docs) for more details.
+
 ## Snapshots
 
 The adapter supports snapshot materialization. It supports both timestamp and check strategy. To create a snapshot
 create a snapshot file in the snapshots directory. If the directory does not exist create one.
 
 ### Timestamp strategy
 
@@ -549,74 +580,181 @@
 To use the check strategy refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy)
 
 ### Hard-deletes
 
 The materialization also supports invalidating hard deletes. Check
 the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to understand usage.
 
-### AWS Lakeformation integration
+### Working example
+
+seed file - employent_indicators_november_2022_csv_tables.csv
+
+```csv
+Series_reference,Period,Data_value,Suppressed
+MEIM.S1WA,1999.04,80267,
+MEIM.S1WA,1999.05,70803,
+MEIM.S1WA,1999.06,65792,
+MEIM.S1WA,1999.07,66194,
+MEIM.S1WA,1999.08,67259,
+MEIM.S1WA,1999.09,69691,
+MEIM.S1WA,1999.1,72475,
+MEIM.S1WA,1999.11,79263,
+MEIM.S1WA,1999.12,86540,
+MEIM.S1WA,2000.01,82552,
+MEIM.S1WA,2000.02,81709,
+MEIM.S1WA,2000.03,84126,
+MEIM.S1WA,2000.04,77089,
+MEIM.S1WA,2000.05,73811,
+MEIM.S1WA,2000.06,70070,
+MEIM.S1WA,2000.07,69873,
+MEIM.S1WA,2000.08,71468,
+MEIM.S1WA,2000.09,72462,
+MEIM.S1WA,2000.1,74897,
+```
+
+model.sql
+
+```sql
+{{ config(
+    materialized='table'
+) }}
+
+select row_number() over() as id
+       , *
+       , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) as refresh_timestamp
+from {{ ref('employment_indicators_november_2022_csv_tables') }}
+```
+
+timestamp strategy - model_snapshot_1
+
+```sql
+{% snapshot model_snapshot_1 %}
+
+{{
+    config(
+      strategy='timestamp',
+      updated_at='refresh_timestamp',
+      unique_key='id'
+    )
+}}
+
+select *
+from {{ ref('model') }} {% endsnapshot %}
+```
+
+invalidate hard deletes - model_snapshot_2
+
+```sql
+{% snapshot model_snapshot_2 %}
+
+{{
+    config
+    (
+        unique_key='id',
+        strategy='timestamp',
+        updated_at='refresh_timestamp',
+        invalidate_hard_deletes=True,
+    )
+}}
+select *
+from {{ ref('model') }} {% endsnapshot %}
+```
+
+check strategy - model_snapshot_3
+
+```sql
+{% snapshot model_snapshot_3 %}
+
+{{
+    config
+    (
+        unique_key='id',
+        strategy='check',
+        check_cols=['series_reference','data_value']
+    )
+}}
+select *
+from {{ ref('model') }} {% endsnapshot %}
+```
+
+### Snapshots Known issues
+
+- Incremental Iceberg models - Sync all columns on schema change can't remove columns used as partitioning.
+  The only way, from a dbt perspective, is to do a full-refresh of the incremental model.
+
+- Tables, schemas and database should only be lowercase
+
+- In order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/dbt-athena) is not
+  installed in the target environment.
+  See <https://github.com/dbt-athena/dbt-athena/issues/103> for more details.
+
+- Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column
+  from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
+
+## AWS Lakeformation integration
 
 The adapter implements AWS Lakeformation tags management in the following way:
 
 - you can enable or disable lf-tags management via [config](#table-configuration) (disabled by default)
 - once you enable the feature, lf-tags will be updated on every dbt run
 - first, all lf-tags for columns are removed to avoid inheritance issues
 - then all redundant lf-tags are removed from table and actual tags from config are applied
 - finally, lf-tags for columns are applied
 
 It's important to understand the following points:
 
 - dbt does not manage lf-tags for database
 - dbt does not manage lakeformation permissions
 
-That's why you should handle this by yourself manually or using some automation tools like terraform, AWS CDK etc.  
+That's why you should handle this by yourself manually or using some automation tools like terraform, AWS CDK etc.
 You may find the following links useful to manage that:
 
 <!-- markdownlint-disable -->
 * [terraform aws_lakeformation_permissions](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions)
 * [terraform aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags)
 <!-- markdownlint-restore -->
 
 ## Python Models
 
 The adapter supports python models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
 
 ### Setup
 
-- A spark enabled work group created in athena
+- A Spark-enabled workgroup created in Athena
 - Spark execution role granted access to Athena, Glue and S3
-- The spark work group is added to the ~/.dbt/profiles.yml file and the profile is referenced in dbt_project.yml
-  that will be created. It is recommended to keep this same as threads.
+- The Spark workgroup is added to the `~/.dbt/profiles.yml` file and the profile
+ is referenced in `dbt_project.yml` that will be created. It is recommended to keep this same as threads.
 
-### Spark specific table configuration
+### Spark-specific table configuration
 
 - `timeout` (`default=43200`)
-  - Time out in seconds for each python model execution. Defaults to 12 hours/43200 seconds.
+  - Time out in seconds for each Python model execution. Defaults to 12 hours/43200 seconds.
 - `spark_encryption` (`default=false`)
   - If this flag is set to true, encrypts data in transit between Spark nodes and also encrypts data at rest stored
    locally by Spark.
 - `spark_cross_account_catalog` (`default=false`)
-  - In spark, you can query the external account catalog and for that the consumer account has to be configured to
+  - In Spark, you can query the external account catalog and for that the consumer account has to be configured to
    access the producer catalog.
   - If this flag is set to true, "/" can be used as the glue catalog separator.
-   Ex: 999999999999/mydatabase.cloudfront_logs (*where *999999999999* is the external catalog id*)
+   Ex: 999999999999/mydatabase.cloudfront_logs (*where *999999999999* is the external catalog ID*)
 - `spark_requester_pays` (`default=false`)
   - When an Amazon S3 bucket is configured as requester pays, the account of the user running the query is charged for
    data access and data transfer fees associated with the query.
   - If this flag is set to true, requester pays S3 buckets are enabled in Athena for Spark.
 
 ### Spark notes
 
 - A session is created for each unique engine configuration defined in the models that are part of the invocation.
 - A session's idle timeout is set to 10 minutes. Within the timeout period, if there is a new calculation
- (spark python model) ready for execution and the engine configuration matches, the process will reuse the same session.
-- Number of python models running at a time depends on the `threads`.  Number of sessions created for the entire run
- depends on number of unique engine configurations and availability of session to maintain threads concurrency.
-- For iceberg table, it is recommended to use table_properties configuration to set the format_version to 2. This is to
- maintain compatability between iceberg tables created by Trino with those created by Spark.
+ (Spark Python model) ready for execution and the engine configuration matches, the process will reuse the same session.
+- The number of Python models running at a time depends on the `threads`. The number of sessions created for the
+ entire run depends on the number of unique engine configurations and the availability of sessions to maintain
+ thread concurrency.
+- For Iceberg tables, it is recommended to use `table_properties` configuration to set the `format_version` to 2.
+ This is to maintain compatibility between Iceberg tables created by Trino with those created by Spark.
 
 ### Example models
 
 #### Simple pandas model
 
 ```python
 import pandas as pd
@@ -710,126 +848,30 @@
     data = [(1, "a"), (2, "b"), (3, "c")]
     cols = ["num", "alpha"]
     df = spark_session.createDataFrame(data, cols)
 
     return df.withColumn("udf_test_col", udf_with_import(col("alpha")))
 ```
 
-#### Known issues in python models
+### Known issues in Python models
 
-- Incremental models do not fully utilize spark capabilities. They depend partially on existing sql based logic which
- runs on trino.
-- Snapshots materializations are not supported.
+- Python models cannot
+ [reference Athena SQL views](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
+- Third-party Python libraries can be used, but they must be [included in the pre-installed list]([pre-installed list])
+ or [imported manually]([imported manually]).
+- Python models can only reference or write to tables with names meeting the
+ regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special characters are not
+ supported by Spark, even though Athena supports them.
+- Incremental models do not fully utilize Spark capabilities. They depend partially on existing SQL-based logic which
+ runs on Trino.
+- Snapshot materializations are not supported.
 - Spark can only reference tables within the same catalog.
 
-### Working example
-
-seed file - employent_indicators_november_2022_csv_tables.csv
-
-```csv
-Series_reference,Period,Data_value,Suppressed
-MEIM.S1WA,1999.04,80267,
-MEIM.S1WA,1999.05,70803,
-MEIM.S1WA,1999.06,65792,
-MEIM.S1WA,1999.07,66194,
-MEIM.S1WA,1999.08,67259,
-MEIM.S1WA,1999.09,69691,
-MEIM.S1WA,1999.1,72475,
-MEIM.S1WA,1999.11,79263,
-MEIM.S1WA,1999.12,86540,
-MEIM.S1WA,2000.01,82552,
-MEIM.S1WA,2000.02,81709,
-MEIM.S1WA,2000.03,84126,
-MEIM.S1WA,2000.04,77089,
-MEIM.S1WA,2000.05,73811,
-MEIM.S1WA,2000.06,70070,
-MEIM.S1WA,2000.07,69873,
-MEIM.S1WA,2000.08,71468,
-MEIM.S1WA,2000.09,72462,
-MEIM.S1WA,2000.1,74897,
-```
-
-model.sql
-
-```sql
-{{ config(
-    materialized='table'
-) }}
-
-select row_number() over() as id
-       , *
-       , cast(from_unixtime(to_unixtime(now())) as timestamp(6)) as refresh_timestamp
-from {{ ref('employment_indicators_november_2022_csv_tables') }}
-```
-
-timestamp strategy - model_snapshot_1
-
-```sql
-{% snapshot model_snapshot_1 %}
-
-{{
-    config(
-      strategy='timestamp',
-      updated_at='refresh_timestamp',
-      unique_key='id'
-    )
-}}
-
-select *
-from {{ ref('model') }} {% endsnapshot %}
-```
-
-invalidate hard deletes - model_snapshot_2
-
-```sql
-{% snapshot model_snapshot_2 %}
-
-{{
-    config
-    (
-        unique_key='id',
-        strategy='timestamp',
-        updated_at='refresh_timestamp',
-        invalidate_hard_deletes=True,
-    )
-}}
-select *
-from {{ ref('model') }} {% endsnapshot %}
-```
-
-check strategy - model_snapshot_3
-
-```sql
-{% snapshot model_snapshot_3 %}
-
-{{
-    config
-    (
-        unique_key='id',
-        strategy='check',
-        check_cols=['series_reference','data_value']
-    )
-}}
-select *
-from {{ ref('model') }} {% endsnapshot %}
-```
-
-### Snapshots Known issues
-
-- Incremental Iceberg models - Sync all columns on schema change can't remove columns used as partitioning.
-  The only way, from a dbt perspective, is to do a full-refresh of the incremental model.
-
-- Tables, schemas and database should only be lowercase
-
-- In order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/dbt-athena) is not
-  installed in the target environment.
-  See <https://github.com/dbt-athena/dbt-athena/issues/103> for more details.
-
-- Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column
-  from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
+[pre-installed list]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark-preinstalled-python-libraries.html
+[imported manually]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-libraries.html
 
 ## Contracts
 
 The adapter partly supports contract definition.
 
 - Concerning the `data_type`, it is supported but needs to be adjusted for complex types. They must be specified
   entirely (for instance `array<int>`) even though they won't be checked. Indeed, as dbt recommends, we only compare
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.0rc1 Summary: The
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.1 Summary: The
 athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
 dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Python: >=3.8,<3.13
 Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
 Dist: dbt-common<2.0,>=1.0.0b2 Requires-Dist: dbt-adapters<2.0,>=1.0.0b2
-Requires-Dist: boto3>=1.28 Requires-Dist: boto3-stubs
-[athena,glue,lakeformation,sts]>=1.28 Requires-Dist: pyathena<4.0,>=2.25
+Requires-Dist: dbt-core>=1.8.0 Requires-Dist: boto3>=1.28 Requires-Dist: boto3-
+stubs[athena,glue,lakeformation,sts]>=1.28 Requires-Dist: pyathena<4.0,>=2.25
 Requires-Dist: mmh3<4.2.0,>=4.0.1 Requires-Dist: pydantic<3.0,>=1.10 Requires-
 Dist: tenacity~=8.2
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
 dbt-athena-long.png]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_._s_v_g_]_[_h_t_t_p_s_:_/
  _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
     _b_a_d_g_e_/_%_2_0_i_m_p_o_r_t_s_-_i_s_o_r_t_-_%_2_3_1_6_7_4_b_1_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_e_f_8_3_3_6_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]_[_h_t_t_p_s_:_/_/_w_w_w_._m_y_p_y_-_l_a_n_g_._o_r_g_/
@@ -24,19 +24,20 @@
 - [Features](#features) - [Quick Start](#quick-start) - [Installation]
 (#installation) - [Prerequisites](#prerequisites) - [Credentials](#credentials)
 - [Configuring your profile](#configuring-your-profile) - [Additional
 information](#additional-information) - [Models](#models) - [Table
 Configuration](#table-configuration) - [Table location](#table-location) -
 [Incremental models](#incremental-models) - [On schema change](#on-schema-
 change) - [Iceberg](#iceberg) - [Highly available table (HA)](#highly-
-available-table-ha) - [HA Known issues](#ha-known-issues) - [Snapshots]
-(#snapshots) - [Timestamp strategy](#timestamp-strategy) - [Check strategy]
-(#check-strategy) - [Hard-deletes](#hard-deletes) - [AWS Lakeformation
-integration](#aws-lakeformation-integration) - [Working example](#working-
-example) - [Snapshots Known issues](#snapshots-known-issues) - [Contracts]
+available-table-ha) - [HA Known issues](#ha-known-issues) - [Update glue data
+catalog](#update-glue-data-catalog) - [Snapshots](#snapshots) - [Timestamp
+strategy](#timestamp-strategy) - [Check strategy](#check-strategy) - [Hard-
+deletes](#hard-deletes) - [Working example](#working-example) - [Snapshots
+Known issues](#snapshots-known-issues) - [AWS Lakeformation integration](#aws-
+lakeformation-integration) - [Python Models](#python-models) - [Contracts]
 (#contracts) - [Contributing](#contributing) - [Contributors â¨]
 (#contributors-) # Features - Supports dbt version `1.7.*` - Support for Python
 - Supports [seeds][seeds] - Correctly detects views and their columns -
 Supports [table materialization][table] - [Iceberg tables][athena-iceberg] are
 supported **only with Athena Engine v3** and **a unique table location** (see
 table location section below) - Hive tables are supported by both Athena
 engines. - Supports [incremental models][incremental] - On Iceberg tables : -
@@ -262,98 +263,35 @@
 the materialization keeps the last 4 table versions, you can change it by
 setting `versions_to_keep`. #### HA Known issues - When swapping from a table
 with partitions to a table without (and the other way around), there could be a
 little downtime. In case high performances are needed consider bucketing
 instead of partitions - By default, Glue "duplicates" the versions internally,
 so the last two versions of a table point to the same location - It's
 recommended to have `versions_to_keep` >= 4, as this will avoid having the
-older location removed ## Snapshots The adapter supports snapshot
-materialization. It supports both timestamp and check strategy. To create a
-snapshot create a snapshot file in the snapshots directory. If the directory
-does not exist create one. ### Timestamp strategy To use the timestamp strategy
-refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
-strategy-recommended) ### Check strategy To use the check strategy refer to the
-[dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
-Hard-deletes The materialization also supports invalidating hard deletes. Check
-the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
-understand usage. ### AWS Lakeformation integration The adapter implements AWS
-Lakeformation tags management in the following way: - you can enable or disable
-lf-tags management via [config](#table-configuration) (disabled by default) -
-once you enable the feature, lf-tags will be updated on every dbt run - first,
-all lf-tags for columns are removed to avoid inheritance issues - then all
-redundant lf-tags are removed from table and actual tags from config are
-applied - finally, lf-tags for columns are applied It's important to understand
-the following points: - dbt does not manage lf-tags for database - dbt does not
-manage lakeformation permissions That's why you should handle this by yourself
-manually or using some automation tools like terraform, AWS CDK etc. You may
-find the following links useful to manage that: * [terraform
-aws_lakeformation_permissions](https://registry.terraform.io/providers/
-hashicorp/aws/latest/docs/resources/lakeformation_permissions) * [terraform
-aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/
-hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags) ## Python
-Models The adapter supports python models using [`spark`](https://
-docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html). ### Setup - A spark
-enabled work group created in athena - Spark execution role granted access to
-Athena, Glue and S3 - The spark work group is added to the ~/.dbt/profiles.yml
-file and the profile is referenced in dbt_project.yml that will be created. It
-is recommended to keep this same as threads. ### Spark specific table
-configuration - `timeout` (`default=43200`) - Time out in seconds for each
-python model execution. Defaults to 12 hours/43200 seconds. -
-`spark_encryption` (`default=false`) - If this flag is set to true, encrypts
-data in transit between Spark nodes and also encrypts data at rest stored
-locally by Spark. - `spark_cross_account_catalog` (`default=false`) - In spark,
-you can query the external account catalog and for that the consumer account
-has to be configured to access the producer catalog. - If this flag is set to
-true, "/" can be used as the glue catalog separator. Ex: 999999999999/
-mydatabase.cloudfront_logs (*where *999999999999* is the external catalog id*)
-- `spark_requester_pays` (`default=false`) - When an Amazon S3 bucket is
-configured as requester pays, the account of the user running the query is
-charged for data access and data transfer fees associated with the query. - If
-this flag is set to true, requester pays S3 buckets are enabled in Athena for
-Spark. ### Spark notes - A session is created for each unique engine
-configuration defined in the models that are part of the invocation. - A
-session's idle timeout is set to 10 minutes. Within the timeout period, if
-there is a new calculation (spark python model) ready for execution and the
-engine configuration matches, the process will reuse the same session. - Number
-of python models running at a time depends on the `threads`. Number of sessions
-created for the entire run depends on number of unique engine configurations
-and availability of session to maintain threads concurrency. - For iceberg
-table, it is recommended to use table_properties configuration to set the
-format_version to 2. This is to maintain compatability between iceberg tables
-created by Trino with those created by Spark. ### Example models #### Simple
-pandas model ```python import pandas as pd def model(dbt, session): dbt.config
-(materialized="table") model_df = pd.DataFrame({"A": [1, 2, 3, 4]}) return
-model_df ``` #### Simple spark ```python def model(dbt, spark_session):
-dbt.config(materialized="table") data = [(1,), (2,), (3,), (4,)] df =
-spark_session.createDataFrame(data, ["A"]) return df ``` #### Spark incremental
-```python def model(dbt, spark_session): dbt.config(materialized="incremental")
-df = dbt.ref("model") if dbt.is_incremental: max_from_this = ( f"select max
-(run_date) from {dbt.this.schema}.{dbt.this.identifier}" ) df = df.filter
-(df.run_date >= spark_session.sql(max_from_this).collect()[0][0]) return df ```
-#### Config spark model ```python def model(dbt, spark_session): dbt.config
-( materialized="table", engine_config={ "CoordinatorDpuSize": 1,
-"MaxConcurrentDpus": 3, "DefaultExecutorDpuSize": 1 }, spark_encryption=True,
-spark_cross_account_catalog=True, spark_requester_pays=True
-polling_interval=15, timeout=120, ) data = [(1,), (2,), (3,), (4,)] df =
-spark_session.createDataFrame(data, ["A"]) return df ``` #### Create pySpark
-udf using imported external python files ```python def model(dbt,
-spark_session): dbt.config( materialized="incremental",
-incremental_strategy="merge", unique_key="num", ) sc =
-spark_session.sparkContext sc.addPyFile("s3://athena-dbt/test/file1.py")
-sc.addPyFile("s3://athena-dbt/test/file2.py") def func(iterator): from file2
-import transform return [transform(i) for i in iterator] from
-pyspark.sql.functions import udf from pyspark.sql.functions import col
-udf_with_import = udf(func) data = [(1, "a"), (2, "b"), (3, "c")] cols =
-["num", "alpha"] df = spark_session.createDataFrame(data, cols) return
-df.withColumn("udf_test_col", udf_with_import(col("alpha"))) ``` #### Known
-issues in python models - Incremental models do not fully utilize spark
-capabilities. They depend partially on existing sql based logic which runs on
-trino. - Snapshots materializations are not supported. - Spark can only
-reference tables within the same catalog. ### Working example seed file -
-employent_indicators_november_2022_csv_tables.csv ```csv
+older location removed ### Update glue data catalog Optionally persist resource
+descriptions as column and relation comments to the glue data catalog, and meta
+as [glue table properties](https://docs.aws.amazon.com/glue/latest/dg/tables-
+described.html#table-properties) and [column parameters](https://
+docs.aws.amazon.com/glue/latest/webapi/API_Column.html). By default,
+documentation persistence is disabled, but it can be enabled for specific
+resources or groups of resources as needed. For example: ```yaml models: -
+name: test_deduplicate description: another value config: persist_docs:
+relation: true columns: true meta: test: value columns: - name: id meta:
+primary_key: true ``` See [persist docs](https://docs.getdbt.com/reference/
+resource-configs/persist_docs) for more details. ## Snapshots The adapter
+supports snapshot materialization. It supports both timestamp and check
+strategy. To create a snapshot create a snapshot file in the snapshots
+directory. If the directory does not exist create one. ### Timestamp strategy
+To use the timestamp strategy refer to the [dbt docs](https://docs.getdbt.com/
+docs/build/snapshots#timestamp-strategy-recommended) ### Check strategy To use
+the check strategy refer to the [dbt docs](https://docs.getdbt.com/docs/build/
+snapshots#check-strategy) ### Hard-deletes The materialization also supports
+invalidating hard deletes. Check the [docs](https://docs.getdbt.com/docs/build/
+snapshots#hard-deletes-opt-in) to understand usage. ### Working example seed
+file - employent_indicators_november_2022_csv_tables.csv ```csv
 Series_reference,Period,Data_value,Suppressed MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803, MEIM.S1WA,1999.06,65792, MEIM.S1WA,1999.07,66194,
 MEIM.S1WA,1999.08,67259, MEIM.S1WA,1999.09,69691, MEIM.S1WA,1999.1,72475,
 MEIM.S1WA,1999.11,79263, MEIM.S1WA,1999.12,86540, MEIM.S1WA,2000.01,82552,
 MEIM.S1WA,2000.02,81709, MEIM.S1WA,2000.03,84126, MEIM.S1WA,2000.04,77089,
 MEIM.S1WA,2000.05,73811, MEIM.S1WA,2000.06,70070, MEIM.S1WA,2000.07,69873,
 MEIM.S1WA,2000.08,71468, MEIM.S1WA,2000.09,72462, MEIM.S1WA,2000.1,74897, ```
@@ -375,19 +313,102 @@
 The only way, from a dbt perspective, is to do a full-refresh of the
 incremental model. - Tables, schemas and database should only be lowercase - In
 order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://
 github.com/Tomme/dbt-athena) is not installed in the target environment. See
 github.com/dbt-athena/dbt-athena/issues/103> for more details. - Snapshot does
 not support dropping columns from the source table. If you drop a column make
 sure to drop the column from the snapshot as well. Another workaround is to
-NULL the column in the snapshot definition to preserve history ## Contracts The
-adapter partly supports contract definition. - Concerning the `data_type`, it
-is supported but needs to be adjusted for complex types. They must be specified
-entirely (for instance `array`) even though they won't be checked. Indeed, as
-dbt recommends, we only compare the broader type (array, map, int, varchar).
-The complete definition is used in order to check that the data types defined
-in athena are ok (pre-flight check). - the adapter does not support the
-constraints since no constraints don't exist in Athena. ## Contributing See
-[CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
-this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
-_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-_a_t_h_e_n_a_]Contributions of any kind welcome!
+NULL the column in the snapshot definition to preserve history ## AWS
+Lakeformation integration The adapter implements AWS Lakeformation tags
+management in the following way: - you can enable or disable lf-tags management
+via [config](#table-configuration) (disabled by default) - once you enable the
+feature, lf-tags will be updated on every dbt run - first, all lf-tags for
+columns are removed to avoid inheritance issues - then all redundant lf-tags
+are removed from table and actual tags from config are applied - finally, lf-
+tags for columns are applied It's important to understand the following points:
+- dbt does not manage lf-tags for database - dbt does not manage lakeformation
+permissions That's why you should handle this by yourself manually or using
+some automation tools like terraform, AWS CDK etc. You may find the following
+links useful to manage that: * [terraform aws_lakeformation_permissions](https:
+//registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/
+lakeformation_permissions) * [terraform aws_lakeformation_resource_lf_tags]
+(https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/
+lakeformation_resource_lf_tags) ## Python Models The adapter supports python
+models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-
+spark.html). ### Setup - A Spark-enabled workgroup created in Athena - Spark
+execution role granted access to Athena, Glue and S3 - The Spark workgroup is
+added to the `~/.dbt/profiles.yml` file and the profile is referenced in
+`dbt_project.yml` that will be created. It is recommended to keep this same as
+threads. ### Spark-specific table configuration - `timeout` (`default=43200`) -
+Time out in seconds for each Python model execution. Defaults to 12 hours/43200
+seconds. - `spark_encryption` (`default=false`) - If this flag is set to true,
+encrypts data in transit between Spark nodes and also encrypts data at rest
+stored locally by Spark. - `spark_cross_account_catalog` (`default=false`) - In
+Spark, you can query the external account catalog and for that the consumer
+account has to be configured to access the producer catalog. - If this flag is
+set to true, "/" can be used as the glue catalog separator. Ex: 999999999999/
+mydatabase.cloudfront_logs (*where *999999999999* is the external catalog ID*)
+- `spark_requester_pays` (`default=false`) - When an Amazon S3 bucket is
+configured as requester pays, the account of the user running the query is
+charged for data access and data transfer fees associated with the query. - If
+this flag is set to true, requester pays S3 buckets are enabled in Athena for
+Spark. ### Spark notes - A session is created for each unique engine
+configuration defined in the models that are part of the invocation. - A
+session's idle timeout is set to 10 minutes. Within the timeout period, if
+there is a new calculation (Spark Python model) ready for execution and the
+engine configuration matches, the process will reuse the same session. - The
+number of Python models running at a time depends on the `threads`. The number
+of sessions created for the entire run depends on the number of unique engine
+configurations and the availability of sessions to maintain thread concurrency.
+- For Iceberg tables, it is recommended to use `table_properties` configuration
+to set the `format_version` to 2. This is to maintain compatibility between
+Iceberg tables created by Trino with those created by Spark. ### Example models
+#### Simple pandas model ```python import pandas as pd def model(dbt, session):
+dbt.config(materialized="table") model_df = pd.DataFrame({"A": [1, 2, 3, 4]})
+return model_df ``` #### Simple spark ```python def model(dbt, spark_session):
+dbt.config(materialized="table") data = [(1,), (2,), (3,), (4,)] df =
+spark_session.createDataFrame(data, ["A"]) return df ``` #### Spark incremental
+```python def model(dbt, spark_session): dbt.config(materialized="incremental")
+df = dbt.ref("model") if dbt.is_incremental: max_from_this = ( f"select max
+(run_date) from {dbt.this.schema}.{dbt.this.identifier}" ) df = df.filter
+(df.run_date >= spark_session.sql(max_from_this).collect()[0][0]) return df ```
+#### Config spark model ```python def model(dbt, spark_session): dbt.config
+( materialized="table", engine_config={ "CoordinatorDpuSize": 1,
+"MaxConcurrentDpus": 3, "DefaultExecutorDpuSize": 1 }, spark_encryption=True,
+spark_cross_account_catalog=True, spark_requester_pays=True
+polling_interval=15, timeout=120, ) data = [(1,), (2,), (3,), (4,)] df =
+spark_session.createDataFrame(data, ["A"]) return df ``` #### Create pySpark
+udf using imported external python files ```python def model(dbt,
+spark_session): dbt.config( materialized="incremental",
+incremental_strategy="merge", unique_key="num", ) sc =
+spark_session.sparkContext sc.addPyFile("s3://athena-dbt/test/file1.py")
+sc.addPyFile("s3://athena-dbt/test/file2.py") def func(iterator): from file2
+import transform return [transform(i) for i in iterator] from
+pyspark.sql.functions import udf from pyspark.sql.functions import col
+udf_with_import = udf(func) data = [(1, "a"), (2, "b"), (3, "c")] cols =
+["num", "alpha"] df = spark_session.createDataFrame(data, cols) return
+df.withColumn("udf_test_col", udf_with_import(col("alpha"))) ``` ### Known
+issues in Python models - Python models cannot [reference Athena SQL views]
+(https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html). - Third-
+party Python libraries can be used, but they must be [included in the pre-
+installed list]([pre-installed list]) or [imported manually]([imported
+manually]). - Python models can only reference or write to tables with names
+meeting the regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special
+characters are not supported by Spark, even though Athena supports them. -
+Incremental models do not fully utilize Spark capabilities. They depend
+partially on existing SQL-based logic which runs on Trino. - Snapshot
+materializations are not supported. - Spark can only reference tables within
+the same catalog. [pre-installed list]: https://docs.aws.amazon.com/athena/
+latest/ug/notebooks-spark-preinstalled-python-libraries.html [imported
+manually]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-
+libraries.html ## Contracts The adapter partly supports contract definition. -
+Concerning the `data_type`, it is supported but needs to be adjusted for
+complex types. They must be specified entirely (for instance `array`) even
+though they won't be checked. Indeed, as dbt recommends, we only compare the
+broader type (array, map, int, varchar). The complete definition is used in
+order to check that the data types defined in athena are ok (pre-flight check).
+- the adapter does not support the constraints since no constraints don't exist
+in Athena. ## Contributing See [CONTRIBUTING](CONTRIBUTING.md) for more
+information on how to contribute to this project. ## Contributors â¨ Thanks
+goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
+en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-
+_a_t_h_e_n_a_]Contributions of any kind welcome!
```

### Comparing `dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/SOURCES.txt` & `dbt_athena_community-1.8.1/dbt_athena_community.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/pyproject.toml` & `dbt_athena_community-1.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0rc1/setup.py` & `dbt_athena_community-1.8.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     license_files=("LICENSE.txt",),
     url="https://github.com/dbt-athena/dbt-athena",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-common>=1.0.0b2,<2.0",
         "dbt-adapters>=1.0.0b2,<2.0",
+        # add dbt-core to ensure backwards compatibility of installation, this is not a functional dependency
+        "dbt-core>=1.8.0",
         "boto3>=1.28",
         "boto3-stubs[athena,glue,lakeformation,sts]>=1.28",
         "pyathena>=2.25,<4.0",
         "mmh3>=4.0.1,<4.2.0",
         "pydantic>=1.10,<3.0",
         "tenacity~=8.2",
     ],
```

