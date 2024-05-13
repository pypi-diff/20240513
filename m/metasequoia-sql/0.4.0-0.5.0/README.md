# Comparing `tmp/metasequoia-sql-0.4.0.tar.gz` & `tmp/metasequoia-sql-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasequoia-sql-0.4.0.tar", last modified: Wed May  1 05:00:48 2024, max compression
+gzip compressed data, was "metasequoia-sql-0.5.0.tar", last modified: Mon May 13 00:45:31 2024, max compression
```

## Comparing `metasequoia-sql-0.4.0.tar` & `metasequoia-sql-0.5.0.tar`

### file list

```diff
@@ -1,59 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.883267 metasequoia-sql-0.4.0/
--rw-rw-rw-   0        0        0     1088 2024-03-11 00:28:43.000000 metasequoia-sql-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     8033 2024-05-01 05:00:48.883267 metasequoia-sql-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     7251 2024-05-01 04:51:45.000000 metasequoia-sql-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.867143 metasequoia-sql-0.4.0/metasequoia_sql/
--rw-rw-rw-   0        0        0      183 2024-04-15 00:51:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.871036 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/
--rw-rw-rw-   0        0        0      372 2024-04-18 23:36:58.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/__init__.py
--rw-rw-rw-   0        0        0     1728 2024-04-25 00:15:28.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/all_level_common_table.py
--rw-rw-rw-   0        0        0    10168 2024-05-01 00:26:31.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/base.py
--rw-rw-rw-   0        0        0    13204 2024-05-01 00:26:31.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/current_level_common_column.py
--rw-rw-rw-   0        0        0     3179 2024-04-25 00:15:28.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/current_level_common_table.py
-drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.872982 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/
--rw-rw-rw-   0        0        0       39 2024-04-26 23:40:20.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/__init__.py
--rw-rw-rw-   0        0        0     2290 2024-05-01 04:30:17.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/node.py
--rw-rw-rw-   0        0        0     4788 2024-05-01 04:36:11.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/table_lineage.py
--rw-rw-rw-   0        0        0    14940 2024-05-01 04:35:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/table_lineage_analyzer.py
--rw-rw-rw-   0        0        0     1811 2024-05-01 03:35:36.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/table_lineage_storage.py
--rw-rw-rw-   0        0        0    12263 2024-04-26 00:42:26.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_lineage_analyzer_by_meta.py
--rw-rw-rw-   0        0        0     4333 2024-04-25 00:15:28.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/tool.py
-drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.873956 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/toolkit/
--rw-rw-rw-   0        0        0      307 2024-05-01 04:00:55.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/toolkit/__init__.py
--rw-rw-rw-   0        0        0     1344 2024-05-01 00:26:31.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/toolkit/current_level_sub_query.py
--rw-rw-rw-   0        0        0     2189 2024-05-01 03:39:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/toolkit/current_level_table_name_analyzer.py
--rw-rw-rw-   0        0        0     1306 2024-05-01 04:27:55.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/toolkit/current_level_used_quote_columns.py
-drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.876444 metasequoia-sql-0.4.0/metasequoia_sql/common/
--rw-rw-rw-   0        0        0      209 2024-04-15 00:51:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/common/__init__.py
--rw-rw-rw-   0        0        0     3937 2024-04-15 00:51:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/common/base_scanner.py
--rw-rw-rw-   0        0        0      601 2024-04-15 00:51:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/common/basic.py
--rw-rw-rw-   0        0        0      226 2024-04-15 00:51:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/common/text_scanner.py
--rw-rw-rw-   0        0        0     5617 2024-04-24 23:58:17.000000 metasequoia-sql-0.4.0/metasequoia_sql/common/token_scanner.py
--rw-rw-rw-   0        0        0     5375 2024-04-24 00:26:00.000000 metasequoia-sql-0.4.0/metasequoia_sql/common/unsed_static.py
-drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.877427 metasequoia-sql-0.4.0/metasequoia_sql/core/
--rw-rw-rw-   0        0        0      171 2024-04-25 00:28:03.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.880347 metasequoia-sql-0.4.0/metasequoia_sql/core/node/
--rw-rw-rw-   0        0        0      256 2024-04-26 00:25:39.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/node/__init__.py
--rw-rw-rw-   0        0        0      808 2024-04-26 00:25:39.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/node/abc_node.py
--rw-rw-rw-   0        0        0     6252 2024-04-26 00:31:00.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/node/enum_node.py
--rw-rw-rw-   0        0        0    63163 2024-04-26 23:40:20.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/node/objects.py
--rw-rw-rw-   0        0        0      295 2024-04-25 00:42:57.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/node/sql_type.py
--rw-rw-rw-   0        0        0    75899 2024-04-26 00:42:26.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/parser.py
--rw-rw-rw-   0        0        0      627 2024-04-18 23:18:49.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/static.py
--rw-rw-rw-   0        0        0      689 2024-04-25 00:02:19.000000 metasequoia-sql-0.4.0/metasequoia_sql/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.881320 metasequoia-sql-0.4.0/metasequoia_sql/lexical/
--rw-rw-rw-   0        0        0      144 2024-04-24 00:21:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/lexical/__init__.py
--rw-rw-rw-   0        0        0     8984 2024-04-26 00:27:19.000000 metasequoia-sql-0.4.0/metasequoia_sql/lexical/nodes.py
--rw-rw-rw-   0        0        0    15442 2024-05-01 03:41:47.000000 metasequoia-sql-0.4.0/metasequoia_sql/lexical/parser.py
--rw-rw-rw-   0        0        0      334 2024-04-26 00:27:42.000000 metasequoia-sql-0.4.0/metasequoia_sql/lexical/static.py
-drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.882294 metasequoia-sql-0.4.0/metasequoia_sql/plugins/
--rw-rw-rw-   0        0        0        0 2024-04-18 23:18:49.000000 metasequoia-sql-0.4.0/metasequoia_sql/plugins/__init__.py
--rw-rw-rw-   0        0        0     5734 2024-04-26 00:25:39.000000 metasequoia-sql-0.4.0/metasequoia_sql/plugins/mybaitis.py
--rw-rw-rw-   0        0        0     1095 2024-04-24 00:26:38.000000 metasequoia-sql-0.4.0/metasequoia_sql/static.py
-drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.883267 metasequoia-sql-0.4.0/metasequoia_sql.egg-info/
--rw-rw-rw-   0        0        0     8033 2024-05-01 05:00:48.000000 metasequoia-sql-0.4.0/metasequoia_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1820 2024-05-01 05:00:48.000000 metasequoia-sql-0.4.0/metasequoia_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 05:00:48.000000 metasequoia-sql-0.4.0/metasequoia_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-01 05:00:48.000000 metasequoia-sql-0.4.0/metasequoia_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 05:00:48.883267 metasequoia-sql-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1153 2024-05-01 04:59:57.000000 metasequoia-sql-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.211845 metasequoia-sql-0.5.0/
+-rw-rw-rw-   0        0        0     1088 2024-03-11 00:28:43.000000 metasequoia-sql-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     3449 2024-05-13 00:45:31.211845 metasequoia-sql-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2669 2024-05-13 00:44:26.000000 metasequoia-sql-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.196271 metasequoia-sql-0.5.0/metasequoia_sql/
+-rw-rw-rw-   0        0        0      249 2024-05-12 04:36:10.000000 metasequoia-sql-0.5.0/metasequoia_sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.199192 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/
+-rw-rw-rw-   0        0        0      499 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/__init__.py
+-rw-rw-rw-   0        0        0     4524 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/base.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.201138 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/
+-rw-rw-rw-   0        0        0       33 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/__init__.py
+-rw-rw-rw-   0        0        0     6767 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/table_lineage.py
+-rw-rw-rw-   0        0        0    18047 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/table_lineage_analyzer.py
+-rw-rw-rw-   0        0        0     1835 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/table_lineage_storage.py
+-rw-rw-rw-   0        0        0     2666 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/node.py
+-rw-rw-rw-   0        0        0     2959 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/tool.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.203085 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/
+-rw-rw-rw-   0        0        0      345 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/__init__.py
+-rw-rw-rw-   0        0        0     2162 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/all_level_standard_table.py
+-rw-rw-rw-   0        0        0     9530 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_column_analyzer.py
+-rw-rw-rw-   0        0        0     1333 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_sub_query.py
+-rw-rw-rw-   0        0        0     2242 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_table_name_analyzer.py
+-rw-rw-rw-   0        0        0     2875 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_used_quote_columns.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.206005 metasequoia-sql-0.5.0/metasequoia_sql/common/
+-rw-rw-rw-   0        0        0      142 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/common/__init__.py
+-rw-rw-rw-   0        0        0     3068 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/common/basic.py
+-rw-rw-rw-   0        0        0      860 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/common/char_set.py
+-rw-rw-rw-   0        0        0      812 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/common/name_set.py
+-rw-rw-rw-   0        0        0     7781 2024-05-12 04:36:10.000000 metasequoia-sql-0.5.0/metasequoia_sql/common/scanner.py
+-rw-rw-rw-   0        0        0     6414 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/common/static.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.207952 metasequoia-sql-0.5.0/metasequoia_sql/core/
+-rw-rw-rw-   0        0        0      173 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/core/__init__.py
+-rw-rw-rw-   0        0        0    88182 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/core/node.py
+-rw-rw-rw-   0        0        0   114838 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/core/parser.py
+-rw-rw-rw-   0        0        0      295 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/core/sql_type.py
+-rw-rw-rw-   0        0        0      683 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.209899 metasequoia-sql-0.5.0/metasequoia_sql/lexical/
+-rw-rw-rw-   0        0        0      421 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/lexical/__init__.py
+-rw-rw-rw-   0        0        0     4196 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/lexical/amt_node.py
+-rw-rw-rw-   0        0        0     6824 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/lexical/fsm_machine.py
+-rw-rw-rw-   0        0        0     4247 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/lexical/fsm_operate.py
+-rw-rw-rw-   0        0        0    13589 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/lexical/fsm_operation_map.py
+-rw-rw-rw-   0        0        0     2404 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/lexical/fsm_status.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.210872 metasequoia-sql-0.5.0/metasequoia_sql/plugins/
+-rw-rw-rw-   0        0        0        0 2024-05-01 05:05:38.000000 metasequoia-sql-0.5.0/metasequoia_sql/plugins/__init__.py
+-rw-rw-rw-   0        0        0     5778 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/plugins/mybaitis.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.211845 metasequoia-sql-0.5.0/metasequoia_sql.egg-info/
+-rw-rw-rw-   0        0        0     3449 2024-05-13 00:45:31.000000 metasequoia-sql-0.5.0/metasequoia_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1606 2024-05-13 00:45:31.000000 metasequoia-sql-0.5.0/metasequoia_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 00:45:31.000000 metasequoia-sql-0.5.0/metasequoia_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-13 00:45:31.000000 metasequoia-sql-0.5.0/metasequoia_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 00:45:31.211845 metasequoia-sql-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1153 2024-05-13 00:45:17.000000 metasequoia-sql-0.5.0/setup.py
```

### Comparing `metasequoia-sql-0.4.0/LICENSE` & `metasequoia-sql-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/node.py` & `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/node.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-基础节点类
+分析器的基本节点类
 
 标准表名对象（`StandardTable`）包含表可选的所属模式名（`schema_name`）和必选的表名（`table_name`）两个属性。
 标准字段对象（`StandardColumn`）包含必选的字段序号（`column_idx`）、字段名（`column_name`）两个属性。
 引用字段对象（`QuoteColumn`）包含可选的字段所属表名（`table_name`）以及必选的字段名（`column_name`）两个属性。
 源字段对象（`SourceColumn`）包含可选的字段所属模式名（`schema_name`），以及必选的所属表名（`table_name`）和字段名（`column_name`）三个属性。
 """
 
@@ -11,18 +11,15 @@
 from typing import Optional
 
 __all__ = ["StandardTable", "StandardColumn", "QuoteColumn", "SourceColumn"]
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class StandardTable:
-    """标准表名对象
-
-    TODO 待支持子查询的形式
-    """
+    """标准表名对象"""
 
     schema_name: Optional[str] = dataclasses.field(kw_only=True, default=None)  # 所属模式名
     table_name: str = dataclasses.field(kw_only=True)  # 表名
 
     def source(self):
         """引用字段的源代码"""
         return f"{self.schema_name}.{self.table_name}" if self.schema_name else f"{self.table_name}"
@@ -31,21 +28,30 @@
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class StandardColumn:
     """标准字段对象"""
 
     column_idx: int = dataclasses.field(kw_only=True)  # 字段序号
     column_name: str = dataclasses.field(kw_only=True)  # 字段名
 
+    def source(self):
+        """引用字段的源代码"""
+        return self.column_name
+
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class QuoteColumn:
     """引用字段对象"""
 
     table_name: Optional[str] = dataclasses.field(kw_only=True, default=None)  # 所属表名
     column_name: Optional[str] = dataclasses.field(kw_only=True)  # 字段名（为空时表示没有直接使用字段的聚集函数）
+    column_idx: Optional[int] = dataclasses.field(kw_only=True, default=None)  # 字段序号（仅在 GROUP BY 和 ORDER BY 语句中使用）
+
+    def source(self):
+        """引用字段的源代码"""
+        return f"{self.table_name}.{self.column_name}" if self.table_name else f"{self.column_name}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class SourceColumn:
     """源字段对象"""
 
     schema_name: Optional[str] = dataclasses.field(kw_only=True, default=None)  # 所属模式名
```

### Comparing `metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/table_lineage.py` & `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/table_lineage.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,70 +17,103 @@
 - 返回字段名的上游源字段对象的列表（`get_source_column_list`）：返回指定字段名的源字段对象的列表（不支持通配符）
 - 返回所有标准字段对象的列表（`get_all_standard_columns`）：返回所有标准字段对象的有序列表（通配符场景）
 - 返回所有上游源字段对象的列表的列表（`get_all_source_column_lists`）：返回所有上游源字段对象的列表的有序列表（通配符场景）
 """
 
 from typing import List, Tuple
 
-from metasequoia_sql.analyzer.data_linage import node
+from metasequoia_sql.analyzer import node
 from metasequoia_sql.core import ASTCreateTableStatement
 
-__all__ = ["TableLineage"]
+__all__ = ["SelectTableLineage", "InsertTableLineage"]
 
 
-class TableLineage:
-    """表数据血缘分析器"""
+class SelectTableLineage:
+    """SELECT 语句表数据血缘对象"""
 
     def __init__(self, data_lineage: List[Tuple[node.StandardColumn, List[node.SourceColumn]]]):
         self._column_name_list = []  # 字段名的有序列表
         self._column_name_to_standard_column_hash = {}  # 字段名到标准字段对象的哈希映射
         self._column_name_to_source_column_list_hash = {}  # 字段名到源字段对象列表的哈希映射
+        self._column_idx_to_source_column_list_hash = {}  # 字段序号到源字段对象列表的哈希映射
         self._standard_table_set = set()  # 使用的上游表列表
         for standard_column, source_column_list in data_lineage:
-            column_name = standard_column.column_name
-            self._column_name_list.append(column_name)
-            self._column_name_to_standard_column_hash[column_name] = standard_column
-            self._column_name_to_source_column_list_hash[column_name] = source_column_list
+            self._column_name_list.append(standard_column.column_name)
+            self._column_name_to_standard_column_hash[standard_column.column_name] = standard_column
+            self._column_name_to_source_column_list_hash[standard_column.column_name] = source_column_list
+            self._column_idx_to_source_column_list_hash[standard_column.column_idx] = source_column_list
             for source_column in source_column_list:
                 self._standard_table_set.add(node.StandardTable(schema_name=source_column.schema_name,
                                                                 table_name=source_column.table_name))
 
     @staticmethod
     def by_create_table_statement(ast: ASTCreateTableStatement):
+        """使用 CREATE TABLE 表达式对象实例化"""
         data_lineage = []
-        schema_name = ast.table_name.schema if ast.table_name.schema is not None else ""
-        table_name = ast.table_name.table
+        schema_name = ast.table_name.schema_name if ast.table_name.schema_name is not None else ""
+        table_name = ast.table_name.table_name
         for column_idx, column_expression in enumerate(ast.columns):
             column_name = column_expression.column_name
             select_column = node.StandardColumn(column_idx=column_idx, column_name=column_name)
             source_column = node.SourceColumn(schema_name=schema_name, table_name=table_name, column_name=column_name)
             data_lineage.append((select_column, [source_column]))
-        return TableLineage(data_lineage)
+        return SelectTableLineage(data_lineage)
 
     def has_column(self, column_name: str) -> bool:
         """查询是否包含字段名：如果包含该字段名则返回 True，否则返回 False（支持通配符）"""
         return column_name in self._column_name_list or column_name == "*"
 
     def get_all_standard_columns(self) -> List[node.StandardColumn]:
         """返回所有标准字段对象的有序列表（通配符场景）"""
         return [self._column_name_to_standard_column_hash[column_name]
                 for column_name in self._column_name_list]
 
-    def get_source_column_list(self, column_name: str) -> List[node.SourceColumn]:
+    def get_source_column_list_by_idx(self, column_idx: int) -> List[node.SourceColumn]:
+        """返回指定字段名的源字段对象的列表"""
+        return self._column_idx_to_source_column_list_hash[column_idx]
+
+    def get_source_column_list_by_name(self, column_name: str) -> List[node.SourceColumn]:
         """返回指定字段名的源字段对象的列表（支持通配符）"""
         if column_name != "*":
             return self._column_name_to_source_column_list_hash[column_name]
         all_source_column_list = []
         for source_column_list in self._column_name_to_source_column_list_hash.values():
             all_source_column_list.extend(source_column_list)
         return all_source_column_list
 
     def get_standard_table_list(self) -> List[node.StandardTable]:
         """获取上游表的列表"""
         return list(self._standard_table_set)
 
     def all_columns(self) -> List[Tuple[node.StandardColumn, List[node.SourceColumn]]]:
+        """获取所有字段的标准字段对象和源字段对象列表的元组的列表"""
         data_lineage = []
         for column_name in self._column_name_list:
             data_lineage.append((self._column_name_to_standard_column_hash.get(column_name),
                                  self._column_name_to_source_column_list_hash.get(column_name)))
         return data_lineage
+
+
+class InsertTableLineage:
+    """INSERT 语句表数据血缘对象"""
+
+    def __init__(self, data_lineage: List[Tuple[node.SourceColumn, List[node.SourceColumn]]]):
+        self._down_column_name_list = []  # 下游表字段名的有序列表
+        self._column_name_to_source_column_list_hash = {}  # 字段名到上游表源字段的映射
+        for down_column, up_column_list in data_lineage:
+            self._down_column_name_list.append(down_column)
+            self._column_name_to_source_column_list_hash[down_column.column_name] = up_column_list
+
+    def get_up_column_list(self, column_name: str):
+        """根据下游表字段名查询上游源字段"""
+        return self._column_name_to_source_column_list_hash[column_name]
+
+    def get_all_down_columns(self):
+        """获取所有下游表字段"""
+        return self._down_column_name_list
+
+    def all_columns(self) -> List[Tuple[node.SourceColumn, List[node.SourceColumn]]]:
+        """获取所有字段的下游表字段对象和上游表源字段对象列表的元组的列表"""
+        data_lineage = []
+        for down_column in self._down_column_name_list:
+            data_lineage.append((down_column, self._column_name_to_source_column_list_hash[down_column.column_name]))
+        return data_lineage
```

### Comparing `metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/table_lineage_analyzer.py` & `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/table_lineage_analyzer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,240 +1,289 @@
 """
 表数据血缘分析器
 """
 
 from typing import Optional, List, Tuple
 
 from metasequoia_sql import core
-from metasequoia_sql.analyzer.data_linage.node import StandardColumn, QuoteColumn, SourceColumn
-from metasequoia_sql.analyzer.data_linage.table_lineage import TableLineage
+from metasequoia_sql.analyzer import toolkit
+from metasequoia_sql.analyzer.data_linage.table_lineage import SelectTableLineage, InsertTableLineage
 from metasequoia_sql.analyzer.data_linage.table_lineage_storage import TableLineageStorage
+from metasequoia_sql.analyzer.node import StandardColumn, QuoteColumn, SourceColumn
 from metasequoia_sql.analyzer.tool import CreateTableStatementGetter
-from metasequoia_sql.analyzer.toolkit import CurrentLevelSubQuery, CurrentLevelTableNameAnalyzer, \
-    CurrentNodeUsedQuoteColumn
 from metasequoia_sql.errors import AnalyzerError
 
 __all__ = ["TableLineageAnalyzer"]
 
 
 class TableLineageAnalyzer:
     """表数据血缘管理器"""
 
     def __init__(self, create_table_statement_getter: CreateTableStatementGetter):
         self._create_table_statement_getter = create_table_statement_getter  # 建表语句查询器
 
-    def get_table_lineage(self,
-                          select_statement: core.ASTSelectStatement,
-                          table_lineage_storage: Optional[TableLineageStorage] = None) -> TableLineage:
-        """获取表数据血缘对象
+    def get_select_table_lineage(self,
+                                 select_statement: core.ASTSelectStatement,
+                                 table_lineage_storage: Optional[TableLineageStorage] = None) -> SelectTableLineage:
+        """获取 SELECT 语句中的表数据血缘对象
 
         TODO 增加对相关子查询的支持
 
         Parameters
         ----------
         select_statement: core.ASTSelectStatement
             查询语句
         table_lineage_storage: Optional[TableLineageStorage], default = None
             在这个表之前的 WITH 临时表存储器（用于递归调用）
         """
-        print("----------------------------------------")
         # 初始化表数据血缘存储器
         if table_lineage_storage is None:
             table_lineage_storage = TableLineageStorage(self._create_table_statement_getter)
 
-        # 逐个遍历 WITH 子句
-        for table_name, with_select_statement in select_statement.with_clause.tables:
-            table_lineage = self.get_table_lineage(with_select_statement, table_lineage_storage)
-            table_lineage_storage.add_with_table(table_name=table_name, table_lineage=table_lineage)
-
-        # 遍历当前层级的所有子查询
-        current_level_sub_query = CurrentLevelSubQuery(select_statement)
-        for alias_name in current_level_sub_query.get_all_sub_query_alias_name():
-            sub_query_select_statement = current_level_sub_query.get_sub_query_statement(alias_name)
-            table_lineage = self.get_table_lineage(sub_query_select_statement, table_lineage_storage)
-            table_lineage_storage.add_sub_query_table(table_name=alias_name, table_lineage=table_lineage)
-
-        print(f"time_lineage_storage: {list(table_lineage_storage._with_table.keys())}")
+        self._analyze_with_clauses(table_lineage_storage, select_statement.with_clause)  # 处理 WITH 语句中临时表的数据血缘
+        self._analyze_sub_query(table_lineage_storage, select_statement)  # 处理子查询中临时表的数据血缘
 
         # 初始化当前层级的表名规范器
-        table_name_analyzer = CurrentLevelTableNameAnalyzer(select_statement)
-        print(f"table_name_analyzer: {table_name_analyzer}")
+        table_name_analyzer = toolkit.CurrentLevelTableNameAnalyzer(select_statement)
 
         # 获取当前层级使用的 LATERAL VIEW 字段属性
-        lateral_view_columns = {column_name: quote_column_list
-                                for column_name, quote_column_list
-                                in self.get_lateral_view_clause_column_name_to_quote_columns(select_statement)}
+        lateral_view_columns = dict(self.get_lateral_view_clause_column_name_to_quote_columns(select_statement))
 
         # 处理当前层级的引用字段逻辑
         data_lineage = []
         for standard_column, quote_columns in self.get_current_level_stand_column_used_quote_columns(
                 select_statement=select_statement,
                 table_lineage_storage=table_lineage_storage,
                 table_name_analyzer=table_name_analyzer):
-            # 处理使用 LATERAL VIEW 子句中字段的情况
-            new_quote_column = []
+            # 将使用的 LATERAL VIEW 子句中字段，映射为原始的引用字段对象
+            new_quote_column: List[QuoteColumn] = []
             for quote_column in quote_columns:
-                if quote_column.table_name is None and quote_column.column_name in lateral_view_columns:
+                if (quote_column.table_name is None and quote_column.column_name is not None
+                        and quote_column.column_name in lateral_view_columns):
                     new_quote_column.extend(lateral_view_columns[quote_column.column_name])
                 else:
                     new_quote_column.append(quote_column)
 
-            # 使用不包含 LATERAL VIEW 子句的其他字段
+            # 处理引用字段的情况
             source_column_list = []
             for quote_column in new_quote_column:
-                if quote_column.table_name is not None:
-                    from_standard_table = table_name_analyzer.get_standard_table(quote_column.table_name)
-                    from_table_lineage = table_lineage_storage.get_table_lineage(from_standard_table)
-                    source_column_list.extend(from_table_lineage.get_source_column_list(quote_column.column_name))
-                elif quote_column.column_name is None:  # 兼容聚集函数的参数中没有直接使用字段的情况，则直接标记引用了所有上游表
-                    for from_standard_table in table_name_analyzer.get_all_standard_table():
-                        from_table_lineage = table_lineage_storage.get_table_lineage(from_standard_table)
-                        for source_table in from_table_lineage.get_standard_table_list():
-                            source_column_list.append(SourceColumn(schema_name=source_table.schema_name,
-                                                                   table_name=source_table.table_name,
-                                                                   column_name=None))
-                else:
-                    already_match = False  # 是否已经匹配到上游表
-                    for from_standard_table in table_name_analyzer.get_all_standard_table():
-                        from_table_lineage = table_lineage_storage.get_table_lineage(from_standard_table)
-                        if not from_table_lineage.has_column(quote_column.column_name):
-                            continue
-                        if already_match is True:
-                            raise AnalyzerError("同一个字段可以匹配到多个上游表")
-                        already_match = True
-                        source_column_list.extend(from_table_lineage.get_source_column_list(quote_column.column_name))
-                    if already_match is False:
-                        for from_standard_table in table_name_analyzer.get_all_standard_table():
-                            from_table_lineage = table_lineage_storage.get_table_lineage(from_standard_table)
-                            print(from_standard_table.table_name, ":", from_table_lineage.all_columns())
-                        raise AnalyzerError(f"没有匹配到合适的上游表字段: 字段={quote_column}, "
-                                            f"上游表={table_name_analyzer.get_all_standard_table()}")
+                source_column_list.extend(self._analyze_quote_column(table_lineage_storage=table_lineage_storage,
+                                                                     table_name_analyzer=table_name_analyzer,
+                                                                     quote_column=quote_column))
             data_lineage.append((standard_column, source_column_list))
-        return TableLineage(data_lineage=data_lineage)
+        return SelectTableLineage(data_lineage=data_lineage)
+
+    def _analyze_with_clauses(self, table_lineage_storage: TableLineageStorage, with_clause: core.ASTWithClause):
+        """处理 WITH 语句中临时表的数据血缘"""
+        for table_name, with_select_statement in with_clause.tables:
+            table_lineage = self.get_select_table_lineage(with_select_statement, table_lineage_storage)
+            table_lineage_storage.add_with_table(table_name=table_name, table_lineage=table_lineage)
+
+    def _analyze_sub_query(self, table_lineage_storage: TableLineageStorage, select_statement: core.ASTSelectStatement):
+        """处理子查询中临时表的数据血缘"""
+        current_level_sub_query = toolkit.CurrentLevelSubQuery(select_statement)
+        for alias_name in current_level_sub_query.get_all_sub_query_alias_name():
+            sub_query_select_statement = current_level_sub_query.get_sub_query_statement(alias_name)
+            table_lineage = self.get_select_table_lineage(sub_query_select_statement, table_lineage_storage)
+            table_lineage_storage.add_sub_query_table(table_name=alias_name, table_lineage=table_lineage)
+
+    @staticmethod
+    def _analyze_quote_column(table_lineage_storage: TableLineageStorage,
+                              table_name_analyzer: toolkit.CurrentLevelTableNameAnalyzer,
+                              quote_column: QuoteColumn
+                              ) -> List[SourceColumn]:
+        """计算引用字段的上游源字段"""
+        # 表名不为空、字段名不为空的引用字段对象：获取上游表指定字段的上游源字段
+        if quote_column.table_name is not None:
+            from_standard_table = table_name_analyzer.get_standard_table(quote_column.table_name)
+            from_table_lineage = table_lineage_storage.get_table_lineage(from_standard_table)
+            return from_table_lineage.get_source_column_list_by_name(quote_column.column_name)
+
+        # 处理表名和字段名均为空的引用对象（聚集函数的参数没有直接使用字段的情况）：获取所有上游表、字段为 None 的源字段对象
+        if quote_column.column_name is None:
+            source_column_list = []
+            for from_standard_table in table_name_analyzer.get_all_standard_table():
+                from_table_lineage = table_lineage_storage.get_table_lineage(from_standard_table)
+                for source_table in from_table_lineage.get_standard_table_list():
+                    source_column_list.append(SourceColumn(schema_name=source_table.schema_name,
+                                                           table_name=source_table.name,
+                                                           column_name=None))
+            return source_column_list
+
+        # 处理表名为空，字段名不为空的引用字段对象：在各个上游表中寻找，若能且仅能匹配到一个上游表字段则返回该字段的上游源字段
+        source_column_list = []
+        already_match = False  # 是否已经匹配到上游表
+        for from_standard_table in table_name_analyzer.get_all_standard_table():
+            from_table_lineage = table_lineage_storage.get_table_lineage(from_standard_table)
+            if not from_table_lineage.has_column(quote_column.column_name):
+                continue
+            if already_match is True:
+                raise AnalyzerError("同一个字段可以匹配到多个上游表")
+            already_match = True
+            source_column_list.extend(
+                from_table_lineage.get_source_column_list_by_name(quote_column.column_name))
+        if already_match is False:
+            for from_standard_table in table_name_analyzer.get_all_standard_table():
+                from_table_lineage = table_lineage_storage.get_table_lineage(from_standard_table)
+                print(from_standard_table.table_name, ":", from_table_lineage.all_columns())
+            raise AnalyzerError(f"没有匹配到合适的上游表字段: 字段={quote_column}, "
+                                f"上游表={table_name_analyzer.get_all_standard_table()}")
+        return source_column_list
+
+    def get_insert_table_lineage(self, insert_statement: core.ASTInsertSelectStatement) -> InsertTableLineage:
+        """获取 INSERT 语句中的表数据血缘对象"""
+        if insert_statement.columns is not None:
+            insert_columns = [SourceColumn(schema_name=insert_statement.table_name.schema_name,
+                                           table_name=insert_statement.table_name.table_name,
+                                           column_name=column.column_name)
+                              for column in insert_statement.columns]
+        else:
+            full_table_name = insert_statement.table_name.source()
+            create_table_statement = self._create_table_statement_getter.get_statement(full_table_name)
+            insert_columns = [SourceColumn(schema_name=insert_statement.table_name.schema_name,
+                                           table_name=insert_statement.table_name.table_name,
+                                           column_name=column.column_name)
+                              for column in create_table_statement.columns]
+
+        select_statement = insert_statement.select_statement.set_with_clauses(insert_statement.with_clause)
+        select_table_lineage = self.get_select_table_lineage(select_statement=select_statement)
+
+        if len(insert_columns) != len(select_table_lineage.all_columns()):
+            raise AnalyzerError("写入字段数量与读取字段数量不一致")
+
+        # 获取 INSERT 每个字段对应的上游源字段
+        data_lineage = []
+        for column_idx, down_column in enumerate(insert_columns):
+            data_lineage.append((down_column, select_table_lineage.get_source_column_list_by_idx(column_idx + 1)))
+        return InsertTableLineage(data_lineage=data_lineage)
 
     def get_current_level_stand_column_used_quote_columns(
             self,
             select_statement: core.ASTSelectStatement,
             table_lineage_storage: TableLineageStorage,
-            table_name_analyzer: CurrentLevelTableNameAnalyzer
+            table_name_analyzer: toolkit.CurrentLevelTableNameAnalyzer
     ) -> List[Tuple[StandardColumn, List[QuoteColumn]]]:
         """获取 ASTSelectStatement 节点当前层级标准字段对象和使用的应用字段对象的映射关系"""
         if isinstance(select_statement, core.ASTSingleSelectStatement):
             return self.get_single_current_level_standard_column_used_quote_columns(
                 select_statement=select_statement,
                 table_lineage_storage=table_lineage_storage,
                 table_name_analyzer=table_name_analyzer
             )
         # 处理 UNION 多个 SELECT 语句
         if isinstance(select_statement, core.ASTUnionSelectStatement):
-            result = None
+            result: Optional[List[Tuple[StandardColumn, List[QuoteColumn]]]] = None
+            n_column: Optional[int] = None
             for element in select_statement.elements:
                 if not isinstance(element, core.ASTSingleSelectStatement):
                     continue
                 if result is None:
                     result = self.get_single_current_level_standard_column_used_quote_columns(
                         select_statement=element,
                         table_lineage_storage=table_lineage_storage,
                         table_name_analyzer=table_name_analyzer
                     )
+                    n_column = len(result)
                 else:
                     merge = self.get_single_current_level_standard_column_used_quote_columns(
                         select_statement=element,
                         table_lineage_storage=table_lineage_storage,
                         table_name_analyzer=table_name_analyzer
                     )
-                    assert len(result) == len(merge), "UNION的多个SELECT语句的字段数不同"
-                    for i in range(len(result)):
+                    assert len(merge) == n_column, "UNION的多个SELECT语句的字段数不同"
+                    for i in range(n_column):
                         standard_column, quote_column_list = result[i]
                         quote_column_list.extend(merge[i][1])
                         result[i] = (standard_column, quote_column_list)
             return result
         raise AnalyzerError("未知的SELECT语句类型")
 
     @classmethod
     def get_single_current_level_standard_column_used_quote_columns(
             cls,
             select_statement: core.ASTSingleSelectStatement,
             table_lineage_storage: TableLineageStorage,
-            table_name_analyzer: CurrentLevelTableNameAnalyzer
+            table_name_analyzer: toolkit.CurrentLevelTableNameAnalyzer
     ) -> List[Tuple[StandardColumn, List[QuoteColumn]]]:
-        """获取 ASTSingleSelectStatement 节点当前层级标准字段对象和使用的应用字段对象的映射关系"""
+        """获取 ASTSingleSelectStatement 节点当前层级标准字段对象和使用的引用字段对象的映射关系
+
+        TODO 多个表的有序性
+        """
         result = []
         column_idx = 1
         for column in select_statement.select_clause.columns:
             if column.alias is not None:  # 有别名的情况（此时一定不是通配符）
                 standard_column = StandardColumn(column_name=column.alias.name, column_idx=column_idx)
                 column_idx += 1
-                result.append((standard_column, CurrentNodeUsedQuoteColumn.handle(column.column)))
-            elif isinstance(column.column, core.ASTColumnNameExpression):  # 直接使用字段的情况
-                # TODO 待修改属性名：column.column_value.column_name
-                if column.column.column == "*":  # 通配符
-                    if column.column.table is not None:  # 有表名的通配符
-                        standard_table = table_name_analyzer.get_standard_table(column.column.table)
+                result.append((standard_column, toolkit.CurrentNodeUsedQuoteColumn.handle(column.value)))
+            elif isinstance(column.value, core.ASTWildcardExpression):  # 通配符的情况
+                if column.value.table_name is not None:  # 有表名的通配符
+                    standard_table = table_name_analyzer.get_standard_table(column.value.table_name)
+                    table_lineage = table_lineage_storage.get_table_lineage(standard_table)
+                    for from_standard_column in table_lineage.get_all_standard_columns():
+                        standard_column = StandardColumn(column_name=from_standard_column.column_name,
+                                                         column_idx=column_idx)
+                        column_idx += 1
+                        quote_column = QuoteColumn(table_name=standard_table.table_name,
+                                                   column_name=from_standard_column.column_name)
+                        result.append((standard_column, [quote_column]))
+                else:  # 没有表名的通配符
+                    for standard_table in table_name_analyzer.get_all_standard_table():
                         table_lineage = table_lineage_storage.get_table_lineage(standard_table)
                         for from_standard_column in table_lineage.get_all_standard_columns():
                             standard_column = StandardColumn(column_name=from_standard_column.column_name,
                                                              column_idx=column_idx)
                             column_idx += 1
                             quote_column = QuoteColumn(table_name=standard_table.table_name,
                                                        column_name=from_standard_column.column_name)
                             result.append((standard_column, [quote_column]))
-                    else:  # 没有表名的通配符
-                        # TODO 多个表的有序性
-                        for standard_table in table_name_analyzer.get_all_standard_table():
-                            table_lineage = table_lineage_storage.get_table_lineage(standard_table)
-                            for from_standard_column in table_lineage.get_all_standard_columns():
-                                standard_column = StandardColumn(column_name=from_standard_column.column_name,
-                                                                 column_idx=column_idx)
-                                column_idx += 1
-                                quote_column = QuoteColumn(table_name=standard_table.table_name,
-                                                           column_name=from_standard_column.column_name)
-                                result.append((standard_column, [quote_column]))
-                else:  # 非通配符
-                    standard_column = StandardColumn(column_name=column.column.column, column_idx=column_idx)
-                    column_idx += 1
-                    quote_column = QuoteColumn(table_name=column.column.table,
-                                               column_name=column.column.column)
-                    result.append((standard_column, [quote_column]))
+            elif isinstance(column.value, core.ASTColumnName):  # 直接使用字段的情况
+                standard_column = StandardColumn(column_name=column.value.column_name, column_idx=column_idx)
+                column_idx += 1
+                quote_column = QuoteColumn(table_name=column.value.table_name,
+                                           column_name=column.value.column_name)
+                result.append((standard_column, [quote_column]))
             else:  # 不是字段名的情况（此时一定不是通配符）
-                standard_column = StandardColumn(column_name=column.column.source(core.SQLType.DEFAULT),
+                standard_column = StandardColumn(column_name=column.value.source(),
                                                  column_idx=column_idx)
                 column_idx += 1
-                result.append((standard_column, CurrentNodeUsedQuoteColumn.handle(column.column)))
+                result.append((standard_column, toolkit.CurrentNodeUsedQuoteColumn.handle(column.value)))
         return result
 
     def get_lateral_view_clause_column_name_to_quote_columns(
             self,
             select_statement: core.ASTSelectStatement
     ) -> List[Tuple[str, List[QuoteColumn]]]:
         """获取 ASTSelectStatement 节点的 LATERAL VIEW 子句中所有字段到引用字段对象列表的映射关系"""
         if isinstance(select_statement, core.ASTSingleSelectStatement):
             return self.get_single_lateral_view_clause_column_name_to_quote_columns(select_statement)
         # 处理 UNION 多个 SELECT 语句
         if isinstance(select_statement, core.ASTUnionSelectStatement):
-            result = None
+            result: Optional[List[Tuple[str, List[QuoteColumn]]]] = None
+            n_column: Optional[int] = None
             for element in select_statement.elements:
                 if not isinstance(element, core.ASTSingleSelectStatement):
                     continue
                 if result is None:
                     result = self.get_single_lateral_view_clause_column_name_to_quote_columns(element)
+                    n_column = len(result)
                 else:
                     merge = self.get_single_lateral_view_clause_column_name_to_quote_columns(element)
-                    assert len(result) == len(merge), "UNION的多个SELECT语句的字段数不同"
-                    for i in range(len(result)):
+                    assert len(merge) == n_column, "UNION的多个SELECT语句的字段数不同"
+                    for i in range(n_column):
                         column_name, quote_column_list = result[i]
                         quote_column_list.extend(merge[i][1])
                         result[i] = (column_name, quote_column_list)
             return result
         raise AnalyzerError("未知的SELECT语句类型")
 
     @classmethod
     def get_single_lateral_view_clause_column_name_to_quote_columns(
             cls,
             select_statement: core.ASTSingleSelectStatement
     ) -> List[Tuple[str, List[QuoteColumn]]]:
         """获取 ASTSingleSelectStatement 节点的 LATERAL VIEW 子句中所有字段到引用字段对象列表的映射关系"""
         result = []
         for lateral_view_clause in select_statement.lateral_view_clauses:  # 遍历 LATERAL VIEW 子句中的所有字段
-            result.append((lateral_view_clause.alias.name,
-                           CurrentNodeUsedQuoteColumn.handle(lateral_view_clause.function)))
+            for name in lateral_view_clause.alias.names:
+                result.append((name, toolkit.CurrentNodeUsedQuoteColumn.handle(lateral_view_clause.function)))
         return result
```

### Comparing `metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/table_lineage_storage.py` & `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/table_lineage_storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
 表数据血缘分析器
 """
 
 from typing import Dict
 
-from metasequoia_sql.analyzer.data_linage.node import StandardTable
-from metasequoia_sql.analyzer.data_linage.table_lineage import TableLineage
+from metasequoia_sql.analyzer.node import StandardTable
+from metasequoia_sql.analyzer.data_linage.table_lineage import SelectTableLineage
 from metasequoia_sql.analyzer.tool import CreateTableStatementGetter
 
 __all__ = ["TableLineageStorage"]
 
 
 class TableLineageStorage:
     """表数据血缘存储器"""
 
     def __init__(self, create_table_statement_getter: CreateTableStatementGetter):
-        self._with_table: Dict[str, TableLineage] = {}  # WITH 语句生成的临时表
-        self._sub_query_table: Dict[str, TableLineage] = {}  # 子查询生成的临时表
+        self._with_table: Dict[str, SelectTableLineage] = {}  # WITH 语句生成的临时表
+        self._sub_query_table: Dict[str, SelectTableLineage] = {}  # 子查询生成的临时表
         self._create_table_statement_getter = create_table_statement_getter  # 建表语句查询器
 
-    def add_with_table(self, table_name: str, table_lineage: TableLineage):
+    def add_with_table(self, table_name: str, table_lineage: SelectTableLineage):
         """添加一个临时表"""
         self._with_table[table_name] = table_lineage
 
-    def add_sub_query_table(self, table_name: str, table_lineage: TableLineage):
+    def add_sub_query_table(self, table_name: str, table_lineage: SelectTableLineage):
         """添加一个子查询表"""
         self._sub_query_table[table_name] = table_lineage
 
     def clear_sub_query_table(self):
         """清空子查询表"""
         self._sub_query_table = {}
 
     def get_table_lineage(self, table: StandardTable):
         """获取表数据血缘对象：优先在 WITH 语句的临时表中查询，如果查询不到则查询建表语句构造"""
         if table.table_name in self._sub_query_table:
             return self._sub_query_table[table.table_name]
         if table.table_name in self._with_table:
             return self._with_table[table.table_name]
         create_table_statement = self._create_table_statement_getter.get_statement(table.source())
-        return TableLineage.by_create_table_statement(create_table_statement)
+        return SelectTableLineage.by_create_table_statement(create_table_statement)
```

### Comparing `metasequoia-sql-0.4.0/metasequoia_sql/analyzer/toolkit/current_level_sub_query.py` & `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_sub_query.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-表名规范化器
+当前层级子查询分析器
 """
 
 from typing import Dict, List
 
 from metasequoia_sql import core
 from metasequoia_sql.analyzer.base import AnalyzerRecursionASTToDictBase
 
@@ -23,13 +23,13 @@
     def get_sub_query_statement(self, alias_name: str) -> core.ASTSelectStatement:
         """获取指定别名的子查询的 SELECT 语句"""
         return self._alias_hash[alias_name]
 
     @classmethod
     def handle(cls, node: object) -> Dict[str, core.ASTSelectStatement]:
         """TODO 待支持不包含别名的子查询"""
-        if (isinstance(node, core.ASTTableExpression)
-                and node.alias is not None and isinstance(node.table, core.ASTSubQueryExpression)):
-            return {node.alias.name: node.table.select_statement}
-        if isinstance(node, core.ASTSubQueryExpression) or isinstance(node, core.ASTWithClause):
+        if (isinstance(node, core.ASTFromTableExpression)
+                and node.alias is not None and isinstance(node.name, core.ASTSubQueryExpression)):
+            return {node.alias.name: node.name.statement}
+        if isinstance(node, (core.ASTSubQueryExpression, core.ASTWithClause)):
             return {}
         return cls.default_handle_node(node)
```

### Comparing `metasequoia-sql-0.4.0/metasequoia_sql/analyzer/toolkit/current_level_table_name_analyzer.py` & `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_table_name_analyzer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
-表名规范化器
+当前层级表明相关分析器
 """
 
 from typing import Dict, Optional, List
 
 from metasequoia_sql import core
 from metasequoia_sql.analyzer.base import AnalyzerRecursionASTToDictBase
-from metasequoia_sql.analyzer.data_linage.node import StandardTable
+from metasequoia_sql.analyzer.node import StandardTable
+
+
+__all__ = ["CurrentLevelTableNameAnalyzer"]
 
 
 class CurrentLevelTableNameAnalyzer(AnalyzerRecursionASTToDictBase):
     """表名规分析器"""
 
     def __init__(self, select_statement: core.ASTSelectStatement):
         self._alias_name_to_standard_table_hash = self.handle(select_statement)
@@ -25,22 +28,23 @@
 
     def get_all_standard_table(self) -> List[StandardTable]:
         """获取所有的标准表对象"""
         return list(self._alias_name_to_standard_table_hash.values())
 
     @classmethod
     def handle(cls, node: object) -> Dict[str, StandardTable]:
-        if isinstance(node, core.ASTTableExpression):
-            if isinstance(node.table, core.ASTTableNameExpression):
-                alias_name = node.alias.name if node.alias is not None else node.table.table
-                standard_table = StandardTable(schema_name=node.table.schema, table_name=node.table.table)
+        """TODO 待支持无别名子查询"""
+        if isinstance(node, core.ASTFromTableExpression):
+            if isinstance(node.name, core.ASTTableName):
+                alias_name = node.alias.name if node.alias is not None else node.name.table_name
+                standard_table = StandardTable(schema_name=node.name.schema_name, table_name=node.name.table_name)
                 return {alias_name: standard_table}
-            if isinstance(node.table, core.ASTSubQueryExpression):
-                alias_name = node.alias.name  # TODO 待支持无别名子查询
+            if isinstance(node.name, core.ASTSubQueryExpression):
+                alias_name = node.alias.name  #
                 standard_table = StandardTable(schema_name=None, table_name=alias_name)  # 待增加中间表标记
                 return {alias_name: standard_table}
-        if isinstance(node, core.ASTSubQueryExpression) or isinstance(node, core.ASTWithClause):
+        if isinstance(node, (core.ASTSubQueryExpression, core.ASTWithClause)):
             return {}
         return cls.default_handle_node(node)
 
     def __repr__(self):
         return ", ".join([f"{key}>{value}" for key, value in self._alias_name_to_standard_table_hash.items()])
```

### Comparing `metasequoia-sql-0.4.0/metasequoia_sql/common/token_scanner.py` & `metasequoia-sql-0.5.0/metasequoia_sql/common/scanner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 抽象语法树扫描器
 """
 
-from typing import List, Union
+from typing import List, Union, Optional
 
-from metasequoia_sql.lexical import AMTBase, AMTMark
-from metasequoia_sql.common.base_scanner import BaseScanner
 from metasequoia_sql.errors import ScannerError
+from metasequoia_sql.lexical import AMTBase, AMTMark
+
+__all__ = ["TokenScanner"]
 
 
-class TokenScanner(BaseScanner):
-    """Token 扫描器"""
+class TokenScanner:
+    """抽象词法树节点扫描器"""
 
     def __init__(self, elements: List[AMTBase],
                  pos: int = 0,
                  ignore_space: bool = False,
                  ignore_comment: bool = False):
         """
 
@@ -33,15 +34,71 @@
                     filtered_elements.append(element)
             elif element.equals(AMTMark.COMMENT):
                 if ignore_comment is False:  # 关闭忽略注释的模式
                     filtered_elements.append(element)
             else:
                 filtered_elements.append(element)
 
-        super().__init__(filtered_elements, pos)
+        if pos < 0:
+            raise ScannerError(f"初始化的指针小于 0: pos={pos}")
+        if pos > len(elements):
+            raise ScannerError(f"初始化指针大于字符串长度: len(text)={len(elements)}, pos={pos}")
+
+        self._elements = filtered_elements
+        self._pos = pos
+        self._len = len(filtered_elements)
+
+    @property
+    def elements(self) -> List[AMTBase]:
+        """返回扫描器中的所有元素"""
+        return self._elements
+
+    @property
+    def pos(self) -> int:
+        """返回当前扫描指针"""
+        return self._pos
+
+    def get(self) -> Optional[AMTBase]:
+        """获取当前指针位置元素，但不移动指针
+
+        - 如果指针已到达字符串末尾，则返回 None
+        - 如果指针超出字符串长度，则抛出异常
+        """
+        if self.pos > self._len:
+            raise ScannerError(f"要获取的指针大于等于字符串长度: len={self._len}, pos={self.pos}")
+        if self.pos == self._len:
+            return None
+        return self._elements[self._pos]
+
+    def pop(self) -> AMTBase:
+        """获取当前指针位置元素，并移动指针
+
+        - 如果要移动到的指针位置超出字符串长度，则抛出异常
+        """
+        if self.pos >= self._len:
+            raise ScannerError(f"要移动到的指针下标大于字符串长度: len={self._len}, pos={self.pos + 1} {self}")
+
+        result = self._elements[self.pos]
+        self._pos += 1  # 移动指针
+        return result
+
+    def _get_by_offset(self, idx: int) -> Optional[AMTBase]:
+        """获取当前指针位置 + idx 位置的元素，但不一定指针
+        """
+        if self.pos + idx >= self._len or self.pos + idx < 0:
+            return None
+        return self._elements[self.pos + idx]
+
+    def close(self) -> None:
+        """关闭扫描器，如果扫描器没有遍历完成则抛出异常"""
+        if not self.is_finish:
+            raise ScannerError(f"关闭了没有遍历完成的扫描器 {self}")
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__} tokens={self.elements[self.pos:]}, pos={self.pos}>"
 
     def search(self, *tokens: Union[str, AMTMark]) -> bool:
         """从当前配置开始匹配 tokens
 
         - 如果匹配成功，则返回 True
         - 如果匹配失败，则返回 False
         """
@@ -69,37 +126,37 @@
         """从当前配置开始匹配 tokens
 
         - 如果匹配成功，则将指针移动到 tokens 后的下一个元素
         - 如果匹配失败，则抛出异常
         """
         for word in tokens:
             if not self.pop().equals(word):
-                raise ScannerError(f"没有解析到目标词语:{self._elements}, 目标词={tokens}")
+                raise ScannerError(f"没有解析到目标词语:目标词={tokens} - {self}")
 
     def get_as_source(self) -> str:
-        """将指针向后移动 1 个元素并返回当前元素的 source"""
-        return self.now.source
+        """不移动指针，并返回当前元素的 source"""
+        return self.get().source
 
     def pop_as_source(self) -> str:
-        """将指针向后移动 1 个元素并返回当前元素的 source"""
+        """将指针向后移动 1 个元素，并返回当前元素的 source"""
         return self.pop().source
 
     def get_as_children_scanner(self, ignore_space: bool = True, ignore_comment: bool = True) -> "TokenScanner":
-        """【不移动指针】返回当前指针位置的插入语节点的子节点的扫描器"""
-        return TokenScanner(self.now.children(), ignore_space=ignore_space, ignore_comment=ignore_comment)
+        """不移动指针，并返回当前指针位置的插入语节点的子节点的扫描器"""
+        return TokenScanner(self.get().children(), ignore_space=ignore_space, ignore_comment=ignore_comment)
 
     def pop_as_children_scanner(self, ignore_space: bool = True, ignore_comment: bool = True) -> "TokenScanner":
-        """【移动指针】返回当前指针位置的插入语节点的子节点的扫描器"""
+        """将指针向后移动 1 个元素，并返回当前指针位置的插入语节点的子节点的扫描器"""
         return TokenScanner(self.pop().children(), ignore_space=ignore_space, ignore_comment=ignore_comment)
 
     def split_by(self,
                  source: str,
                  ignore_space: bool = True,
                  ignore_comment: bool = True) -> List["TokenScanner"]:
-        """【移动指针（到末尾）】将后续元素拆分为使用 source 分隔的扫描器列表"""
+        """将指针移动到末尾，并将后续元素拆分为使用 source 分隔的扫描器列表"""
         result = []
         tokens = []
         while not self.is_finish:
             token: AMTBase = self.pop()
             if token.equals(source):
                 if len(tokens) > 0:
                     result.append(TokenScanner(tokens, ignore_space=ignore_space, ignore_comment=ignore_comment))
@@ -110,15 +167,15 @@
             result.append(TokenScanner(tokens, ignore_space=ignore_space, ignore_comment=ignore_comment))
         return result
 
     def pop_as_children_scanner_list_split_by(self,
                                               source: str,
                                               ignore_space: bool = True,
                                               ignore_comment: bool = True) -> List["TokenScanner"]:
-        """【移动指针】返回当前指针位置的插入语结点的子节点使用 source 分隔的扫描器列表"""
+        """将指针向后移动一个元素，并返回当前指针位置的插入语结点的子节点使用 source 分隔的扫描器列表"""
         result = []
         tokens = []
         for token in self.pop().children():
             if token.equals(source):
                 if len(tokens) > 0:
                     result.append(TokenScanner(tokens, ignore_space=ignore_space, ignore_comment=ignore_comment))
                     tokens = []
@@ -127,8 +184,8 @@
         if len(tokens) > 0:
             result.append(TokenScanner(tokens, ignore_space=ignore_space, ignore_comment=ignore_comment))
         return result
 
     @property
     def is_finish(self) -> bool:
         """返回是否已匹配结束"""
-        return not self._pos < self._len
+        return self._pos >= self._len
```

### Comparing `metasequoia-sql-0.4.0/metasequoia_sql/common/unsed_static.py` & `metasequoia-sql-0.5.0/metasequoia_sql/common/static.py`

 * *Files 27% similar despite different names*

```diff
@@ -58,7 +58,49 @@
     "TIME": (0, 0),  # 格式为 HH:MM:SS
     "YEAR": (0, 0),  # 用两位数字表示，范围是 70（1970年）~ 69（2069年）；用四位数字表示，范围是 1901 年 ~ 2155 年
     "TINYBLOB": (0, 1),  # 二进制数据类型，最大长度为 255 字节
     "BLOB": (0, 1),  # 二进制数据类型，最大长度为 64KB
     "MEDIUMBLOB": (0, 1),  # 二进制数据类型，最大长度为 16MB
     "LONGBLOB": (0, 1),  # 二进制数据类型，最大长度为 4GB
 }
+
+# 将每个 Mysql 类型转换为 Hive 类型
+HASHMAP_MYSQL_TO_HIVE = {
+    # 串数据类型
+    "CHAR": "STRING",
+    "VARCHAR": "STRING",
+    "ENUM": "STRING",
+    "SET": "STRING",
+    "TINYTEXT": "STRING",
+    "TEXT": "STRING",
+    "MEDIUMTEXT": "STRING",
+    "LONGTEXT": "STRING",
+    "JSON": "STRING",
+    # 数值数据类型
+    "BIT": "TINYINT",
+    "BOOLEAN": "TINYINT",
+    "BOOL": "TINYINT",
+    "TINYINT": "TINYINT",
+    "SMALLINT": "SMALLINT",
+    "MEDIUMINT": "BIGINT",
+    "BIGINT": "BIGINT",
+    "INT": "INT",
+    "INTEGER": "INT",
+    "FLOAT": "FLOAT",
+    "REAL": "FLOAT",
+    "DOUBLE": "DOUBLE",
+    "DECIMAL": "DECIMAL",
+    "DEC": "DECIMAL",
+    # 日期和时间数据类型
+    "DATE": "STRING",
+    "TIME": "STRING",
+    "DATETIME": "STRING",
+    "TIMESTAMP": "STRING",
+    "YEAR": "INT",
+    # 二进制数据类型
+    "BLOB": "STRING",
+    "MEDIUMBLOB": "STRING",
+    "LONGBLOB": "STRING",
+    "TINYBLOB": "STRING",
+    "BINARY": "STRING",
+    "VARBINARY": "STRING"
+}
```

### Comparing `metasequoia-sql-0.4.0/metasequoia_sql/errors.py` & `metasequoia-sql-0.5.0/metasequoia_sql/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 在 metasequoia_sql 中年可能抛出的异常
 """
 
-__all__ = ["SqlParseError", "AMTParseError", "UnSupportDataSourceError", "ScannerError", "AnalyzerError"]
+__all__ = ["SqlParseError", "AMTParseError", "UnSupportSqlTypeError", "ScannerError", "AnalyzerError"]
 
 
 class SqlParseError(Exception):
     """SQL解析失败的异常"""
 
     def __init__(self, reason: str):
         self.reason = reason
 
 
 class AMTParseError(SqlParseError):
     """抽象词法树 AMT 解析失败"""
 
 
-class UnSupportDataSourceError(Exception):
+class UnSupportSqlTypeError(Exception):
     """数据源不支持的语法异常"""
 
     def __init__(self, reason: str):
         self.reason = reason
 
 
 class ScannerError(Exception):
```

### Comparing `metasequoia-sql-0.4.0/metasequoia_sql/plugins/mybaitis.py` & `metasequoia-sql-0.5.0/metasequoia_sql/plugins/mybaitis.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,146 +7,137 @@
 
 重写句法分析逻辑：
 1. 增加 MyBatis 元素节点作为一般表达式的子类（SQLMyBatisExpression）
 2. 继承并重写解析器以支持 MyBatis 元素解析（SQLParserMyBatis）
 """
 
 import dataclasses
-import enum
-from typing import Union, List, Optional, Any
+from typing import Union, List
 
 from metasequoia_sql import SQLType, ASTBase
-from metasequoia_sql.analyzer import AnalyzerRecursionListBase, CurrentUsedQuoteColumn
-from metasequoia_sql.lexical import ASTParser, AstParseStatus, AMTBaseSingle, AMTMark
+from metasequoia_sql.analyzer import AnalyzerRecursionASTToListBase, CurrentUsedQuoteColumn
 from metasequoia_sql.common import TokenScanner
-from metasequoia_sql.core import SQLParser, ASTGeneralExpression, ASTSingleSelectStatement
+from metasequoia_sql.core import SQLParser, ASTExpressionBase, ASTSingleSelectStatement
+from metasequoia_sql.errors import AMTParseError
+from metasequoia_sql.lexical import FSMMachine, FSMStatus, AMTSingle, AMTMark
 
 
-class ASTParseStatusMyBatis(enum.Enum):
-    """新增的 MyBaits 匹配状态"""
-    IN_MYBATIS = enum.auto()
-
-
-class ASTParserMyBatis(ASTParser):
+class FSMMachineMyBatis(FSMMachine):
     """继承并重写支持 MaBatis 语法的状态机处理方法"""
 
-    def handle_change(self):
+    def handle(self, ch: str) -> bool:
         """处理单个变化"""
-        # 进入 MyBatis 匹配状态
-        if self.status == AstParseStatus.WAIT_TOKEN and self.scanner.now == "#" and self.scanner.next1 == "{":
-            self.set_status(ASTParseStatusMyBatis.IN_MYBATIS)
-            self.cache_add()
-            self.cache_add()
-            return
-
-        # 处理 MyBatis 匹配状态
-        if self.status == ASTParseStatusMyBatis.IN_MYBATIS:
-            if self.scanner.now == "}":
-                self.cache_add_and_handle_end_word()
-                self.set_status(AstParseStatus.WAIT_TOKEN)
+        if self.status == FSMStatus.WAIT and ch == "#":
+            self.cache.append(ch)
+            self.status = FSMStatus.CUSTOM_1
+            return True
+        if self.status == FSMStatus.CUSTOM_1:  # 在 # 之后
+            if ch == "{":
+                self.cache.append(ch)
+                self.status = FSMStatus.CUSTOM_2
+                need_move = True
+            elif ch == "<END>":
+                self.stack[-1].append(AMTSingle(self._cache_get_and_reset(), {AMTMark.NAME, AMTMark.COMMENT}))
+                need_move = False
             else:
-                self.cache_add()
-            return
-
-        super().handle_change()
-
-    def handle_end_word(self):
-        """处理词语"""
-        origin = self.cache_get()
-        if origin.startswith("#{") and origin.endswith("}"):
-            self.cache_reset()
-            self.stack[-1].append(AMTBaseSingle(origin, {AMTMark.NAME, AMTMark.CUSTOM}))
-            return
-        super().handle_end_word()
-
-    def handle_last(self):
-        """处理最后一个词语是 MyBatis 参数的情况"""
-        if self.status == ASTParseStatusMyBatis.IN_MYBATIS:
-            self.handle_end_word()
-            self.set_status(AstParseStatus.WAIT_TOKEN)
-            return
-        super().handle_last()
+                self.cache.append(ch)
+                self.status = FSMStatus.IN_EXPLAIN_1
+                need_move = True
+            return need_move
+        if self.status == FSMStatus.CUSTOM_2:  # MyBatis 匹配状态
+            if ch == "}":
+                self.cache.append(ch)
+                self.stack[-1].append(AMTSingle(self._cache_get_and_reset(), {AMTMark.NAME, AMTMark.CUSTOM_1}))
+                self.status = FSMStatus.WAIT
+            elif ch == "<END>":
+                raise AMTParseError(f"当前状态={self.status} 出现结束标记符")
+            else:
+                self.cache.append(ch)
+                self.status = FSMStatus.CUSTOM_2
+            return True
+        return super().handle(ch)
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class SQLMyBatisExpression(ASTGeneralExpression):
+class SQLMyBatisExpression(ASTExpressionBase):
     """增加 MyBatis 元素节点作为一般表达式的子类"""
 
     mybatis_source: str = dataclasses.field(kw_only=True)
 
-    def source(self, data_source: SQLType) -> str:
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         return self.mybatis_source
 
 
 class SQLParserMyBatis(SQLParser):
     """继承并重写解析器以支持 MyBatis 元素解析"""
 
     @classmethod
     def build_token_scanner(cls, string: str) -> TokenScanner:
         """构造词法扫描器"""
-        context_automaton = ASTParserMyBatis(string)
-        context_automaton.parse()
-        return TokenScanner(context_automaton.result(), ignore_space=True, ignore_comment=True)
+        return TokenScanner(FSMMachineMyBatis.parse(string), ignore_space=True, ignore_comment=True)
 
     @classmethod
-    def parse_general_expression_element(cls, scanner_or_string: Union[TokenScanner, str],
-                                         maybe_window: bool) -> ASTGeneralExpression:
+    def parse_monomial_expression(cls, scanner_or_string: Union[TokenScanner, str],
+                                  maybe_window: bool,
+                                  sql_type: SQLType = SQLType.DEFAULT
+                                  ) -> ASTExpressionBase:
         """重写一般表达式元素解析逻辑"""
-        scanner = cls._unify_input_scanner(scanner_or_string)
-        if scanner.search(AMTMark.CUSTOM):
+        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        if scanner.search(AMTMark.CUSTOM_1):
             return SQLMyBatisExpression(mybatis_source=scanner.pop_as_source())
-        return super().parse_general_expression_element(scanner, maybe_window)
+        return super().parse_monomial_expression(scanner, maybe_window, sql_type=sql_type)
 
 
-class GetAllMybatisParams(AnalyzerRecursionListBase):
+class GetAllMybatisParams(AnalyzerRecursionASTToListBase):
     """获取使用的 MyBatis 参数"""
 
     @classmethod
-    def custom_handle_node(cls, node: ASTBase) -> Optional[List[Any]]:
+    def handle(cls, node: ASTBase) -> List[str]:
         """自定义的处理规则"""
         if isinstance(node, SQLMyBatisExpression):
-            return [node.source(SQLType.DEFAULT)[2:-1]]
-        return None
+            return [node.source()[2:-1]]
+        return cls.default_handle_node(node)
 
 
-class GetMybatisParamInWhereClause(AnalyzerRecursionListBase):
+class GetMybatisParamInWhereClause(AnalyzerRecursionASTToListBase):
     """获取 WHERE 子句中的 Mybatis 参数"""
 
     @classmethod
-    def custom_handle_node(cls, node: ASTBase) -> Optional[List[Any]]:
+    def handle(cls, node: ASTBase) -> List[str]:
         """自定义的处理规则"""
         if isinstance(node, SQLMyBatisExpression):
-            return [node.source(SQLType.DEFAULT)[2:-1]]
+            return [node.source()[2:-1]]
         if isinstance(node, ASTSingleSelectStatement):
-            return cls.handle_node(node.where_clause)
-        return None
+            return cls.handle(node.where_clause)
+        return cls.default_handle_node(node)
 
 
-class GetMybatisParamInGroupByClause(AnalyzerRecursionListBase):
+class GetMybatisParamInGroupByClause(AnalyzerRecursionASTToListBase):
     """获取 GROUP BY 子句中的 Mybatis 参数"""
 
     @classmethod
-    def custom_handle_node(cls, node: ASTBase) -> Optional[List[Any]]:
+    def handle(cls, node: ASTBase) -> List[str]:
         """自定义的处理规则"""
         if isinstance(node, SQLMyBatisExpression):
-            return [node.source(SQLType.DEFAULT)[2:-1]]
+            return [node.source()[2:-1]]
         if isinstance(node, ASTSingleSelectStatement):
-            return cls.handle_node(node.group_by_clause)
-        return None
+            return cls.handle(node.group_by_clause)
+        return cls.default_handle_node(node)
 
 
 if __name__ == "__main__":
     def test_main():
         """测试主逻辑"""
         test_sql = "SELECT shohin_mei FROM Shohin WHERE #{hanbai_tanka} > 500 GROUP BY #{tanka};"
 
         statements = SQLParserMyBatis.parse_statements(test_sql)
         for statement in statements:
-            print(statement)
-            print(statement.source(SQLType.MYSQL))
-            print(CurrentUsedQuoteColumn.handle(statement))
-            print(GetAllMybatisParams().handle(statement))
-            print(GetMybatisParamInWhereClause().handle(statement))
-            print(GetMybatisParamInGroupByClause().handle(statement))
+            if isinstance(statement, ASTSingleSelectStatement):
+                print(statement)
+                print(statement.source(SQLType.MYSQL))
+                print(CurrentUsedQuoteColumn.handle(statement))
+                print(GetAllMybatisParams().handle(statement))
+                print(GetMybatisParamInWhereClause().handle(statement))
+                print(GetMybatisParamInGroupByClause().handle(statement))
 
 
     test_main()
```

### Comparing `metasequoia-sql-0.4.0/metasequoia_sql.egg-info/SOURCES.txt` & `metasequoia-sql-0.5.0/metasequoia_sql.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 LICENSE
 README.md
 setup.py
 metasequoia_sql/__init__.py
 metasequoia_sql/errors.py
-metasequoia_sql/static.py
 metasequoia_sql.egg-info/PKG-INFO
 metasequoia_sql.egg-info/SOURCES.txt
 metasequoia_sql.egg-info/dependency_links.txt
 metasequoia_sql.egg-info/top_level.txt
 metasequoia_sql/analyzer/__init__.py
-metasequoia_sql/analyzer/all_level_common_table.py
 metasequoia_sql/analyzer/base.py
-metasequoia_sql/analyzer/current_level_common_column.py
-metasequoia_sql/analyzer/current_level_common_table.py
-metasequoia_sql/analyzer/data_lineage_analyzer_by_meta.py
+metasequoia_sql/analyzer/node.py
 metasequoia_sql/analyzer/tool.py
 metasequoia_sql/analyzer/data_linage/__init__.py
-metasequoia_sql/analyzer/data_linage/node.py
 metasequoia_sql/analyzer/data_linage/table_lineage.py
 metasequoia_sql/analyzer/data_linage/table_lineage_analyzer.py
 metasequoia_sql/analyzer/data_linage/table_lineage_storage.py
 metasequoia_sql/analyzer/toolkit/__init__.py
+metasequoia_sql/analyzer/toolkit/all_level_standard_table.py
+metasequoia_sql/analyzer/toolkit/current_level_column_analyzer.py
 metasequoia_sql/analyzer/toolkit/current_level_sub_query.py
 metasequoia_sql/analyzer/toolkit/current_level_table_name_analyzer.py
 metasequoia_sql/analyzer/toolkit/current_level_used_quote_columns.py
 metasequoia_sql/common/__init__.py
-metasequoia_sql/common/base_scanner.py
 metasequoia_sql/common/basic.py
-metasequoia_sql/common/text_scanner.py
-metasequoia_sql/common/token_scanner.py
-metasequoia_sql/common/unsed_static.py
+metasequoia_sql/common/char_set.py
+metasequoia_sql/common/name_set.py
+metasequoia_sql/common/scanner.py
+metasequoia_sql/common/static.py
 metasequoia_sql/core/__init__.py
+metasequoia_sql/core/node.py
 metasequoia_sql/core/parser.py
-metasequoia_sql/core/static.py
-metasequoia_sql/core/node/__init__.py
-metasequoia_sql/core/node/abc_node.py
-metasequoia_sql/core/node/enum_node.py
-metasequoia_sql/core/node/objects.py
-metasequoia_sql/core/node/sql_type.py
+metasequoia_sql/core/sql_type.py
 metasequoia_sql/lexical/__init__.py
-metasequoia_sql/lexical/nodes.py
-metasequoia_sql/lexical/parser.py
-metasequoia_sql/lexical/static.py
+metasequoia_sql/lexical/amt_node.py
+metasequoia_sql/lexical/fsm_machine.py
+metasequoia_sql/lexical/fsm_operate.py
+metasequoia_sql/lexical/fsm_operation_map.py
+metasequoia_sql/lexical/fsm_status.py
 metasequoia_sql/plugins/__init__.py
 metasequoia_sql/plugins/mybaitis.py
```

### Comparing `metasequoia-sql-0.4.0/setup.py` & `metasequoia-sql-0.5.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="metasequoia-sql",
-    version="0.4.0",
-    description="SQL解析器：提供词法解析、句法解析以及配套的分析器、插件功能",
+    version="0.5.0",
+    description="SQL语法解析器，包含词法树解析、语法树解析和语法树分析功能。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="changxing",
     author_email="1278729001@qq.com",
     url="https://github.com/ChangxingJiang/metasequoia-sql",
     install_requires=[],
     license="MIT License",
```

