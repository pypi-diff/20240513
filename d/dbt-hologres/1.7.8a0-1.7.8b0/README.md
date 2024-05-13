# Comparing `tmp/dbt_hologres-1.7.8a0.tar.gz` & `tmp/dbt_hologres-1.7.8b0.tar.gz`

## Comparing `dbt_hologres-1.7.8a0.tar` & `dbt_hologres-1.7.8b0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/adapters/hologres/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/adapters/hologres/__version__.py
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/adapters/hologres/date.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/adapters/hologres/impl.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/adapters/hologres/relation.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/dbt_project.yml
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros.yml
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/profile_template.yml
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/sample_profiles.yml
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/adapters.sql
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/catalog.sql
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations.sql
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/timestamps.sql
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/incremental.sql
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/incremental_strategies.sql
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/seed.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/snapshot_merge.sql
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/table.sql
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/view.sql
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/alter.sql
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/create.sql
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/describe.sql
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/drop.sql
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/rename.sql
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/table/drop.sql
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/table/rename.sql
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/table/replace.sql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/view/drop.sql
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/view/rename.sql
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/view/replace.sql
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/any_value.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/columns_spec_ddl.sql
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/dateadd.sql
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/datediff.sql
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/dateutil.sql
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/last_day.sql
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/listagg.sql
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/split_part.sql
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/LICENSE
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/README.md
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/pyproject.toml
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/PKG-INFO
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/adapters/hologres/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/adapters/hologres/__version__.py
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/adapters/hologres/date.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/adapters/hologres/impl.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/adapters/hologres/relation.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/dbt_project.yml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros.yml
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/profile_template.yml
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/sample_profiles.yml
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/adapters.sql
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/catalog.sql
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations.sql
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/timestamps.sql
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/materializations/incremental.sql
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/materializations/incremental_strategies.sql
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/materializations/seed.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/materializations/table.sql
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/materializations/view.sql
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/materialized_view/create.sql
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/materialized_view/describe.sql
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/materialized_view/rename.sql
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/table/drop.sql
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/table/rename.sql
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/table/replace.sql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/view/drop.sql
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/view/rename.sql
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/view/replace.sql
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/utils/any_value.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/utils/columns_spec_ddl.sql
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/utils/dateutil.sql
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/dbt/include/hologres/macros/utils/split_part.sql
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/LICENSE
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/README.md
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/pyproject.toml
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8b0/PKG-INFO
```

### Comparing `dbt_hologres-1.7.8a0/dbt/adapters/hologres/__init__.py` & `dbt_hologres-1.7.8b0/dbt/adapters/hologres/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/adapters/hologres/date.py` & `dbt_hologres-1.7.8b0/dbt/adapters/hologres/date.py`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/adapters/hologres/impl.py` & `dbt_hologres-1.7.8b0/dbt/adapters/hologres/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/adapters.sql` & `dbt_hologres-1.7.8b0/dbt/include/hologres/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/catalog.sql` & `dbt_hologres-1.7.8b0/dbt/include/hologres/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations.sql` & `dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/timestamps.sql` & `dbt_hologres-1.7.8b0/dbt/include/hologres/macros/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/incremental.sql` & `dbt_hologres-1.7.8b0/dbt/include/hologres/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/seed.sql` & `dbt_hologres-1.7.8b0/dbt/include/hologres/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/snapshot_merge.sql` & `dbt_hologres-1.7.8b0/dbt/include/hologres/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/table.sql` & `dbt_hologres-1.7.8b0/dbt/include/hologres/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/view.sql` & `dbt_hologres-1.7.8b0/dbt/include/hologres/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/alter.sql` & `dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/table/replace.sql` & `dbt_hologres-1.7.8b0/dbt/include/hologres/macros/relations/table/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/datediff.sql` & `dbt_hologres-1.7.8b0/dbt/include/hologres/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/listagg.sql` & `dbt_hologres-1.7.8b0/dbt/include/hologres/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/.gitignore` & `dbt_hologres-1.7.8b0/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/LICENSE` & `dbt_hologres-1.7.8b0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/README.md` & `dbt_hologres-1.7.8b0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8a0/pyproject.toml` & `dbt_hologres-1.7.8b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "psycopg2>=2.9,<3.0"
+    "psycopg2-binary"
 ]
 [project.urls]
 Homepage = "https://github.com/winwin-inc/dbt-hologres"
 Documentation = "https://docs.getdbt.com"
 Repository = "https://github.com/winwin-inc/dbt-hologres.git"
 Issues = "https://github.com/winwin-inc/dbt-hologres/issues"
 Changelog = "https://github.com/winwin-inc/dbt-hologres/blob/main/CHANGELOG.md"
```

### Comparing `dbt_hologres-1.7.8a0/PKG-INFO` & `dbt_hologres-1.7.8b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-hologres
-Version: 1.7.8a0
+Version: 1.7.8b0
 Summary: The set of adapter protocols and base functionality that supports integration with dbt-core
 Project-URL: Homepage, https://github.com/winwin-inc/dbt-hologres
 Project-URL: Documentation, https://docs.getdbt.com
 Project-URL: Repository, https://github.com/winwin-inc/dbt-hologres.git
 Project-URL: Issues, https://github.com/winwin-inc/dbt-hologres/issues
 Project-URL: Changelog, https://github.com/winwin-inc/dbt-hologres/blob/main/CHANGELOG.md
 Author-email: dbt Labs <info@dbtlabs.com>
@@ -17,15 +17,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
-Requires-Dist: psycopg2<3.0,>=2.9
+Requires-Dist: psycopg2-binary
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
   <a href="https://github.com/dbt-labs/dbt-core/actions/workflows/main.yml">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-hologres Version: 1.7.8a0 Summary: The set of
+Metadata-Version: 2.1 Name: dbt-hologres Version: 1.7.8b0 Summary: The set of
 adapter protocols and base functionality that supports integration with dbt-
 core Project-URL: Homepage, https://github.com/winwin-inc/dbt-hologres Project-
 URL: Documentation, https://docs.getdbt.com Project-URL: Repository, https://
 github.com/winwin-inc/dbt-hologres.git Project-URL: Issues, https://github.com/
 winwin-inc/dbt-hologres/issues Project-URL: Changelog, https://github.com/
 winwin-inc/dbt-hologres/blob/main/CHANGELOG.md Author-email: dbt Labs
 dbtlabs.com> Maintainer-email: dbt Labs
@@ -10,15 +10,15 @@
 Cloud,dbt Core,dbt Labs,dbt-core,elt,hologres Classifier: Development Status ::
 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8.0
-Requires-Dist: psycopg2<3.0,>=2.9 Description-Content-Type: text/markdown
+Requires-Dist: psycopg2-binary Description-Content-Type: text/markdown
                                   [dbt logo]
                                   _[_C_I_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-hologres The `dbt-hologres` package contains all of
```

