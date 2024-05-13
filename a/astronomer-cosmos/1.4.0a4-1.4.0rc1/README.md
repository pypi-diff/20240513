# Comparing `tmp/astronomer_cosmos-1.4.0a4.tar.gz` & `tmp/astronomer_cosmos-1.4.0rc1.tar.gz`

## Comparing `astronomer_cosmos-1.4.0a4.tar` & `astronomer_cosmos-1.4.0rc1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/__init__.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/cache.py
--rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/config.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/constants.py
--rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/converter.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/exceptions.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/log.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/airflow/__init__.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/airflow/dag.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/airflow/graph.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/airflow/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/core/__init__.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/executable.py
--rw-r--r--   0        0        0    18527 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/graph.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/project.py
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/selector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/parser/__init__.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/parser/output.py
--rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/parser/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/hooks/__init__.py
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/hooks/subprocess.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/__init__.py
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/azure_container_instance.py
--rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/base.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/docker.py
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/kubernetes.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/lazy_load.py
--rw-r--r--   0        0        0    32095 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/local.py
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/virtualenv.py
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/plugin/__init__.py
--rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/plugin/static/iframeResizer.contentWindow.min.js
--rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/plugin/static/iframeResizer.min.js
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/plugin/templates/dbt_docs.html
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/plugin/templates/dbt_docs_not_set_up.html
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/__init__.py
--rwxr-xr-x   0        0        0    11351 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/base.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/athena/__init__.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/athena/access_key.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/oauth.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/service_account_keyfile_dict.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/databricks/token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_privatekey.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/spark/thrift.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/base.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/ldap.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/vertica/__init__.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/vertica/user_pass.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/LICENSE
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/README.rst
--rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/pyproject.toml
--rw-r--r--   0        0        0     7718 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/PKG-INFO
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/__init__.py
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/cache.py
+-rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/config.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/constants.py
+-rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/converter.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/exceptions.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/log.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/airflow/__init__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/airflow/dag.py
+-rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/airflow/graph.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/airflow/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/executable.py
+-rw-r--r--   0        0        0    18527 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/graph.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/project.py
+-rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/selector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/parser/__init__.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/parser/output.py
+-rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/parser/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/hooks/__init__.py
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/hooks/subprocess.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/__init__.py
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/azure_container_instance.py
+-rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/base.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/docker.py
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/kubernetes.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/lazy_load.py
+-rw-r--r--   0        0        0    32840 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/local.py
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/virtualenv.py
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/plugin/__init__.py
+-rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/plugin/static/iframeResizer.contentWindow.min.js
+-rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/plugin/static/iframeResizer.min.js
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/plugin/templates/dbt_docs.html
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/plugin/templates/dbt_docs_not_set_up.html
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/__init__.py
+-rwxr-xr-x   0        0        0    11351 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/base.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/athena/__init__.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/athena/access_key.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/oauth.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/service_account_keyfile_dict.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/databricks/token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_privatekey.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/spark/thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/base.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/ldap.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/vertica/__init__.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/vertica/user_pass.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/LICENSE
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/README.rst
+-rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/PKG-INFO
```

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/__init__.py` & `astronomer_cosmos-1.4.0rc1/cosmos/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # type: ignore # ignores "Cannot assign to a type" MyPy error
 
 """
 Astronomer Cosmos is a library for rendering dbt workflows in Airflow.
 
 Contains dags, task groups, and operators.
 """
-__version__ = "1.4.0a4"
+__version__ = "1.4.0rc1"
 
 
 from cosmos.airflow.dag import DbtDag
 from cosmos.airflow.task_group import DbtTaskGroup
 from cosmos.config import (
     ExecutionConfig,
     ProfileConfig,
```

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/cache.py` & `astronomer_cosmos-1.4.0rc1/cosmos/cache.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import shutil
 from pathlib import Path
 
+import msgpack
 from airflow.models.dag import DAG
 from airflow.utils.task_group import TaskGroup
 
 from cosmos import settings
 from cosmos.constants import DBT_MANIFEST_FILE_NAME, DBT_TARGET_DIR_NAME
 from cosmos.dbt.project import get_partial_parse_path
 
@@ -117,8 +118,25 @@
     target_partial_parse_file = get_partial_parse_path(project_path)
     tmp_target_dir = project_path / DBT_TARGET_DIR_NAME
     tmp_target_dir.mkdir(exist_ok=True)
 
     source_manifest_filepath = partial_parse_filepath.parent / DBT_MANIFEST_FILE_NAME
     target_manifest_filepath = target_partial_parse_file.parent / DBT_MANIFEST_FILE_NAME
     shutil.copy(str(partial_parse_filepath), str(target_partial_parse_file))
+
+    # Update root_path in partial parse file to point to the needed project directory. This is necessary because
+    # an issue is observed where on specific earlier versions of dbt-core like 1.5.4 and 1.6.5, the commands fail to
+    # locate project files as they are pointed to a stale directory by the root_path in the partial parse file.
+    # This issue was not observed on recent versions of dbt-core 1.5.8, 1.6.6, 1.7.0 and 1.8.0 as tested on.
+    # It is suspected that PR dbt-labs/dbt-core#8762 is likely the fix and the fix appears to be backported to later
+    # version releases of 1.5.x and 1.6.x. However, the below modification is applied to ensure that the root_path is
+    # correctly set to the needed project directory and the feature is compatible across all dbt-core versions.
+    with target_partial_parse_file.open("rb") as f:
+        data = msgpack.unpack(f)
+    for node in data["nodes"].values():
+        if node.get("root_path"):
+            node["root_path"] = str(project_path)
+    with target_partial_parse_file.open("wb") as f:
+        packed = msgpack.packb(data)
+        f.write(packed)
+
     shutil.copy(str(source_manifest_filepath), str(target_manifest_filepath))
```

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/config.py` & `astronomer_cosmos-1.4.0rc1/cosmos/config.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/constants.py` & `astronomer_cosmos-1.4.0rc1/cosmos/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from enum import Enum
 from pathlib import Path
 
 import aenum
+from packaging.version import Version
 
 DBT_PROFILE_PATH = Path(os.path.expanduser("~")).joinpath(".dbt/profiles.yml")
 DEFAULT_DBT_PROFILE_NAME = "cosmos_profile"
 DEFAULT_DBT_TARGET_NAME = "cosmos_target"
 DEFAULT_COSMOS_CACHE_DIR_NAME = "cosmos"
 DBT_LOG_PATH_ENVVAR = "DBT_LOG_PATH"
 DBT_LOG_DIR_NAME = "logs"
@@ -16,14 +17,18 @@
 DBT_MANIFEST_FILE_NAME = "manifest.json"
 DBT_LOG_FILENAME = "dbt.log"
 DBT_BINARY_NAME = "dbt"
 
 DEFAULT_OPENLINEAGE_NAMESPACE = "cosmos"
 OPENLINEAGE_PRODUCER = "https://github.com/astronomer/astronomer-cosmos/"
 
+# Cosmos will not emit datasets for the following Airflow versions, due to a breaking change that's fixed in later Airflow 2.x versions
+# https://github.com/apache/airflow/issues/39486
+PARTIALLY_SUPPORTED_AIRFLOW_VERSIONS = [Version("2.9.0"), Version("2.9.1")]
+
 
 class LoadMode(Enum):
     """
     Supported ways to load a `dbt` project into a `DbtGraph` instance.
     """
 
     AUTOMATIC = "automatic"
```

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/converter.py` & `astronomer_cosmos-1.4.0rc1/cosmos/converter.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/log.py` & `astronomer_cosmos-1.4.0rc1/cosmos/log.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/airflow/dag.py` & `astronomer_cosmos-1.4.0rc1/cosmos/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/airflow/graph.py` & `astronomer_cosmos-1.4.0rc1/cosmos/airflow/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/airflow/task_group.py` & `astronomer_cosmos-1.4.0rc1/cosmos/airflow/task_group.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/core/airflow.py` & `astronomer_cosmos-1.4.0rc1/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/core/graph/entities.py` & `astronomer_cosmos-1.4.0rc1/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/dbt/graph.py` & `astronomer_cosmos-1.4.0rc1/cosmos/dbt/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/dbt/project.py` & `astronomer_cosmos-1.4.0rc1/cosmos/dbt/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/dbt/selector.py` & `astronomer_cosmos-1.4.0rc1/cosmos/dbt/selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         "Checks if a single node should be included. Only runs once per node with caching."
         logger.debug("Inspecting if the node <%s> should be included.", node_id)
         if node_id in self.visited_nodes:
             return node_id in self.selected_nodes
 
         self.visited_nodes.add(node_id)
 
-        if node.resource_type == DbtResourceType.TEST and node.depends_on:
+        if node.resource_type == DbtResourceType.TEST and node.depends_on and len(node.depends_on) > 0:
             node.tags = getattr(self.nodes.get(node.depends_on[0]), "tags", [])
             logger.debug(
                 "The test node <%s> inherited these tags from the parent node <%s>: %s",
                 node_id,
                 node.depends_on[0],
                 node.tags,
             )
```

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/dbt/parser/output.py` & `astronomer_cosmos-1.4.0rc1/cosmos/dbt/parser/output.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/dbt/parser/project.py` & `astronomer_cosmos-1.4.0rc1/cosmos/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/hooks/subprocess.py` & `astronomer_cosmos-1.4.0rc1/cosmos/hooks/subprocess.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/operators/__init__.py` & `astronomer_cosmos-1.4.0rc1/cosmos/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/operators/azure_container_instance.py` & `astronomer_cosmos-1.4.0rc1/cosmos/operators/azure_container_instance.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/operators/base.py` & `astronomer_cosmos-1.4.0rc1/cosmos/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/operators/docker.py` & `astronomer_cosmos-1.4.0rc1/cosmos/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/operators/kubernetes.py` & `astronomer_cosmos-1.4.0rc1/cosmos/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/operators/local.py` & `astronomer_cosmos-1.4.0rc1/cosmos/operators/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from airflow.utils.context import Context
 from airflow.utils.session import NEW_SESSION, create_session, provide_session
 from attr import define
 
 from cosmos import cache
 from cosmos.constants import InvocationMode
 from cosmos.dbt.project import get_partial_parse_path
+from cosmos.exceptions import AirflowCompatibilityError
 
 try:
     from airflow.datasets import Dataset
     from openlineage.common.provider.dbt.local import DbtLocalArtifactProcessor
 except ModuleNotFoundError:
     is_openlineage_available = False
     DbtLocalArtifactProcessor = None
@@ -403,15 +404,29 @@
         """
         uris = []
         for completed in self.openlineage_events_completes:
             for output in getattr(completed, source):
                 dataset_uri = output.namespace + "/" + output.name
                 uris.append(dataset_uri)
         logger.debug("URIs to be converted to Dataset: %s", uris)
-        return [Dataset(uri) for uri in uris]
+
+        datasets = []
+        try:
+            datasets = [Dataset(uri) for uri in uris]
+        except ValueError as e:
+            raise AirflowCompatibilityError(
+                """
+                Apache Airflow 2.9.0 & 2.9.1 introduced a breaking change in Dataset URIs, to be fixed in newer versions:
+                https://github.com/apache/airflow/issues/39486
+
+                If you want to use Cosmos with one of these Airflow versions, you will have to disable emission of Datasets:
+                By setting ``emit_datasets=False`` in ``RenderConfig``. For more information, see https://astronomer.github.io/astronomer-cosmos/configuration/render-config.html.
+                """
+            )
+        return datasets
 
     def register_dataset(self, new_inlets: list[Dataset], new_outlets: list[Dataset]) -> None:
         """
         Register a list of datasets as outlets of the current task.
         Until Airflow 2.7, there was not a better interface to associate outlets to a task during execution.
         """
         with create_session() as session:
```

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/operators/virtualenv.py` & `astronomer_cosmos-1.4.0rc1/cosmos/operators/virtualenv.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/plugin/__init__.py` & `astronomer_cosmos-1.4.0rc1/cosmos/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/plugin/static/iframeResizer.contentWindow.min.js` & `astronomer_cosmos-1.4.0rc1/cosmos/plugin/static/iframeResizer.contentWindow.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/plugin/static/iframeResizer.min.js` & `astronomer_cosmos-1.4.0rc1/cosmos/plugin/static/iframeResizer.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/__init__.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/base.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/athena/access_key.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/athena/access_key.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/oauth.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/oauth.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/service_account_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/service_account_keyfile_dict.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/service_account_keyfile_dict.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/databricks/token.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/databricks/token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/exasol/user_pass.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/exasol/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/postgres/user_pass.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/postgres/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/redshift/user_pass.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/redshift/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/__init__.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_pass.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_privatekey.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_privatekey.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/spark/thrift.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/spark/thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/base.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/certificate.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/certificate.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/jwt.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/jwt.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/ldap.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/ldap.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/cosmos/profiles/vertica/user_pass.py` & `astronomer_cosmos-1.4.0rc1/cosmos/profiles/vertica/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/.gitignore` & `astronomer_cosmos-1.4.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/LICENSE` & `astronomer_cosmos-1.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/README.rst` & `astronomer_cosmos-1.4.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a4/pyproject.toml` & `astronomer_cosmos-1.4.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 ]
 dependencies = [
     "aenum",
     "attrs",
     "apache-airflow>=2.3.0",
     "importlib-metadata; python_version < '3.8'",
     "Jinja2>=3.0.0",
+    "msgpack",
     "pydantic>=1.10.0",
     "typing-extensions; python_version < '3.8'",
     "virtualenv",
 ]
 
 [project.optional-dependencies]
 dbt-all = [
@@ -113,14 +114,15 @@
 ######################################
 # TESTING
 ######################################
 
 [tool.hatch.envs.tests]
 dependencies = [
     "astronomer-cosmos[tests]",
+    "apache-airflow-providers-postgres",
     "apache-airflow-providers-cncf-kubernetes>=5.1.1",
     "apache-airflow-providers-docker>=3.5.0",
     "apache-airflow-providers-microsoft-azure",
     "types-PyYAML",
     "types-attrs",
     "types-requests",
     "types-python-dateutil",
@@ -131,49 +133,51 @@
 
 [[tool.hatch.envs.tests.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11"]
 airflow = ["2.3", "2.4", "2.5", "2.6", "2.7", "2.8", "2.9"]
 
 [tool.hatch.envs.tests.overrides]
 matrix.airflow.dependencies = [
-    { value = "typing_extensions<4.6", if = ["2.6"] }
+    { value = "typing_extensions<4.6", if = ["2.6"] },
 ]
 
 [tool.hatch.envs.tests.scripts]
 freeze = "pip freeze"
-type-check = "mypy cosmos"
 test = 'sh scripts/test/unit.sh'
 test-cov = 'sh scripts/test/unit-cov.sh'
-test-integration-setup = 'sh scripts/test/integration-setup.sh'
 test-integration = 'sh scripts/test/integration.sh'
+test-integration-dbt-1-5-4 = 'sh scripts/test/integration-dbt-1-5-4.sh'
 test-integration-expensive = 'sh scripts/test/integration-expensive.sh'
-test-integration-sqlite-setup = 'sh scripts/test/integration-sqlite-setup.sh'
+test-integration-setup = 'sh scripts/test/integration-setup.sh'
 test-integration-sqlite = 'sh scripts/test/integration-sqlite.sh'
-test-performance-setup = 'sh scripts/test/performance-setup.sh'
+test-integration-sqlite-setup = 'sh scripts/test/integration-sqlite-setup.sh'
 test-performance = 'sh scripts/test/performance.sh'
+test-performance-setup = 'sh scripts/test/performance-setup.sh'
+type-check = "mypy cosmos"
 
 [tool.pytest.ini_options]
 filterwarnings = ["ignore::DeprecationWarning"]
 minversion = "6.0"
 markers = ["integration", "sqlite", "perf"]
 
 ######################################
 # DOCS
 ######################################
 
 [tool.hatch.envs.docs]
 dependencies = [
     "aenum",
-    "sphinx",
-    "pydata-sphinx-theme",
-    "sphinx-autobuild",
-    "sphinx-autoapi",
-    "openlineage-airflow",
     "apache-airflow-providers-cncf-kubernetes>=5.1.1",
+    "msgpack",
+    "openlineage-airflow",
     "pydantic>=1.10.0",
+    "pydata-sphinx-theme",
+    "sphinx",
+    "sphinx-autoapi",
+    "sphinx-autobuild",
 ]
 
 [tool.hatch.envs.docs.scripts]
 build = "sphinx-build -b html docs docs/_build"
 serve = "sphinx-autobuild docs docs/_build"
 
 ######################################
```

### Comparing `astronomer_cosmos-1.4.0a4/PKG-INFO` & `astronomer_cosmos-1.4.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: astronomer-cosmos
-Version: 1.4.0a4
+Version: 1.4.0rc1
 Summary: Orchestrate your dbt projects in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://astronomer.github.io/astronomer-cosmos
 Project-URL: Source code, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: aenum
 Requires-Dist: apache-airflow>=2.3.0
 Requires-Dist: attrs
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: jinja2>=3.0.0
+Requires-Dist: msgpack
 Requires-Dist: pydantic>=1.10.0
 Requires-Dist: typing-extensions; python_version < '3.8'
 Requires-Dist: virtualenv
 Provides-Extra: all
 Requires-Dist: dbt-athena; extra == 'all'
 Requires-Dist: dbt-bigquery; extra == 'all'
 Requires-Dist: dbt-databricks; extra == 'all'
```

