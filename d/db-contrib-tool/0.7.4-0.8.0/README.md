# Comparing `tmp/db_contrib_tool-0.7.4.tar.gz` & `tmp/db_contrib_tool-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_contrib_tool-0.7.4.tar", max compression
+gzip compressed data, was "db_contrib_tool-0.8.0.tar", max compression
```

## Comparing `db_contrib_tool-0.7.4.tar` & `db_contrib_tool-0.8.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     6286 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/README.md
--rw-r--r--   0        0        0     2184 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/pyproject.toml
--rw-r--r--   0        0        0       13 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/__init__.py
--rw-r--r--   0        0        0      989 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/cli.py
--rw-r--r--   0        0        0        0 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/__init__.py
--rw-r--r--   0        0        0     7143 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/download_client.py
--rw-r--r--   0        0        0     1733 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/file_service.py
--rw-r--r--   0        0        0     2636 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/git_client.py
--rw-r--r--   0        0        0      305 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/io_client.py
--rw-r--r--   0        0        0      984 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/platform_details.py
--rw-r--r--   0        0        0     2737 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/resmoke_proxy.py
--rw-r--r--   0        0        0    10275 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/config/setup_repro_env_config.yml
--rw-r--r--   0        0        0     5999 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/config.py
--rw-r--r--   0        0        0      445 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/README.md
--rw-r--r--   0        0        0     8844 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/__init__.py
--rw-r--r--   0        0        0     4639 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/cli.py
--rw-r--r--   0        0        0      110 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
--rw-r--r--   0        0        0      418 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
--rw-r--r--   0        0        0       52 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
--rw-r--r--   0        0        0        0 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/services/__init__.py
--rw-r--r--   0        0        0     9277 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/services/evergreen_service.py
--rw-r--r--   0        0        0     2404 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/services/git_service.py
--rw-r--r--   0        0        0     2029 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/services/platform_service.py
--rw-r--r--   0        0        0       13 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_mongot_repro_env/__init__.py
--rw-r--r--   0        0        0     3990 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_mongot_repro_env/cli.py
--rw-r--r--   0        0        0    13806 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/README.md
--rw-r--r--   0        0        0       13 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/__init__.py
--rw-r--r--   0        0        0    18510 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
--rw-r--r--   0        0        0     9894 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/cli.py
--rw-r--r--   0        0        0    10159 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/download_service.py
--rw-r--r--   0        0        0     4796 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
--rw-r--r--   0        0        0     5586 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/release_models.py
--rw-r--r--   0        0        0     4167 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/request_models.py
--rw-r--r--   0        0        0    10710 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
--rw-r--r--   0        0        0      615 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/README.md
--rw-r--r--   0        0        0        0 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/__init__.py
--rw-r--r--   0        0        0     4190 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/cli.py
--rw-r--r--   0        0        0     4798 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
--rw-r--r--   0        0        0    24229 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/mongosymb.py
--rw-r--r--   0        0        0     2269 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/usage_analytics.py
--rw-r--r--   0        0        0      235 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/utils/__init__.py
--rw-r--r--   0        0        0     1855 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/utils/build_system_options.py
--rw-r--r--   0        0        0     2108 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/utils/evergreen_conn.py
--rw-r--r--   0        0        0     1085 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/utils/filesystem.py
--rw-r--r--   0        0        0    10608 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/utils/oauth.py
--rw-r--r--   0        0        0     7972 1970-01-01 00:00:00.000000 db_contrib_tool-0.7.4/setup.py
--rw-r--r--   0        0        0     7542 1970-01-01 00:00:00.000000 db_contrib_tool-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     6286 2024-05-13 07:31:04.077683 db_contrib_tool-0.8.0/README.md
+-rw-r--r--   0        0        0     2184 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       13 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/__init__.py
+-rw-r--r--   0        0        0      989 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/cli.py
+-rw-r--r--   0        0        0        0 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/clients/__init__.py
+-rw-r--r--   0        0        0     7143 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/clients/download_client.py
+-rw-r--r--   0        0        0     1733 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/clients/file_service.py
+-rw-r--r--   0        0        0     2636 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/clients/git_client.py
+-rw-r--r--   0        0        0      305 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/clients/io_client.py
+-rw-r--r--   0        0        0      984 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/clients/platform_details.py
+-rw-r--r--   0        0        0     2916 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/clients/resmoke_proxy.py
+-rw-r--r--   0        0        0    10275 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/config/setup_repro_env_config.yml
+-rw-r--r--   0        0        0     5999 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/config.py
+-rw-r--r--   0        0        0      445 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/evg_aware_bisect/README.md
+-rw-r--r--   0        0        0     8844 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/evg_aware_bisect/__init__.py
+-rw-r--r--   0        0        0     4639 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/evg_aware_bisect/cli.py
+-rw-r--r--   0        0        0      110 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
+-rw-r--r--   0        0        0      418 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
+-rw-r--r--   0        0        0       52 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
+-rw-r--r--   0        0        0        0 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/services/__init__.py
+-rw-r--r--   0        0        0     9277 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/services/evergreen_service.py
+-rw-r--r--   0        0        0     2404 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/services/git_service.py
+-rw-r--r--   0        0        0     2029 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/services/platform_service.py
+-rw-r--r--   0        0        0       13 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/setup_mongot_repro_env/__init__.py
+-rw-r--r--   0        0        0     3990 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/setup_mongot_repro_env/cli.py
+-rw-r--r--   0        0        0    15034 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/README.md
+-rw-r--r--   0        0        0       13 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/__init__.py
+-rw-r--r--   0        0        0    18488 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
+-rw-r--r--   0        0        0    10648 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/cli.py
+-rw-r--r--   0        0        0    10159 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/download_service.py
+-rw-r--r--   0        0        0     4796 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
+-rw-r--r--   0        0        0     5586 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/release_models.py
+-rw-r--r--   0        0        0     4110 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/request_models.py
+-rw-r--r--   0        0        0    11556 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
+-rw-r--r--   0        0        0      615 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/symbolizer/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/symbolizer/__init__.py
+-rw-r--r--   0        0        0     4190 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/symbolizer/cli.py
+-rw-r--r--   0        0        0     4798 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
+-rw-r--r--   0        0        0    24229 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/symbolizer/mongosymb.py
+-rw-r--r--   0        0        0     2269 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/usage_analytics.py
+-rw-r--r--   0        0        0      235 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/utils/__init__.py
+-rw-r--r--   0        0        0     1855 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/utils/build_system_options.py
+-rw-r--r--   0        0        0     2108 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/utils/evergreen_conn.py
+-rw-r--r--   0        0        0     1085 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/utils/filesystem.py
+-rw-r--r--   0        0        0    10608 2024-05-13 07:31:04.081683 db_contrib_tool-0.8.0/src/db_contrib_tool/utils/oauth.py
+-rw-r--r--   0        0        0     7972 1970-01-01 00:00:00.000000 db_contrib_tool-0.8.0/setup.py
+-rw-r--r--   0        0        0     7542 1970-01-01 00:00:00.000000 db_contrib_tool-0.8.0/PKG-INFO
```

### Comparing `db_contrib_tool-0.7.4/README.md` & `db_contrib_tool-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/pyproject.toml` & `db_contrib_tool-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "db-contrib-tool"
-version = "0.7.4"
+version = "0.8.0"
 description = "The `db-contrib-tool` - MongoDB's tool for contributors."
 authors = ["DAG team <dev-prod-dag@mongodb.com>"]
 readme = "README.md"
 repository = "https://github.com/10gen/db-contrib-tool"
 include = [
     "src/db_contrib_tool/bisect/*.sh",
     "src/db_contrib_tool/config/*.yml",
```

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/cli.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/clients/download_client.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/clients/download_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/clients/file_service.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/clients/file_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/clients/git_client.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/clients/platform_details.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/clients/platform_details.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/clients/resmoke_proxy.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/clients/resmoke_proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,18 @@
                     " this error, please reach out in #server-testing slack channel."
                 )
                 raise
             with open(file_name, "r") as file:
                 config_contents = file.read()
             os.remove(file_name)
             self.multiversion_constants = MultiversionConfig(**yaml.safe_load(config_contents))
+            LOGGER.debug(
+                "Received multiversion constants from resmoke",
+                multiversion_constants=self.multiversion_constants.dict(),
+            )
 
     def get_multiversion_constants(self) -> MultiversionConfig:
         """
         Get the multiversion constants from resmoke.
 
         :return: Multiversion config.
         """
```

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/config/setup_repro_env_config.yml` & `db_contrib_tool-0.8.0/src/db_contrib_tool/config/setup_repro_env_config.yml`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/config.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/config.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/__init__.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/evg_aware_bisect/__init__.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/cli.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/evg_aware_bisect/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/services/evergreen_service.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/services/evergreen_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/services/git_service.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/services/git_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/services/platform_service.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/services/platform_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_mongot_repro_env/cli.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/setup_mongot_repro_env/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/README.md` & `db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,19 +22,31 @@
 ```bash
 db-contrib-tool setup-repro-env --help
 ```
 
 ### Cheat Sheet of Common Use Cases
 
 ```bash
-# Download the latest last-lts & last-continuous binaries. Need to run from the root of mongodb/mongo repo.
+# Download the latest last-lts & last-continuous binaries.
+# Need to run from the root of mongodb/mongo or 10gen/mongo repo.
 db-contrib-tool setup-repro-env
 
-# Download a specific version
-db-contrib-tool setup-repro-env [5.2, githash123abc, evgversion123abc, evgtask123abc]
+# Download specific versions
+db-contrib-tool setup-repro-env \
+  5.2 \
+  githash123abc \
+  evg_version_123abc \
+  evg_task_123abc
+
+# Download specific versions and apply specific binary link suffixes.
+# To interpret `last-lts`, `last-continuous` aliases need to run from the root of mongodb/mongo or 10gen/mongo repo.
+db-contrib-tool setup-repro-env \
+  githash123abc=6.0 \
+  evg_version_123abc=last-lts \
+  evg_task_123abc=last-continuous
 
 # Set up a full repro env
 db-contrib-tool setup-repro-env -ds -dv -da \
   mongodb_mongo_master_enterprise_rhel_80_64_bit_dynamic_required_jsCore_9adc8c129a972b7e098bd8c50c9b222f98dd2edb_22_02_16_03_30_27
 
 db-contrib-tool setup-repro-env -ds -dv -da \
   --variant enterprise-rhel-80-64-bit-dynamic-required \
@@ -193,20 +205,44 @@
 Evergreen version and the same `! Shared Library Enterprise RHEL 8.0` Evergreen buildvariant the task was running on.
 
 ```bash
 db-contrib-tool setup-repro-env \
   mongodb_mongo_master_enterprise_rhel_80_64_bit_dynamic_required_jsCore_9adc8c129a972b7e098bd8c50c9b222f98dd2edb_22_02_16_03_30_27
 ```
 
+To specify binary suffix that will be appended to binary links it can be passed together with the version as a key=value
+pair, e.g. `<version>=<bin_suffix>`
+
+```bash
+db-contrib-tool setup-repro-env \
+  mongodb_mongo_master_nightly_b4d0ac2e6631481803423081c92687a422ec7b86=8.1
+```
+
+`last-lts` and `last-continuous` version aliases as bin suffixes could be translated into release version numbers.
+
+The following commands should be run from the root of mongodb/mongo or 10gen/mongo repo or from the `installDir` of the
+[artifacts](#setup-artifacts-including-resmoke-python-scripts-jstests-etc).
+
+```bash
+db-contrib-tool setup-repro-env \
+  mongodb_mongo_master_nightly_b4d0ac2e6631481803423081c92687a422ec7b86=last-lts
+```
+
+```bash
+db-contrib-tool setup-repro-env \
+  mongodb_mongo_master_nightly_b4d0ac2e6631481803423081c92687a422ec7b86=last-continuous
+```
+
 #### Setting up last-LTS and last-continuous versions
 
 If `--installLastLTS` and/or `--installLastContinuous` flags are passed, last-LTS and last-continuous versions will be
-automatically calculated and downloaded, but this requires mongodb/mongo repo or downloaded artifacts on your machine.
+automatically calculated and downloaded, but this requires mongodb/mongo or 10gen/mongo repo or downloaded artifacts on
+your machine.
 
-The following command should be run from the root of mongodb/mongo repo or from the `installDir` of the
+The following command should be run from the root of mongodb/mongo or 10gen/mongo repo or from the `installDir` of the
 [artifacts](#setup-artifacts-including-resmoke-python-scripts-jstests-etc).
 
 ```bash
 db-contrib-tool setup-repro-env \
   --installLastLTS \
   --installLastContinuous \
   master
```

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                 if err.response.status_code == 404 and fallback_to_master:
                     LOGGER.warning(
                         "Unable to find requested mongo version, falling back to default branch",
                         requested_version=request.identifier,
                         default_branch=BRANCH_FALLBACK,
                     )
                     return self.find_artifacts(
-                        RequestTarget.previous_release(BRANCH_FALLBACK),
+                        request.branch_fallback(),
                         requested_variant,
                         target,
                         ignore_failed_push,
                         False,
                     )
                 raise
```

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/cli.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
 @click.command(cls=CommandWithUsageTracking)
 @click.pass_context
 @click.argument(
     "versions",
     nargs=-1,
     required=False,
+    metavar="[VERSION=BIN_SUFFIX]...",
 )
 @click.option(
     "-i",
     "--installDir",
     "install_dir",
     type=click.Path(),
     default=DEFAULT_INSTALL_DIR,
@@ -246,20 +247,35 @@
     Set up MongoDB repro environment.
 
     Downloads and installs particular MongoDB versions into install directory
     and symlinks the binaries to another directory. Each symlink name will
     include the binary release version, e.g. mongod-6.1. This script supports
     community and enterprise builds.
 
-    Accepts binary versions, `master`, full git commit hashes, evergreen
-    version ids, evergreen task ids.
+    Accepts the following values:
 
-    Binary version examples: <major.minor>, 4.2, 4.4, 5.0 etc.
+        - binary versions - examples: <major.minor>, 4.2, 4.4, 5.0 etc.
 
-    If no version is specified the last LTS and the last continuous versions
+        - `last-lts` and `last-continuous` - will be translated into
+        corresponding versions, e.g. 8.0, 8.1
+
+        - `master` and release branch names
+
+        - full git commit hashes
+
+        - evergreen version ids
+
+        - evergreen task ids
+
+    Optionally with the version accepts binary suffix, e.g. <version>=<bin_suffix>:
+
+        - aliases `last-lts`, `last-continuous` will be translated into
+        corresponding versions, e.g. 8.0, 8.1.
+
+    If no versions are specified the last LTS and the last continuous versions
     will be installed.
     """
     if ctx.get_parameter_source("install_dir") == ParameterSource.DEFAULT and download_artifacts:
         install_dir = DEFAULT_WITH_ARTIFACTS_INSTALL_DIR
     if ctx.get_parameter_source("link_dir") == ParameterSource.DEFAULT and download_artifacts:
         link_dir = DEFAULT_WITH_ARTIFACTS_LINK_DIR
 
@@ -319,17 +335,27 @@
     Process input parameters to get the list of version requests.
 
     :param install_last_continuous: Whether the last continuous version requested.
     :param install_last_lts: Whether the last lts version requested.
     :param input_versions: Requested versions.
     :return: The list of version requests.
     """
-    versions = list(input_versions)
+    versions = []
+    for version in input_versions:
+        if version in [LTS_RELEASE_ALIAS, CONTINUOUS_RELEASE_ALIAS]:
+            versions.append(f"{version}={version}")
+        else:
+            versions.append(version)
+
     if install_last_lts:
-        versions.append(LTS_RELEASE_ALIAS)
+        versions.append(f"{LTS_RELEASE_ALIAS}={LTS_RELEASE_ALIAS}")
+
     if install_last_continuous:
-        versions.append(CONTINUOUS_RELEASE_ALIAS)
+        versions.append(f"{CONTINUOUS_RELEASE_ALIAS}={CONTINUOUS_RELEASE_ALIAS}")
+
     if len(versions) == 0:
-        versions = [LTS_RELEASE_ALIAS, CONTINUOUS_RELEASE_ALIAS]
-    versions = list(set(versions))
+        versions = [
+            f"{LTS_RELEASE_ALIAS}={LTS_RELEASE_ALIAS}",
+            f"{CONTINUOUS_RELEASE_ALIAS}={CONTINUOUS_RELEASE_ALIAS}",
+        ]
 
-    return versions
+    return list(set(versions))
```

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/download_service.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/download_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/release_discovery_service.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/release_discovery_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/release_models.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/release_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/request_models.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/request_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,30 +64,32 @@
 
 class RequestTarget(NamedTuple):
     """
     Version of mongo binaries that was requested.
 
     * request_type: Type of the identifier.
     * identifier: Identifier used to find request.
+    * bin_suffix: Multiversion bin suffix.
     """
 
     request_type: RequestType
     identifier: str
+    bin_suffix: Optional[str] = None
 
-    @classmethod
-    def previous_release(cls, identifier: str) -> RequestTarget:
+    def branch_fallback(self) -> RequestTarget:
         """
-        Build a target for either the previous LTS or Continuous release.
+        Make a target from the current target for the default fallback branch.
 
-        :param identifier: Identifier of release to download.
         :return: Request target to download given release.
         """
-        if identifier == BRANCH_FALLBACK:
-            return cls(request_type=RequestType.GIT_BRANCH, identifier=identifier)
-        return cls(request_type=RequestType.MONGO_RELEASE_VERSION, identifier=identifier)
+        return RequestTarget(
+            request_type=RequestType.GIT_BRANCH,
+            identifier=BRANCH_FALLBACK,
+            bin_suffix=self.bin_suffix,
+        )
 
     def __str__(self) -> str:
         """Display item as a string."""
         return f"{self.request_type}({self.identifier})"
 
 
 class DownloadRequest(NamedTuple):
```

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/setup_repro_env.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/setup_repro_env/setup_repro_env.py`

 * *Files 12% similar despite different names*

```diff
@@ -126,72 +126,94 @@
     def interpret_discovery_request(self, request: str) -> RequestTarget:
         """
         Translate the request from the user into an item we can understand.
 
         :param request: Request from user.
         :return: Targeted request to download.
         """
-        if request in [LTS_RELEASE_ALIAS, CONTINUOUS_RELEASE_ALIAS]:
-            return self._get_release_versions(request)
+        if "=" in request:
+            version, bin_suffix = request.split("=", 1)
+        else:
+            version, bin_suffix = request, None
+
+        request_type = RequestType.GIT_COMMIT
+        identifier = version
+
+        if version in [LTS_RELEASE_ALIAS, CONTINUOUS_RELEASE_ALIAS]:
+            request_type = RequestType.MONGO_RELEASE_VERSION
+            identifier = self._get_release_version(version)
+        elif version in KNOWN_BRANCHES or BRANCH_RE.match(version):
+            request_type = RequestType.GIT_BRANCH
+        elif RELEASE_VERSION_RE.match(version):
+            request_type = RequestType.MONGO_RELEASE_VERSION
+        elif PATCH_VERSION_RE.match(version):
+            request_type = RequestType.MONGO_PATCH_VERSION
+        elif self.evg_service.query_task_existence(version):
+            request_type = RequestType.EVG_TASK
+        elif self.evg_service.query_version_existence(version):
+            request_type = RequestType.EVG_VERSION
+
+        if bin_suffix in [LTS_RELEASE_ALIAS, CONTINUOUS_RELEASE_ALIAS]:
+            bin_suffix = self._get_release_version(bin_suffix)
+
+        request_target = RequestTarget(
+            request_type=request_type,
+            identifier=identifier,
+            bin_suffix=bin_suffix,
+        )
 
-        if request in KNOWN_BRANCHES or BRANCH_RE.match(request):
-            return RequestTarget(RequestType.GIT_BRANCH, request)
+        LOGGER.debug("Interpreted setup request", original=request, interpreted=request_target)
 
-        if RELEASE_VERSION_RE.match(request):
-            return RequestTarget(RequestType.MONGO_RELEASE_VERSION, request)
-
-        if PATCH_VERSION_RE.match(request):
-            return RequestTarget(RequestType.MONGO_PATCH_VERSION, request)
-
-        if self.evg_service.query_task_existence(request):
-            return RequestTarget(RequestType.EVG_TASK, request)
-
-        if self.evg_service.query_version_existence(request):
-            return RequestTarget(RequestType.EVG_VERSION, request)
-
-        return RequestTarget(RequestType.GIT_COMMIT, request)
+        return request_target
 
     def interpret_discovery_requests(self, request_list: List[str]) -> List[RequestTarget]:
         """
         Translate all the requests from the user into a request for discovering the download information.
 
         :param request_list: Requests from user.
         :return: List of targeted request to download.
         """
         requests = [self.interpret_discovery_request(request) for request in request_list]
 
         return requests
 
-    def _get_release_versions(self, version_alias: str) -> RequestTarget:
+    def _get_release_version(self, version_alias: str) -> str:
         """
-        Create a multiversion version that should be included.
+        Translate version alias to a release version.
 
-        :return: multiversion version to include.
+        :param version_alias: Alias like `last-lts`, `last-continuous`.
+        :return: Release version.
         """
         multiversionconstants = self.resmoke_proxy.get_multiversion_constants()
 
         releases = {
             LTS_RELEASE_ALIAS: multiversionconstants.last_lts_fcv,
             CONTINUOUS_RELEASE_ALIAS: multiversionconstants.last_continuous_fcv,
         }
-        LOGGER.debug("LTS and continuous release inclusions", releases=releases)
-        return RequestTarget.previous_release(releases[version_alias])
+
+        release_version = releases[version_alias]
+        LOGGER.debug("Got release version from alias", alias=version_alias, release=release_version)
+
+        return release_version
 
     @staticmethod
-    def _get_bin_suffix(version: str, evg_project_id: str) -> str:
+    def _get_bin_suffix(request: RequestTarget, evg_project_id: str) -> str:
         """
         Get the multiversion bin suffix from the evergreen project ID.
 
-        :param version: Version from the cmdline.
+        :param request: Targeted request to download.
         :param evg_project_id: Evergreen project ID.
         :return: Bin suffix.
         """
-        if re.match(r"(\d+\.\d+)", version):
+        if request.bin_suffix is not None:
+            return request.bin_suffix
+
+        if re.match(r"(\d+\.\d+)", request.identifier):
             # If the cmdline version is already a semvar, just use that.
-            return version
+            return request.identifier
 
         project_version_search = re.search(r"(\d+\.\d+$)", evg_project_id)
         if project_version_search:
             # Extract version from the Evergreen project ID as fallback.
             return project_version_search.group(0)
 
         # If the version is not a semvar, we can't add a suffix.
@@ -223,24 +245,25 @@
                 evg_urls_info = self.artifact_discovery_service.find_artifacts(
                     discovery_request,
                     setup_repro_params.variant,
                     download_target,
                     setup_repro_params.ignore_failed_push,
                     setup_repro_params.fallback_to_master,
                 )
-            except (EvergreenVersionIsTooOld, MissingBuildVariantError):
+            except (EvergreenVersionIsTooOld, MissingBuildVariantError, ValueError) as err:
+                LOGGER.warning("Could not find URLs in Evergreen", error=err)
                 evg_urls_info = None
 
             LOGGER.info("Fetching fallback download URLs from Downloads json")
             release_urls_info = self.release_discovery_service.find_release_urls(
                 discovery_request, download_target
             )
 
             bin_suffix = self._get_bin_suffix(
-                discovery_request.identifier,
+                discovery_request,
                 evg_urls_info.project_identifier if evg_urls_info else "",
             )
             download_request = DownloadRequest(
                 bin_suffix, discovery_request, evg_urls_info, release_urls_info
             )
             download_request_set.add(download_request)
```

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/README.md` & `db_contrib_tool-0.8.0/src/db_contrib_tool/symbolizer/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/cli.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/symbolizer/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/mongosymb.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/symbolizer/mongosymb.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/usage_analytics.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/usage_analytics.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/utils/build_system_options.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/utils/build_system_options.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/utils/evergreen_conn.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/utils/evergreen_conn.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/utils/filesystem.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/src/db_contrib_tool/utils/oauth.py` & `db_contrib_tool-0.8.0/src/db_contrib_tool/utils/oauth.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.4/setup.py` & `db_contrib_tool-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
  'tenacity>=8.0.1,<9.0.0']
 
 entry_points = \
 {'console_scripts': ['db-contrib-tool = db_contrib_tool.cli:cli']}
 
 setup_kwargs = {
     'name': 'db-contrib-tool',
-    'version': '0.7.4',
+    'version': '0.8.0',
     'description': "The `db-contrib-tool` - MongoDB's tool for contributors.",
     'long_description': '# db-contrib-tool\n\nThe `db-contrib-tool` - MongoDB\'s tools for contributors.\n\n## Table of contents\n\n- [db-contrib-tool](#db-contrib-tool)\n  - [Table of contents](#table-of-contents)\n  - [Description](#description)\n  - [Dependencies](#dependencies)\n  - [Installation](#installation)\n  - [Usage](#usage)\n  - [Contributor\'s Guide (local development)](#contributors-guide-local-development)\n    - [Install project dependencies](#install-project-dependencies)\n    - [Run command line tool (local development)](#run-command-line-tool-local-development)\n    - [Run linters](#run-linters)\n    - [Run tests](#run-tests)\n    - [Pre-commit](#pre-commit)\n    - [Testing changes in mongo](#testing-changes-in-mongo)\n    - [Testing changes locally](#testing-changes-locally)\n    - [Versioning](#versioning)\n    - [Code Review](#code-review)\n    - [Deployment](#deployment)\n\n## Description\n\nThe command line tool with various subcommands:\n- `bisect`\n  - [README.md](src/db_contrib_tool/evg_aware_bisect/README.md)\n  - performs an evergreen-aware git-bisect to find the \'last passing version\' and \'first failing version\' of mongo\n- `setup-repro-env`\n  - [README.md](src/db_contrib_tool/setup_repro_env/README.md)\n  - downloads and installs:\n    - particular MongoDB versions\n    - debug symbols\n    - artifacts (including resmoke, python scripts etc)\n    - python venv for resmoke, python scripts etc\n- `symbolize`\n  - [README.md](src/db_contrib_tool/symbolizer/README.md)\n  - Symbolizes stacktraces from recent `mongod` and `mongos` binaries compiled in Evergreen, including patch builds, mainline builds, and release/production builds.\n  - Requires authenticating to an internal MongoDB symbol mapping service.\n\n## Dependencies\n\n- Python 3.9 or later (python3 from the [MongoDB Toolchain](https://github.com/10gen/toolchain-builder/blob/master/INSTALL.md) is highly recommended)\n\n## Installation\n\nMake sure [dependencies](#dependencies) are installed.\nUse [pipx](https://pypa.github.io/pipx/) to install db-contrib-tool that will be available globally on your machine:\n\n```bash\npython3 -m pip install pipx\npython3 -m pipx ensurepath\n```\n\nInstalling db-contrib-tool:\n\n```bash\npython3 -m pipx install db-contrib-tool\n```\n\nUpgrading db-contrib-tool:\n\n```bash\npython3 -m pipx upgrade db-contrib-tool\n```\n\nIn case of installation errors, some of them may be related to pipx and could be fixed by re-installing pipx.\n\nRemoving pipx completely (WARNING! This will delete everything that is installed and managed by pipx):\n\n```bash\npython3 -m pip uninstall pipx\nrm -rf ~/.local/pipx  # in case you\'re using the default pipx home directory\n```\n\nNow you can try to install again from scratch.\n\n## Usage\n\nPrint out help message:\n\n```bash\ndb-contrib-tool --help\n```\n\nFor more information see [description](#description) section.\n\n## Contributor\'s Guide (local development)\n\n### Install project dependencies\n\nThis project uses [poetry](https://python-poetry.org/) for dependency management.\n\n```bash\npoetry install\n```\n\n### Run command line tool (local development)\n\nSome subcommands like `bisect` and `symbolize` could be tested from the db-contrib-tool repo root:\n\n```bash\npoetry run db-contrib-tool --help\n```\n\nFor `setup-repro-env` some features can also be tested from the db-contrib-tool repo root,\nbut full features are available when running from mongo repo root.\nSee [testing changes locally](#testing-changes-locally) section.\n\n### Run linters\n\n```bash\npoetry run isort src tests\npoetry run black src tests\n```\n\n### Run tests\n\n```bash\npoetry run pytest\n```\n\n### Pre-commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time.<br>\nTo enable pre-commit on your local repository run:\n```bash\npoetry run pre-commit install\n```\n\nTo run pre-commit manually:\n```bash\npoetry run pre-commit run\n```\n\n### Testing changes in mongo\n\nThis tool is used to help run tests in the mongodb/mongo repository. On occasion, it may be\ndesirable to run a mongodb-mongo-* patch build with in-flight changes to this repository. The\nfollowing steps can be taken to accomplish that.\n\n- Create a branch with the changes you wish to test.\n- Push the branch to the origin repository: `git push -u origin <branch_name>`.\n- In the "mongo" repository, edit the [evergreen/prelude_db_contrib_tool.sh](https://github.com/10gen/mongo/blob/bbdc1347cdf2533f81b6fd05715c4ef1a092f5a6/evergreen/prelude_db_contrib_tool.sh#L12)\n  to install from the git repository instead of from pypi:\n\n  ```bash\n  pipx install "git+ssh://git@github.com/<user_name>/db-contrib-tool.git@<branch_name>" || exit 1\n  ```\n\n- Create a patch build.\n\nThe patch build should now pull down the changes from your branch instead of using the published\ndb-contrib-tool.\n\n**Note**: Since the db-contrib-tool is pulled from your branch, if you need to make additional\nchanges to the tool, you can just push to the branch and then restart the desired tasks. There is\nno need to create an additional patch build unless you also need to make updates to the mongo\nrepository.\n\n### Testing changes locally\n\nPipx installation recommendations can be found in [installation](#installation) section.\n\nThe tool can be installed via pipx from your local repo:\n\n```bash\npython3 -m pipx install /path/to/db-contrib-tool/repo/root/dir\n```\n\nIf the tool is already installed you can force install an updated version using --force flag:\n\n```bash\npython3 -m pipx install --force /path/to/db-contrib-tool/repo/root/dir\n```\n\nAfter these steps you can run in-development version of db-contrib-tool from any directory:\n\n```bash\ndb-contrib-tool --help\n```\n\n### Versioning\n\nThis project uses [semver](https://semver.org/) for versioning.\nPlease include a description what is added for each new version in `CHANGELOG.md`.\n\n### Code Review\n\nPlease open a GitHub Pull Request for code review.\nThis project uses the [Evergreen Commit Queue](https://docs.devprod.prod.corp.mongodb.com/evergreen/Project-Configuration/Commit-Queue).\nAdd a PR comment with `evergreen merge` to trigger a merge.\n\n### Deployment\n\nDeployment to pypi is done by [deploy](https://spruce.mongodb.com/commits/db-contrib-tool?taskNames=deploy)\ntask of `db-contrib-tool` project in Evergreen.\nA new version in Evergreen is created on merges to `main` branch.\n',
     'author': 'DAG team',
     'author_email': 'dev-prod-dag@mongodb.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/10gen/db-contrib-tool',
```

### Comparing `db_contrib_tool-0.7.4/PKG-INFO` & `db_contrib_tool-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-contrib-tool
-Version: 0.7.4
+Version: 0.8.0
 Summary: The `db-contrib-tool` - MongoDB's tool for contributors.
 Home-page: https://github.com/10gen/db-contrib-tool
 Author: DAG team
 Author-email: dev-prod-dag@mongodb.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

