# Comparing `tmp/types-sqlalchemy-utils-1.0.1.tar.gz` & `tmp/types_sqlalchemy_utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-sqlalchemy-utils-1.0.1.tar", last modified: Thu Aug 11 10:55:26 2022, max compression
+gzip compressed data, was "types_sqlalchemy_utils-1.1.0.tar", last modified: Mon May 13 08:32:52 2024, max compression
```

## Comparing `types-sqlalchemy-utils-1.0.1.tar` & `types_sqlalchemy_utils-1.1.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:55:26.385076 types-sqlalchemy-utils-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-08-11 10:55:26.385076 types-sqlalchemy-utils-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-08-11 10:55:26.385076 types-sqlalchemy-utils-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2144 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:55:26.377076 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)     4002 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/aggregates.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/asserts.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/batch.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/expression_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/expressions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:55:26.381076 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/functions/
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/functions/database.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/functions/defer_except.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/functions/foreign_keys.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/functions/mock.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/functions/orm.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/functions/render.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/functions/sort_query.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/generic.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/i18n.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/listeners.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/models.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/observer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/operators.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/path.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:55:26.381076 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/primitives/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/primitives/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/primitives/country.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/primitives/currency.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/primitives/ltree.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/primitives/weekday.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/primitives/weekdays.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/proxy_dict.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/query_chain.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:55:26.381076 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/relationships/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/relationships/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/relationships/chained_join.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:55:26.381076 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/arrow.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/bit.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/choice.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/color.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/country.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/currency.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/email.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:55:26.381076 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/encrypted/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/encrypted/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/encrypted/encrypted_type.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/encrypted/padding.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:55:26.385076 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/enriched_datetime/
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/enriched_datetime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/enriched_datetime/arrow_datetime.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/enriched_datetime/enriched_date_type.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/enriched_datetime/enriched_datetime_type.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/enriched_datetime/pendulum_date.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/enriched_datetime/pendulum_datetime.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/ip_address.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/json.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/locale.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/ltree.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/password.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/pg_composite.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/phone_number.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/range.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/scalar_coercible.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/scalar_list.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/timezone.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/ts_vector.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/url.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/uuid.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/weekdays.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-08-11 10:54:47.000000 types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/view.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 10:55:26.385076 types-sqlalchemy-utils-1.0.1/types_sqlalchemy_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-08-11 10:55:26.000000 types-sqlalchemy-utils-1.0.1/types_sqlalchemy_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3298 2022-08-11 10:55:26.000000 types-sqlalchemy-utils-1.0.1/types_sqlalchemy_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-11 10:55:26.000000 types-sqlalchemy-utils-1.0.1/types_sqlalchemy_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-11 10:55:26.000000 types-sqlalchemy-utils-1.0.1/types_sqlalchemy_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-11 10:55:26.000000 types-sqlalchemy-utils-1.0.1/types_sqlalchemy_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:32:52.938516 types_sqlalchemy_utils-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-13 08:32:52.938516 types_sqlalchemy_utils-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-13 08:32:52.942516 types_sqlalchemy_utils-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:32:52.926516 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/aggregates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/asserts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/expression_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/expressions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:32:52.930516 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/functions/database.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/functions/defer_except.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/functions/foreign_keys.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/functions/mock.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/functions/orm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/functions/render.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/functions/sort_query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/generic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/i18n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/listeners.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/observer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/operators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/path.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:32:52.930516 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/primitives/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/primitives/country.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/primitives/currency.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/primitives/ltree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/primitives/weekday.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/primitives/weekdays.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/proxy_dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/query_chain.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:32:52.930516 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/relationships/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/relationships/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/relationships/chained_join.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:32:52.934516 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/arrow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/bit.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/choice.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/color.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/country.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/currency.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/email.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:32:52.938516 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/encrypted/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/encrypted/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/encrypted/encrypted_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/encrypted/padding.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:32:52.938516 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/enriched_datetime/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/enriched_datetime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/enriched_datetime/arrow_datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/enriched_datetime/enriched_date_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/enriched_datetime/enriched_datetime_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/enriched_datetime/pendulum_date.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/enriched_datetime/pendulum_datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/ip_address.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/locale.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/ltree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/password.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/pg_composite.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/phone_number.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/range.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/scalar_coercible.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/scalar_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/timezone.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/ts_vector.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/url.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/uuid.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/weekdays.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-13 08:32:10.000000 types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/view.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:32:52.938516 types_sqlalchemy_utils-1.1.0/types_sqlalchemy_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-13 08:32:52.000000 types_sqlalchemy_utils-1.1.0/types_sqlalchemy_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-13 08:32:52.000000 types_sqlalchemy_utils-1.1.0/types_sqlalchemy_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:32:52.000000 types_sqlalchemy_utils-1.1.0/types_sqlalchemy_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-13 08:32:52.000000 types_sqlalchemy_utils-1.1.0/types_sqlalchemy_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 08:32:52.000000 types_sqlalchemy_utils-1.1.0/types_sqlalchemy_utils.egg-info/top_level.txt
```

### Comparing `types-sqlalchemy-utils-1.0.1/LICENSE` & `types_sqlalchemy_utils-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `types-sqlalchemy-utils-1.0.1/PKG-INFO` & `types_sqlalchemy_utils-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-sqlalchemy-utils
-Version: 1.0.1
+Version: 1.1.0
 Summary: Type Stubs for sqlalchemy-utils
 Home-page: https://github.com/cex-solutions/sqlalchemy-utils
 Author: Binovate Labs
 Author-email: cex-dev@binovate.com
 License: GPLv3
 Project-URL: Bug Reports, https://github.com/cex-solutions/types-sqlalchemy-utils/issues
 Project-URL: Source, https://github.com/cex-solutions/types-sqlalchemy-utils
@@ -16,16 +16,21 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: sqlalchemy-utils==0.41.2; extra == "dev"
+Requires-Dist: sqlalchemy2-stubs==0.0.2a38; extra == "dev"
+Requires-Dist: mypy==1.10.0; extra == "dev"
+Requires-Dist: pipenv-setup==3.2.0; extra == "dev"
+Requires-Dist: twine==5.0.0; extra == "dev"
 
 # types-sqlalchemy-utils
 
 This is a package containing type annotations
 for [sqlalchemy-utils](https://pypi.org/project/sqlalchemy-utils/).
 
 ### Installing:
```

### Comparing `types-sqlalchemy-utils-1.0.1/README.md` & `types_sqlalchemy_utils-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `types-sqlalchemy-utils-1.0.1/setup.py` & `types_sqlalchemy_utils-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-"""A setuptools based setup module.
-See:
-https://packaging.python.org/guides/distributing-packages-using-setuptools/
-https://github.com/pypa/sampleproject
-Modified by Madoshakalaka@Github (dependency links added)
-"""
 from os import path
 
 from setuptools import glob
 from setuptools import setup
 
 # Always prefer setuptools over distutils
 
@@ -45,19 +39,19 @@
         + ["METADATA.toml"]
     },
     packages=["sqlalchemy_utils-stubs"],
     python_requires=">=3.7, <4",
     install_requires=[],
     extras_require={
         "dev": [
-            "sqlalchemy-utils==0.38.3",
-            "sqlalchemy2-stubs==0.0.2a25",
-            "mypy==0.971",
+            "sqlalchemy-utils==0.41.2",
+            "sqlalchemy2-stubs==0.0.2a38",
+            "mypy==1.10.0",
             "pipenv-setup==3.2.0",
-            "twine==4.0.1",
+            "twine==5.0.0",
         ]
     },
     dependency_links=[],
     project_urls={
         "Bug Reports": "https://github.com/cex-solutions/types-sqlalchemy-utils/issues",
         "Source": "https://github.com/cex-solutions/types-sqlalchemy-utils",
     },
```

### Comparing `types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/__init__.pyi` & `types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/functions/__init__.pyi` & `types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/functions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/functions/database.pyi` & `types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/functions/database.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from sqlalchemy import Column, ForeignKeyConstraint
 from sqlalchemy.engine import URL
 from sqlalchemy.sql.functions import Function
 from typing_extensions import TypeAlias
 
 from ..utils import starts_with as starts_with
 from .orm import quote as quote
-from typing import Union, Optional, Any
+from typing import Any
 
 # Should be `_VT: TypeAlias = Union[int, float, str, Mapping[str, "_VT"], Sequence["_VT"]]`
 # But recursive types are not yet fully supported by mypy. See https://github.com/python/mypy/issues/731
-_VT: TypeAlias = Union[int, float, str, Mapping[str, Any], Sequence[Any]]
+_VT: TypeAlias = int | float | str | Mapping[str, Any] | Sequence[Any]
 
 def escape_like(string: str, escape_char: str = ...) -> str: ...
 def json_sql(value: _VT, scalars_to_json: bool = ...) -> Function[Any]: ...
 def jsonb_sql(value: _VT, scalars_to_jsonb: bool = ...) -> Function[Any]: ...
-def has_index(column_or_constraint: Union[Column[Any], ForeignKeyConstraint]) -> bool: ...
-def has_unique_index(column_or_constraint: Union[Column[Any], ForeignKeyConstraint]) -> bool: ...
+def has_index(column_or_constraint: Column[Any] | ForeignKeyConstraint) -> bool: ...
+def has_unique_index(column_or_constraint: Column[Any] | ForeignKeyConstraint) -> bool: ...
 def is_auto_assigned_date_column(column: Column[Any]) -> bool: ...
-def database_exists(url: Union[URL, str]) -> bool: ...
-def create_database(url: Union[URL, str], encoding: str = ..., template: Optional[str] = ...) -> None: ...
-def drop_database(url: Union[URL, str]) -> None: ...
+def database_exists(url: URL | str) -> bool: ...
+def create_database(url: URL | str, encoding: str = ..., template: str | None = ...) -> None: ...
+def drop_database(url: URL | str) -> None: ...
```

### Comparing `types-sqlalchemy-utils-1.0.1/sqlalchemy_utils-stubs/types/__init__.pyi` & `types_sqlalchemy_utils-1.1.0/sqlalchemy_utils-stubs/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-sqlalchemy-utils-1.0.1/types_sqlalchemy_utils.egg-info/PKG-INFO` & `types_sqlalchemy_utils-1.1.0/types_sqlalchemy_utils.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-sqlalchemy-utils
-Version: 1.0.1
+Version: 1.1.0
 Summary: Type Stubs for sqlalchemy-utils
 Home-page: https://github.com/cex-solutions/sqlalchemy-utils
 Author: Binovate Labs
 Author-email: cex-dev@binovate.com
 License: GPLv3
 Project-URL: Bug Reports, https://github.com/cex-solutions/types-sqlalchemy-utils/issues
 Project-URL: Source, https://github.com/cex-solutions/types-sqlalchemy-utils
@@ -16,16 +16,21 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: sqlalchemy-utils==0.41.2; extra == "dev"
+Requires-Dist: sqlalchemy2-stubs==0.0.2a38; extra == "dev"
+Requires-Dist: mypy==1.10.0; extra == "dev"
+Requires-Dist: pipenv-setup==3.2.0; extra == "dev"
+Requires-Dist: twine==5.0.0; extra == "dev"
 
 # types-sqlalchemy-utils
 
 This is a package containing type annotations
 for [sqlalchemy-utils](https://pypi.org/project/sqlalchemy-utils/).
 
 ### Installing:
```

### Comparing `types-sqlalchemy-utils-1.0.1/types_sqlalchemy_utils.egg-info/SOURCES.txt` & `types_sqlalchemy_utils-1.1.0/types_sqlalchemy_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

