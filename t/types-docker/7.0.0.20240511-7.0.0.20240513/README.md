# Comparing `tmp/types-docker-7.0.0.20240511.tar.gz` & `tmp/types-docker-7.0.0.20240513.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-docker-7.0.0.20240511.tar", last modified: Sat May 11 02:18:14 2024, max compression
+gzip compressed data, was "types-docker-7.0.0.20240513.tar", last modified: Mon May 13 02:23:39 2024, max compression
```

## Comparing `types-docker-7.0.0.20240511.tar` & `types-docker-7.0.0.20240513.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.462194 types-docker-7.0.0.20240511/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-11 02:18:13.000000 types-docker-7.0.0.20240511/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 02:18:13.000000 types-docker-7.0.0.20240511/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-11 02:18:14.462194 types-docker-7.0.0.20240511/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.454193 types-docker-7.0.0.20240511/docker-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-11 02:18:13.000000 types-docker-7.0.0.20240511/docker-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.454193 types-docker-7.0.0.20240511/docker-stubs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/container.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/exec_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/image.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/network.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/secret.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/api/volume.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/constants.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.454193 types-docker-7.0.0.20240511/docker-stubs/context/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/context/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/context/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/context/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/context/context.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.454193 types-docker-7.0.0.20240511/docker-stubs/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/credentials/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/credentials/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/credentials/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/credentials/store.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/credentials/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/errors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.458193 types-docker-7.0.0.20240511/docker-stubs/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/configs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/images.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/secrets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/models/volumes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:13.000000 types-docker-7.0.0.20240511/docker-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/tls.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.458193 types-docker-7.0.0.20240511/docker-stubs/transport/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/transport/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/transport/basehttpadapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/transport/npipeconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/transport/npipesocket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/transport/sshconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/transport/unixconn.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.458193 types-docker-7.0.0.20240511/docker-stubs/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/healthcheck.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/types/swarm.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.458193 types-docker-7.0.0.20240511/docker-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/fnmatch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/json_stream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/ports.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/socket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/utils/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-11 02:17:34.000000 types-docker-7.0.0.20240511/docker-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 02:18:14.462194 types-docker-7.0.0.20240511/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-11 02:18:13.000000 types-docker-7.0.0.20240511/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:14.462194 types-docker-7.0.0.20240511/types_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-11 02:18:14.000000 types-docker-7.0.0.20240511/types_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-11 02:18:14.000000 types-docker-7.0.0.20240511/types_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:18:14.000000 types-docker-7.0.0.20240511/types_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-11 02:18:14.000000 types-docker-7.0.0.20240511/types_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 02:18:14.000000 types-docker-7.0.0.20240511/types_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.522142 types-docker-7.0.0.20240513/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-13 02:23:38.000000 types-docker-7.0.0.20240513/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 02:23:38.000000 types-docker-7.0.0.20240513/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-13 02:23:39.522142 types-docker-7.0.0.20240513/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.514142 types-docker-7.0.0.20240513/docker-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 02:23:38.000000 types-docker-7.0.0.20240513/docker-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.514142 types-docker-7.0.0.20240513/docker-stubs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/container.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/exec_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/network.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/secret.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/api/volume.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/constants.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.518142 types-docker-7.0.0.20240513/docker-stubs/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/context/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/context/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/context/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/context/context.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.518142 types-docker-7.0.0.20240513/docker-stubs/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/credentials/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/credentials/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/credentials/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/credentials/store.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/credentials/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/errors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.518142 types-docker-7.0.0.20240513/docker-stubs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/configs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/secrets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/models/volumes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:38.000000 types-docker-7.0.0.20240513/docker-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/tls.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.518142 types-docker-7.0.0.20240513/docker-stubs/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/transport/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/transport/basehttpadapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/transport/npipeconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/transport/npipesocket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/transport/sshconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/transport/unixconn.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.522142 types-docker-7.0.0.20240513/docker-stubs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/healthcheck.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/types/swarm.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.522142 types-docker-7.0.0.20240513/docker-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/fnmatch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/json_stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/ports.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/socket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/utils/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 02:23:18.000000 types-docker-7.0.0.20240513/docker-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 02:23:39.522142 types-docker-7.0.0.20240513/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-13 02:23:38.000000 types-docker-7.0.0.20240513/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:39.522142 types-docker-7.0.0.20240513/types_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-13 02:23:39.000000 types-docker-7.0.0.20240513/types_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-13 02:23:39.000000 types-docker-7.0.0.20240513/types_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 02:23:39.000000 types-docker-7.0.0.20240513/types_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 02:23:39.000000 types-docker-7.0.0.20240513/types_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 02:23:39.000000 types-docker-7.0.0.20240513/types_docker.egg-info/top_level.txt
```

### Comparing `types-docker-7.0.0.20240511/CHANGELOG.md` & `types-docker-7.0.0.20240513/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+## 7.0.0.20240513 (2024-05-13)
+
+Add many types to docker.api.container (#11911)
+
+Add types to all "container" parameters in docker.api.container (#11908)
+
+Add remaining parameter types to docker.api.container logs (#11907)
+
+Add return type to Docker Container.logs (#11888)
+
+Add return type for Docker container start (#11905)
+
+Fix "tail" parameter type for Docker container logs (#11906)
+
+Allow Image type for docker container run image parameter (#11900)
+
 ## 7.0.0.20240511 (2024-05-11)
 
 Add some types to Docker ContainerCollection parameters (#11857)
 
 ## 7.0.0.20240507 (2024-05-07)
 
 Add return type to Docker Container.stop (#11869)
```

### Comparing `types-docker-7.0.0.20240511/PKG-INFO` & `types-docker-7.0.0.20240513/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240511
+Version: 7.0.0.20240513
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+This package was generated from typeshed commit `0382803c4c228229295ae601dc431e452980fbd2` and was tested
 with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240511/docker-stubs/api/build.pyi` & `types-docker-7.0.0.20240513/docker-stubs/api/build.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/api/client.pyi` & `types-docker-7.0.0.20240513/docker-stubs/api/client.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/api/container.pyi` & `types-docker-7.0.0.20240513/docker-stubs/types/containers.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,164 @@
 from _typeshed import Incomplete
 
-class ContainerApiMixin:
-    def attach(
-        self, container, stdout: bool = True, stderr: bool = True, stream: bool = False, logs: bool = False, demux: bool = False
-    ): ...
-    def attach_socket(self, container, params: Incomplete | None = None, ws: bool = False): ...
-    def commit(
-        self,
-        container,
-        repository: str | None = None,
-        tag: str | None = None,
-        message: Incomplete | None = None,
-        author: Incomplete | None = None,
-        pause: bool = True,
-        changes: Incomplete | None = None,
-        conf: Incomplete | None = None,
-    ): ...
-    def containers(
+from .base import DictType
+
+class LogConfigTypesEnum:
+    JSON: Incomplete
+    SYSLOG: Incomplete
+    JOURNALD: Incomplete
+    GELF: Incomplete
+    FLUENTD: Incomplete
+    NONE: Incomplete
+
+class LogConfig(DictType):
+    types: type[LogConfigTypesEnum]
+    def __init__(self, **kwargs) -> None: ...
+    @property
+    def type(self): ...
+    @type.setter
+    def type(self, value) -> None: ...
+    @property
+    def config(self): ...
+    def set_config_value(self, key, value) -> None: ...
+    def unset_config(self, key) -> None: ...
+
+class Ulimit(DictType):
+    def __init__(self, **kwargs) -> None: ...
+    @property
+    def name(self): ...
+    @name.setter
+    def name(self, value) -> None: ...
+    @property
+    def soft(self): ...
+    @soft.setter
+    def soft(self, value) -> None: ...
+    @property
+    def hard(self): ...
+    @hard.setter
+    def hard(self, value) -> None: ...
+
+class DeviceRequest(DictType):
+    def __init__(self, **kwargs) -> None: ...
+    @property
+    def driver(self): ...
+    @driver.setter
+    def driver(self, value) -> None: ...
+    @property
+    def count(self): ...
+    @count.setter
+    def count(self, value) -> None: ...
+    @property
+    def device_ids(self): ...
+    @device_ids.setter
+    def device_ids(self, value) -> None: ...
+    @property
+    def capabilities(self): ...
+    @capabilities.setter
+    def capabilities(self, value) -> None: ...
+    @property
+    def options(self): ...
+    @options.setter
+    def options(self, value) -> None: ...
+
+class HostConfig(dict[str, Incomplete]):
+    def __init__(
         self,
-        quiet: bool = False,
-        all: bool = False,
-        trunc: bool = False,
-        latest: bool = False,
-        since: Incomplete | None = None,
-        before: Incomplete | None = None,
-        limit: int = -1,
-        size: bool = False,
-        filters: Incomplete | None = None,
-    ): ...
-    def create_container(
+        version,
+        binds: Incomplete | None = None,
+        port_bindings: Incomplete | None = None,
+        lxc_conf: Incomplete | None = None,
+        publish_all_ports: bool = False,
+        links: Incomplete | None = None,
+        privileged: bool = False,
+        dns: Incomplete | None = None,
+        dns_search: Incomplete | None = None,
+        volumes_from: Incomplete | None = None,
+        network_mode: Incomplete | None = None,
+        restart_policy: Incomplete | None = None,
+        cap_add: Incomplete | None = None,
+        cap_drop: Incomplete | None = None,
+        devices: Incomplete | None = None,
+        extra_hosts: Incomplete | None = None,
+        read_only: Incomplete | None = None,
+        pid_mode: Incomplete | None = None,
+        ipc_mode: Incomplete | None = None,
+        security_opt: Incomplete | None = None,
+        ulimits: Incomplete | None = None,
+        log_config: Incomplete | None = None,
+        mem_limit: Incomplete | None = None,
+        memswap_limit: Incomplete | None = None,
+        mem_reservation: Incomplete | None = None,
+        kernel_memory: Incomplete | None = None,
+        mem_swappiness: Incomplete | None = None,
+        cgroup_parent: Incomplete | None = None,
+        group_add: Incomplete | None = None,
+        cpu_quota: Incomplete | None = None,
+        cpu_period: Incomplete | None = None,
+        blkio_weight: Incomplete | None = None,
+        blkio_weight_device: Incomplete | None = None,
+        device_read_bps: Incomplete | None = None,
+        device_write_bps: Incomplete | None = None,
+        device_read_iops: Incomplete | None = None,
+        device_write_iops: Incomplete | None = None,
+        oom_kill_disable: bool = False,
+        shm_size: Incomplete | None = None,
+        sysctls: Incomplete | None = None,
+        tmpfs: Incomplete | None = None,
+        oom_score_adj: Incomplete | None = None,
+        dns_opt: Incomplete | None = None,
+        cpu_shares: Incomplete | None = None,
+        cpuset_cpus: Incomplete | None = None,
+        userns_mode: Incomplete | None = None,
+        uts_mode: Incomplete | None = None,
+        pids_limit: Incomplete | None = None,
+        isolation: Incomplete | None = None,
+        auto_remove: bool = False,
+        storage_opt: Incomplete | None = None,
+        init: Incomplete | None = None,
+        init_path: Incomplete | None = None,
+        volume_driver: Incomplete | None = None,
+        cpu_count: Incomplete | None = None,
+        cpu_percent: Incomplete | None = None,
+        nano_cpus: Incomplete | None = None,
+        cpuset_mems: Incomplete | None = None,
+        runtime: Incomplete | None = None,
+        mounts: Incomplete | None = None,
+        cpu_rt_period: Incomplete | None = None,
+        cpu_rt_runtime: Incomplete | None = None,
+        device_cgroup_rules: Incomplete | None = None,
+        device_requests: Incomplete | None = None,
+        cgroupns: Incomplete | None = None,
+    ) -> None: ...
+
+def host_config_type_error(param, param_value, expected): ...
+def host_config_version_error(param, version, less_than: bool = True): ...
+def host_config_value_error(param, param_value): ...
+def host_config_incompatible_error(param, param_value, incompatible_param): ...
+
+class ContainerConfig(dict[str, Incomplete]):
+    def __init__(
         self,
+        version,
         image,
-        command: Incomplete | None = None,
+        command,
         hostname: Incomplete | None = None,
         user: Incomplete | None = None,
         detach: bool = False,
         stdin_open: bool = False,
         tty: bool = False,
         ports: Incomplete | None = None,
         environment: Incomplete | None = None,
         volumes: Incomplete | None = None,
         network_disabled: bool = False,
-        name: Incomplete | None = None,
         entrypoint: Incomplete | None = None,
         working_dir: Incomplete | None = None,
         domainname: Incomplete | None = None,
         host_config: Incomplete | None = None,
         mac_address: Incomplete | None = None,
         labels: Incomplete | None = None,
         stop_signal: Incomplete | None = None,
         networking_config: Incomplete | None = None,
         healthcheck: Incomplete | None = None,
         stop_timeout: Incomplete | None = None,
         runtime: Incomplete | None = None,
-        use_config_proxy: bool = True,
-        platform: Incomplete | None = None,
-    ): ...
-    def create_container_config(self, *args, **kwargs): ...
-    def create_container_from_config(self, config, name: Incomplete | None = None, platform: Incomplete | None = None): ...
-    def create_host_config(self, *args, **kwargs): ...
-    def create_networking_config(self, *args, **kwargs): ...
-    def create_endpoint_config(self, *args, **kwargs): ...
-    def diff(self, container): ...
-    def export(self, container, chunk_size=2097152): ...
-    def get_archive(self, container, path, chunk_size=2097152, encode_stream: bool = False): ...
-    def inspect_container(self, container): ...
-    def kill(self, container, signal: Incomplete | None = None) -> None: ...
-    def logs(
-        self,
-        container,
-        stdout: bool = True,
-        stderr: bool = True,
-        stream: bool = False,
-        timestamps: bool = False,
-        tail: str = "all",
-        since: Incomplete | None = None,
-        follow: Incomplete | None = None,
-        until: Incomplete | None = None,
-    ): ...
-    def pause(self, container) -> None: ...
-    def port(self, container, private_port): ...
-    def put_archive(self, container, path, data): ...
-    def prune_containers(self, filters: Incomplete | None = None): ...
-    def remove_container(self, container, v: bool = False, link: bool = False, force: bool = False) -> None: ...
-    def rename(self, container, name) -> None: ...
-    def resize(self, container, height, width) -> None: ...
-    def restart(self, container, timeout: int = 10) -> None: ...
-    def start(self, container, *args, **kwargs) -> None: ...
-    def stats(self, container, decode: Incomplete | None = None, stream: bool = True, one_shot: Incomplete | None = None): ...
-    def stop(self, container, timeout: Incomplete | None = None) -> None: ...
-    def top(self, container, ps_args: Incomplete | None = None): ...
-    def unpause(self, container) -> None: ...
-    def update_container(
-        self,
-        container,
-        blkio_weight: Incomplete | None = None,
-        cpu_period: Incomplete | None = None,
-        cpu_quota: Incomplete | None = None,
-        cpu_shares: Incomplete | None = None,
-        cpuset_cpus: Incomplete | None = None,
-        cpuset_mems: Incomplete | None = None,
-        mem_limit: Incomplete | None = None,
-        mem_reservation: Incomplete | None = None,
-        memswap_limit: Incomplete | None = None,
-        kernel_memory: Incomplete | None = None,
-        restart_policy: Incomplete | None = None,
-    ): ...
-    def wait(self, container, timeout: Incomplete | None = None, condition: Incomplete | None = None): ...
+    ) -> None: ...
```

### Comparing `types-docker-7.0.0.20240511/docker-stubs/api/daemon.pyi` & `types-docker-7.0.0.20240513/docker-stubs/api/daemon.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/api/exec_api.pyi` & `types-docker-7.0.0.20240513/docker-stubs/api/exec_api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/api/image.pyi` & `types-docker-7.0.0.20240513/docker-stubs/api/image.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/api/network.pyi` & `types-docker-7.0.0.20240513/docker-stubs/api/network.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/api/plugin.pyi` & `types-docker-7.0.0.20240513/docker-stubs/api/plugin.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/api/service.pyi` & `types-docker-7.0.0.20240513/docker-stubs/api/service.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/api/swarm.pyi` & `types-docker-7.0.0.20240513/docker-stubs/api/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/api/volume.pyi` & `types-docker-7.0.0.20240513/docker-stubs/api/volume.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/auth.pyi` & `types-docker-7.0.0.20240513/docker-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/client.pyi` & `types-docker-7.0.0.20240513/docker-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/constants.pyi` & `types-docker-7.0.0.20240513/docker-stubs/constants.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/context/api.pyi` & `types-docker-7.0.0.20240513/docker-stubs/context/api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/context/context.pyi` & `types-docker-7.0.0.20240513/docker-stubs/context/context.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/errors.pyi` & `types-docker-7.0.0.20240513/docker-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/models/containers.pyi` & `types-docker-7.0.0.20240513/docker-stubs/models/containers.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from _typeshed import Incomplete
 from typing import NamedTuple
 
+from docker.types.daemon import CancellableStream
+
+from .images import Image
 from .resource import Collection, Model
 
 class Container(Model):
     @property
     def name(self): ...
     @property
     def image(self): ...
@@ -35,34 +38,34 @@
         environment: Incomplete | None = None,
         workdir: Incomplete | None = None,
         demux: bool = False,
     ): ...
     def export(self, chunk_size=2097152): ...
     def get_archive(self, path, chunk_size=2097152, encode_stream: bool = False): ...
     def kill(self, signal: Incomplete | None = None): ...
-    def logs(self, **kwargs): ...
+    def logs(self, **kwargs) -> CancellableStream | bytes: ...
     def pause(self): ...
     def put_archive(self, path, data): ...
     def remove(self, **kwargs) -> None: ...
     def rename(self, name): ...
     def resize(self, height, width): ...
     def restart(self, **kwargs): ...
-    def start(self, **kwargs): ...
+    def start(self, **kwargs) -> None: ...
     def stats(self, **kwargs): ...
     def stop(self, **kwargs) -> None: ...
     def top(self, **kwargs): ...
     def unpause(self): ...
     def update(self, **kwargs): ...
     def wait(self, **kwargs): ...
 
 class ContainerCollection(Collection[Container]):
     model: type[Container]
     def run(
         self,
-        image: str,
+        image: str | Image,
         command: str | list[str] | None = None,
         stdout: bool = True,
         stderr: bool = False,
         remove: bool = False,
         **kwargs,
     ): ...
     def create(self, image: str, command: str | list[str] | None = None, **kwargs): ...  # type:ignore[override]
```

### Comparing `types-docker-7.0.0.20240511/docker-stubs/models/images.pyi` & `types-docker-7.0.0.20240513/docker-stubs/models/images.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/models/networks.pyi` & `types-docker-7.0.0.20240513/docker-stubs/models/networks.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/models/plugins.pyi` & `types-docker-7.0.0.20240513/docker-stubs/models/plugins.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/models/resource.pyi` & `types-docker-7.0.0.20240513/docker-stubs/models/resource.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/models/services.pyi` & `types-docker-7.0.0.20240513/docker-stubs/models/services.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/models/swarm.pyi` & `types-docker-7.0.0.20240513/docker-stubs/models/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/models/volumes.pyi` & `types-docker-7.0.0.20240513/docker-stubs/models/volumes.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/transport/npipeconn.pyi` & `types-docker-7.0.0.20240513/docker-stubs/transport/npipeconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/transport/npipesocket.pyi` & `types-docker-7.0.0.20240513/docker-stubs/transport/npipesocket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/transport/sshconn.pyi` & `types-docker-7.0.0.20240513/docker-stubs/transport/sshconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/transport/unixconn.pyi` & `types-docker-7.0.0.20240513/docker-stubs/transport/unixconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/types/__init__.pyi` & `types-docker-7.0.0.20240513/docker-stubs/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/types/containers.pyi` & `types-docker-7.0.0.20240513/docker-stubs/types/services.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,164 +1,170 @@
 from _typeshed import Incomplete
 
-from .base import DictType
-
-class LogConfigTypesEnum:
-    JSON: Incomplete
-    SYSLOG: Incomplete
-    JOURNALD: Incomplete
-    GELF: Incomplete
-    FLUENTD: Incomplete
-    NONE: Incomplete
-
-class LogConfig(DictType):
-    types: type[LogConfigTypesEnum]
-    def __init__(self, **kwargs) -> None: ...
-    @property
-    def type(self): ...
-    @type.setter
-    def type(self, value) -> None: ...
+class TaskTemplate(dict[str, Incomplete]):
+    def __init__(
+        self,
+        container_spec,
+        resources: Incomplete | None = None,
+        restart_policy: Incomplete | None = None,
+        placement: Incomplete | None = None,
+        log_driver: Incomplete | None = None,
+        networks: Incomplete | None = None,
+        force_update: Incomplete | None = None,
+    ) -> None: ...
     @property
-    def config(self): ...
-    def set_config_value(self, key, value) -> None: ...
-    def unset_config(self, key) -> None: ...
-
-class Ulimit(DictType):
-    def __init__(self, **kwargs) -> None: ...
+    def container_spec(self): ...
     @property
-    def name(self): ...
-    @name.setter
-    def name(self, value) -> None: ...
+    def resources(self): ...
     @property
-    def soft(self): ...
-    @soft.setter
-    def soft(self, value) -> None: ...
+    def restart_policy(self): ...
     @property
-    def hard(self): ...
-    @hard.setter
-    def hard(self, value) -> None: ...
+    def placement(self): ...
 
-class DeviceRequest(DictType):
-    def __init__(self, **kwargs) -> None: ...
-    @property
-    def driver(self): ...
-    @driver.setter
-    def driver(self, value) -> None: ...
-    @property
-    def count(self): ...
-    @count.setter
-    def count(self, value) -> None: ...
-    @property
-    def device_ids(self): ...
-    @device_ids.setter
-    def device_ids(self, value) -> None: ...
-    @property
-    def capabilities(self): ...
-    @capabilities.setter
-    def capabilities(self, value) -> None: ...
-    @property
-    def options(self): ...
-    @options.setter
-    def options(self, value) -> None: ...
-
-class HostConfig(dict[str, Incomplete]):
-    def __init__(
-        self,
-        version,
-        binds: Incomplete | None = None,
-        port_bindings: Incomplete | None = None,
-        lxc_conf: Incomplete | None = None,
-        publish_all_ports: bool = False,
-        links: Incomplete | None = None,
-        privileged: bool = False,
-        dns: Incomplete | None = None,
-        dns_search: Incomplete | None = None,
-        volumes_from: Incomplete | None = None,
-        network_mode: Incomplete | None = None,
-        restart_policy: Incomplete | None = None,
+class ContainerSpec(dict[str, Incomplete]):
+    def __init__(
+        self,
+        image,
+        command: Incomplete | None = None,
+        args: Incomplete | None = None,
+        hostname: Incomplete | None = None,
+        env: Incomplete | None = None,
+        workdir: Incomplete | None = None,
+        user: Incomplete | None = None,
+        labels: Incomplete | None = None,
+        mounts: Incomplete | None = None,
+        stop_grace_period: Incomplete | None = None,
+        secrets: Incomplete | None = None,
+        tty: Incomplete | None = None,
+        groups: Incomplete | None = None,
+        open_stdin: Incomplete | None = None,
+        read_only: Incomplete | None = None,
+        stop_signal: Incomplete | None = None,
+        healthcheck: Incomplete | None = None,
+        hosts: Incomplete | None = None,
+        dns_config: Incomplete | None = None,
+        configs: Incomplete | None = None,
+        privileges: Incomplete | None = None,
+        isolation: Incomplete | None = None,
+        init: Incomplete | None = None,
         cap_add: Incomplete | None = None,
         cap_drop: Incomplete | None = None,
-        devices: Incomplete | None = None,
-        extra_hosts: Incomplete | None = None,
-        read_only: Incomplete | None = None,
-        pid_mode: Incomplete | None = None,
-        ipc_mode: Incomplete | None = None,
-        security_opt: Incomplete | None = None,
-        ulimits: Incomplete | None = None,
-        log_config: Incomplete | None = None,
+        sysctls: Incomplete | None = None,
+    ) -> None: ...
+
+class Mount(dict[str, Incomplete]):
+    def __init__(
+        self,
+        target,
+        source,
+        type: str = "volume",
+        read_only: bool = False,
+        consistency: Incomplete | None = None,
+        propagation: Incomplete | None = None,
+        no_copy: bool = False,
+        labels: Incomplete | None = None,
+        driver_config: Incomplete | None = None,
+        tmpfs_size: Incomplete | None = None,
+        tmpfs_mode: Incomplete | None = None,
+    ) -> None: ...
+    @classmethod
+    def parse_mount_string(cls, string): ...
+
+class Resources(dict[str, Incomplete]):
+    def __init__(
+        self,
+        cpu_limit: Incomplete | None = None,
         mem_limit: Incomplete | None = None,
-        memswap_limit: Incomplete | None = None,
+        cpu_reservation: Incomplete | None = None,
         mem_reservation: Incomplete | None = None,
-        kernel_memory: Incomplete | None = None,
-        mem_swappiness: Incomplete | None = None,
-        cgroup_parent: Incomplete | None = None,
-        group_add: Incomplete | None = None,
-        cpu_quota: Incomplete | None = None,
-        cpu_period: Incomplete | None = None,
-        blkio_weight: Incomplete | None = None,
-        blkio_weight_device: Incomplete | None = None,
-        device_read_bps: Incomplete | None = None,
-        device_write_bps: Incomplete | None = None,
-        device_read_iops: Incomplete | None = None,
-        device_write_iops: Incomplete | None = None,
-        oom_kill_disable: bool = False,
-        shm_size: Incomplete | None = None,
-        sysctls: Incomplete | None = None,
-        tmpfs: Incomplete | None = None,
-        oom_score_adj: Incomplete | None = None,
-        dns_opt: Incomplete | None = None,
-        cpu_shares: Incomplete | None = None,
-        cpuset_cpus: Incomplete | None = None,
-        userns_mode: Incomplete | None = None,
-        uts_mode: Incomplete | None = None,
-        pids_limit: Incomplete | None = None,
-        isolation: Incomplete | None = None,
-        auto_remove: bool = False,
-        storage_opt: Incomplete | None = None,
-        init: Incomplete | None = None,
-        init_path: Incomplete | None = None,
-        volume_driver: Incomplete | None = None,
-        cpu_count: Incomplete | None = None,
-        cpu_percent: Incomplete | None = None,
-        nano_cpus: Incomplete | None = None,
-        cpuset_mems: Incomplete | None = None,
-        runtime: Incomplete | None = None,
-        mounts: Incomplete | None = None,
-        cpu_rt_period: Incomplete | None = None,
-        cpu_rt_runtime: Incomplete | None = None,
-        device_cgroup_rules: Incomplete | None = None,
-        device_requests: Incomplete | None = None,
-        cgroupns: Incomplete | None = None,
+        generic_resources: Incomplete | None = None,
+    ) -> None: ...
+
+class UpdateConfig(dict[str, Incomplete]):
+    def __init__(
+        self,
+        parallelism: int = 0,
+        delay: Incomplete | None = None,
+        failure_action: str = "continue",
+        monitor: Incomplete | None = None,
+        max_failure_ratio: Incomplete | None = None,
+        order: Incomplete | None = None,
     ) -> None: ...
 
-def host_config_type_error(param, param_value, expected): ...
-def host_config_version_error(param, version, less_than: bool = True): ...
-def host_config_value_error(param, param_value): ...
-def host_config_incompatible_error(param, param_value, incompatible_param): ...
+class RollbackConfig(UpdateConfig): ...
+
+class RestartConditionTypesEnum:
+    NONE: Incomplete
+    ON_FAILURE: Incomplete
+    ANY: Incomplete
+
+class RestartPolicy(dict[str, Incomplete]):
+    condition_types: type[RestartConditionTypesEnum]
+    def __init__(self, condition="none", delay: int = 0, max_attempts: int = 0, window: int = 0) -> None: ...
 
-class ContainerConfig(dict[str, Incomplete]):
+class DriverConfig(dict[str, Incomplete]):
+    def __init__(self, name, options: Incomplete | None = None) -> None: ...
+
+class EndpointSpec(dict[str, Incomplete]):
+    def __init__(self, mode: Incomplete | None = None, ports: Incomplete | None = None) -> None: ...
+
+def convert_service_ports(ports): ...
+
+class ServiceMode(dict[str, Incomplete]):
+    mode: Incomplete
+    def __init__(self, mode, replicas: Incomplete | None = None, concurrency: Incomplete | None = None) -> None: ...
+    @property
+    def replicas(self): ...
+
+class SecretReference(dict[str, Incomplete]):
     def __init__(
         self,
-        version,
-        image,
-        command,
-        hostname: Incomplete | None = None,
-        user: Incomplete | None = None,
-        detach: bool = False,
-        stdin_open: bool = False,
-        tty: bool = False,
-        ports: Incomplete | None = None,
-        environment: Incomplete | None = None,
-        volumes: Incomplete | None = None,
-        network_disabled: bool = False,
-        entrypoint: Incomplete | None = None,
-        working_dir: Incomplete | None = None,
-        domainname: Incomplete | None = None,
-        host_config: Incomplete | None = None,
-        mac_address: Incomplete | None = None,
-        labels: Incomplete | None = None,
-        stop_signal: Incomplete | None = None,
-        networking_config: Incomplete | None = None,
-        healthcheck: Incomplete | None = None,
-        stop_timeout: Incomplete | None = None,
-        runtime: Incomplete | None = None,
+        secret_id,
+        secret_name,
+        filename: Incomplete | None = None,
+        uid: Incomplete | None = None,
+        gid: Incomplete | None = None,
+        mode: int = 292,
+    ) -> None: ...
+
+class ConfigReference(dict[str, Incomplete]):
+    def __init__(
+        self,
+        config_id,
+        config_name,
+        filename: Incomplete | None = None,
+        uid: Incomplete | None = None,
+        gid: Incomplete | None = None,
+        mode: int = 292,
+    ) -> None: ...
+
+class Placement(dict[str, Incomplete]):
+    def __init__(
+        self,
+        constraints: Incomplete | None = None,
+        preferences: Incomplete | None = None,
+        platforms: Incomplete | None = None,
+        maxreplicas: Incomplete | None = None,
     ) -> None: ...
+
+class PlacementPreference(dict[str, Incomplete]):
+    def __init__(self, strategy, descriptor) -> None: ...
+
+class DNSConfig(dict[str, Incomplete]):
+    def __init__(
+        self, nameservers: Incomplete | None = None, search: Incomplete | None = None, options: Incomplete | None = None
+    ) -> None: ...
+
+class Privileges(dict[str, Incomplete]):
+    def __init__(
+        self,
+        credentialspec_file: Incomplete | None = None,
+        credentialspec_registry: Incomplete | None = None,
+        selinux_disable: Incomplete | None = None,
+        selinux_user: Incomplete | None = None,
+        selinux_role: Incomplete | None = None,
+        selinux_type: Incomplete | None = None,
+        selinux_level: Incomplete | None = None,
+    ) -> None: ...
+
+class NetworkAttachmentConfig(dict[str, Incomplete]):
+    def __init__(self, target, aliases: Incomplete | None = None, options: Incomplete | None = None) -> None: ...
```

### Comparing `types-docker-7.0.0.20240511/docker-stubs/types/healthcheck.pyi` & `types-docker-7.0.0.20240513/docker-stubs/types/healthcheck.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/types/networks.pyi` & `types-docker-7.0.0.20240513/docker-stubs/types/networks.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/types/swarm.pyi` & `types-docker-7.0.0.20240513/docker-stubs/types/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/utils/__init__.pyi` & `types-docker-7.0.0.20240513/docker-stubs/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/utils/build.pyi` & `types-docker-7.0.0.20240513/docker-stubs/utils/build.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/utils/proxy.pyi` & `types-docker-7.0.0.20240513/docker-stubs/utils/proxy.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/utils/socket.pyi` & `types-docker-7.0.0.20240513/docker-stubs/utils/socket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/docker-stubs/utils/utils.pyi` & `types-docker-7.0.0.20240513/docker-stubs/utils/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240511/setup.py` & `types-docker-7.0.0.20240513/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+This package was generated from typeshed commit `0382803c4c228229295ae601dc431e452980fbd2` and was tested
 with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="7.0.0.20240511",
+      version="7.0.0.20240513",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md",
```

### Comparing `types-docker-7.0.0.20240511/types_docker.egg-info/PKG-INFO` & `types-docker-7.0.0.20240513/types_docker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240511
+Version: 7.0.0.20240513
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+This package was generated from typeshed commit `0382803c4c228229295ae601dc431e452980fbd2` and was tested
 with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240511/types_docker.egg-info/SOURCES.txt` & `types-docker-7.0.0.20240513/types_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

