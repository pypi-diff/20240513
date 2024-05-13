# Comparing `tmp/eric_devtools-0.1.0.tar.gz` & `tmp/eric_devtools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eric_devtools-0.1.0.tar", max compression
+gzip compressed data, was "eric_devtools-0.2.0.tar", max compression
```

## Comparing `eric_devtools-0.1.0.tar` & `eric_devtools-0.2.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0       21 2024-05-10 18:11:19.147060 eric_devtools-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-21 22:43:10.206477 eric_devtools-0.1.0/devtools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 22:14:28.239755 eric_devtools-0.1.0/devtools/adapters/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 22:43:02.145983 eric_devtools-0.1.0/devtools/adapters/database/__init__.py
--rw-r--r--   0        0        0    11120 2024-05-10 17:46:17.839233 eric_devtools-0.1.0/devtools/adapters/database/aiomysql.py
--rw-r--r--   0        0        0    11086 2024-05-10 17:46:17.839233 eric_devtools-0.1.0/devtools/adapters/database/asyncmy.py
--rw-r--r--   0        0        0     9592 2024-05-09 15:45:12.999368 eric_devtools-0.1.0/devtools/adapters/database/asyncpg.py
--rw-r--r--   0        0        0      759 2024-05-07 18:49:43.032060 eric_devtools-0.1.0/devtools/adapters/database/config.py
--rw-r--r--   0        0        0      721 2024-04-21 22:42:55.028730 eric_devtools-0.1.0/devtools/attrs/__init__.py
--rw-r--r--   0        0        0     3514 2024-03-17 16:05:50.108601 eric_devtools-0.1.0/devtools/attrs/camel.py
--rw-r--r--   0        0        0      146 2024-04-04 19:39:45.843803 eric_devtools-0.1.0/devtools/attrs/converters/__init__.py
--rw-r--r--   0        0        0      726 2024-03-18 15:59:47.703808 eric_devtools-0.1.0/devtools/attrs/converters/json.py
--rw-r--r--   0        0        0     1289 2024-04-21 22:43:02.726018 eric_devtools-0.1.0/devtools/attrs/converters/utils.py
--rw-r--r--   0        0        0     9333 2024-04-21 22:43:04.016097 eric_devtools-0.1.0/devtools/attrs/field.py
--rw-r--r--   0        0        0     6257 2024-05-10 17:46:17.779230 eric_devtools-0.1.0/devtools/attrs/helpers.py
--rw-r--r--   0        0        0    29321 2024-05-10 17:46:17.789231 eric_devtools-0.1.0/devtools/attrs/main.py
--rw-r--r--   0        0        0     5078 2024-04-21 22:42:39.007742 eric_devtools-0.1.0/devtools/attrs/methods.py
--rw-r--r--   0        0        0     4351 2024-04-21 22:42:59.465869 eric_devtools-0.1.0/devtools/attrs/resolver.py
--rw-r--r--   0        0        0     4000 2024-04-04 19:38:26.289839 eric_devtools-0.1.0/devtools/attrs/schema.py
--rw-r--r--   0        0        0     5559 2024-05-10 17:46:17.789231 eric_devtools-0.1.0/devtools/attrs/shortcuts.py
--rw-r--r--   0        0        0        0 2024-03-16 02:20:39.153487 eric_devtools-0.1.0/devtools/attrs/utils/__init__.py
--rw-r--r--   0        0        0      627 2024-03-16 03:12:25.208751 eric_devtools-0.1.0/devtools/attrs/utils/factory.py
--rw-r--r--   0        0        0     5650 2024-04-21 22:42:40.317827 eric_devtools-0.1.0/devtools/attrs/utils/functions.py
--rw-r--r--   0        0        0      640 2024-03-18 01:58:29.274268 eric_devtools-0.1.0/devtools/attrs/utils/typedef.py
--rw-r--r--   0        0        0        0 2024-05-07 17:45:34.992103 eric_devtools-0.1.0/devtools/cache/__init__.py
--rw-r--r--   0        0        0      933 2024-05-10 17:46:17.749228 eric_devtools-0.1.0/devtools/config/__init__.py
--rw-r--r--   0        0        0       78 2024-05-05 22:01:38.006258 eric_devtools-0.1.0/devtools/config/adapter/__init__.py
--rw-r--r--   0        0        0     1263 2024-05-05 22:43:21.724738 eric_devtools-0.1.0/devtools/config/adapter/attrs.py
--rw-r--r--   0        0        0     1011 2024-05-07 17:59:46.908235 eric_devtools-0.1.0/devtools/config/adapter/dataclass.py
--rw-r--r--   0        0        0      986 2024-05-08 15:54:08.339353 eric_devtools-0.1.0/devtools/config/adapter/dattrs.py
--rw-r--r--   0        0        0     8206 2024-05-10 17:46:17.759229 eric_devtools-0.1.0/devtools/config/adapter/factory.py
--rw-r--r--   0        0        0     6764 2024-05-05 22:43:21.724738 eric_devtools-0.1.0/devtools/config/adapter/helpers.py
--rw-r--r--   0        0        0     2047 2024-05-10 17:46:17.759229 eric_devtools-0.1.0/devtools/config/adapter/interface.py
--rw-r--r--   0        0        0     2026 2024-05-05 22:33:39.353269 eric_devtools-0.1.0/devtools/config/adapter/mark.py
--rw-r--r--   0        0        0     2046 2024-05-05 22:43:21.714738 eric_devtools-0.1.0/devtools/config/adapter/pydantic.py
--rw-r--r--   0        0        0      341 2024-05-10 17:46:17.769230 eric_devtools-0.1.0/devtools/context/__init__.py
--rw-r--r--   0        0        0      253 2024-04-28 12:58:49.476345 eric_devtools-0.1.0/devtools/context/atomic_/__init__.py
--rw-r--r--   0        0        0     2300 2024-05-10 17:46:17.769230 eric_devtools-0.1.0/devtools/context/atomic_/bound.py
--rw-r--r--   0        0        0     2479 2024-05-10 17:46:17.769230 eric_devtools-0.1.0/devtools/context/atomic_/core.py
--rw-r--r--   0        0        0     1252 2024-05-05 21:56:29.734124 eric_devtools-0.1.0/devtools/context/atomic_/resolver.py
--rw-r--r--   0        0        0     5662 2024-05-05 21:56:28.824075 eric_devtools-0.1.0/devtools/context/context.py
--rw-r--r--   0        0        0       82 2024-05-05 21:56:29.724124 eric_devtools-0.1.0/devtools/context/interfaces/__init__.py
--rw-r--r--   0        0        0     1528 2024-05-05 21:56:28.784072 eric_devtools-0.1.0/devtools/context/interfaces/adapter.py
--rw-r--r--   0        0        0       45 2024-05-05 21:55:01.167155 eric_devtools-0.1.0/devtools/context/typedef.py
--rw-r--r--   0        0        0      732 2024-05-07 17:59:43.498042 eric_devtools-0.1.0/devtools/database/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 15:45:14.839455 eric_devtools-0.1.0/devtools/database/config.py
--rw-r--r--   0        0        0        0 2024-05-09 15:45:15.609492 eric_devtools-0.1.0/devtools/database/drivers.py
--rw-r--r--   0        0        0      821 2024-05-07 17:51:49.783408 eric_devtools-0.1.0/devtools/database/entity.py
--rw-r--r--   0        0        0       50 2024-05-07 17:59:42.617992 eric_devtools-0.1.0/devtools/database/metadata.py
--rw-r--r--   0        0        0     3759 2024-05-09 15:45:14.249427 eric_devtools-0.1.0/devtools/database/utils.py
--rw-r--r--   0        0        0      790 2024-05-10 17:46:17.799231 eric_devtools-0.1.0/devtools/env_vars/__init__.py
--rw-r--r--   0        0        0      790 2024-05-10 17:46:17.809232 eric_devtools-0.1.0/devtools/env_vars/config/__init__.py
--rw-r--r--   0        0        0     1549 2024-05-05 22:35:03.201010 eric_devtools-0.1.0/devtools/env_vars/config/_helpers.py
--rw-r--r--   0        0        0     8439 2024-05-10 17:46:17.809232 eric_devtools-0.1.0/devtools/env_vars/config/config.py
--rw-r--r--   0        0        0     2177 2024-05-05 22:41:40.644798 eric_devtools-0.1.0/devtools/env_vars/config/enums.py
--rw-r--r--   0        0        0     4822 2024-05-05 22:43:21.784740 eric_devtools-0.1.0/devtools/env_vars/config/envconfig.py
--rw-r--r--   0        0        0     1414 2024-05-05 22:35:02.090967 eric_devtools-0.1.0/devtools/env_vars/config/exceptions.py
--rw-r--r--   0        0        0      926 2024-05-05 22:33:39.403271 eric_devtools-0.1.0/devtools/env_vars/config/interface.py
--rw-r--r--   0        0        0     7142 2024-05-05 22:35:14.920526 eric_devtools-0.1.0/devtools/env_vars/config/utils.py
--rw-r--r--   0        0        0     1297 2024-04-21 22:43:00.915927 eric_devtools-0.1.0/devtools/exc.py
--rw-r--r--   0        0        0      185 2024-05-07 17:32:51.140666 eric_devtools-0.1.0/devtools/filetree/__init__.py
--rw-r--r--   0        0        0     1734 2024-05-07 17:32:51.140666 eric_devtools-0.1.0/devtools/filetree/filetree.py
--rw-r--r--   0        0        0      351 2024-05-07 17:32:50.210634 eric_devtools-0.1.0/devtools/filetree/helpers.py
--rw-r--r--   0        0        0     3137 2024-05-07 17:32:51.150666 eric_devtools-0.1.0/devtools/filetree/interface.py
--rw-r--r--   0        0        0     2837 2024-05-07 17:32:51.150666 eric_devtools-0.1.0/devtools/filetree/typedef.py
--rw-r--r--   0        0        0     2775 2024-05-07 17:32:51.140666 eric_devtools-0.1.0/devtools/filetree/virtual.py
--rw-r--r--   0        0        0      293 2024-05-10 17:46:17.859234 eric_devtools-0.1.0/devtools/lazyfields/__init__.py
--rw-r--r--   0        0        0    10006 2024-05-05 21:56:28.864077 eric_devtools-0.1.0/devtools/lazyfields/_lazyfields.py
--rw-r--r--   0        0        0       99 2024-05-07 17:32:51.140666 eric_devtools-0.1.0/devtools/models/__init__.py
--rw-r--r--   0        0        0      916 2024-04-21 22:43:07.396305 eric_devtools-0.1.0/devtools/models/model.py
--rw-r--r--   0        0        0        0 2024-05-06 13:04:58.756863 eric_devtools-0.1.0/devtools/models/v1/__init__.py
--rw-r--r--   0        0        0     1807 2024-05-07 17:32:50.240635 eric_devtools-0.1.0/devtools/models/v1/model.py
--rw-r--r--   0        0        0        0 2024-04-28 12:32:58.725984 eric_devtools-0.1.0/devtools/query/__init__.py
--rw-r--r--   0        0        0      113 2024-04-28 12:58:49.526347 eric_devtools-0.1.0/devtools/query/_helpers.py
--rw-r--r--   0        0        0     2998 2024-05-07 17:51:49.683402 eric_devtools-0.1.0/devtools/query/attribute.py
--rw-r--r--   0        0        0     3417 2024-05-05 22:07:05.103477 eric_devtools-0.1.0/devtools/query/comp.py
--rw-r--r--   0        0        0      303 2024-05-05 22:07:05.013469 eric_devtools-0.1.0/devtools/query/exc.py
--rw-r--r--   0        0        0     1538 2024-05-05 22:07:05.943546 eric_devtools-0.1.0/devtools/query/group.py
--rw-r--r--   0        0        0     1739 2024-05-05 22:07:05.943546 eric_devtools-0.1.0/devtools/query/interface.py
--rw-r--r--   0        0        0      266 2024-05-05 22:07:05.023470 eric_devtools-0.1.0/devtools/query/null.py
--rw-r--r--   0        0        0     1324 2024-05-05 22:07:05.933545 eric_devtools-0.1.0/devtools/query/order_by.py
--rw-r--r--   0        0        0     1223 2024-05-05 22:07:05.933545 eric_devtools-0.1.0/devtools/query/paginate.py
--rw-r--r--   0        0        0      186 2024-05-05 22:07:05.023470 eric_devtools-0.1.0/devtools/query/typedef.py
--rw-r--r--   0        0        0      887 2024-05-05 22:07:05.053472 eric_devtools-0.1.0/devtools/query/utils.py
--rw-r--r--   0        0        0     2242 2024-05-05 22:07:05.933545 eric_devtools-0.1.0/devtools/query/where.py
--rw-r--r--   0        0        0        0 2024-04-21 22:42:47.548292 eric_devtools-0.1.0/devtools/tests/__init__.py
--rw-r--r--   0        0        0      186 2024-05-07 17:32:50.220634 eric_devtools-0.1.0/devtools/url/__init__.py
--rw-r--r--   0        0        0     7229 2024-05-07 17:32:50.340639 eric_devtools-0.1.0/devtools/url/core.py
--rw-r--r--   0        0        0      423 2024-05-07 17:32:50.240635 eric_devtools-0.1.0/devtools/url/encode.py
--rw-r--r--   0        0        0     1640 2024-05-07 17:32:50.240635 eric_devtools-0.1.0/devtools/url/fragment.py
--rw-r--r--   0        0        0     5036 2024-05-07 17:32:50.320638 eric_devtools-0.1.0/devtools/url/netloc.py
--rw-r--r--   0        0        0     4839 2024-05-07 17:32:50.320638 eric_devtools-0.1.0/devtools/url/path.py
--rw-r--r--   0        0        0     4028 2024-05-07 17:32:50.300637 eric_devtools-0.1.0/devtools/url/query.py
--rw-r--r--   0        0        0     1121 2024-05-07 17:32:51.120666 eric_devtools-0.1.0/devtools/url/utils.py
--rw-r--r--   0        0        0      504 2024-05-09 15:45:16.969556 eric_devtools-0.1.0/devtools/utils/__init__.py
--rw-r--r--   0        0        0      156 2024-05-05 21:56:28.734070 eric_devtools-0.1.0/devtools/utils/exc.py
--rw-r--r--   0        0        0     7823 2024-05-05 21:56:29.684121 eric_devtools-0.1.0/devtools/utils/finder.py
--rw-r--r--   0        0        0     1359 2024-05-09 15:45:16.389529 eric_devtools-0.1.0/devtools/utils/helpers.py
--rw-r--r--   0        0        0      174 2024-05-05 21:56:28.754071 eric_devtools-0.1.0/devtools/utils/json.py
--rw-r--r--   0        0        0     2610 2024-05-05 21:56:28.804073 eric_devtools-0.1.0/devtools/utils/lazy.py
--rw-r--r--   0        0        0     1700 2024-05-05 21:56:29.694122 eric_devtools-0.1.0/devtools/utils/strings.py
--rw-r--r--   0        0        0      134 2024-05-05 21:56:28.754071 eric_devtools-0.1.0/devtools/utils/timezone.py
--rw-r--r--   0        0        0     1211 2024-05-06 02:38:57.954941 eric_devtools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 eric_devtools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       21 2024-05-10 18:11:19.147060 eric_devtools-0.2.0/README.md
+-rw-r--r--   0        0        0      157 2024-05-13 18:39:55.689943 eric_devtools-0.2.0/devtools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 22:14:28.239755 eric_devtools-0.2.0/devtools/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-21 22:43:02.145983 eric_devtools-0.2.0/devtools/adapters/database/__init__.py
+-rw-r--r--   0        0        0    11120 2024-05-10 17:46:17.839233 eric_devtools-0.2.0/devtools/adapters/database/aiomysql.py
+-rw-r--r--   0        0        0    11086 2024-05-10 17:46:17.839233 eric_devtools-0.2.0/devtools/adapters/database/asyncmy.py
+-rw-r--r--   0        0        0     9592 2024-05-09 15:45:12.999368 eric_devtools-0.2.0/devtools/adapters/database/asyncpg.py
+-rw-r--r--   0        0        0      759 2024-05-07 18:49:43.032060 eric_devtools-0.2.0/devtools/adapters/database/config.py
+-rw-r--r--   0        0        0      721 2024-04-21 22:42:55.028730 eric_devtools-0.2.0/devtools/attrs/__init__.py
+-rw-r--r--   0        0        0     3514 2024-03-17 16:05:50.108601 eric_devtools-0.2.0/devtools/attrs/camel.py
+-rw-r--r--   0        0        0      146 2024-04-04 19:39:45.843803 eric_devtools-0.2.0/devtools/attrs/converters/__init__.py
+-rw-r--r--   0        0        0      726 2024-03-18 15:59:47.703808 eric_devtools-0.2.0/devtools/attrs/converters/json.py
+-rw-r--r--   0        0        0     1289 2024-04-21 22:43:02.726018 eric_devtools-0.2.0/devtools/attrs/converters/utils.py
+-rw-r--r--   0        0        0     9333 2024-04-21 22:43:04.016097 eric_devtools-0.2.0/devtools/attrs/field.py
+-rw-r--r--   0        0        0     6257 2024-05-10 17:46:17.779230 eric_devtools-0.2.0/devtools/attrs/helpers.py
+-rw-r--r--   0        0        0    29321 2024-05-10 17:46:17.789231 eric_devtools-0.2.0/devtools/attrs/main.py
+-rw-r--r--   0        0        0     5078 2024-04-21 22:42:39.007742 eric_devtools-0.2.0/devtools/attrs/methods.py
+-rw-r--r--   0        0        0     4351 2024-04-21 22:42:59.465869 eric_devtools-0.2.0/devtools/attrs/resolver.py
+-rw-r--r--   0        0        0     4000 2024-04-04 19:38:26.289839 eric_devtools-0.2.0/devtools/attrs/schema.py
+-rw-r--r--   0        0        0     5559 2024-05-10 17:46:17.789231 eric_devtools-0.2.0/devtools/attrs/shortcuts.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:20:39.153487 eric_devtools-0.2.0/devtools/attrs/utils/__init__.py
+-rw-r--r--   0        0        0      627 2024-03-16 03:12:25.208751 eric_devtools-0.2.0/devtools/attrs/utils/factory.py
+-rw-r--r--   0        0        0     5650 2024-04-21 22:42:40.317827 eric_devtools-0.2.0/devtools/attrs/utils/functions.py
+-rw-r--r--   0        0        0      640 2024-03-18 01:58:29.274268 eric_devtools-0.2.0/devtools/attrs/utils/typedef.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:45:34.992103 eric_devtools-0.2.0/devtools/cache/__init__.py
+-rw-r--r--   0        0        0      933 2024-05-10 17:46:17.749228 eric_devtools-0.2.0/devtools/config/__init__.py
+-rw-r--r--   0        0        0       78 2024-05-05 22:01:38.006258 eric_devtools-0.2.0/devtools/config/adapter/__init__.py
+-rw-r--r--   0        0        0     1263 2024-05-05 22:43:21.724738 eric_devtools-0.2.0/devtools/config/adapter/attrs.py
+-rw-r--r--   0        0        0     1011 2024-05-07 17:59:46.908235 eric_devtools-0.2.0/devtools/config/adapter/dataclass.py
+-rw-r--r--   0        0        0      989 2024-05-12 16:35:13.402399 eric_devtools-0.2.0/devtools/config/adapter/dattrs.py
+-rw-r--r--   0        0        0     8212 2024-05-13 18:39:09.132381 eric_devtools-0.2.0/devtools/config/adapter/factory.py
+-rw-r--r--   0        0        0     6764 2024-05-05 22:43:21.724738 eric_devtools-0.2.0/devtools/config/adapter/helpers.py
+-rw-r--r--   0        0        0     2047 2024-05-10 17:46:17.759229 eric_devtools-0.2.0/devtools/config/adapter/interface.py
+-rw-r--r--   0        0        0     2026 2024-05-05 22:33:39.353269 eric_devtools-0.2.0/devtools/config/adapter/mark.py
+-rw-r--r--   0        0        0     2046 2024-05-05 22:43:21.714738 eric_devtools-0.2.0/devtools/config/adapter/pydantic.py
+-rw-r--r--   0        0        0      341 2024-05-10 17:46:17.769230 eric_devtools-0.2.0/devtools/context/__init__.py
+-rw-r--r--   0        0        0      253 2024-04-28 12:58:49.476345 eric_devtools-0.2.0/devtools/context/atomic_/__init__.py
+-rw-r--r--   0        0        0     2300 2024-05-10 17:46:17.769230 eric_devtools-0.2.0/devtools/context/atomic_/bound.py
+-rw-r--r--   0        0        0     2479 2024-05-10 17:46:17.769230 eric_devtools-0.2.0/devtools/context/atomic_/core.py
+-rw-r--r--   0        0        0     1252 2024-05-05 21:56:29.734124 eric_devtools-0.2.0/devtools/context/atomic_/resolver.py
+-rw-r--r--   0        0        0     5662 2024-05-05 21:56:28.824075 eric_devtools-0.2.0/devtools/context/context.py
+-rw-r--r--   0        0        0       82 2024-05-05 21:56:29.724124 eric_devtools-0.2.0/devtools/context/interfaces/__init__.py
+-rw-r--r--   0        0        0     1528 2024-05-05 21:56:28.784072 eric_devtools-0.2.0/devtools/context/interfaces/adapter.py
+-rw-r--r--   0        0        0       45 2024-05-05 21:55:01.167155 eric_devtools-0.2.0/devtools/context/typedef.py
+-rw-r--r--   0        0        0      732 2024-05-07 17:59:43.498042 eric_devtools-0.2.0/devtools/database/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 15:45:14.839455 eric_devtools-0.2.0/devtools/database/config.py
+-rw-r--r--   0        0        0        0 2024-05-09 15:45:15.609492 eric_devtools-0.2.0/devtools/database/drivers.py
+-rw-r--r--   0        0        0      821 2024-05-07 17:51:49.783408 eric_devtools-0.2.0/devtools/database/entity.py
+-rw-r--r--   0        0        0       50 2024-05-07 17:59:42.617992 eric_devtools-0.2.0/devtools/database/metadata.py
+-rw-r--r--   0        0        0     3759 2024-05-09 15:45:14.249427 eric_devtools-0.2.0/devtools/database/utils.py
+-rw-r--r--   0        0        0      790 2024-05-10 17:46:17.799231 eric_devtools-0.2.0/devtools/env_vars/__init__.py
+-rw-r--r--   0        0        0      790 2024-05-10 17:46:17.809232 eric_devtools-0.2.0/devtools/env_vars/config/__init__.py
+-rw-r--r--   0        0        0     1549 2024-05-05 22:35:03.201010 eric_devtools-0.2.0/devtools/env_vars/config/_helpers.py
+-rw-r--r--   0        0        0     8439 2024-05-10 17:46:17.809232 eric_devtools-0.2.0/devtools/env_vars/config/config.py
+-rw-r--r--   0        0        0     2177 2024-05-05 22:41:40.644798 eric_devtools-0.2.0/devtools/env_vars/config/enums.py
+-rw-r--r--   0        0        0     4822 2024-05-05 22:43:21.784740 eric_devtools-0.2.0/devtools/env_vars/config/envconfig.py
+-rw-r--r--   0        0        0     1414 2024-05-05 22:35:02.090967 eric_devtools-0.2.0/devtools/env_vars/config/exceptions.py
+-rw-r--r--   0        0        0      926 2024-05-05 22:33:39.403271 eric_devtools-0.2.0/devtools/env_vars/config/interface.py
+-rw-r--r--   0        0        0     7142 2024-05-05 22:35:14.920526 eric_devtools-0.2.0/devtools/env_vars/config/utils.py
+-rw-r--r--   0        0        0     1297 2024-04-21 22:43:00.915927 eric_devtools-0.2.0/devtools/exc.py
+-rw-r--r--   0        0        0      185 2024-05-07 17:32:51.140666 eric_devtools-0.2.0/devtools/filetree/__init__.py
+-rw-r--r--   0        0        0     1734 2024-05-07 17:32:51.140666 eric_devtools-0.2.0/devtools/filetree/filetree.py
+-rw-r--r--   0        0        0      351 2024-05-07 17:32:50.210634 eric_devtools-0.2.0/devtools/filetree/helpers.py
+-rw-r--r--   0        0        0     3137 2024-05-07 17:32:51.150666 eric_devtools-0.2.0/devtools/filetree/interface.py
+-rw-r--r--   0        0        0     2837 2024-05-07 17:32:51.150666 eric_devtools-0.2.0/devtools/filetree/typedef.py
+-rw-r--r--   0        0        0     2775 2024-05-07 17:32:51.140666 eric_devtools-0.2.0/devtools/filetree/virtual.py
+-rw-r--r--   0        0        0      293 2024-05-10 17:46:17.859234 eric_devtools-0.2.0/devtools/lazyfields/__init__.py
+-rw-r--r--   0        0        0    10006 2024-05-05 21:56:28.864077 eric_devtools-0.2.0/devtools/lazyfields/_lazyfields.py
+-rw-r--r--   0        0        0       99 2024-05-07 17:32:51.140666 eric_devtools-0.2.0/devtools/models/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-21 22:43:07.396305 eric_devtools-0.2.0/devtools/models/model.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:04:58.756863 eric_devtools-0.2.0/devtools/models/v1/__init__.py
+-rw-r--r--   0        0        0     1807 2024-05-07 17:32:50.240635 eric_devtools-0.2.0/devtools/models/v1/model.py
+-rw-r--r--   0        0        0        0 2024-04-28 12:32:58.725984 eric_devtools-0.2.0/devtools/query/__init__.py
+-rw-r--r--   0        0        0      113 2024-04-28 12:58:49.526347 eric_devtools-0.2.0/devtools/query/_helpers.py
+-rw-r--r--   0        0        0     2998 2024-05-07 17:51:49.683402 eric_devtools-0.2.0/devtools/query/attribute.py
+-rw-r--r--   0        0        0     3417 2024-05-05 22:07:05.103477 eric_devtools-0.2.0/devtools/query/comp.py
+-rw-r--r--   0        0        0      303 2024-05-05 22:07:05.013469 eric_devtools-0.2.0/devtools/query/exc.py
+-rw-r--r--   0        0        0     1538 2024-05-05 22:07:05.943546 eric_devtools-0.2.0/devtools/query/group.py
+-rw-r--r--   0        0        0     1739 2024-05-05 22:07:05.943546 eric_devtools-0.2.0/devtools/query/interface.py
+-rw-r--r--   0        0        0      266 2024-05-05 22:07:05.023470 eric_devtools-0.2.0/devtools/query/null.py
+-rw-r--r--   0        0        0     1324 2024-05-05 22:07:05.933545 eric_devtools-0.2.0/devtools/query/order_by.py
+-rw-r--r--   0        0        0     1223 2024-05-05 22:07:05.933545 eric_devtools-0.2.0/devtools/query/paginate.py
+-rw-r--r--   0        0        0      186 2024-05-05 22:07:05.023470 eric_devtools-0.2.0/devtools/query/typedef.py
+-rw-r--r--   0        0        0      887 2024-05-05 22:07:05.053472 eric_devtools-0.2.0/devtools/query/utils.py
+-rw-r--r--   0        0        0     2242 2024-05-05 22:07:05.933545 eric_devtools-0.2.0/devtools/query/where.py
+-rw-r--r--   0        0        0        0 2024-04-21 22:42:47.548292 eric_devtools-0.2.0/devtools/tests/__init__.py
+-rw-r--r--   0        0        0      186 2024-05-07 17:32:50.220634 eric_devtools-0.2.0/devtools/url/__init__.py
+-rw-r--r--   0        0        0     7229 2024-05-07 17:32:50.340639 eric_devtools-0.2.0/devtools/url/core.py
+-rw-r--r--   0        0        0      423 2024-05-07 17:32:50.240635 eric_devtools-0.2.0/devtools/url/encode.py
+-rw-r--r--   0        0        0     1640 2024-05-07 17:32:50.240635 eric_devtools-0.2.0/devtools/url/fragment.py
+-rw-r--r--   0        0        0     5036 2024-05-07 17:32:50.320638 eric_devtools-0.2.0/devtools/url/netloc.py
+-rw-r--r--   0        0        0     4839 2024-05-07 17:32:50.320638 eric_devtools-0.2.0/devtools/url/path.py
+-rw-r--r--   0        0        0     4028 2024-05-07 17:32:50.300637 eric_devtools-0.2.0/devtools/url/query.py
+-rw-r--r--   0        0        0     1121 2024-05-07 17:32:51.120666 eric_devtools-0.2.0/devtools/url/utils.py
+-rw-r--r--   0        0        0      504 2024-05-09 15:45:16.969556 eric_devtools-0.2.0/devtools/utils/__init__.py
+-rw-r--r--   0        0        0      156 2024-05-05 21:56:28.734070 eric_devtools-0.2.0/devtools/utils/exc.py
+-rw-r--r--   0        0        0     7823 2024-05-05 21:56:29.684121 eric_devtools-0.2.0/devtools/utils/finder.py
+-rw-r--r--   0        0        0     1359 2024-05-09 15:45:16.389529 eric_devtools-0.2.0/devtools/utils/helpers.py
+-rw-r--r--   0        0        0      174 2024-05-05 21:56:28.754071 eric_devtools-0.2.0/devtools/utils/json.py
+-rw-r--r--   0        0        0     2610 2024-05-05 21:56:28.804073 eric_devtools-0.2.0/devtools/utils/lazy.py
+-rw-r--r--   0        0        0     1700 2024-05-05 21:56:29.694122 eric_devtools-0.2.0/devtools/utils/strings.py
+-rw-r--r--   0        0        0      134 2024-05-05 21:56:28.754071 eric_devtools-0.2.0/devtools/utils/timezone.py
+-rw-r--r--   0        0        0     1211 2024-05-13 18:40:15.100670 eric_devtools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 eric_devtools-0.2.0/PKG-INFO
```

### Comparing `eric_devtools-0.1.0/devtools/adapters/database/aiomysql.py` & `eric_devtools-0.2.0/devtools/adapters/database/aiomysql.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/adapters/database/asyncmy.py` & `eric_devtools-0.2.0/devtools/adapters/database/asyncmy.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/adapters/database/asyncpg.py` & `eric_devtools-0.2.0/devtools/adapters/database/asyncpg.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/adapters/database/config.py` & `eric_devtools-0.2.0/devtools/adapters/database/config.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/__init__.py` & `eric_devtools-0.2.0/devtools/attrs/__init__.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/camel.py` & `eric_devtools-0.2.0/devtools/attrs/camel.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/converters/json.py` & `eric_devtools-0.2.0/devtools/attrs/converters/json.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/converters/utils.py` & `eric_devtools-0.2.0/devtools/attrs/converters/utils.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/field.py` & `eric_devtools-0.2.0/devtools/attrs/field.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/helpers.py` & `eric_devtools-0.2.0/devtools/attrs/helpers.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/main.py` & `eric_devtools-0.2.0/devtools/attrs/main.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/methods.py` & `eric_devtools-0.2.0/devtools/attrs/methods.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/resolver.py` & `eric_devtools-0.2.0/devtools/attrs/resolver.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/schema.py` & `eric_devtools-0.2.0/devtools/attrs/schema.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/shortcuts.py` & `eric_devtools-0.2.0/devtools/attrs/shortcuts.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/utils/factory.py` & `eric_devtools-0.2.0/devtools/attrs/utils/factory.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/utils/functions.py` & `eric_devtools-0.2.0/devtools/attrs/utils/functions.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/attrs/utils/typedef.py` & `eric_devtools-0.2.0/devtools/attrs/utils/typedef.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/config/__init__.py` & `eric_devtools-0.2.0/devtools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/config/adapter/attrs.py` & `eric_devtools-0.2.0/devtools/config/adapter/attrs.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/config/adapter/dataclass.py` & `eric_devtools-0.2.0/devtools/config/adapter/dataclass.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/config/adapter/dattrs.py` & `eric_devtools-0.2.0/devtools/config/adapter/dattrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from devtools.attrs.field import Field
 from devtools.attrs.utils.typedef import MISSING as NOTHING
 from devtools.config import MISSING
 from devtools.config.adapter.interface import FieldResolverStrategy
 
 
 @define
-class GyverAttrsResolverStrategy(FieldResolverStrategy[Field]):
+class DevtoolsAttrsResolverStrategy(FieldResolverStrategy[Field]):
     field: Field
 
     def cast(self) -> type:
         return self.field.declared_type
 
     def names(self) -> Sequence[str]:
         return self.field.name, self.field.alias
```

### Comparing `eric_devtools-0.1.0/devtools/config/adapter/factory.py` & `eric_devtools-0.2.0/devtools/config/adapter/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from devtools.env_vars.config.interface import ConfigLike
 from devtools.env_vars.config.utils import (LiteralType, boolean_cast,
                                             literal_cast)
 from devtools.utils import finder, json, panic
 from devtools.utils.strings import make_lex_separator
 
 from .dataclass import DataclassResolverStrategy
-from .dattrs import GyverAttrsResolverStrategy
+from .dattrs import DevtoolsAttrsResolverStrategy
 from .interface import FieldResolverStrategy
 from .mark import is_config
 from .pydantic import PydanticResolverStrategy
 
 _DEFAULT_CONFIG = Config()
 
 T = TypeVar("T")
@@ -88,15 +88,15 @@
 
         Returns:
             type[FieldResolverStrategy]: The strategy class for resolving fields.
         """
         klass = config_class.origin or config_class.type_
         base_model_cls: list[type] = [BaseModel, v1.BaseModel]
         if hasattr(klass, "__devtools_attrs__"):
-            return GyverAttrsResolverStrategy
+            return DevtoolsAttrsResolverStrategy
         elif is_dataclass(klass):
             return DataclassResolverStrategy
         elif issubclass(klass, tuple(base_model_cls)):
             return PydanticResolverStrategy
         elif hasattr(klass, "__attrs_attrs__"):
             from .attrs import AttrsResolverStrategy
```

### Comparing `eric_devtools-0.1.0/devtools/config/adapter/helpers.py` & `eric_devtools-0.2.0/devtools/config/adapter/helpers.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/config/adapter/interface.py` & `eric_devtools-0.2.0/devtools/config/adapter/interface.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/config/adapter/mark.py` & `eric_devtools-0.2.0/devtools/config/adapter/mark.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/config/adapter/pydantic.py` & `eric_devtools-0.2.0/devtools/config/adapter/pydantic.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/context/atomic_/bound.py` & `eric_devtools-0.2.0/devtools/context/atomic_/bound.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/context/atomic_/core.py` & `eric_devtools-0.2.0/devtools/context/atomic_/core.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/context/atomic_/resolver.py` & `eric_devtools-0.2.0/devtools/context/atomic_/resolver.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/context/context.py` & `eric_devtools-0.2.0/devtools/context/context.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/context/interfaces/adapter.py` & `eric_devtools-0.2.0/devtools/context/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/database/__init__.py` & `eric_devtools-0.2.0/devtools/database/__init__.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/database/entity.py` & `eric_devtools-0.2.0/devtools/database/entity.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/database/utils.py` & `eric_devtools-0.2.0/devtools/database/utils.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/env_vars/__init__.py` & `eric_devtools-0.2.0/devtools/env_vars/__init__.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/env_vars/config/__init__.py` & `eric_devtools-0.2.0/devtools/env_vars/config/__init__.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/env_vars/config/_helpers.py` & `eric_devtools-0.2.0/devtools/env_vars/config/_helpers.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/env_vars/config/config.py` & `eric_devtools-0.2.0/devtools/env_vars/config/config.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/env_vars/config/enums.py` & `eric_devtools-0.2.0/devtools/env_vars/config/enums.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/env_vars/config/envconfig.py` & `eric_devtools-0.2.0/devtools/env_vars/config/envconfig.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/env_vars/config/exceptions.py` & `eric_devtools-0.2.0/devtools/env_vars/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/env_vars/config/interface.py` & `eric_devtools-0.2.0/devtools/env_vars/config/interface.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/env_vars/config/utils.py` & `eric_devtools-0.2.0/devtools/env_vars/config/utils.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/exc.py` & `eric_devtools-0.2.0/devtools/exc.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/filetree/filetree.py` & `eric_devtools-0.2.0/devtools/filetree/filetree.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/filetree/interface.py` & `eric_devtools-0.2.0/devtools/filetree/interface.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/filetree/typedef.py` & `eric_devtools-0.2.0/devtools/filetree/typedef.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/filetree/virtual.py` & `eric_devtools-0.2.0/devtools/filetree/virtual.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/lazyfields/_lazyfields.py` & `eric_devtools-0.2.0/devtools/lazyfields/_lazyfields.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/models/model.py` & `eric_devtools-0.2.0/devtools/models/model.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/models/v1/model.py` & `eric_devtools-0.2.0/devtools/models/v1/model.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/query/attribute.py` & `eric_devtools-0.2.0/devtools/query/attribute.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/query/comp.py` & `eric_devtools-0.2.0/devtools/query/comp.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/query/group.py` & `eric_devtools-0.2.0/devtools/query/group.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/query/interface.py` & `eric_devtools-0.2.0/devtools/query/interface.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/query/order_by.py` & `eric_devtools-0.2.0/devtools/query/order_by.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/query/paginate.py` & `eric_devtools-0.2.0/devtools/query/paginate.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/query/utils.py` & `eric_devtools-0.2.0/devtools/query/utils.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/query/where.py` & `eric_devtools-0.2.0/devtools/query/where.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/url/core.py` & `eric_devtools-0.2.0/devtools/url/core.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/url/fragment.py` & `eric_devtools-0.2.0/devtools/url/fragment.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/url/netloc.py` & `eric_devtools-0.2.0/devtools/url/netloc.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/url/path.py` & `eric_devtools-0.2.0/devtools/url/path.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/url/query.py` & `eric_devtools-0.2.0/devtools/url/query.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/url/utils.py` & `eric_devtools-0.2.0/devtools/url/utils.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/utils/finder.py` & `eric_devtools-0.2.0/devtools/utils/finder.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/utils/helpers.py` & `eric_devtools-0.2.0/devtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/utils/lazy.py` & `eric_devtools-0.2.0/devtools/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/devtools/utils/strings.py` & `eric_devtools-0.2.0/devtools/utils/strings.py`

 * *Files identical despite different names*

### Comparing `eric_devtools-0.1.0/pyproject.toml` & `eric_devtools-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eric-devtools"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Eric Batista <klose.eric31@gmail.com>"]
 readme = "README.md"
 packages = [{include = "devtools"}]
 
 
 [tool.poetry.dependencies]
```

### Comparing `eric_devtools-0.1.0/PKG-INFO` & `eric_devtools-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eric-devtools
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Eric Batista
 Author-email: klose.eric31@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

