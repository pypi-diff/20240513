# Comparing `tmp/turntable_spoonbill-9.0.4.tar.gz` & `tmp/turntable_spoonbill-9.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turntable_spoonbill-9.0.4.tar", max compression
+gzip compressed data, was "turntable_spoonbill-9.0.5.tar", max compression
```

## Comparing `turntable_spoonbill-9.0.4.tar` & `turntable_spoonbill-9.0.5.tar`

### file list

```diff
@@ -1,1897 +1,1897 @@
--rw-r--r--   0        0        0    11346 2024-03-22 20:15:42.439351 turntable_spoonbill-9.0.4/LICENSE.txt
--rw-r--r--   0        0        0    11115 2024-03-22 20:15:42.439351 turntable_spoonbill-9.0.4/README.md
--rw-r--r--   0        0        0     4167 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/__init__.py
--rw-r--r--   0        0        0    39475 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/__init__.py
--rw-r--r--   0        0        0    43203 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/__init__.py
--rw-r--r--   0        0        0     6319 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/client.py
--rw-r--r--   0        0        0    27701 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/compiler.py
--rw-r--r--   0        0        0      466 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/converter.py
--rw-r--r--   0        0        0     2473 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/datatypes.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/__init__.py
--rw-r--r--   0        0        0    10849 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/__init__.py
--rw-r--r--   0        0        0     3206 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/conftest.py
--rw-r--r--   0        0        0      146 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/snapshots/test_client/test_cross_project_query/out.sql
--rw-r--r--   0        0        0      173 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/snapshots/test_client/test_multiple_project_queries/out.sql
--rw-r--r--   0        0        0      155 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/snapshots/test_client/test_multiple_project_queries_database_api/out.sql
--rw-r--r--   0        0        0      408 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/snapshots/test_client/test_subquery_scalar_params/out.sql
--rw-r--r--   0        0        0    13227 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/test_client.py
--rw-r--r--   0        0        0     6609 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/test_connect.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/udf/__init__.py
--rw-r--r--   0        0        0      389 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/udf/snapshots/test_udf_execute/test_udf_with_struct/out.sql
--rw-r--r--   0        0        0     4701 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/udf/test_udf_execute.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.555352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/__init__.py
--rw-r--r--   0        0        0      196 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_approx/filter-approx_median/out.sql
--rw-r--r--   0        0        0      166 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_approx/filter-approx_nunique/out.sql
--rw-r--r--   0        0        0      122 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_approx/no_filter-approx_median/out.sql
--rw-r--r--   0        0        0      120 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_approx/no_filter-approx_nunique/out.sql
--rw-r--r--   0        0        0       77 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_binary/out.sql
--rw-r--r--   0        0        0      143 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/filter-bit_and/out.sql
--rw-r--r--   0        0        0      141 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/filter-bit_or/out.sql
--rw-r--r--   0        0        0      143 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/filter-bit_xor/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/no_filter-bit_and/out.sql
--rw-r--r--   0        0        0       85 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/no_filter-bit_or/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/no_filter-bit_xor/out.sql
--rw-r--r--   0        0        0       98 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bool_reducers/mean/out.sql
--rw-r--r--   0        0        0       97 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bool_reducers/sum/out.sql
--rw-r--r--   0        0        0      253 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bool_reducers_where_conj/out.sql
--rw-r--r--   0        0        0      144 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bool_reducers_where_simple/out.sql
--rw-r--r--   0        0        0      249 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bucket/out.sql
--rw-r--r--   0        0        0      111 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_cast_float_to_int/out.sql
--rw-r--r--   0        0        0       55 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_compile_toplevel/out.sql
--rw-r--r--   0        0        0      130 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_cov/pop/out.sql
--rw-r--r--   0        0        0      131 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_cov/sample/out.sql
--rw-r--r--   0        0        0      106 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/date/index.sql
--rw-r--r--   0        0        0      107 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/date/name.sql
--rw-r--r--   0        0        0      136 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/datetime/index.sql
--rw-r--r--   0        0        0      137 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/datetime/name.sql
--rw-r--r--   0        0        0      106 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/string_date/index.sql
--rw-r--r--   0        0        0      107 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/string_date/name.sql
--rw-r--r--   0        0        0      136 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/string_timestamp/index.sql
--rw-r--r--   0        0        0      137 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/string_timestamp/name.sql
--rw-r--r--   0        0        0      136 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/timestamp/index.sql
--rw-r--r--   0        0        0      137 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/timestamp/name.sql
--rw-r--r--   0        0        0      106 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/timestamp_date/index.sql
--rw-r--r--   0        0        0      107 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/timestamp_date/name.sql
--rw-r--r--   0        0        0      130 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_divide_by_zero/floordiv/out.sql
--rw-r--r--   0        0        0      103 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_divide_by_zero/truediv/out.sql
--rw-r--r--   0        0        0       50 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_extract_temporal_from_timestamp/date/out.sql
--rw-r--r--   0        0        0       50 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_extract_temporal_from_timestamp/time/out.sql
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_azimuth/out.sql
--rw-r--r--   0        0        0       74 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/contains/out.sql
--rw-r--r--   0        0        0       75 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/covered_by/out.sql
--rw-r--r--   0        0        0       72 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/covers/out.sql
--rw-r--r--   0        0        0       78 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/d_within/out.sql
--rw-r--r--   0        0        0       76 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/difference/out.sql
--rw-r--r--   0        0        0       74 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/disjoint/out.sql
--rw-r--r--   0        0        0       74 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/distance/out.sql
--rw-r--r--   0        0        0       72 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/geo_equals/out.sql
--rw-r--r--   0        0        0       78 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/intersection/out.sql
--rw-r--r--   0        0        0       76 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/intersects/out.sql
--rw-r--r--   0        0        0       77 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/max_distance/out.sql
--rw-r--r--   0        0        0       73 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/touches/out.sql
--rw-r--r--   0        0        0       71 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/union/out.sql
--rw-r--r--   0        0        0       72 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/within/out.sql
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_minmax/x_max/out.sql
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_minmax/x_min/out.sql
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_minmax/y_max/out.sql
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_minmax/y_min/out.sql
--rw-r--r--   0        0        0       71 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_point/out.sql
--rw-r--r--   0        0        0       64 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_simplify/out.sql
--rw-r--r--   0        0        0       55 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/aread/out.sql
--rw-r--r--   0        0        0       59 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/as_binary/out.sql
--rw-r--r--   0        0        0       57 2024-03-22 20:15:42.559352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/as_text/out.sql
--rw-r--r--   0        0        0       62 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/buffer/out.sql
--rw-r--r--   0        0        0       59 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/centroid/out.sql
--rw-r--r--   0        0        0       59 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/end_point/out.sql
--rw-r--r--   0        0        0       63 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/geometry_type/out.sql
--rw-r--r--   0        0        0       57 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/length/out.sql
--rw-r--r--   0        0        0       60 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/npoints/out.sql
--rw-r--r--   0        0        0       60 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/perimeter/out.sql
--rw-r--r--   0        0        0       60 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/point_n/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/start_point/out.sql
--rw-r--r--   0        0        0       60 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary_union/out.sql
--rw-r--r--   0        0        0       50 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_xy/x/out.sql
--rw-r--r--   0        0        0       50 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_xy/y/out.sql
--rw-r--r--   0        0        0      107 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hash/binary/out.sql
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hash/string/out.sql
--rw-r--r--   0        0        0       69 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/md5-test-binary/out.sql
--rw-r--r--   0        0        0       37 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/md5-test-string/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha1-test-binary/out.sql
--rw-r--r--   0        0        0       29 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha1-test-string/out.sql
--rw-r--r--   0        0        0       64 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha256-test-binary/out.sql
--rw-r--r--   0        0        0       32 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha256-test-string/out.sql
--rw-r--r--   0        0        0       64 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha512-test-binary/out.sql
--rw-r--r--   0        0        0       32 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha512-test-string/out.sql
--rw-r--r--   0        0        0      404 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_identical_to/out.sql
--rw-r--r--   0        0        0       46 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_integer_to_timestamp/ms/out.sql
--rw-r--r--   0        0        0       78 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_integer_to_timestamp/ns/out.sql
--rw-r--r--   0        0        0       46 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_integer_to_timestamp/s/out.sql
--rw-r--r--   0        0        0       45 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_integer_to_timestamp/us/out.sql
--rw-r--r--   0        0        0       71 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_string/escape_ascii_sequences/out.sql
--rw-r--r--   0        0        0       31 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_string/escape_backslash/out.sql
--rw-r--r--   0        0        0       31 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_string/escape_quote/out.sql
--rw-r--r--   0        0        0       63 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_string/not_escape_special_characters/out.sql
--rw-r--r--   0        0        0       68 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/datetime/out.sql
--rw-r--r--   0        0        0       52 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/string_time/out.sql
--rw-r--r--   0        0        0       68 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/string_timestamp/out.sql
--rw-r--r--   0        0        0       52 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/time/out.sql
--rw-r--r--   0        0        0       68 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/timestamp/out.sql
--rw-r--r--   0        0        0       86 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/date/out.sql
--rw-r--r--   0        0        0      116 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/datetime/out.sql
--rw-r--r--   0        0        0       86 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/string_date/out.sql
--rw-r--r--   0        0        0      116 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/string_timestamp/out.sql
--rw-r--r--   0        0        0      116 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/timestamp/out.sql
--rw-r--r--   0        0        0       86 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/timestamp_date/out.sql
--rw-r--r--   0        0        0       46 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_now/out.sql
--rw-r--r--   0        0        0      417 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_projection_fusion_only_peeks_at_immediate_parent/out.sql
--rw-r--r--   0        0        0      443 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_range_window_function/prec_foll/out.sql
--rw-r--r--   0        0        0      451 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_range_window_function/prec_prec/out.sql
--rw-r--r--   0        0        0      122 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_set_operation/difference/out.sql
--rw-r--r--   0        0        0      125 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_set_operation/intersect/out.sql
--rw-r--r--   0        0        0      116 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_set_operation/union_all/out.sql
--rw-r--r--   0        0        0      121 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_set_operation/union_distinct/out.sql
--rw-r--r--   0        0        0      148 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_substring/out.sql
--rw-r--r--   0        0        0       60 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/day-date/out.sql
--rw-r--r--   0        0        0       65 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/day-timestamp/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/hour-time/out.sql
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/hour-timestamp/out.sql
--rw-r--r--   0        0        0       68 2024-03-22 20:15:42.563352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/micros-time/out.sql
--rw-r--r--   0        0        0       73 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/micros-timestamp/out.sql
--rw-r--r--   0        0        0       68 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/millis-time/out.sql
--rw-r--r--   0        0        0       73 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/millis-timestamp/out.sql
--rw-r--r--   0        0        0       63 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/minute-time/out.sql
--rw-r--r--   0        0        0       68 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/minute-timestamp/out.sql
--rw-r--r--   0        0        0       62 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/month-date/out.sql
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/month-timestamp/out.sql
--rw-r--r--   0        0        0       64 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/quarter-date/out.sql
--rw-r--r--   0        0        0       69 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/quarter-timestamp/out.sql
--rw-r--r--   0        0        0       63 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/second-time/out.sql
--rw-r--r--   0        0        0       68 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/second-timestamp/out.sql
--rw-r--r--   0        0        0       69 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/week-date/out.sql
--rw-r--r--   0        0        0       74 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/week-timestamp/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/year-date/out.sql
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/year-timestamp/out.sql
--rw-r--r--   0        0        0      141 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_to_timestamp_no_timezone/out.sql
--rw-r--r--   0        0        0      173 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_to_timestamp_timezone/out.sql
--rw-r--r--   0        0        0      448 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/days/out.sql
--rw-r--r--   0        0        0      420 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/five/out.sql
--rw-r--r--   0        0        0      450 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/hours/out.sql
--rw-r--r--   0        0        0      464 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/micros/out.sql
--rw-r--r--   0        0        0      454 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/minutes/out.sql
--rw-r--r--   0        0        0      416 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/nanos/out.sql
--rw-r--r--   0        0        0      454 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/seconds/out.sql
--rw-r--r--   0        0        0      485 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/two_days/out.sql
--rw-r--r--   0        0        0      450 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/week/out.sql
--rw-r--r--   0        0        0      237 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/years/out.sql
--rw-r--r--   0        0        0      397 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union/False/out.sql
--rw-r--r--   0        0        0      402 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union/True/out.sql
--rw-r--r--   0        0        0      476 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union_cte/False-False/out.sql
--rw-r--r--   0        0        0      481 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union_cte/False-True/out.sql
--rw-r--r--   0        0        0      481 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union_cte/True-False/out.sql
--rw-r--r--   0        0        0      486 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union_cte/True-True/out.sql
--rw-r--r--   0        0        0      490 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_unnest/out_one_unnest.sql
--rw-r--r--   0        0        0      905 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_unnest/out_two_unnests.sql
--rw-r--r--   0        0        0      444 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_function/current_foll/out.sql
--rw-r--r--   0        0        0      444 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_function/prec_current/out.sql
--rw-r--r--   0        0        0      444 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_function/prec_prec/out.sql
--rw-r--r--   0        0        0      104 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_unbounded/following/out.sql
--rw-r--r--   0        0        0      104 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_unbounded/preceding/out.sql
--rw-r--r--   0        0        0      955 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/test_client.py
--rw-r--r--   0        0        0    20048 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/test_compiler.py
--rw-r--r--   0        0        0     2954 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/test_datatypes.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/__init__.py
--rw-r--r--   0        0        0       58 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_builtin/test_bqutil_fn_from_hex/out.sql
--rw-r--r--   0        0        0      124 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_builtin/test_farm_fingerprint/out.sql
--rw-r--r--   0        0        0       76 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_assign/out.js
--rw-r--r--   0        0        0       42 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_binary_operators/add/out.js
--rw-r--r--   0        0        0       42 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_binary_operators/div/out.js
--rw-r--r--   0        0        0       42 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_binary_operators/mul/out.js
--rw-r--r--   0        0        0       42 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_binary_operators/sub/out.js
--rw-r--r--   0        0        0      178 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_class/out.js
--rw-r--r--   0        0        0      125 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_class_with_properties/out.js
--rw-r--r--   0        0        0      139 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_continue/out.js
--rw-r--r--   0        0        0      154 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_delete/out.js
--rw-r--r--   0        0        0       64 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_dict/out.js
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.567352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_floordiv/out.js
--rw-r--r--   0        0        0       40 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_function_def/out.js
--rw-r--r--   0        0        0      249 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_lambda_with_splat/out.js
--rw-r--r--   0        0        0       44 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_len_rewrite/out.js
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_list_comp/out.js
--rw-r--r--   0        0        0       80 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_logical_not/out.js
--rw-r--r--   0        0        0       56 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_missing_vararg/out.js
--rw-r--r--   0        0        0       58 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_pow/out.js
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_scope_with_while/out.js
--rw-r--r--   0        0        0       85 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_set_to_object/out.js
--rw-r--r--   0        0        0       78 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_setitem/out.js
--rw-r--r--   0        0        0      134 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_splat/out.js
--rw-r--r--   0        0        0       49 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_str/out.js
--rw-r--r--   0        0        0      106 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_true_false_none/out.js
--rw-r--r--   0        0        0       59 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_tuple/out.js
--rw-r--r--   0        0        0       48 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_unary_minus/out.js
--rw-r--r--   0        0        0       48 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_unary_plus/out.js
--rw-r--r--   0        0        0       48 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_varargs/out.js
--rw-r--r--   0        0        0       51 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_variable_declaration/out.js
--rw-r--r--   0        0        0       40 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_yield/out.js
--rw-r--r--   0        0        0       40 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_yield_from/out.js
--rw-r--r--   0        0        0      798 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/test_builtin.py
--rw-r--r--   0        0        0     6533 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/test_core.py
--rw-r--r--   0        0        0     2002 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/test_find.py
--rw-r--r--   0        0        0     1926 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/test_usage.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/udf/__init__.py
--rw-r--r--   0        0        0    17057 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/udf/core.py
--rw-r--r--   0        0        0     1599 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/udf/find.py
--rw-r--r--   0        0        0     1255 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/bigquery/udf/rewrite.py
--rw-r--r--   0        0        0    24527 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/__init__.py
--rw-r--r--   0        0        0    22408 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/compiler.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/__init__.py
--rw-r--r--   0        0        0     3415 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/conftest.py
--rw-r--r--   0        0        0      139 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/count/out.sql
--rw-r--r--   0        0        0      135 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/max/out.sql
--rw-r--r--   0        0        0      136 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/mean/out.sql
--rw-r--r--   0        0        0      135 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/min/out.sql
--rw-r--r--   0        0        0      150 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/std/out.sql
--rw-r--r--   0        0        0      135 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/sum/out.sql
--rw-r--r--   0        0        0      144 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/var/out.sql
--rw-r--r--   0        0        0      149 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_std_var_pop/std/out.sql
--rw-r--r--   0        0        0      143 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_std_var_pop/var/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/float/out.sql
--rw-r--r--   0        0        0      119 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/float32/out.sql
--rw-r--r--   0        0        0      110 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/float64/out.sql
--rw-r--r--   0        0        0      115 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/int16/out.sql
--rw-r--r--   0        0        0      113 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/int8/out.sql
--rw-r--r--   0        0        0      113 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/date/out.sql
--rw-r--r--   0        0        0      115 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/int16/out.sql
--rw-r--r--   0        0        0      113 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/int8/out.sql
--rw-r--r--   0        0        0      142 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/mapstring_int64/out.sql
--rw-r--r--   0        0        0      108 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/string/out.sql
--rw-r--r--   0        0        0      167 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/structa_string_b_int64/out.sql
--rw-r--r--   0        0        0      122 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/timestamp/out.sql
--rw-r--r--   0        0        0      317 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_column_regexp_extract/out.sql
--rw-r--r--   0        0        0      142 2024-03-22 20:15:42.571352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_column_regexp_replace/out.sql
--rw-r--r--   0        0        0       88 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_greatest_least/out1.sql
--rw-r--r--   0        0        0      103 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_greatest_least/out2.sql
--rw-r--r--   0        0        0       82 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_greatest_least/out3.sql
--rw-r--r--   0        0        0       97 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_greatest_least/out4.sql
--rw-r--r--   0        0        0      211 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_group_concat/comma_none/out.sql
--rw-r--r--   0        0        0      278 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_group_concat/comma_zero/out.sql
--rw-r--r--   0        0        0      211 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_group_concat/minus_none/out.sql
--rw-r--r--   0        0        0       94 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_hash/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/bigint_col/out.sql
--rw-r--r--   0        0        0       59 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/bool_col/out.sql
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/date_string_col/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/double_col/out.sql
--rw-r--r--   0        0        0       60 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/float_col/out.sql
--rw-r--r--   0        0        0       53 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/id/out.sql
--rw-r--r--   0        0        0        5 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/index/out.sql
--rw-r--r--   0        0        0       58 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/int_col/out.sql
--rw-r--r--   0        0        0       56 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/month/out.sql
--rw-r--r--   0        0        0       63 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/smallint_col/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/string_col/out.sql
--rw-r--r--   0        0        0       64 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/timestamp_col/out.sql
--rw-r--r--   0        0        0       62 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/tinyint_col/out.sql
--rw-r--r--   0        0        0       55 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/year/out.sql
--rw-r--r--   0        0        0      111 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_find/out1.sql
--rw-r--r--   0        0        0      132 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_find/out2.sql
--rw-r--r--   0        0        0      118 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_find_in_set/out.sql
--rw-r--r--   0        0        0      112 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_like/out1.sql
--rw-r--r--   0        0        0      184 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_like/out2.sql
--rw-r--r--   0        0        0      218 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_substring/out1.sql
--rw-r--r--   0        0        0      227 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_substring/out2.sql
--rw-r--r--   0        0        0      119 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_cast/out1.sql
--rw-r--r--   0        0        0      107 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_cast/out2.sql
--rw-r--r--   0        0        0      110 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_from_integer/out.sql
--rw-r--r--   0        0        0       34 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_now/out.sql
--rw-r--r--   0        0        0      135 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/d/out.sql
--rw-r--r--   0        0        0      143 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/h/out.sql
--rw-r--r--   0        0        0      147 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/m/out.sql
--rw-r--r--   0        0        0      147 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/minute/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/w/out.sql
--rw-r--r--   0        0        0      143 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/y/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/abs/out.sql
--rw-r--r--   0        0        0      114 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/ceil/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/exp/out.sql
--rw-r--r--   0        0        0       86 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/log/out.sql
--rw-r--r--   0        0        0       91 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/log10/out.sql
--rw-r--r--   0        0        0       89 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/log2/out.sql
--rw-r--r--   0        0        0       91 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/round/out.sql
--rw-r--r--   0        0        0       97 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/round_0/out.sql
--rw-r--r--   0        0        0       97 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/round_2/out.sql
--rw-r--r--   0        0        0      121 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/sign/out.sql
--rw-r--r--   0        0        0       89 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/sqrt/out.sql
--rw-r--r--   0        0        0      122 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_fine_grained_timestamp_literals/micros/out.sql
--rw-r--r--   0        0        0      151 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_fine_grained_timestamp_literals/micros_tz/out.sql
--rw-r--r--   0        0        0      122 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_fine_grained_timestamp_literals/millis/out.sql
--rw-r--r--   0        0        0      151 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_fine_grained_timestamp_literals/millis_tz/out.sql
--rw-r--r--   0        0        0       10 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_literals/nested_quote/out.sql
--rw-r--r--   0        0        0       13 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_literals/nested_token/out.sql
--rw-r--r--   0        0        0        8 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_literals/simple/out.sql
--rw-r--r--   0        0        0       25 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/false/out.sql
--rw-r--r--   0        0        0       21 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/float/out.sql
--rw-r--r--   0        0        0       17 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/int/out.sql
--rw-r--r--   0        0        0       36 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/nested_quote/out.sql
--rw-r--r--   0        0        0       43 2024-03-22 20:15:42.575352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/nested_token/out.sql
--rw-r--r--   0        0        0       31 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/simple/out.sql
--rw-r--r--   0        0        0       23 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/true/out.sql
--rw-r--r--   0        0        0      102 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_timestamp_literals/expr0/out.sql
--rw-r--r--   0        0        0      102 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_timestamp_literals/expr1/out.sql
--rw-r--r--   0        0        0      102 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_literals/test_timestamp_literals/expr2/out.sql
--rw-r--r--   0        0        0      104 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_between/out.sql
--rw-r--r--   0        0        0      110 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/add/out.sql
--rw-r--r--   0        0        0      113 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/eq/out.sql
--rw-r--r--   0        0        0      120 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/ge/out.sql
--rw-r--r--   0        0        0      114 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/gt/out.sql
--rw-r--r--   0        0        0      117 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/le/out.sql
--rw-r--r--   0        0        0      111 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/lt/out.sql
--rw-r--r--   0        0        0      115 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/mul/out.sql
--rw-r--r--   0        0        0      117 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/ne/out.sql
--rw-r--r--   0        0        0      118 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/pow/out.sql
--rw-r--r--   0        0        0      115 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/sub/out.sql
--rw-r--r--   0        0        0      113 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/truediv/out.sql
--rw-r--r--   0        0        0      157 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_parenthesization/lambda0/out.sql
--rw-r--r--   0        0        0      117 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_parenthesization/lambda1/out.sql
--rw-r--r--   0        0        0      166 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_parenthesization/lambda2/out.sql
--rw-r--r--   0        0        0       92 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_negate/bool_col/out.sql
--rw-r--r--   0        0        0       94 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_negate/float_col/out.sql
--rw-r--r--   0        0        0       90 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_negate/int_col/out.sql
--rw-r--r--   0        0        0      198 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_search_case/out.sql
--rw-r--r--   0        0        0      168 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_operators/test_simple_case/out.sql
--rw-r--r--   0        0        0      136 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_array_join_in_subquery/out.sql
--rw-r--r--   0        0        0      227 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_complex_array_expr_projection/out.sql
--rw-r--r--   0        0        0      256 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_complex_join/out.sql
--rw-r--r--   0        0        0      150 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_count_name/out.sql
--rw-r--r--   0        0        0      177 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_ifelse_use_if/out.sql
--rw-r--r--   0        0        0      343 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_isin_notin_in_select/out1.sql
--rw-r--r--   0        0        0      357 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_isin_notin_in_select/out2.sql
--rw-r--r--   0        0        0      145 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_isnull_case_expr_rewrite_failure/out.sql
--rw-r--r--   0        0        0      367 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_join_self_reference/out.sql
--rw-r--r--   0        0        0      216 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_named_from_filter_groupby/out1.sql
--rw-r--r--   0        0        0      216 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_named_from_filter_groupby/out2.sql
--rw-r--r--   0        0        0       37 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_physical_table_reference_translate/out.sql
--rw-r--r--   0        0        0       29 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_scalar_exprs_no_table_refs/add/out.sql
--rw-r--r--   0        0        0       34 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_scalar_exprs_no_table_refs/now/out.sql
--rw-r--r--   0        0        0       45 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_self_reference_simple/out.sql
--rw-r--r--   0        0        0      409 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-awardID-any_inner_join/out.sql
--rw-r--r--   0        0        0      414 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-awardID-any_left_join/out.sql
--rw-r--r--   0        0        0      411 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-awardID-inner_join/out.sql
--rw-r--r--   0        0        0      416 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-awardID-left_join/out.sql
--rw-r--r--   0        0        0      410 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-playerID-any_inner_join/out.sql
--rw-r--r--   0        0        0      415 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-playerID-any_left_join/out.sql
--rw-r--r--   0        0        0      412 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-playerID-inner_join/out.sql
--rw-r--r--   0        0        0      417 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-playerID-left_join/out.sql
--rw-r--r--   0        0        0      428 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_scalar_aggregates/out.sql
--rw-r--r--   0        0        0      561 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_table_column_unbox/out.sql
--rw-r--r--   0        0        0      307 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_timestamp_extract_field/out.sql
--rw-r--r--   0        0        0      380 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_where_simple_comparisons/out.sql
--rw-r--r--   0        0        0      363 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_where_with_between/out.sql
--rw-r--r--   0        0        0      119 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_where_with_timestamp/out.sql
--rw-r--r--   0        0        0     5069 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_aggregations.py
--rw-r--r--   0        0        0     9060 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_client.py
--rw-r--r--   0        0        0     9902 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_datatypes.py
--rw-r--r--   0        0        0    14466 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_functions.py
--rw-r--r--   0        0        0     1931 2024-03-22 20:15:42.579352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_literals.py
--rw-r--r--   0        0        0     7328 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_operators.py
--rw-r--r--   0        0        0    11840 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_select.py
--rw-r--r--   0        0        0    21760 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/conftest.py
--rw-r--r--   0        0        0     6116 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/__init__.py
--rw-r--r--   0        0        0     3022 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/convert.py
--rw-r--r--   0        0        0    14114 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/executor.py
--rw-r--r--   0        0        0     6623 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/helpers.py
--rw-r--r--   0        0        0     1876 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/kernels.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/__init__.py
--rw-r--r--   0        0        0    11178 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/conftest.py
--rw-r--r--   0        0        0     5854 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_arrays.py
--rw-r--r--   0        0        0     5242 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_cast.py
--rw-r--r--   0        0        0     3483 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_client.py
--rw-r--r--   0        0        0     1049 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_core.py
--rw-r--r--   0        0        0     5782 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_functions.py
--rw-r--r--   0        0        0    12016 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_join.py
--rw-r--r--   0        0        0     2609 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_maps.py
--rw-r--r--   0        0        0    28046 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_operations.py
--rw-r--r--   0        0        0     3860 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_strings.py
--rw-r--r--   0        0        0     2548 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_structs.py
--rw-r--r--   0        0        0     6771 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_temporal.py
--rw-r--r--   0        0        0    10915 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_udf.py
--rw-r--r--   0        0        0    16722 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_window.py
--rw-r--r--   0        0        0    21597 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/datafusion/__init__.py
--rw-r--r--   0        0        0    17397 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/datafusion/compiler.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/__init__.py
--rw-r--r--   0        0        0     1303 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/conftest.py
--rw-r--r--   0        0        0     1091 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/test_connect.py
--rw-r--r--   0        0        0     1214 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/test_register.py
--rw-r--r--   0        0        0      799 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/test_select.py
--rw-r--r--   0        0        0      177 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/test_string.py
--rw-r--r--   0        0        0      760 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/test_temporal.py
--rw-r--r--   0        0        0     2060 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/test_udf.py
--rw-r--r--   0        0        0     3603 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/datafusion/udfs.py
--rw-r--r--   0        0        0     5602 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/druid/__init__.py
--rw-r--r--   0        0        0     6259 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/druid/compiler.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/druid/tests/__init__.py
--rw-r--r--   0        0        0     4793 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/druid/tests/conftest.py
--rw-r--r--   0        0        0    49168 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/__init__.py
--rw-r--r--   0        0        0    14608 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/compiler.py
--rw-r--r--   0        0        0      240 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/converter.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/__init__.py
--rw-r--r--   0        0        0     3987 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/conftest.py
--rw-r--r--   0        0        0       37 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_client/test_to_other_sql/out.sql
--rw-r--r--   0        0        0       54 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_to_floating_point_type/float32/out.sql
--rw-r--r--   0        0        0       56 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_to_floating_point_type/float64/out.sql
--rw-r--r--   0        0        0       74 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_uints/uint16/out.sql
--rw-r--r--   0        0        0       73 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_uints/uint32/out.sql
--rw-r--r--   0        0        0       72 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_uints/uint64/out.sql
--rw-r--r--   0        0        0       72 2024-03-22 20:15:42.583352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_uints/uint8/out.sql
--rw-r--r--   0        0        0       92 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_geospatial_dwithin/out.sql
--rw-r--r--   0        0        0       57 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_geospatial_unary_snapshot/as_text/out.sql
--rw-r--r--   0        0        0       58 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_geospatial_unary_snapshot/n_points/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr0/out.sql
--rw-r--r--   0        0        0       83 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr0-POINT_1_0/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr1/out.sql
--rw-r--r--   0        0        0      102 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp0-0_0/out.sql
--rw-r--r--   0        0        0      102 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp1-1_1/out.sql
--rw-r--r--   0        0        0      102 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp2-2_2/out.sql
--rw-r--r--   0        0        0      117 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp3-0_0_1_1_2_2/out.sql
--rw-r--r--   0        0        0      117 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp4-2_2_1_1_0_0/out.sql
--rw-r--r--   0        0        0      121 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp5-0_0_1_1_2_2_0_0/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp6-0_0_1_1_2_2_0_0/out.sql
--rw-r--r--   0        0        0      141 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp7-0_0_1_1_2_2_2_2_1_1_0_0/out.sql
--rw-r--r--   0        0        0      123 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp8-0_0_1_1_2_2/out.sql
--rw-r--r--   0        0        0     8259 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/test_client.py
--rw-r--r--   0        0        0     3612 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/test_datatypes.py
--rw-r--r--   0        0        0    11219 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/test_geospatial.py
--rw-r--r--   0        0        0    14798 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/test_register.py
--rw-r--r--   0        0        0     2171 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/test_udf.py
--rw-r--r--   0        0        0    14804 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/exasol/__init__.py
--rw-r--r--   0        0        0     6805 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/exasol/compiler.py
--rw-r--r--   0        0        0     1260 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/exasol/converter.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/exasol/tests/__init__.py
--rw-r--r--   0        0        0     3524 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/exasol/tests/conftest.py
--rw-r--r--   0        0        0    33390 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/__init__.py
--rw-r--r--   0        0        0    19772 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/compiler.py
--rw-r--r--   0        0        0     6885 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/datatypes.py
--rw-r--r--   0        0        0    10797 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/ddl.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/__init__.py
--rw-r--r--   0        0        0     5368 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/conftest.py
--rw-r--r--   0        0        0      237 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_complex_filtered_agg/out.sql
--rw-r--r--   0        0        0      246 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_complex_groupby_aggregation/out.sql
--rw-r--r--   0        0        0      220 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_complex_projections/out.sql
--rw-r--r--   0        0        0       92 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_count_star/out.sql
--rw-r--r--   0        0        0       65 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/day/out.sql
--rw-r--r--   0        0        0       58 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/day_of_year/out.sql
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/hour/out.sql
--rw-r--r--   0        0        0       68 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/minute/out.sql
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/month/out.sql
--rw-r--r--   0        0        0       69 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/quarter/out.sql
--rw-r--r--   0        0        0       68 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/second/out.sql
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/week_of_year/out.sql
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/year/out.sql
--rw-r--r--   0        0        0      260 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_filter/out.sql
--rw-r--r--   0        0        0      225 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_having/out.sql
--rw-r--r--   0        0        0      132 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_simple_filtered_agg/out.sql
--rw-r--r--   0        0        0       55 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_sum/out.sql
--rw-r--r--   0        0        0      117 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_timestamp_from_unix/timestamp_ms/out.sql
--rw-r--r--   0        0        0      112 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_timestamp_from_unix/timestamp_s/out.sql
--rw-r--r--   0        0        0      202 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_value_counts/out.sql
--rw-r--r--   0        0        0      275 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_window_aggregation/out.sql
--rw-r--r--   0        0        0      719 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_window_topn/out.sql
--rw-r--r--   0        0        0      129 2024-03-22 20:15:42.587352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_windowing_tvf/cumulate_window/out.sql
--rw-r--r--   0        0        0      124 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_windowing_tvf/hop_window/out.sql
--rw-r--r--   0        0        0       99 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_windowing_tvf/tumble_window/out.sql
--rw-r--r--   0        0        0      160 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_window/test_range_window/out.sql
--rw-r--r--   0        0        0      139 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_window/test_rows_window/out.sql
--rw-r--r--   0        0        0     4962 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/test_compiler.py
--rw-r--r--   0        0        0     1181 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/test_datatypes.py
--rw-r--r--   0        0        0    16229 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/test_ddl.py
--rw-r--r--   0        0        0     4795 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/test_join.py
--rw-r--r--   0        0        0      632 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/test_udf.py
--rw-r--r--   0        0        0     1975 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/flink/tests/test_window.py
--rw-r--r--   0        0        0    11772 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/flink/utils.py
--rw-r--r--   0        0        0    40475 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/__init__.py
--rw-r--r--   0        0        0    10149 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/client.py
--rw-r--r--   0        0        0    12545 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/compiler.py
--rw-r--r--   0        0        0    17678 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/ddl.py
--rw-r--r--   0        0        0     8596 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/metadata.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/__init__.py
--rw-r--r--   0        0        0     6735 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/conftest.py
--rw-r--r--   0        0        0      212 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/mocks.py
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/first/out.sql
--rw-r--r--   0        0        0      129 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lag_arg/out.sql
--rw-r--r--   0        0        0      123 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lag_default/out.sql
--rw-r--r--   0        0        0      132 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lag_explicit_default/out.sql
--rw-r--r--   0        0        0      136 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/last/out.sql
--rw-r--r--   0        0        0      131 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lead_arg/out.sql
--rw-r--r--   0        0        0      125 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lead_default/out.sql
--rw-r--r--   0        0        0      134 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lead_explicit_default/out.sql
--rw-r--r--   0        0        0      119 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/ntile/out.sql
--rw-r--r--   0        0        0      126 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/percent_rank/out.sql
--rw-r--r--   0        0        0      695 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_assign_labels/out.sql
--rw-r--r--   0        0        0      331 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/close_extreme_false/out.sql
--rw-r--r--   0        0        0      331 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/close_extreme_false_closed_right/out.sql
--rw-r--r--   0        0        0      399 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/close_extreme_false_include_under_include_over/out.sql
--rw-r--r--   0        0        0      332 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/closed_right/out.sql
--rw-r--r--   0        0        0      365 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/closed_right_close_extreme_false_include_under/out.sql
--rw-r--r--   0        0        0      158 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/closed_right_include_over_include_under/out.sql
--rw-r--r--   0        0        0      332 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/default/out.sql
--rw-r--r--   0        0        0      158 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_over_include_under0/out.sql
--rw-r--r--   0        0        0      184 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_over_include_under1/out.sql
--rw-r--r--   0        0        0      189 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_over_include_under2/out.sql
--rw-r--r--   0        0        0      365 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_under/out.sql
--rw-r--r--   0        0        0      399 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_under_include_over/out.sql
--rw-r--r--   0        0        0       89 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_case_exprs/test_decimal_fillna_cast_arg/fillna_l_extendedprice/out.sql
--rw-r--r--   0        0        0       91 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_case_exprs/test_decimal_fillna_cast_arg/fillna_l_extendedprice_double/out.sql
--rw-r--r--   0        0        0       84 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_case_exprs/test_decimal_fillna_cast_arg/fillna_l_quantity/out.sql
--rw-r--r--   0        0        0      110 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_case_exprs/test_identical_to/out.sql
--rw-r--r--   0        0        0       80 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_case_exprs/test_identical_to_special_case/out.sql
--rw-r--r--   0        0        0      102 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_case_exprs/test_ifelse_use_if/out.sql
--rw-r--r--   0        0        0       88 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_case_exprs/test_isnull_1_0/out1.sql
--rw-r--r--   0        0        0       98 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_case_exprs/test_isnull_1_0/out2.sql
--rw-r--r--   0        0        0      148 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_case_exprs/test_nullif_ifnull/nullif_boolean/out.sql
--rw-r--r--   0        0        0      118 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_case_exprs/test_nullif_ifnull/nullif_input/out.sql
--rw-r--r--   0        0        0      152 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_case_exprs/test_nullif_ifnull/nullif_negate_boolean/out.sql
--rw-r--r--   0        0        0      198 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_case_exprs/test_search_case/out.sql
--rw-r--r--   0        0        0      139 2024-03-22 20:15:42.591352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_case_exprs/test_simple_case/out.sql
--rw-r--r--   0        0        0      103 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/coalesce_columns/out.sql
--rw-r--r--   0        0        0       94 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/coalesce_scalar/out.sql
--rw-r--r--   0        0        0      103 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/greatest_columns/out.sql
--rw-r--r--   0        0        0       94 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/greatest_scalar/out.sql
--rw-r--r--   0        0        0       97 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/least_columns/out.sql
--rw-r--r--   0        0        0       88 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/least_scalar/out.sql
--rw-r--r--   0        0        0       50 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_add_partition/out.sql
--rw-r--r--   0        0        0       48 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_add_partition_string_key/out.sql
--rw-r--r--   0        0        0       80 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_add_partition_with_props/out.sql
--rw-r--r--   0        0        0       80 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_partition_properties/out1.sql
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_partition_properties/out2.sql
--rw-r--r--   0        0        0       93 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_partition_properties/out3.sql
--rw-r--r--   0        0        0       82 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_partition_properties/out4.sql
--rw-r--r--   0        0        0       80 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_table_properties/out1.sql
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_table_properties/out2.sql
--rw-r--r--   0        0        0       93 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_table_properties/out3.sql
--rw-r--r--   0        0        0       82 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_table_properties/out4.sql
--rw-r--r--   0        0        0       90 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_avro_other_formats/out.sql
--rw-r--r--   0        0        0       47 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_cache_table_pool_name/out1.sql
--rw-r--r--   0        0        0       47 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_cache_table_pool_name/out2.sql
--rw-r--r--   0        0        0      114 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_external_table_as/out.sql
--rw-r--r--   0        0        0      491 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_external_table_avro/out.sql
--rw-r--r--   0        0        0      241 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_delimited/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_like_parquet/out.sql
--rw-r--r--   0        0        0      382 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_parquet/out.sql
--rw-r--r--   0        0        0      106 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_parquet_like_other/out.sql
--rw-r--r--   0        0        0      140 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_parquet_with_schema/out.sql
--rw-r--r--   0        0        0      126 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_with_location_compile/out.sql
--rw-r--r--   0        0        0       51 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_drop_partition/out.sql
--rw-r--r--   0        0        0       22 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_drop_table_compile/out1.sql
--rw-r--r--   0        0        0       32 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_drop_table_compile/out2.sql
--rw-r--r--   0        0        0      102 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_load_data_partitioned/out1.sql
--rw-r--r--   0        0        0      112 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_load_data_partitioned/out2.sql
--rw-r--r--   0        0        0       71 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_load_data_unpartitioned/out1.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_load_data_unpartitioned/out2.sql
--rw-r--r--   0        0        0      385 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_no_overwrite/out.sql
--rw-r--r--   0        0        0       88 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_select_basics/out1.sql
--rw-r--r--   0        0        0       93 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_select_basics/out2.sql
--rw-r--r--   0        0        0      266 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_exprs/test_filter_with_analytic/out.sql
--rw-r--r--   0        0        0      207 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_exprs/test_named_from_filter_group_by/abc.sql
--rw-r--r--   0        0        0      207 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_exprs/test_named_from_filter_group_by/foo.sql
--rw-r--r--   0        0        0      134 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_exprs/test_nunique_where/out.sql
--rw-r--r--   0        0        0      117 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_exprs/test_where_with_timestamp/out.sql
--rw-r--r--   0        0        0       83 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_in_not_in/test_field_in_literals/isin/out.sql
--rw-r--r--   0        0        0      102 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_in_not_in/test_field_in_literals/notin/out.sql
--rw-r--r--   0        0        0      196 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_in_not_in/test_isin_notin_in_select/isin/out.sql
--rw-r--r--   0        0        0      210 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_in_not_in/test_isin_notin_in_select/notin/out.sql
--rw-r--r--   0        0        0       85 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_in_not_in/test_literal_in_fields/isin/out.sql
--rw-r--r--   0        0        0      104 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_in_not_in/test_literal_in_fields/notin/out.sql
--rw-r--r--   0        0        0      169 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_group_by_with_window_preserves_range/out.sql
--rw-r--r--   0        0        0      114 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_is_parens/isnull/out.sql
--rw-r--r--   0        0        0      102 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_is_parens/notnull/out.sql
--rw-r--r--   0        0        0      130 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_is_parens_identical_to/out.sql
--rw-r--r--   0        0        0     1165 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_join_aliasing/out.sql
--rw-r--r--   0        0        0     1971 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_join_key_name/out.sql
--rw-r--r--   0        0        0      921 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_join_key_name2/out.sql
--rw-r--r--   0        0        0      111 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_join_no_predicates_for_impala/cross_join/out.sql
--rw-r--r--   0        0        0      121 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_join_no_predicates_for_impala/inner_join/out.sql
--rw-r--r--   0        0        0      126 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_join_no_predicates_for_impala/left_join/out.sql
--rw-r--r--   0        0        0      126 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_join_no_predicates_for_impala/outer_join/out.sql
--rw-r--r--   0        0        0      183 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_join_with_nested_or_condition/out.sql
--rw-r--r--   0        0        0      241 2024-03-22 20:15:42.595352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_join_with_nested_xor_condition/out.sql
--rw-r--r--   0        0        0      397 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_limit_cte_extract/out.sql
--rw-r--r--   0        0        0       93 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_logically_negate_complex_boolean_expr/out.sql
--rw-r--r--   0        0        0      268 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_multiple_filters/out.sql
--rw-r--r--   0        0        0      289 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_multiple_filters2/out.sql
--rw-r--r--   0        0        0      337 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_nested_join_base/out.sql
--rw-r--r--   0        0        0      914 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_nested_join_multiple_ctes/out.sql
--rw-r--r--   0        0        0      557 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_nested_joins_single_cte/out.sql
--rw-r--r--   0        0        0       71 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_relabel_projection/out.sql
--rw-r--r--   0        0        0      148 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_find/out.sql
--rw-r--r--   0        0        0       97 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/ascii_str/out.sql
--rw-r--r--   0        0        0      532 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/capitalize/out.sql
--rw-r--r--   0        0        0      109 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/extract_host/out.sql
--rw-r--r--   0        0        0      111 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/find/out.sql
--rw-r--r--   0        0        0      131 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/find_in_set_multiple/out.sql
--rw-r--r--   0        0        0      126 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/find_in_set_single/out.sql
--rw-r--r--   0        0        0      121 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/find_with_offset/out.sql
--rw-r--r--   0        0        0       99 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/length/out.sql
--rw-r--r--   0        0        0      112 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/like/out.sql
--rw-r--r--   0        0        0      184 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/like_multiple/out.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/lower/out.sql
--rw-r--r--   0        0        0      105 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/lpad_char/out.sql
--rw-r--r--   0        0        0      107 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/lpad_default/out.sql
--rw-r--r--   0        0        0       92 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/lstrip/out.sql
--rw-r--r--   0        0        0      133 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/re_extract/out.sql
--rw-r--r--   0        0        0      141 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/re_replace/out.sql
--rw-r--r--   0        0        0      115 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/re_search/out.sql
--rw-r--r--   0        0        0       99 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/repeat/out.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/reverse/out.sql
--rw-r--r--   0        0        0      115 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/rlike/out.sql
--rw-r--r--   0        0        0      105 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/rpad_char/out.sql
--rw-r--r--   0        0        0      107 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/rpad_default/out.sql
--rw-r--r--   0        0        0       92 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/rstrip/out.sql
--rw-r--r--   0        0        0       90 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/strip/out.sql
--rw-r--r--   0        0        0      146 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/strright/out.sql
--rw-r--r--   0        0        0      229 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/substr_0_3/out.sql
--rw-r--r--   0        0        0      220 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/substr_2/out.sql
--rw-r--r--   0        0        0      119 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/translate/out.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/upper/out.sql
--rw-r--r--   0        0        0       54 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_join/out.sql
--rw-r--r--   0        0        0      171 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_create_uda/False/out.sql
--rw-r--r--   0        0        0      196 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_create_uda/True/out.sql
--rw-r--r--   0        0        0       99 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_create_udf/out.sql
--rw-r--r--   0        0        0      115 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_create_udf_type_conversions/out.sql
--rw-r--r--   0        0        0       51 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_delete_udf_aggregate/out.sql
--rw-r--r--   0        0        0       48 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_delete_udf_db/out.sql
--rw-r--r--   0        0        0       51 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_delete_udf_if_exists/out.sql
--rw-r--r--   0        0        0       41 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_delete_udf_simple/out.sql
--rw-r--r--   0        0        0       32 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_list_udafs/out.sql
--rw-r--r--   0        0        0       48 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_list_udafs_like/out.sql
--rw-r--r--   0        0        0       22 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_list_udf/out.sql
--rw-r--r--   0        0        0       38 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_list_udfs_like/out.sql
--rw-r--r--   0        0        0       75 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_sql_generation/out.sql
--rw-r--r--   0        0        0       54 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_udf/test_sql_generation_from_infoclass/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_hash/out.sql
--rw-r--r--   0        0        0       93 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/log_with_base/out.sql
--rw-r--r--   0        0        0      124 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/round_expr/out.sql
--rw-r--r--   0        0        0      107 2024-03-22 20:15:42.599352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/round_no_args/out.sql
--rw-r--r--   0        0        0       97 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/round_two/out.sql
--rw-r--r--   0        0        0       97 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/round_zero/out.sql
--rw-r--r--   0        0        0      105 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/sign_double/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/sign_float/out.sql
--rw-r--r--   0        0        0      108 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/sign_tinyint/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-abs/out.sql
--rw-r--r--   0        0        0      104 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-approx_median/out.sql
--rw-r--r--   0        0        0      103 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-approx_nunique/out.sql
--rw-r--r--   0        0        0      105 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-ceil/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-exp/out.sql
--rw-r--r--   0        0        0      107 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-floor/out.sql
--rw-r--r--   0        0        0       85 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-ln/out.sql
--rw-r--r--   0        0        0       86 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-log/out.sql
--rw-r--r--   0        0        0       91 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-log10/out.sql
--rw-r--r--   0        0        0       89 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-log2/out.sql
--rw-r--r--   0        0        0       99 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-nullif_zero/out.sql
--rw-r--r--   0        0        0       23 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-nullifzero/out.sql
--rw-r--r--   0        0        0       89 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-sqrt/out.sql
--rw-r--r--   0        0        0       90 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-zero_ifnull/out.sql
--rw-r--r--   0        0        0       25 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-zeroifnull/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-abs/out.sql
--rw-r--r--   0        0        0       98 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-approx_median/out.sql
--rw-r--r--   0        0        0       97 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-approx_nunique/out.sql
--rw-r--r--   0        0        0       99 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-ceil/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-exp/out.sql
--rw-r--r--   0        0        0      101 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-floor/out.sql
--rw-r--r--   0        0        0       79 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-ln/out.sql
--rw-r--r--   0        0        0       80 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-log/out.sql
--rw-r--r--   0        0        0       85 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-log10/out.sql
--rw-r--r--   0        0        0       83 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-log2/out.sql
--rw-r--r--   0        0        0       93 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-nullif_zero/out.sql
--rw-r--r--   0        0        0       20 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-nullifzero/out.sql
--rw-r--r--   0        0        0       83 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-sqrt/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-zero_ifnull/out.sql
--rw-r--r--   0        0        0       22 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-zeroifnull/out.sql
--rw-r--r--   0        0        0      144 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/avg/out.sql
--rw-r--r--   0        0        0      147 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/count/out.sql
--rw-r--r--   0        0        0      143 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/max/out.sql
--rw-r--r--   0        0        0      143 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/min/out.sql
--rw-r--r--   0        0        0      158 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/stddev_pop/out.sql
--rw-r--r--   0        0        0      159 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/stddev_samp/out.sql
--rw-r--r--   0        0        0      143 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/sum/out.sql
--rw-r--r--   0        0        0      157 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/var_pop/out.sql
--rw-r--r--   0        0        0      153 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/var_samp/out.sql
--rw-r--r--   0        0        0       73 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_any_all/all/out.sql
--rw-r--r--   0        0        0       73 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_any_all/any/out.sql
--rw-r--r--   0        0        0       92 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_any_all/not_all/out.sql
--rw-r--r--   0        0        0       92 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_any_all/not_any/out.sql
--rw-r--r--   0        0        0       79 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_between/out.sql
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/add/out.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/and/out.sql
--rw-r--r--   0        0        0       70 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/div/out.sql
--rw-r--r--   0        0        0       70 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/eq/out.sql
--rw-r--r--   0        0        0       77 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/ge/out.sql
--rw-r--r--   0        0        0       71 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/gt/out.sql
--rw-r--r--   0        0        0       74 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/le/out.sql
--rw-r--r--   0        0        0       68 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/lt/out.sql
--rw-r--r--   0        0        0       72 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/mul/out.sql
--rw-r--r--   0        0        0       74 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/ne/out.sql
--rw-r--r--   0        0        0       93 2024-03-22 20:15:42.603352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/or/out.sql
--rw-r--r--   0        0        0       75 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/pow/out.sql
--rw-r--r--   0        0        0       72 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/sub/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/xor/out.sql
--rw-r--r--   0        0        0       76 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_parenthesization/function_call/out.sql
--rw-r--r--   0        0        0      105 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_parenthesization/negation/out.sql
--rw-r--r--   0        0        0       96 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_parenthesization/parens_left/out.sql
--rw-r--r--   0        0        0       79 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/a-int16/out.sql
--rw-r--r--   0        0        0       74 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/a-int32/out.sql
--rw-r--r--   0        0        0       77 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/a-int64/out.sql
--rw-r--r--   0        0        0       78 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/a-string/out.sql
--rw-r--r--   0        0        0       77 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/d-int8/out.sql
--rw-r--r--   0        0        0       79 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/g-double/out.sql
--rw-r--r--   0        0        0       84 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/g-timestamp/out.sql
--rw-r--r--   0        0        0       15 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_correlated_predicate_subquery/out.sql
--rw-r--r--   0        0        0      189 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_correlated_predicate_subquery/out1.sql
--rw-r--r--   0        0        0      189 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_correlated_predicate_subquery/out2.sql
--rw-r--r--   0        0        0       94 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_decimal_casts/column/out.sql
--rw-r--r--   0        0        0       83 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_decimal_casts/literal/out.sql
--rw-r--r--   0        0        0       93 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_isnull_notnull/compound_isnull/out.sql
--rw-r--r--   0        0        0       64 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_isnull_notnull/isnull/out.sql
--rw-r--r--   0        0        0       69 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_isnull_notnull/notnull/out.sql
--rw-r--r--   0        0        0       41 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/embedded_double_quote/out.sql
--rw-r--r--   0        0        0       34 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/embedded_single_quote/out.sql
--rw-r--r--   0        0        0       25 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/false/out.sql
--rw-r--r--   0        0        0       21 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/float/out.sql
--rw-r--r--   0        0        0       17 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/int/out.sql
--rw-r--r--   0        0        0       31 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/simple/out.sql
--rw-r--r--   0        0        0       23 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/true/out.sql
--rw-r--r--   0        0        0       70 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_misc_conditionals/out.sql
--rw-r--r--   0        0        0       68 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_named_expressions/cast/out.sql
--rw-r--r--   0        0        0       83 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_named_expressions/compound_expr/out.sql
--rw-r--r--   0        0        0       58 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_named_expressions/spaces/out.sql
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_negate/a/out.sql
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_negate/f/out.sql
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_negate/h/out.sql
--rw-r--r--   0        0        0      152 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_sql_extract/out.sql
--rw-r--r--   0        0        0       99 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_day_of_week/full_name/out.sql
--rw-r--r--   0        0        0      115 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_day_of_week/index/out.sql
--rw-r--r--   0        0        0      121 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/days/out1.sql
--rw-r--r--   0        0        0       83 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/days/out2.sql
--rw-r--r--   0        0        0      122 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/hours/out1.sql
--rw-r--r--   0        0        0       84 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/hours/out2.sql
--rw-r--r--   0        0        0      124 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/minutes/out1.sql
--rw-r--r--   0        0        0       86 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/minutes/out2.sql
--rw-r--r--   0        0        0      123 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/months/out1.sql
--rw-r--r--   0        0        0       85 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/months/out2.sql
--rw-r--r--   0        0        0      124 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/seconds/out1.sql
--rw-r--r--   0        0        0       86 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/seconds/out2.sql
--rw-r--r--   0        0        0      122 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/weeks/out1.sql
--rw-r--r--   0        0        0       84 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/weeks/out2.sql
--rw-r--r--   0        0        0      122 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/years/out1.sql
--rw-r--r--   0        0        0       84 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/years/out2.sql
--rw-r--r--   0        0        0       78 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/day/out.sql
--rw-r--r--   0        0        0       80 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/hour/out.sql
--rw-r--r--   0        0        0      104 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/microsecond/out.sql
--rw-r--r--   0        0        0      101 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/millisecond/out.sql
--rw-r--r--   0        0        0       84 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/minute/out.sql
--rw-r--r--   0        0        0       82 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/month/out.sql
--rw-r--r--   0        0        0       84 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/second/out.sql
--rw-r--r--   0        0        0       80 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/year/out.sql
--rw-r--r--   0        0        0      122 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_from_integer/default/out.sql
--rw-r--r--   0        0        0      147 2024-03-22 20:15:42.607352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_from_integer/ms/out.sql
--rw-r--r--   0        0        0      150 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_from_integer/us/out.sql
--rw-r--r--   0        0        0       77 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_literals/pd_timestamp/out.sql
--rw-r--r--   0        0        0       77 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_literals/pydatetime/out.sql
--rw-r--r--   0        0        0       77 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_literals/timestamp_function/out.sql
--rw-r--r--   0        0        0       48 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_now/out.sql
--rw-r--r--   0        0        0      621 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_add_default_order_by/out.sql
--rw-r--r--   0        0        0      239 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_aggregate_in_projection/out.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/max/out1.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/max/out2.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/mean/out1.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/mean/out2.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/min/out1.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/min/out2.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/sum/out1.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/sum/out2.sql
--rw-r--r--   0        0        0      180 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_multiple_windows/out.sql
--rw-r--r--   0        0        0      151 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_nested_analytic_function/out.sql
--rw-r--r--   0        0        0      104 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_order_by_desc/out1.sql
--rw-r--r--   0        0        0      188 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_order_by_desc/out2.sql
--rw-r--r--   0        0        0      203 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_propagate_nested_windows/out.sql
--rw-r--r--   0        0        0      177 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_rank_functions/out.sql
--rw-r--r--   0        0        0      244 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_row_number_does_not_require_order_by/out1.sql
--rw-r--r--   0        0        0      252 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_row_number_does_not_require_order_by/out2.sql
--rw-r--r--   0        0        0      244 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_row_number_properly_composes_with_arithmetic/out.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/cumulative/out.sql
--rw-r--r--   0        0        0       95 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_0/out.sql
--rw-r--r--   0        0        0      137 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_10_5/out.sql
--rw-r--r--   0        0        0      144 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_2/out.sql
--rw-r--r--   0        0        0      136 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_2_prec_0/out.sql
--rw-r--r--   0        0        0      137 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_5_10/out.sql
--rw-r--r--   0        0        0      144 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/prec_0/out.sql
--rw-r--r--   0        0        0      144 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/prec_5/out.sql
--rw-r--r--   0        0        0      136 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/prec_5_foll_0/out.sql
--rw-r--r--   0        0        0      136 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/prec_5_foll_2/out.sql
--rw-r--r--   0        0        0      137 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/trailing_10/out.sql
--rw-r--r--   0        0        0     1215 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_analytic_functions.py
--rw-r--r--   0        0        0     2861 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_bucket_histogram.py
--rw-r--r--   0        0        0     2846 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_case_exprs.py
--rw-r--r--   0        0        0     6938 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_client.py
--rw-r--r--   0        0        0     1076 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_coalesce_greater_least.py
--rw-r--r--   0        0        0     8439 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_ddl.py
--rw-r--r--   0        0        0     8913 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_ddl_compilation.py
--rw-r--r--   0        0        0    19387 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_exprs.py
--rw-r--r--   0        0        0     1135 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_in_not_in.py
--rw-r--r--   0        0        0     3857 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_metadata.py
--rw-r--r--   0        0        0     2486 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_parquet_ddl.py
--rw-r--r--   0        0        0     7271 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_partition.py
--rw-r--r--   0        0        0     1704 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_patched.py
--rw-r--r--   0        0        0     9252 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_sql.py
--rw-r--r--   0        0        0     2586 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_string_builtins.py
--rw-r--r--   0        0        0    16540 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_udf.py
--rw-r--r--   0        0        0     3800 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_unary_builtins.py
--rw-r--r--   0        0        0     7357 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_value_exprs.py
--rw-r--r--   0        0        0     4311 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_window.py
--rw-r--r--   0        0        0     7085 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/impala/udf.py
--rw-r--r--   0        0        0    16984 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/mssql/__init__.py
--rw-r--r--   0        0        0    15609 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/mssql/compiler.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/mssql/tests/__init__.py
--rw-r--r--   0        0        0     1707 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/mssql/tests/conftest.py
--rw-r--r--   0        0        0     3394 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/mssql/tests/test_client.py
--rw-r--r--   0        0        0    15883 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/mysql/__init__.py
--rw-r--r--   0        0        0    12174 2024-03-22 20:15:42.611352 turntable_spoonbill-9.0.4/ibis/backends/mysql/compiler.py
--rw-r--r--   0        0        0      855 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/mysql/converter.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/mysql/tests/__init__.py
--rw-r--r--   0        0        0     2508 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/mysql/tests/conftest.py
--rw-r--r--   0        0        0     6291 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/mysql/tests/test_client.py
--rw-r--r--   0        0        0    18423 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/oracle/__init__.py
--rw-r--r--   0        0        0    16558 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/oracle/compiler.py
--rw-r--r--   0        0        0      451 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/oracle/converter.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/oracle/tests/__init__.py
--rw-r--r--   0        0        0     5014 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/oracle/tests/conftest.py
--rw-r--r--   0        0        0     1575 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/oracle/tests/test_client.py
--rw-r--r--   0        0        0      672 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/oracle/tests/test_datatypes.py
--rw-r--r--   0        0        0    10502 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/__init__.py
--rw-r--r--   0        0        0     3122 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/convert.py
--rw-r--r--   0        0        0    26760 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/executor.py
--rw-r--r--   0        0        0     7176 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/helpers.py
--rw-r--r--   0        0        0    16143 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/kernels.py
--rw-r--r--   0        0        0    10393 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/rewrites.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/__init__.py
--rw-r--r--   0        0        0     9098 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/conftest.py
--rw-r--r--   0        0        0     6431 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_arrays.py
--rw-r--r--   0        0        0     5603 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_cast.py
--rw-r--r--   0        0        0     2288 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_client.py
--rw-r--r--   0        0        0     1763 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_core.py
--rw-r--r--   0        0        0     8621 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_functions.py
--rw-r--r--   0        0        0     1943 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_helpers.py
--rw-r--r--   0        0        0    21442 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_join.py
--rw-r--r--   0        0        0     2813 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_maps.py
--rw-r--r--   0        0        0    25980 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_operations.py
--rw-r--r--   0        0        0     5619 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_strings.py
--rw-r--r--   0        0        0     2386 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_structs.py
--rw-r--r--   0        0        0     5977 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_temporal.py
--rw-r--r--   0        0        0    12258 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_udf.py
--rw-r--r--   0        0        0    20161 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_window.py
--rw-r--r--   0        0        0      741 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/pandas/udf.py
--rw-r--r--   0        0        0    17597 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/polars/__init__.py
--rw-r--r--   0        0        0    37062 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/polars/compiler.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/polars/tests/__init__.py
--rw-r--r--   0        0        0     1688 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/polars/tests/conftest.py
--rw-r--r--   0        0        0      724 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/polars/tests/test_join.py
--rw-r--r--   0        0        0     3257 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/polars/tests/test_udf.py
--rw-r--r--   0        0        0    24072 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/__init__.py
--rw-r--r--   0        0        0    18588 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/compiler.py
--rw-r--r--   0        0        0      615 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/converter.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/__init__.py
--rw-r--r--   0        0        0     2890 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/conftest.py
--rw-r--r--   0        0        0       56 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_client/test_compile_toplevel/out.sql
--rw-r--r--   0        0        0      246 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_client/test_timezone_from_column/out.sql
--rw-r--r--   0        0        0      668 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_functions/test_analytic_functions/out.sql
--rw-r--r--   0        0        0      108 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_functions/test_cast/double_to_int16/out.sql
--rw-r--r--   0        0        0      107 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_functions/test_cast/double_to_int8/out.sql
--rw-r--r--   0        0        0      109 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_functions/test_cast/string_to_decimal_no_params/out.sql
--rw-r--r--   0        0        0      121 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_functions/test_cast/string_to_decimal_params/out.sql
--rw-r--r--   0        0        0      118 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_functions/test_cast/string_to_double/out.sql
--rw-r--r--   0        0        0      106 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_functions/test_cast/string_to_float/out.sql
--rw-r--r--   0        0        0      113 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_functions/test_date_cast/out.sql
--rw-r--r--   0        0        0       64 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_functions/test_timestamp_cast_noop/out1.sql
--rw-r--r--   0        0        0      102 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_functions/test_timestamp_cast_noop/out2.sql
--rw-r--r--   0        0        0      364 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_functions/test_union_cte/False/out.sql
--rw-r--r--   0        0        0      356 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_functions/test_union_cte/True/out.sql
--rw-r--r--   0        0        0      338 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_equals/out1.sql
--rw-r--r--   0        0        0       97 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_equals/out2.sql
--rw-r--r--   0        0        0       82 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_equals/out3.sql
--rw-r--r--   0        0        0      229 2024-03-22 20:15:42.615352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/linestring-geography/out.sql
--rw-r--r--   0        0        0      229 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/linestring-geometry/out.sql
--rw-r--r--   0        0        0      223 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/linestring-none/out.sql
--rw-r--r--   0        0        0      229 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/linestring-srid/out.sql
--rw-r--r--   0        0        0      377 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multilinestring-geography/out.sql
--rw-r--r--   0        0        0      377 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multilinestring-geometry/out.sql
--rw-r--r--   0        0        0      371 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multilinestring-none/out.sql
--rw-r--r--   0        0        0      377 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multilinestring-srid/out.sql
--rw-r--r--   0        0        0      257 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipoint-geography/out.sql
--rw-r--r--   0        0        0      257 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipoint-geometry/out.sql
--rw-r--r--   0        0        0      251 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipoint-none/out.sql
--rw-r--r--   0        0        0      257 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipoint-srid/out.sql
--rw-r--r--   0        0        0      486 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipolygon-geography/out.sql
--rw-r--r--   0        0        0      486 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipolygon-geometry/out.sql
--rw-r--r--   0        0        0      474 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipolygon-none/out.sql
--rw-r--r--   0        0        0      486 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipolygon-srid/out.sql
--rw-r--r--   0        0        0      153 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/point-geography/out.sql
--rw-r--r--   0        0        0      153 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/point-geometry/out.sql
--rw-r--r--   0        0        0      147 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/point-none/out.sql
--rw-r--r--   0        0        0      153 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/point-srid/out.sql
--rw-r--r--   0        0        0      441 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon-geography/out.sql
--rw-r--r--   0        0        0      441 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon-geometry/out.sql
--rw-r--r--   0        0        0      429 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon-none/out.sql
--rw-r--r--   0        0        0      441 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon-srid/out.sql
--rw-r--r--   0        0        0      281 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon_single-geography/out.sql
--rw-r--r--   0        0        0      281 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon_single-geometry/out.sql
--rw-r--r--   0        0        0      275 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon_single-none/out.sql
--rw-r--r--   0        0        0      281 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon_single-srid/out.sql
--rw-r--r--   0        0        0      124 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/linestring_contains/out.sql
--rw-r--r--   0        0        0      106 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/linestring_end_point/out.sql
--rw-r--r--   0        0        0       91 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/linestring_length/out.sql
--rw-r--r--   0        0        0      110 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/linestring_start_point/out.sql
--rw-r--r--   0        0        0       97 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/multipolygon_n_points/out.sql
--rw-r--r--   0        0        0      106 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/point_set_srid/out.sql
--rw-r--r--   0        0        0       77 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/point_srid/out.sql
--rw-r--r--   0        0        0       71 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/point_x/out.sql
--rw-r--r--   0        0        0       71 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/point_y/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/polygon_area/out.sql
--rw-r--r--   0        0        0       91 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/polygon_perimeter/out.sql
--rw-r--r--   0        0        0      103 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr0/out.sql
--rw-r--r--   0        0        0      109 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr1/out.sql
--rw-r--r--   0        0        0      109 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr2/out.sql
--rw-r--r--   0        0        0      109 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr3/out.sql
--rw-r--r--   0        0        0      109 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr4/out.sql
--rw-r--r--   0        0        0      109 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr5/out.sql
--rw-r--r--   0        0        0      109 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr6/out.sql
--rw-r--r--   0        0        0      109 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr7/out.sql
--rw-r--r--   0        0        0      139 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp0/out.sql
--rw-r--r--   0        0        0      139 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp1/out.sql
--rw-r--r--   0        0        0      139 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp2/out.sql
--rw-r--r--   0        0        0      199 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp3/out.sql
--rw-r--r--   0        0        0      199 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp4/out.sql
--rw-r--r--   0        0        0      215 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp5/out.sql
--rw-r--r--   0        0        0      243 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp6/out.sql
--rw-r--r--   0        0        0      295 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp7/out.sql
--rw-r--r--   0        0        0      199 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp8/out.sql
--rw-r--r--   0        0        0       80 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_postgis/test_select_linestring_geodata/out.sql
--rw-r--r--   0        0        0       84 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_postgis/test_select_multipolygon_geodata/out.sql
--rw-r--r--   0        0        0       70 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_postgis/test_select_point_geodata/out.sql
--rw-r--r--   0        0        0       74 2024-03-22 20:15:42.619352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_postgis/test_select_polygon_geodata/out.sql
--rw-r--r--   0        0        0     7544 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/test_client.py
--rw-r--r--   0        0        0    38740 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/test_functions.py
--rw-r--r--   0        0        0    17043 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/test_geospatial.py
--rw-r--r--   0        0        0      416 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/test_json.py
--rw-r--r--   0        0        0     9321 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/test_postgis.py
--rw-r--r--   0        0        0      488 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/test_string.py
--rw-r--r--   0        0        0     5188 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/test_udf.py
--rw-r--r--   0        0        0    24362 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/pyspark/__init__.py
--rw-r--r--   0        0        0    16406 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/pyspark/compiler.py
--rw-r--r--   0        0        0     1263 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/pyspark/converter.py
--rw-r--r--   0        0        0     4491 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/pyspark/datatypes.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/__init__.py
--rw-r--r--   0        0        0    11767 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/conftest.py
--rw-r--r--   0        0        0      665 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/test_aggregation.py
--rw-r--r--   0        0        0     4658 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/test_array.py
--rw-r--r--   0        0        0     3805 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/test_basic.py
--rw-r--r--   0        0        0     4895 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/test_ddl.py
--rw-r--r--   0        0        0      801 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/test_null.py
--rw-r--r--   0        0        0     2340 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/test_window.py
--rw-r--r--   0        0        0     8473 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/risingwave/__init__.py
--rw-r--r--   0        0        0     2747 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/risingwave/compiler.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/risingwave/tests/__init__.py
--rw-r--r--   0        0        0     2386 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/risingwave/tests/conftest.py
--rw-r--r--   0        0        0       56 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/risingwave/tests/snapshots/test_client/test_compile_toplevel/out.sql
--rw-r--r--   0        0        0      349 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/risingwave/tests/snapshots/test_functions/test_analytic_functions/out.sql
--rw-r--r--   0        0        0      364 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/risingwave/tests/snapshots/test_functions/test_union_cte/False/out.sql
--rw-r--r--   0        0        0      356 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/risingwave/tests/snapshots/test_functions/test_union_cte/True/out.sql
--rw-r--r--   0        0        0     3511 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/risingwave/tests/test_client.py
--rw-r--r--   0        0        0    25860 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/risingwave/tests/test_functions.py
--rw-r--r--   0        0        0      416 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/risingwave/tests/test_json.py
--rw-r--r--   0        0        0    37436 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/snowflake/__init__.py
--rw-r--r--   0        0        0    21366 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/snowflake/compiler.py
--rw-r--r--   0        0        0     2914 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/snowflake/converter.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/snowflake/tests/__init__.py
--rw-r--r--   0        0        0     6274 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/snowflake/tests/conftest.py
--rw-r--r--   0        0        0     8646 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/snowflake/tests/test_client.py
--rw-r--r--   0        0        0     3971 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/snowflake/tests/test_datatypes.py
--rw-r--r--   0        0        0     4165 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/snowflake/tests/test_udf.py
--rw-r--r--   0        0        0    12441 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/sql/__init__.py
--rw-r--r--   0        0        0    46975 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/sql/compiler.py
--rw-r--r--   0        0        0    35488 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/sql/datatypes.py
--rw-r--r--   0        0        0     3520 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/sql/ddl.py
--rw-r--r--   0        0        0     9985 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/sql/dialects.py
--rw-r--r--   0        0        0     9852 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/sql/rewrites.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/sql/tests/__init__.py
--rw-r--r--   0        0        0      550 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/sql/tests/test_compiler.py
--rw-r--r--   0        0        0     2565 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/sql/tests/test_datatypes.py
--rw-r--r--   0        0        0    18080 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/sqlite/__init__.py
--rw-r--r--   0        0        0    15477 2024-03-22 20:15:42.623352 turntable_spoonbill-9.0.4/ibis/backends/sqlite/compiler.py
--rw-r--r--   0        0        0      751 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/sqlite/converter.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/sqlite/tests/__init__.py
--rw-r--r--   0        0        0     2608 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/sqlite/tests/conftest.py
--rw-r--r--   0        0        0     2059 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/sqlite/tests/test_client.py
--rw-r--r--   0        0        0     3053 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/sqlite/tests/test_types.py
--rw-r--r--   0        0        0     9750 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/sqlite/udf.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/__init__.py
--rw-r--r--   0        0        0    12682 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/base.py
--rw-r--r--   0        0        0     2637 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/data.py
--rw-r--r--   0        0        0     4954 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/errors.py
--rw-r--r--   0        0        0      600 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/bigquery/out.sql
--rw-r--r--   0        0        0      714 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/clickhouse/out.sql
--rw-r--r--   0        0        0      714 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/datafusion/out.sql
--rw-r--r--   0        0        0      714 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/druid/out.sql
--rw-r--r--   0        0        0      748 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/duckdb/out.sql
--rw-r--r--   0        0        0      600 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/exasol/out.sql
--rw-r--r--   0        0        0      622 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/flink/out.sql
--rw-r--r--   0        0        0      622 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/impala/out.sql
--rw-r--r--   0        0        0      765 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/mssql/out.sql
--rw-r--r--   0        0        0      702 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/mysql/out.sql
--rw-r--r--   0        0        0      598 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/oracle/out.sql
--rw-r--r--   0        0        0      714 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/postgres/out.sql
--rw-r--r--   0        0        0      622 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/pyspark/out.sql
--rw-r--r--   0        0        0      714 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/risingwave/out.sql
--rw-r--r--   0        0        0      600 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/snowflake/out.sql
--rw-r--r--   0        0        0      736 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/sqlite/out.sql
--rw-r--r--   0        0        0      714 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/trino/out.sql
--rw-r--r--   0        0        0      111 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/bigquery/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/clickhouse/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/datafusion/out.sql
--rw-r--r--   0        0        0      111 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/druid/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/duckdb/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/exasol/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/flink/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/impala/out.sql
--rw-r--r--   0        0        0      174 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/mssql/out.sql
--rw-r--r--   0        0        0       99 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/mysql/out.sql
--rw-r--r--   0        0        0      112 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/oracle/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/postgres/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/pyspark/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/risingwave/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/snowflake/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/sqlite/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_default_limit/trino/out.sql
--rw-r--r--   0        0        0      111 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/bigquery/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/clickhouse/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/datafusion/out.sql
--rw-r--r--   0        0        0      111 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/druid/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/duckdb/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/exasol/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/flink/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/impala/out.sql
--rw-r--r--   0        0        0      174 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/mssql/out.sql
--rw-r--r--   0        0        0       99 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/mysql/out.sql
--rw-r--r--   0        0        0      112 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/oracle/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/postgres/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/pyspark/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/risingwave/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/snowflake/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/sqlite/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.627352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/trino/out.sql
--rw-r--r--   0        0        0      116 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/bigquery/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/clickhouse/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/datafusion/out.sql
--rw-r--r--   0        0        0      452 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/druid/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/duckdb/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/exasol/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/flink/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/impala/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/mssql/out.sql
--rw-r--r--   0        0        0      417 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/mysql/out.sql
--rw-r--r--   0        0        0      411 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/oracle/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/postgres/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/pyspark/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/risingwave/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/snowflake/out.sql
--rw-r--r--   0        0        0      399 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/sqlite/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/trino/out.sql
--rw-r--r--   0        0        0      158 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/bigquery/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/clickhouse/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/datafusion/out.sql
--rw-r--r--   0        0        0      162 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/druid/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/duckdb/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/exasol/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/flink/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/impala/out.sql
--rw-r--r--   0        0        0      229 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/mssql/out.sql
--rw-r--r--   0        0        0      146 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/mysql/out.sql
--rw-r--r--   0        0        0      172 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/oracle/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/postgres/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/pyspark/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/risingwave/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/snowflake/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/sqlite/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/trino/out.sql
--rw-r--r--   0        0        0      324 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_join/test_complex_join_agg/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/bigquery/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/clickhouse/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/datafusion/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/druid/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/duckdb/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/exasol/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/flink/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/impala/out.sql
--rw-r--r--   0        0        0      356 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/mssql/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/mysql/out.sql
--rw-r--r--   0        0        0      305 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/oracle/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/postgres/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/pyspark/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/risingwave/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/snowflake/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/sqlite/out.sql
--rw-r--r--   0        0        0      323 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/trino/out.sql
--rw-r--r--   0        0        0      395 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/bigquery/out.sql
--rw-r--r--   0        0        0      691 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/clickhouse/out.sql
--rw-r--r--   0        0        0      514 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/datafusion/out.sql
--rw-r--r--   0        0        0      395 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/druid/out.sql
--rw-r--r--   0        0        0      395 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/duckdb/out.sql
--rw-r--r--   0        0        0      395 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/exasol/out.sql
--rw-r--r--   0        0        0      691 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/flink/out.sql
--rw-r--r--   0        0        0      395 2024-03-22 20:15:42.631352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/impala/out.sql
--rw-r--r--   0        0        0      691 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/mssql/out.sql
--rw-r--r--   0        0        0      395 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/mysql/out.sql
--rw-r--r--   0        0        0      688 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/oracle/out.sql
--rw-r--r--   0        0        0      395 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/postgres/out.sql
--rw-r--r--   0        0        0      395 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/pyspark/out.sql
--rw-r--r--   0        0        0      395 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/risingwave/out.sql
--rw-r--r--   0        0        0      395 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/snowflake/out.sql
--rw-r--r--   0        0        0      395 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/sqlite/out.sql
--rw-r--r--   0        0        0      395 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/trino/out.sql
--rw-r--r--   0        0        0      137 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/bigquery/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/clickhouse/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/datafusion/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/druid/out.sql
--rw-r--r--   0        0        0      155 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/duckdb/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/exasol/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/flink/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/impala/out.sql
--rw-r--r--   0        0        0      177 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/mssql/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/mysql/out.sql
--rw-r--r--   0        0        0      132 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/oracle/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/postgres/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/pyspark/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/risingwave/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/snowflake/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/sqlite/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_isin_bug/trino/out.sql
--rw-r--r--   0        0        0     6419 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/bigquery/out.sql
--rw-r--r--   0        0        0     3435 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/clickhouse/out.sql
--rw-r--r--   0        0        0     2512 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/duckdb/out.sql
--rw-r--r--   0        0        0     2850 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/postgres/out.sql
--rw-r--r--   0        0        0     3024 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/pyspark/out.sql
--rw-r--r--   0        0        0     2850 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/risingwave/out.sql
--rw-r--r--   0        0        0     7590 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/trino/out.sql
--rw-r--r--   0        0        0       55 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/bigquery-date/out.sql
--rw-r--r--   0        0        0       98 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/bigquery-timestamp/out.sql
--rw-r--r--   0        0        0       60 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/clickhouse-date/out.sql
--rw-r--r--   0        0        0      119 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/clickhouse-timestamp/out.sql
--rw-r--r--   0        0        0       71 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/datafusion-date/out.sql
--rw-r--r--   0        0        0      133 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/datafusion-timestamp/out.sql
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/druid-date/out.sql
--rw-r--r--   0        0        0      108 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/druid-timestamp/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/duckdb-date/out.sql
--rw-r--r--   0        0        0      103 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/duckdb-timestamp/out.sql
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/exasol-date/out.sql
--rw-r--r--   0        0        0      105 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/exasol-timestamp/out.sql
--rw-r--r--   0        0        0       52 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/impala-date/out.sql
--rw-r--r--   0        0        0       89 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/impala-timestamp/out.sql
--rw-r--r--   0        0        0       65 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/mssql-date/out.sql
--rw-r--r--   0        0        0      111 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/mssql-timestamp/out.sql
--rw-r--r--   0        0        0       58 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/mysql-date/out.sql
--rw-r--r--   0        0        0      100 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/mysql-timestamp/out.sql
--rw-r--r--   0        0        0       77 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/oracle-date/out.sql
--rw-r--r--   0        0        0      134 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/oracle-timestamp/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/postgres-date/out.sql
--rw-r--r--   0        0        0      108 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/postgres-timestamp/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/pyspark-date/out.sql
--rw-r--r--   0        0        0      108 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/pyspark-timestamp/out.sql
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/risingwave-date/out.sql
--rw-r--r--   0        0        0      108 2024-03-22 20:15:42.635352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/risingwave-timestamp/out.sql
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/snowflake-date/out.sql
--rw-r--r--   0        0        0      113 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/snowflake-timestamp/out.sql
--rw-r--r--   0        0        0       52 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/sqlite-date/out.sql
--rw-r--r--   0        0        0       89 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/sqlite-timestamp/out.sql
--rw-r--r--   0        0        0       71 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/trino-date/out.sql
--rw-r--r--   0        0        0      132 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/trino-timestamp/out.sql
--rw-r--r--   0        0        0       49 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-bigquery/out.sql
--rw-r--r--   0        0        0       71 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-clickhouse/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-datafusion/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-druid/out.sql
--rw-r--r--   0        0        0       57 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-duckdb/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-exasol/out.sql
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-impala/out.sql
--rw-r--r--   0        0        0       65 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-mssql/out.sql
--rw-r--r--   0        0        0       56 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-mysql/out.sql
--rw-r--r--   0        0        0       92 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-oracle/out.sql
--rw-r--r--   0        0        0      109 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-postgres/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-risingwave/out.sql
--rw-r--r--   0        0        0       64 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-snowflake/out.sql
--rw-r--r--   0        0        0       47 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-sqlite/out.sql
--rw-r--r--   0        0        0       61 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-trino/out.sql
--rw-r--r--   0        0        0       57 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-bigquery/out.sql
--rw-r--r--   0        0        0       86 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-clickhouse/out.sql
--rw-r--r--   0        0        0       76 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-datafusion/out.sql
--rw-r--r--   0        0        0       76 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-druid/out.sql
--rw-r--r--   0        0        0       70 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-duckdb/out.sql
--rw-r--r--   0        0        0       76 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-exasol/out.sql
--rw-r--r--   0        0        0       81 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-impala/out.sql
--rw-r--r--   0        0        0       73 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-mssql/out.sql
--rw-r--r--   0        0        0       69 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-mysql/out.sql
--rw-r--r--   0        0        0      107 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-oracle/out.sql
--rw-r--r--   0        0        0      122 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-postgres/out.sql
--rw-r--r--   0        0        0       76 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-risingwave/out.sql
--rw-r--r--   0        0        0       80 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-snowflake/out.sql
--rw-r--r--   0        0        0       62 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-sqlite/out.sql
--rw-r--r--   0        0        0       76 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-trino/out.sql
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/__init__.py
--rw-r--r--   0        0        0     4714 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/conftest.py
--rw-r--r--   0        0        0      335 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_agg_and_non_agg_filter/out.sql
--rw-r--r--   0        0        0      372 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_agg_filter/out.sql
--rw-r--r--   0        0        0      372 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_agg_filter_with_alias/out.sql
--rw-r--r--   0        0        0      582 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_column_distinct/decompiled.py
--rw-r--r--   0        0        0      104 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_column_distinct/out.sql
--rw-r--r--   0        0        0      128 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_column_expr_default_name/decompiled.py
--rw-r--r--   0        0        0       94 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_column_expr_default_name/out.sql
--rw-r--r--   0        0        0      142 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_column_expr_retains_name/decompiled.py
--rw-r--r--   0        0        0       82 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_column_expr_retains_name/out.sql
--rw-r--r--   0        0        0      649 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_count_distinct/decompiled.py
--rw-r--r--   0        0        0      484 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_count_distinct/out.sql
--rw-r--r--   0        0        0      898 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_difference_project_column/decompiled.py
--rw-r--r--   0        0        0      475 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_difference_project_column/out.sql
--rw-r--r--   0        0        0      236 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_having_from_filter/decompiled.py
--rw-r--r--   0        0        0      304 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_having_from_filter/out.sql
--rw-r--r--   0        0        0      320 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_having_size/out.sql
--rw-r--r--   0        0        0      903 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_intersect_project_column/decompiled.py
--rw-r--r--   0        0        0      478 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_intersect_project_column/out.sql
--rw-r--r--   0        0        0      737 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_multiple_count_distinct/decompiled.py
--rw-r--r--   0        0        0      180 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_multiple_count_distinct/out.sql
--rw-r--r--   0        0        0      377 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_pushdown_with_or/out.sql
--rw-r--r--   0        0        0      314 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_simple_agg_filter/out.sql
--rw-r--r--   0        0        0      407 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_subquery_where_location/decompiled.py
--rw-r--r--   0        0        0      378 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_subquery_where_location/out.sql
--rw-r--r--   0        0        0      851 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_table_difference/decompiled.py
--rw-r--r--   0        0        0      491 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_table_difference/out.sql
--rw-r--r--   0        0        0      617 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_table_distinct/decompiled.py
--rw-r--r--   0        0        0      124 2024-03-22 20:15:42.639352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_table_distinct/out.sql
--rw-r--r--   0        0        0      446 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_table_drop_with_filter/decompiled.py
--rw-r--r--   0        0        0      355 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_table_drop_with_filter/out.sql
--rw-r--r--   0        0        0      850 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_table_intersect/decompiled.py
--rw-r--r--   0        0        0      494 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_table_intersect/out.sql
--rw-r--r--   0        0        0      846 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_union/decompiled.py
--rw-r--r--   0        0        0      490 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_union/out.sql
--rw-r--r--   0        0        0      124 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_union_order_by/decompiled.py
--rw-r--r--   0        0        0      228 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_union_order_by/out.sql
--rw-r--r--   0        0        0      857 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_union_project_column/decompiled.py
--rw-r--r--   0        0        0      478 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_union_project_column/out.sql
--rw-r--r--   0        0        0      661 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_count_joined/decompiled.py
--rw-r--r--   0        0        0      290 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_count_joined/out.sql
--rw-r--r--   0        0        0      195 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_having/explicit.sql
--rw-r--r--   0        0        0      243 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_having/inline.sql
--rw-r--r--   0        0        0      267 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_projection_alias_bug/out.sql
--rw-r--r--   0        0        0      366 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_projection_subquery/agg_filtered.sql
--rw-r--r--   0        0        0      405 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_projection_subquery/agg_filtered2.sql
--rw-r--r--   0        0        0      252 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_projection_subquery/filtered.sql
--rw-r--r--   0        0        0      231 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_projection_subquery/proj.sql
--rw-r--r--   0        0        0      369 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_anti_join/decompiled.py
--rw-r--r--   0        0        0      145 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_anti_join/out.sql
--rw-r--r--   0        0        0      197 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_bool_bool/decompiled.py
--rw-r--r--   0        0        0      154 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_bool_bool/out.sql
--rw-r--r--   0        0        0      574 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_bug_duplicated_where/out.sql
--rw-r--r--   0        0        0     1096 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_bug_project_multiple_times/out.sql
--rw-r--r--   0        0        0      930 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_case_in_projection/decompiled.py
--rw-r--r--   0        0        0      388 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_case_in_projection/out.sql
--rw-r--r--   0        0        0      611 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_chain_limit_doesnt_collapse/result.sql
--rw-r--r--   0        0        0      384 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_complex_union/result.sql
--rw-r--r--   0        0        0      374 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_double_nested_subquery_no_aliases/out.sql
--rw-r--r--   0        0        0      202 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_endswith/decompiled.py
--rw-r--r--   0        0        0       67 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_endswith/out.sql
--rw-r--r--   0        0        0      173 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_exists_subquery/out.sql
--rw-r--r--   0        0        0      245 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_filter_inside_exists/out.sql
--rw-r--r--   0        0        0      172 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_filter_predicates/out.sql
--rw-r--r--   0        0        0      513 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_filter_self_join_analysis_bug/result.sql
--rw-r--r--   0        0        0      379 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_filter_subquery_derived_reduction/expr3.sql
--rw-r--r--   0        0        0      440 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_filter_subquery_derived_reduction/expr4.sql
--rw-r--r--   0        0        0      242 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_fuse_projections/decompiled.py
--rw-r--r--   0        0        0      148 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_fuse_projections/project.sql
--rw-r--r--   0        0        0      190 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_fuse_projections/project_filter.sql
--rw-r--r--   0        0        0       79 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_identifier_quoting/out.sql
--rw-r--r--   0        0        0      131 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_incorrect_predicate_pushdown/result.sql
--rw-r--r--   0        0        0       99 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_incorrect_predicate_pushdown_with_literal/result.sql
--rw-r--r--   0        0        0     1188 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_between_joins/decompiled.py
--rw-r--r--   0        0        0      403 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_between_joins/out.sql
--rw-r--r--   0        0        0      637 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_filtered_tables_no_pushdown/out.sql
--rw-r--r--   0        0        0     1369 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_just_materialized/decompiled.py
--rw-r--r--   0        0        0      490 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_just_materialized/out.sql
--rw-r--r--   0        0        0      430 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_projection_subquery_bug/out.sql
--rw-r--r--   0        0        0      565 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_with_conditional_aggregate/result.sql
--rw-r--r--   0        0        0      192 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_with_limited_table/out.sql
--rw-r--r--   0        0        0      397 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_limit_cte_extract/out.sql
--rw-r--r--   0        0        0     1981 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_limit_with_self_join/decompiled.py
--rw-r--r--   0        0        0     1051 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_limit_with_self_join/out.sql
--rw-r--r--   0        0        0      429 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_loj_subquery_filter_handling/out.sql
--rw-r--r--   0        0        0      540 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_multiple_joins/decompiled.py
--rw-r--r--   0        0        0      247 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_multiple_joins/out.sql
--rw-r--r--   0        0        0      552 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_multiple_limits/decompiled.py
--rw-r--r--   0        0        0       99 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_multiple_limits/out.sql
--rw-r--r--   0        0        0       72 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_nameless_table/decompiled.py
--rw-r--r--   0        0        0       23 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_nameless_table/out.sql
--rw-r--r--   0        0        0      696 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_order_by_on_limit_yield_subquery/decompiled.py
--rw-r--r--   0        0        0      212 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_order_by_on_limit_yield_subquery/out.sql
--rw-r--r--   0        0        0       98 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_projection_filter_fuse/out.sql
--rw-r--r--   0        0        0      174 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_scalar_subquery_different_table/out.sql
--rw-r--r--   0        0        0      213 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/agg_explicit_column/decompiled.py
--rw-r--r--   0        0        0       84 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/agg_explicit_column/out.sql
--rw-r--r--   0        0        0      227 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/agg_string_columns/decompiled.py
--rw-r--r--   0        0        0      106 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/agg_string_columns/out.sql
--rw-r--r--   0        0        0      161 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/aggregate_table_count_metric/decompiled.py
--rw-r--r--   0        0        0       60 2024-03-22 20:15:42.643352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/aggregate_table_count_metric/out.sql
--rw-r--r--   0        0        0      183 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/filter_then_limit/decompiled.py
--rw-r--r--   0        0        0      131 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/filter_then_limit/out.sql
--rw-r--r--   0        0        0      163 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/limit_simple/decompiled.py
--rw-r--r--   0        0        0       40 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/limit_simple/out.sql
--rw-r--r--   0        0        0      197 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/limit_then_filter/decompiled.py
--rw-r--r--   0        0        0      167 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/limit_then_filter/out.sql
--rw-r--r--   0        0        0      166 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/limit_with_offset/decompiled.py
--rw-r--r--   0        0        0       49 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/limit_with_offset/out.sql
--rw-r--r--   0        0        0      195 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/mixed_columns_ascending/decompiled.py
--rw-r--r--   0        0        0       58 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/mixed_columns_ascending/out.sql
--rw-r--r--   0        0        0      138 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/self_reference_simple/decompiled.py
--rw-r--r--   0        0        0       34 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/self_reference_simple/out.sql
--rw-r--r--   0        0        0      177 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/single_column/decompiled.py
--rw-r--r--   0        0        0      108 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/single_column/out.sql
--rw-r--r--   0        0        0      328 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/test_physical_table_reference_translate/decompiled.py
--rw-r--r--   0        0        0       26 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/test_physical_table_reference_translate/out.sql
--rw-r--r--   0        0        0      485 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_self_join_subquery_distinct_equal/out.sql
--rw-r--r--   0        0        0      369 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_semi_join/decompiled.py
--rw-r--r--   0        0        0      145 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_semi_join/out.sql
--rw-r--r--   0        0        0      402 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_simple_joins/decompiled.py
--rw-r--r--   0        0        0      146 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_simple_joins/inner.sql
--rw-r--r--   0        0        0      180 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_simple_joins/inner_two_preds.sql
--rw-r--r--   0        0        0      151 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_simple_joins/left.sql
--rw-r--r--   0        0        0      151 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_simple_joins/outer.sql
--rw-r--r--   0        0        0      141 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_sort_then_group_by_propagates_keys/result1.sql
--rw-r--r--   0        0        0      141 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_sort_then_group_by_propagates_keys/result2.sql
--rw-r--r--   0        0        0      204 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_startswith/decompiled.py
--rw-r--r--   0        0        0       72 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_startswith/out.sql
--rw-r--r--   0        0        0     1991 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_factor_correlated_subquery/out.sql
--rw-r--r--   0        0        0      178 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_in_filter_predicate/expr.sql
--rw-r--r--   0        0        0      341 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_in_filter_predicate/expr2.sql
--rw-r--r--   0        0        0      629 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_in_union/decompiled.py
--rw-r--r--   0        0        0      420 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_in_union/out.sql
--rw-r--r--   0        0        0      512 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_used_for_self_join/out.sql
--rw-r--r--   0        0        0      656 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_analysis_bug/out.sql
--rw-r--r--   0        0        0      369 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_operation/e1.sql
--rw-r--r--   0        0        0      382 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_operation/e2.sql
--rw-r--r--   0        0        0     1178 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_predicate_pushdown_bug/out.sql
--rw-r--r--   0        0        0      223 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_to_aggregate/out.sql
--rw-r--r--   0        0        0      841 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_tpch_self_join_failure/out.sql
--rw-r--r--   0        0        0      728 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_analyze_scalar_op/decompiled.py
--rw-r--r--   0        0        0      591 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_analyze_scalar_op/out.sql
--rw-r--r--   0        0        0      458 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_no_pushdown_possible/decompiled.py
--rw-r--r--   0        0        0      339 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_no_pushdown_possible/out.sql
--rw-r--r--   0        0        0      438 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_with_between/decompiled.py
--rw-r--r--   0        0        0      264 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_with_between/out.sql
--rw-r--r--   0        0        0      469 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_with_join/decompiled.py
--rw-r--r--   0        0        0      396 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_with_join/out.sql
--rw-r--r--   0        0        0      243 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_aggregate/having_count/out.sql
--rw-r--r--   0        0        0      195 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_aggregate/having_sum/out.sql
--rw-r--r--   0        0        0       84 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_aggregate/single/out.sql
--rw-r--r--   0        0        0      106 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_aggregate/two/out.sql
--rw-r--r--   0        0        0      121 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_between/out.sql
--rw-r--r--   0        0        0      156 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_boolean_conjunction/and/out.sql
--rw-r--r--   0        0        0      155 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_boolean_conjunction/or/out.sql
--rw-r--r--   0        0        0      211 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_coalesce/out.sql
--rw-r--r--   0        0        0       91 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_comparisons/eq/out.sql
--rw-r--r--   0        0        0       92 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_comparisons/ge/out.sql
--rw-r--r--   0        0        0       91 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_comparisons/gt/out.sql
--rw-r--r--   0        0        0       92 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_comparisons/le/out.sql
--rw-r--r--   0        0        0       91 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_comparisons/lt/out.sql
--rw-r--r--   0        0        0       92 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_comparisons/ne/out.sql
--rw-r--r--   0        0        0      291 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_cte_factor_distinct_but_equal/out.sql
--rw-r--r--   0        0        0       87 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_distinct/count_distinct/out.sql
--rw-r--r--   0        0        0      121 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_distinct/group_by_count_distinct/out.sql
--rw-r--r--   0        0        0      124 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_distinct/projection_distinct/out.sql
--rw-r--r--   0        0        0      104 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_distinct/single_column_projection_distinct/out.sql
--rw-r--r--   0        0        0       54 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_distinct/table_distinct/out.sql
--rw-r--r--   0        0        0      179 2024-03-22 20:15:42.647352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_exists/e1.sql
--rw-r--r--   0        0        0      239 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_exists/e2.sql
--rw-r--r--   0        0        0      217 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_filter_group_by_agg_with_same_name/out.sql
--rw-r--r--   0        0        0      704 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_gh_1045/out.sql
--rw-r--r--   0        0        0       78 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_isnull_notnull/isnull/out.sql
--rw-r--r--   0        0        0       82 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_isnull_notnull/notnull/out.sql
--rw-r--r--   0        0        0      490 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_join_just_materialized/out.sql
--rw-r--r--   0        0        0      250 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_joins/inner/out.sql
--rw-r--r--   0        0        0      191 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_joins/inner_select/out.sql
--rw-r--r--   0        0        0      255 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_joins/left/out.sql
--rw-r--r--   0        0        0      196 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_joins/left_select/out.sql
--rw-r--r--   0        0        0      255 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_joins/outer/out.sql
--rw-r--r--   0        0        0      196 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_joins/outer_select/out.sql
--rw-r--r--   0        0        0       40 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_limit/expr_fn0/out.sql
--rw-r--r--   0        0        0       49 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_limit/expr_fn1/out.sql
--rw-r--r--   0        0        0      131 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_limit_filter/out.sql
--rw-r--r--   0        0        0      167 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_limit_subquery/out.sql
--rw-r--r--   0        0        0      512 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_lower_projection_sort_key/decompiled.py
--rw-r--r--   0        0        0      405 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_lower_projection_sort_key/out.sql
--rw-r--r--   0        0        0      330 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_multi_join/out.sql
--rw-r--r--   0        0        0      100 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_mutate_filter_join_no_cross_join/out.sql
--rw-r--r--   0        0        0       91 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_named_expr/out.sql
--rw-r--r--   0        0        0      105 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_negate/out.sql
--rw-r--r--   0        0        0      986 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_no_cart_join/out.sql
--rw-r--r--   0        0        0     1517 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_no_cartesian_join/out.sql
--rw-r--r--   0        0        0      319 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_no_cross_join/out.sql
--rw-r--r--   0        0        0      205 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_not_exists/out.sql
--rw-r--r--   0        0        0      108 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_order_by/column/out.sql
--rw-r--r--   0        0        0      108 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_order_by/random/out.sql
--rw-r--r--   0        0        0      115 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_order_by_expr/out.sql
--rw-r--r--   0        0        0      238 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_searched_case/out.sql
--rw-r--r--   0        0        0      457 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_self_reference_in_not_exists/anti.sql
--rw-r--r--   0        0        0      431 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_self_reference_in_not_exists/semi.sql
--rw-r--r--   0        0        0      146 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_self_reference_join/out.sql
--rw-r--r--   0        0        0      118 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_simple_case/out.sql
--rw-r--r--   0        0        0      206 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_sort_aggregation_translation_failure/out.sql
--rw-r--r--   0        0        0      231 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_subquery_aliased/out.sql
--rw-r--r--   0        0        0      349 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_where_correlated_subquery/out.sql
--rw-r--r--   0        0        0      699 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_where_correlated_subquery_with_join/out.sql
--rw-r--r--   0        0        0      198 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_where_simple_comparisons/decompiled.py
--rw-r--r--   0        0        0      177 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_where_simple_comparisons/out.sql
--rw-r--r--   0        0        0      162 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_where_uncorrelated_subquery/out.sql
--rw-r--r--   0        0        0       94 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_aggregate/having_count/out.sql
--rw-r--r--   0        0        0       94 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_aggregate/having_sum/out.sql
--rw-r--r--   0        0        0       70 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_aggregate/single/out.sql
--rw-r--r--   0        0        0       88 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_aggregate/two/out.sql
--rw-r--r--   0        0        0       77 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_between/out.sql
--rw-r--r--   0        0        0       86 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_boolean_conjunction/and/out.sql
--rw-r--r--   0        0        0       85 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_boolean_conjunction/or/out.sql
--rw-r--r--   0        0        0      168 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_coalesce/out.sql
--rw-r--r--   0        0        0       64 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_comparisons/eq/out.sql
--rw-r--r--   0        0        0       65 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_comparisons/ge/out.sql
--rw-r--r--   0        0        0       64 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_comparisons/gt/out.sql
--rw-r--r--   0        0        0       65 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_comparisons/le/out.sql
--rw-r--r--   0        0        0       64 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_comparisons/lt/out.sql
--rw-r--r--   0        0        0       65 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_comparisons/ne/out.sql
--rw-r--r--   0        0        0      167 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_cte_factor_distinct_but_equal/out.sql
--rw-r--r--   0        0        0       77 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_distinct/count_distinct/out.sql
--rw-r--r--   0        0        0      107 2024-03-22 20:15:42.651352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_distinct/group_by_count_distinct/out.sql
--rw-r--r--   0        0        0       76 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_distinct/projection_distinct/out.sql
--rw-r--r--   0        0        0       62 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_distinct/single_column_projection_distinct/out.sql
--rw-r--r--   0        0        0      252 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_distinct/table_distinct/out.sql
--rw-r--r--   0        0        0      161 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_exists/e1.sql
--rw-r--r--   0        0        0      181 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_exists/e2.sql
--rw-r--r--   0        0        0      183 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_filter_group_by_agg_with_same_name/out.sql
--rw-r--r--   0        0        0      631 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_gh_1045/out.sql
--rw-r--r--   0        0        0       68 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_isnull_notnull/isnull/out.sql
--rw-r--r--   0        0        0       72 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_isnull_notnull/notnull/out.sql
--rw-r--r--   0        0        0      390 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_join_just_materialized/out.sql
--rw-r--r--   0        0        0      200 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_joins/inner/out.sql
--rw-r--r--   0        0        0      153 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_joins/inner_select/out.sql
--rw-r--r--   0        0        0      211 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_joins/left/out.sql
--rw-r--r--   0        0        0      164 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_joins/left_select/out.sql
--rw-r--r--   0        0        0      211 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_joins/outer/out.sql
--rw-r--r--   0        0        0      164 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_joins/outer_select/out.sql
--rw-r--r--   0        0        0       73 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_limit/expr_fn0/out.sql
--rw-r--r--   0        0        0       82 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_limit/expr_fn1/out.sql
--rw-r--r--   0        0        0       90 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_limit_filter/out.sql
--rw-r--r--   0        0        0      197 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_limit_subquery/out.sql
--rw-r--r--   0        0        0      489 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_lower_projection_sort_key/decompiled.py
--rw-r--r--   0        0        0      459 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_lower_projection_sort_key/out.sql
--rw-r--r--   0        0        0      252 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_multi_join/out.sql
--rw-r--r--   0        0        0      173 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_mutate_filter_join_no_cross_join/out.sql
--rw-r--r--   0        0        0       64 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_named_expr/out.sql
--rw-r--r--   0        0        0       65 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_negate/out.sql
--rw-r--r--   0        0        0      592 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_no_cart_join/out.sql
--rw-r--r--   0        0        0      237 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_no_cross_join/out.sql
--rw-r--r--   0        0        0      187 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_not_exists/out.sql
--rw-r--r--   0        0        0       96 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_order_by/column/out.sql
--rw-r--r--   0        0        0      100 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_order_by/random/out.sql
--rw-r--r--   0        0        0      155 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_order_by_expr/out.sql
--rw-r--r--   0        0        0      176 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_searched_case/out.sql
--rw-r--r--   0        0        0      399 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_self_reference_in_not_exists/anti.sql
--rw-r--r--   0        0        0      373 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_self_reference_in_not_exists/semi.sql
--rw-r--r--   0        0        0      108 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_self_reference_join/out.sql
--rw-r--r--   0        0        0      108 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_simple_case/out.sql
--rw-r--r--   0        0        0      192 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_sort_aggregation_translation_failure/out.sql
--rw-r--r--   0        0        0      203 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_subquery_aliased/out.sql
--rw-r--r--   0        0        0      840 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_tpc_h11/out.sql
--rw-r--r--   0        0        0      344 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_tpc_h17/out.sql
--rw-r--r--   0        0        0      183 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_where_correlated_subquery/out.sql
--rw-r--r--   0        0        0      767 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_where_correlated_subquery_with_join/out.sql
--rw-r--r--   0        0        0      200 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_where_simple_comparisons/decompiled.py
--rw-r--r--   0        0        0      101 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_where_simple_comparisons/out.sql
--rw-r--r--   0        0        0      130 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_where_uncorrelated_subquery/out.sql
--rw-r--r--   0        0        0     7554 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/test_compiler.py
--rw-r--r--   0        0        0    26440 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/test_select_sql.py
--rw-r--r--   0        0        0    16629 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/sql/test_sql.py
--rw-r--r--   0        0        0    53832 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_aggregation.py
--rw-r--r--   0        0        0     3980 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_api.py
--rw-r--r--   0        0        0    39186 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_array.py
--rw-r--r--   0        0        0     4261 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_asof_join.py
--rw-r--r--   0        0        0      982 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_binary.py
--rw-r--r--   0        0        0    48297 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_client.py
--rw-r--r--   0        0        0     1126 2024-03-22 20:15:42.655352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_column.py
--rw-r--r--   0        0        0     3916 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_dataframe_interchange.py
--rw-r--r--   0        0        0    10230 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_dot_sql.py
--rw-r--r--   0        0        0     1439 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_examples.py
--rw-r--r--   0        0        0    16675 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_export.py
--rw-r--r--   0        0        0    57186 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_generic.py
--rw-r--r--   0        0        0     2960 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_interactive.py
--rw-r--r--   0        0        0    12333 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_join.py
--rw-r--r--   0        0        0     2759 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_json.py
--rw-r--r--   0        0        0    10926 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_map.py
--rw-r--r--   0        0        0     1541 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_markers.py
--rw-r--r--   0        0        0     4046 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_network.py
--rw-r--r--   0        0        0    52300 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_numeric.py
--rw-r--r--   0        0        0     6498 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_param.py
--rw-r--r--   0        0        0    14141 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_register.py
--rw-r--r--   0        0        0     8795 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_set_ops.py
--rw-r--r--   0        0        0     5635 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_sql.py
--rw-r--r--   0        0        0    34670 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_string.py
--rw-r--r--   0        0        0     4840 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_struct.py
--rw-r--r--   0        0        0    82007 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_temporal.py
--rw-r--r--   0        0        0     4372 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_timecontext.py
--rw-r--r--   0        0        0     5122 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_udf.py
--rw-r--r--   0        0        0     1844 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_uuid.py
--rw-r--r--   0        0        0    25106 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_vectorized_udf.py
--rw-r--r--   0        0        0    40444 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/test_window.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/__init__.py
--rw-r--r--   0        0        0     4113 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/conftest.py
--rw-r--r--   0        0        0      545 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h01.sql
--rw-r--r--   0        0        0      841 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h02.sql
--rw-r--r--   0        0        0      468 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h03.sql
--rw-r--r--   0        0        0      408 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h04.sql
--rw-r--r--   0        0        0      522 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h05.sql
--rw-r--r--   0        0        0      243 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h06.sql
--rw-r--r--   0        0        0      954 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h07.sql
--rw-r--r--   0        0        0      950 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h08.sql
--rw-r--r--   0        0        0      678 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h09.sql
--rw-r--r--   0        0        0      580 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h10.sql
--rw-r--r--   0        0        0      582 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h11.sql
--rw-r--r--   0        0        0      704 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h12.sql
--rw-r--r--   0        0        0      366 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h13.sql
--rw-r--r--   0        0        0      364 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h14.sql
--rw-r--r--   0        0        0      951 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h15.sql
--rw-r--r--   0        0        0      553 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h16.sql
--rw-r--r--   0        0        0      329 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h17.sql
--rw-r--r--   0        0        0      555 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h18.sql
--rw-r--r--   0        0        0     1043 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h19.sql
--rw-r--r--   0        0        0      909 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h20.sql
--rw-r--r--   0        0        0      803 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h21.sql
--rw-r--r--   0        0        0      807 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h22.sql
--rw-r--r--   0        0        0     1470 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h01/test_tpc_h01/duckdb/h01.sql
--rw-r--r--   0        0        0     1728 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h01/test_tpc_h01/snowflake/h01.sql
--rw-r--r--   0        0        0     1607 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h01/test_tpc_h01/trino/h01.sql
--rw-r--r--   0        0        0     3009 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h02/test_tpc_h02/duckdb/h02.sql
--rw-r--r--   0        0        0     5688 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h02/test_tpc_h02/snowflake/h02.sql
--rw-r--r--   0        0        0     5022 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h02/test_tpc_h02/trino/h02.sql
--rw-r--r--   0        0        0     2552 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h03/test_tpc_h03/duckdb/h03.sql
--rw-r--r--   0        0        0     4324 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h03/test_tpc_h03/snowflake/h03.sql
--rw-r--r--   0        0        0     3967 2024-03-22 20:15:42.659352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h03/test_tpc_h03/trino/h03.sql
--rw-r--r--   0        0        0      854 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h04/test_tpc_h04/duckdb/h04.sql
--rw-r--r--   0        0        0     1382 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h04/test_tpc_h04/snowflake/h04.sql
--rw-r--r--   0        0        0     1243 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h04/test_tpc_h04/trino/h04.sql
--rw-r--r--   0        0        0     3449 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h05/test_tpc_h05/duckdb/h05.sql
--rw-r--r--   0        0        0     6105 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h05/test_tpc_h05/snowflake/h05.sql
--rw-r--r--   0        0        0     5531 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h05/test_tpc_h05/trino/h05.sql
--rw-r--r--   0        0        0      733 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h06/test_tpc_h06/duckdb/h06.sql
--rw-r--r--   0        0        0      999 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h06/test_tpc_h06/snowflake/h06.sql
--rw-r--r--   0        0        0      962 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h06/test_tpc_h06/trino/h06.sql
--rw-r--r--   0        0        0     1785 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h07/test_tpc_h07/duckdb/h07.sql
--rw-r--r--   0        0        0     4153 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h07/test_tpc_h07/snowflake/h07.sql
--rw-r--r--   0        0        0     3651 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h07/test_tpc_h07/trino/h07.sql
--rw-r--r--   0        0        0     1611 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h08/test_tpc_h08/duckdb/h08.sql
--rw-r--r--   0        0        0     4614 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h08/test_tpc_h08/snowflake/h08.sql
--rw-r--r--   0        0        0     3963 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h08/test_tpc_h08/trino/h08.sql
--rw-r--r--   0        0        0     1257 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h09/test_tpc_h09/duckdb/h09.sql
--rw-r--r--   0        0        0     3990 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h09/test_tpc_h09/snowflake/h09.sql
--rw-r--r--   0        0        0     3410 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h09/test_tpc_h09/trino/h09.sql
--rw-r--r--   0        0        0     2981 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h10/test_tpc_h10/duckdb/h10.sql
--rw-r--r--   0        0        0     5069 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h10/test_tpc_h10/snowflake/h10.sql
--rw-r--r--   0        0        0     4641 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h10/test_tpc_h10/trino/h10.sql
--rw-r--r--   0        0        0     2806 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h11/test_tpc_h11/duckdb/h11.sql
--rw-r--r--   0        0        0     4797 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h11/test_tpc_h11/snowflake/h11.sql
--rw-r--r--   0        0        0     4370 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h11/test_tpc_h11/trino/h11.sql
--rw-r--r--   0        0        0     2413 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h12/test_tpc_h12/duckdb/h12.sql
--rw-r--r--   0        0        0     3560 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h12/test_tpc_h12/snowflake/h12.sql
--rw-r--r--   0        0        0     3314 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h12/test_tpc_h12/trino/h12.sql
--rw-r--r--   0        0        0     1003 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h13/test_tpc_h13/duckdb/h13.sql
--rw-r--r--   0        0        0     1954 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h13/test_tpc_h13/snowflake/h13.sql
--rw-r--r--   0        0        0     1705 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h13/test_tpc_h13/trino/h13.sql
--rw-r--r--   0        0        0     1800 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h14/test_tpc_h14/duckdb/h14.sql
--rw-r--r--   0        0        0     2906 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h14/test_tpc_h14/snowflake/h14.sql
--rw-r--r--   0        0        0     2702 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h14/test_tpc_h14/trino/h14.sql
--rw-r--r--   0        0        0     2656 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h15/test_tpc_h15/duckdb/h15.sql
--rw-r--r--   0        0        0     3962 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h15/test_tpc_h15/snowflake/h15.sql
--rw-r--r--   0        0        0     3568 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h15/test_tpc_h15/trino/h15.sql
--rw-r--r--   0        0        0     1759 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h16/test_tpc_h16/duckdb/h16.sql
--rw-r--r--   0        0        0     2457 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h16/test_tpc_h16/snowflake/h16.sql
--rw-r--r--   0        0        0     2255 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h16/test_tpc_h16/trino/h16.sql
--rw-r--r--   0        0        0     2301 2024-03-22 20:15:42.663352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h17/test_tpc_h17/duckdb/h17.sql
--rw-r--r--   0        0        0     3785 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h17/test_tpc_h17/snowflake/h17.sql
--rw-r--r--   0        0        0     3466 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h17/test_tpc_h17/trino/h17.sql
--rw-r--r--   0        0        0     2788 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h18/test_tpc_h18/duckdb/h18.sql
--rw-r--r--   0        0        0     4477 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h18/test_tpc_h18/snowflake/h18.sql
--rw-r--r--   0        0        0     4114 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h18/test_tpc_h18/trino/h18.sql
--rw-r--r--   0        0        0     3630 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h19/test_tpc_h19/duckdb/h19.sql
--rw-r--r--   0        0        0     4622 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h19/test_tpc_h19/snowflake/h19.sql
--rw-r--r--   0        0        0     4396 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h19/test_tpc_h19/trino/h19.sql
--rw-r--r--   0        0        0     1769 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h20/test_tpc_h20/duckdb/h20.sql
--rw-r--r--   0        0        0     2984 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h20/test_tpc_h20/snowflake/h20.sql
--rw-r--r--   0        0        0     2644 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h20/test_tpc_h20/trino/h20.sql
--rw-r--r--   0        0        0     1773 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h21/test_tpc_h21/duckdb/h21.sql
--rw-r--r--   0        0        0     3652 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h21/test_tpc_h21/snowflake/h21.sql
--rw-r--r--   0        0        0     3229 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h21/test_tpc_h21/trino/h21.sql
--rw-r--r--   0        0        0     1976 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h22/test_tpc_h22/duckdb/h22.sql
--rw-r--r--   0        0        0     2252 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h22/test_tpc_h22/snowflake/h22.sql
--rw-r--r--   0        0        0     2076 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h22/test_tpc_h22/trino/h22.sql
--rw-r--r--   0        0        0     1445 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h01.py
--rw-r--r--   0        0        0     1417 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h02.py
--rw-r--r--   0        0        0      778 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h03.py
--rw-r--r--   0        0        0      663 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h04.py
--rw-r--r--   0        0        0     1046 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h05.py
--rw-r--r--   0        0        0      666 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h06.py
--rw-r--r--   0        0        0     1413 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h07.py
--rw-r--r--   0        0        0     1516 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h08.py
--rw-r--r--   0        0        0     1100 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h09.py
--rw-r--r--   0        0        0     1019 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h10.py
--rw-r--r--   0        0        0      908 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h11.py
--rw-r--r--   0        0        0     1337 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h12.py
--rw-r--r--   0        0        0      775 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h13.py
--rw-r--r--   0        0        0      689 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h14.py
--rw-r--r--   0        0        0      986 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h15.py
--rw-r--r--   0        0        0     1098 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h16.py
--rw-r--r--   0        0        0      850 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h17.py
--rw-r--r--   0        0        0     1025 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h18.py
--rw-r--r--   0        0        0     1758 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h19.py
--rw-r--r--   0        0        0     1161 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h20.py
--rw-r--r--   0        0        0     1451 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h21.py
--rw-r--r--   0        0        0     1085 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h22.py
--rw-r--r--   0        0        0    17392 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/trino/__init__.py
--rw-r--r--   0        0        0    15984 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/trino/compiler.py
--rw-r--r--   0        0        0      754 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/trino/converter.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/trino/tests/__init__.py
--rw-r--r--   0        0        0     5875 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/trino/tests/conftest.py
--rw-r--r--   0        0        0      174 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/trino/tests/snapshots/test_client/test_builtin_scalar_udf/result.txt
--rw-r--r--   0        0        0     4524 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/trino/tests/test_client.py
--rw-r--r--   0        0        0     2239 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/backends/trino/tests/test_datatypes.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/common/__init__.py
--rw-r--r--   0        0        0    19763 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/common/annotations.py
--rw-r--r--   0        0        0     7859 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/common/bases.py
--rw-r--r--   0        0        0     4706 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/common/caching.py
--rw-r--r--   0        0        0    10691 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/common/collections.py
--rw-r--r--   0        0        0    18211 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/common/deferred.py
--rw-r--r--   0        0        0     7283 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/common/dispatch.py
--rw-r--r--   0        0        0    25639 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/common/egraph.py
--rw-r--r--   0        0        0     4225 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/common/exceptions.py
--rw-r--r--   0        0        0    22452 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/common/graph.py
--rw-r--r--   0        0        0     8146 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/common/grounds.py
--rw-r--r--   0        0        0     1395 2024-03-22 20:15:42.667352 turntable_spoonbill-9.0.4/ibis/common/numeric.py
--rw-r--r--   0        0        0    49056 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/patterns.py
--rw-r--r--   0        0        0     6684 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/temporal.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/__init__.py
--rw-r--r--   0        0        0      161 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/conftest.py
--rw-r--r--   0        0        0       96 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/snapshots/test_annotations/test_annotated_function_without_decoration/error.txt
--rw-r--r--   0        0        0      114 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/snapshots/test_annotations/test_signature_from_callable_with_keyword_only_arguments/too_many_positional_arguments.txt
--rw-r--r--   0        0        0      131 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/snapshots/test_annotations/test_signature_from_callable_with_positional_only_arguments/parameter_is_positional_only.txt
--rw-r--r--   0        0        0      375 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/snapshots/test_grounds/test_error_message/error_message.txt
--rw-r--r--   0        0        0      385 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/snapshots/test_grounds/test_error_message/error_message_py311.txt
--rw-r--r--   0        0        0    13351 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_annotations.py
--rw-r--r--   0        0        0     7544 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_bases.py
--rw-r--r--   0        0        0    12557 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_collections.py
--rw-r--r--   0        0        0    15334 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_deferred.py
--rw-r--r--   0        0        0     4578 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_dispatch.py
--rw-r--r--   0        0        0    12986 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_egraph.py
--rw-r--r--   0        0        0    11228 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_graph.py
--rw-r--r--   0        0        0     1405 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_graph_benchmarks.py
--rw-r--r--   0        0        0    26781 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_grounds.py
--rw-r--r--   0        0        0      937 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_grounds_benchmarks.py
--rw-r--r--   0        0        0     1011 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_grounds_py310.py
--rw-r--r--   0        0        0     2314 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_numeric.py
--rw-r--r--   0        0        0    39898 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_patterns.py
--rw-r--r--   0        0        0     8384 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_temporal.py
--rw-r--r--   0        0        0     3698 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/tests/test_typing.py
--rw-r--r--   0        0        0     6963 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/common/typing.py
--rw-r--r--   0        0        0     6038 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/config.py
--rw-r--r--   0        0        0     1356 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/conftest.py
--rw-r--r--   0        0        0      758 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/examples/CITATIONS.md
--rw-r--r--   0        0        0     4689 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/examples/__init__.py
--rw-r--r--   0        0        0    38919 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/examples/metadata.json
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/examples/tests/__init__.py
--rw-r--r--   0        0        0     2358 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/examples/tests/test_examples.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/__init__.py
--rw-r--r--   0        0        0      896 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/analysis.py
--rw-r--r--   0        0        0    65639 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/api.py
--rw-r--r--   0        0        0    11712 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/builders.py
--rw-r--r--   0        0        0     1327 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/datashape.py
--rw-r--r--   0        0        0      523 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/datatypes/__init__.py
--rw-r--r--   0        0        0     5036 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/datatypes/cast.py
--rw-r--r--   0        0        0    29349 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/datatypes/core.py
--rw-r--r--   0        0        0     5992 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/datatypes/parse.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/datatypes/tests/__init__.py
--rw-r--r--   0        0        0     3110 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/datatypes/tests/test_cast.py
--rw-r--r--   0        0        0    17967 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/datatypes/tests/test_core.py
--rw-r--r--   0        0        0     8028 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/datatypes/tests/test_parse.py
--rw-r--r--   0        0        0    13969 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/datatypes/tests/test_value.py
--rw-r--r--   0        0        0    11347 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/datatypes/value.py
--rw-r--r--   0        0        0    12321 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/decompile.py
--rw-r--r--   0        0        0    10822 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/format.py
--rw-r--r--   0        0        0     1247 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/operations/__init__.py
--rw-r--r--   0        0        0     1610 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/operations/analytic.py
--rw-r--r--   0        0        0     4265 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/operations/arrays.py
--rw-r--r--   0        0        0     5188 2024-03-22 20:15:42.671352 turntable_spoonbill-9.0.4/ibis/expr/operations/core.py
--rw-r--r--   0        0        0     6029 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/generic.py
--rw-r--r--   0        0        0    10593 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/geospatial.py
--rw-r--r--   0        0        0     1427 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/histograms.py
--rw-r--r--   0        0        0      579 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/json.py
--rw-r--r--   0        0        0     3220 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/logical.py
--rw-r--r--   0        0        0     1523 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/maps.py
--rw-r--r--   0        0        0     5933 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/numeric.py
--rw-r--r--   0        0        0     7152 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/reductions.py
--rw-r--r--   0        0        0    10149 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/relations.py
--rw-r--r--   0        0        0     1270 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/sortkeys.py
--rw-r--r--   0        0        0     5352 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/strings.py
--rw-r--r--   0        0        0     1229 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/structs.py
--rw-r--r--   0        0        0     1832 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/subqueries.py
--rw-r--r--   0        0        0     6658 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/temporal.py
--rw-r--r--   0        0        0     1997 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/temporal_windows.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/__init__.py
--rw-r--r--   0        0        0      158 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/conftest.py
--rw-r--r--   0        0        0      166 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/snapshots/test_generic/test_error_message_when_constructing_literal/call0-missing_a_required_argument/missing_a_required_argument.txt
--rw-r--r--   0        0        0      187 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/snapshots/test_generic/test_error_message_when_constructing_literal/call1-too_many_positional_arguments/too_many_positional_arguments.txt
--rw-r--r--   0        0        0      204 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/snapshots/test_generic/test_error_message_when_constructing_literal/call2-got_an_unexpected_keyword/got_an_unexpected_keyword.txt
--rw-r--r--   0        0        0      215 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/snapshots/test_generic/test_error_message_when_constructing_literal/call3-multiple_values_for_argument/multiple_values_for_argument.txt
--rw-r--r--   0        0        0      216 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/snapshots/test_generic/test_error_message_when_constructing_literal/call4-invalid_dtype/invalid_dtype.txt
--rw-r--r--   0        0        0       46 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/snapshots/test_generic/test_error_message_when_constructing_literal/call5-unable_to_normalize/unable_to_normalize.txt
--rw-r--r--   0        0        0     5645 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/test_core.py
--rw-r--r--   0        0        0      789 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/test_core_py310.py
--rw-r--r--   0        0        0     5054 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/test_generic.py
--rw-r--r--   0        0        0     3058 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/test_rewrites.py
--rw-r--r--   0        0        0      432 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/test_sortkeys.py
--rw-r--r--   0        0        0      909 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/tests/test_structs.py
--rw-r--r--   0        0        0    16316 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/udf.py
--rw-r--r--   0        0        0     1138 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/vectorized.py
--rw-r--r--   0        0        0     3790 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/operations/window.py
--rw-r--r--   0        0        0     8966 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/rewrites.py
--rw-r--r--   0        0        0     4393 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/rules.py
--rw-r--r--   0        0        0     8490 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/schema.py
--rw-r--r--   0        0        0    10410 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/sql.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/__init__.py
--rw-r--r--   0        0        0    11451 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/conftest.py
--rw-r--r--   0        0        0      254 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_aggregate_arg_names/repr.txt
--rw-r--r--   0        0        0      116 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_argument_repr_shows_name/repr.txt
--rw-r--r--   0        0        0      396 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_asof_join/repr.txt
--rw-r--r--   0        0        0      206 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_complex_repr/repr.txt
--rw-r--r--   0        0        0      394 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_destruct_selection/repr.txt
--rw-r--r--   0        0        0       79 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_fillna/fillna_dict_repr.txt
--rw-r--r--   0        0        0      105 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_fillna/fillna_int_repr.txt
--rw-r--r--   0        0        0      109 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_fillna/fillna_str_repr.txt
--rw-r--r--   0        0        0       28 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_format_dummy_table/repr.txt
--rw-r--r--   0        0        0      153 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_format_in_memory_table/repr.txt
--rw-r--r--   0        0        0      478 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_format_multiple_join_with_projection/repr.txt
--rw-r--r--   0        0        0      479 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_format_new_relational_operation/repr.txt
--rw-r--r--   0        0        0      204 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_format_projection/repr.txt
--rw-r--r--   0        0        0      155 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_format_table_column/repr.txt
--rw-r--r--   0        0        0       32 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_format_table_with_empty_schema/repr.txt
--rw-r--r--   0        0        0      315 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_memoize_filtered_table/repr.txt
--rw-r--r--   0        0        0      455 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_memoize_filtered_tables_in_join/repr.txt
--rw-r--r--   0        0        0      172 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_named_value_expr_show_name/repr.txt
--rw-r--r--   0        0        0      161 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_named_value_expr_show_name/repr2.txt
--rw-r--r--   0        0        0      153 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_repr_exact/repr.txt
--rw-r--r--   0        0        0       88 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_same_column_multiple_aliases/repr.txt
--rw-r--r--   0        0        0       26 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_schema_truncation/repr1.txt
--rw-r--r--   0        0        0      116 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_schema_truncation/repr8.txt
--rw-r--r--   0        0        0      235 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_schema_truncation/repr_all.txt
--rw-r--r--   0        0        0       74 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_table_count_expr/cnt_repr.txt
--rw-r--r--   0        0        0      242 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_table_count_expr/join_repr.txt
--rw-r--r--   0        0        0      194 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_table_count_expr/union_repr.txt
--rw-r--r--   0        0        0      168 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_table_type_output/repr.txt
--rw-r--r--   0        0        0      489 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_two_inner_joins/repr.txt
--rw-r--r--   0        0        0      134 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_window_group_by/repr.txt
--rw-r--r--   0        0        0      164 2024-03-22 20:15:42.675352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_format/test_window_no_group_by/repr.txt
--rw-r--r--   0        0        0     1041 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_aggregation_with_multiple_joins/decompiled.py
--rw-r--r--   0        0        0      341 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_aggregation/decompiled.py
--rw-r--r--   0        0        0      726 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_aggregation_with_join/decompiled.py
--rw-r--r--   0        0        0      885 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_join/inner/decompiled.py
--rw-r--r--   0        0        0      884 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_join/left/decompiled.py
--rw-r--r--   0        0        0      885 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_join/right/decompiled.py
--rw-r--r--   0        0        0      280 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_projection/decompiled.py
--rw-r--r--   0        0        0      423 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_in_clause/decompiled.py
--rw-r--r--   0        0        0      884 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_join_with_filter/decompiled.py
--rw-r--r--   0        0        0      920 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_multiple_joins/decompiled.py
--rw-r--r--   0        0        0      531 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_scalar_subquery/decompiled.py
--rw-r--r--   0        0        0      309 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_simple_reduction/decompiled.py
--rw-r--r--   0        0        0      210 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_simple_select_count/decompiled.py
--rw-r--r--   0        0        0      133 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_table_alias/decompiled.py
--rw-r--r--   0        0        0     4616 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/test_api.py
--rw-r--r--   0        0        0     2006 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/test_datashape.py
--rw-r--r--   0        0        0     2288 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/test_decompile.py
--rw-r--r--   0        0        0     1023 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/test_dereference.py
--rw-r--r--   0        0        0    11559 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/test_format.py
--rw-r--r--   0        0        0    47733 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/test_newrels.py
--rw-r--r--   0        0        0     3216 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/test_reductions.py
--rw-r--r--   0        0        0     2721 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/test_rewrites.py
--rw-r--r--   0        0        0    13287 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/test_schema.py
--rw-r--r--   0        0        0     4095 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/test_sql.py
--rw-r--r--   0        0        0     4676 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/tests/test_visualize.py
--rw-r--r--   0        0        0      931 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/__init__.py
--rw-r--r--   0        0        0    50191 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/arrays.py
--rw-r--r--   0        0        0      819 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/binary.py
--rw-r--r--   0        0        0      271 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/collections.py
--rw-r--r--   0        0        0    23300 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/core.py
--rw-r--r--   0        0        0     5402 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/dataframe_interchange.py
--rw-r--r--   0        0        0    76495 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/generic.py
--rw-r--r--   0        0        0    66172 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/geospatial.py
--rw-r--r--   0        0        0    11482 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/groupby.py
--rw-r--r--   0        0        0      446 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/inet.py
--rw-r--r--   0        0        0    18273 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/joins.py
--rw-r--r--   0        0        0     5142 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/json.py
--rw-r--r--   0        0        0    20054 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/logical.py
--rw-r--r--   0        0        0    17251 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/maps.py
--rw-r--r--   0        0        0    37520 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/numeric.py
--rw-r--r--   0        0        0    12899 2024-03-22 20:15:42.679352 turntable_spoonbill-9.0.4/ibis/expr/types/pretty.py
--rw-r--r--   0        0        0   243607 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/expr/types/relations.py
--rw-r--r--   0        0        0    57776 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/expr/types/strings.py
--rw-r--r--   0        0        0    14388 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/expr/types/structs.py
--rw-r--r--   0        0        0    31164 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/expr/types/temporal.py
--rw-r--r--   0        0        0     4743 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/expr/types/temporal_windows.py
--rw-r--r--   0        0        0      173 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/expr/types/typing.py
--rw-r--r--   0        0        0      276 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/expr/types/uuid.py
--rw-r--r--   0        0        0     7259 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/expr/visualize.py
--rw-r--r--   0        0        0     6772 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/formats/__init__.py
--rw-r--r--   0        0        0     3551 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/formats/numpy.py
--rw-r--r--   0        0        0    13701 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/formats/pandas.py
--rw-r--r--   0        0        0     5896 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/formats/polars.py
--rw-r--r--   0        0        0     9661 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/formats/pyarrow.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/formats/tests/__init__.py
--rw-r--r--   0        0        0     4370 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/formats/tests/test_numpy.py
--rw-r--r--   0        0        0    14006 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/formats/tests/test_pandas.py
--rw-r--r--   0        0        0     4787 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/formats/tests/test_polars.py
--rw-r--r--   0        0        0     6829 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/formats/tests/test_pyarrow.py
--rw-r--r--   0        0        0      235 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/interactive.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/legacy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/legacy/udf/__init__.py
--rw-r--r--   0        0        0     2149 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/legacy/udf/validate.py
--rw-r--r--   0        0        0    11957 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/legacy/udf/vectorized.py
--rw-r--r--   0        0        0    24142 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/selectors.py
--rw-r--r--   0        0        0     2236 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/streamlit/__init__.py
--rw-r--r--   0        0        0      609 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/benchmarks/__init__.py
--rw-r--r--   0        0        0    21311 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/benchmarks/test_benchmarks.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/__init__.py
--rw-r--r--   0        0        0     1729 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/conftest.py
--rw-r--r--   0        0        0     2962 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/mocks.py
--rw-r--r--   0        0        0     1984 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/snapshots/test_format_sql_operations/test_format_sql_query_result/repr.txt
--rw-r--r--   0        0        0      421 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/snapshots/test_format_sql_operations/test_memoize_database_table/repr.txt
--rw-r--r--   0        0        0     1276 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/snapshots/test_format_sql_operations/test_memoize_insert_sort_key/repr.txt
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/snapshots/test_interactive/test_default_limit/out.sql
--rw-r--r--   0        0        0       66 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/snapshots/test_interactive/test_disable_query_limit/out.sql
--rw-r--r--   0        0        0      105 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/snapshots/test_interactive/test_respect_set_limit/out.sql
--rw-r--r--   0        0        0     8899 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_analysis.py
--rw-r--r--   0        0        0     2844 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_analytics.py
--rw-r--r--   0        0        0     4470 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_case.py
--rw-r--r--   0        0        0     4125 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_decimal.py
--rw-r--r--   0        0        0     1643 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_format_sql_operations.py
--rw-r--r--   0        0        0      769 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_geospatial.py
--rw-r--r--   0        0        0     5008 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_literal.py
--rw-r--r--   0        0        0     1599 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_pipe.py
--rw-r--r--   0        0        0     6127 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_pretty_repr.py
--rw-r--r--   0        0        0     3250 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_relocate.py
--rw-r--r--   0        0        0    14328 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_selectors.py
--rw-r--r--   0        0        0     1243 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_set_operations.py
--rw-r--r--   0        0        0     6326 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_sql_builtins.py
--rw-r--r--   0        0        0     3549 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_string.py
--rw-r--r--   0        0        0     2641 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_struct.py
--rw-r--r--   0        0        0    60536 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_table.py
--rw-r--r--   0        0        0    26786 2024-03-22 20:15:42.683352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_temporal.py
--rw-r--r--   0        0        0     2703 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_temporal_windows.py
--rw-r--r--   0        0        0     5714 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_timestamp.py
--rw-r--r--   0        0        0     4482 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_udf.py
--rw-r--r--   0        0        0      181 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_uuid.py
--rw-r--r--   0        0        0    49864 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_value_exprs.py
--rw-r--r--   0        0        0    16910 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_window_frames.py
--rw-r--r--   0        0        0     2008 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/expr/test_window_functions.py
--rw-r--r--   0        0        0     7581 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/strategies.py
--rw-r--r--   0        0        0     2029 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/test_api.py
--rw-r--r--   0        0        0      401 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/test_config.py
--rw-r--r--   0        0        0     5025 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/test_strategies.py
--rw-r--r--   0        0        0     3741 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/test_util.py
--rw-r--r--   0        0        0      226 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/test_version.py
--rw-r--r--   0        0        0     1898 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/tests/util.py
--rw-r--r--   0        0        0    17130 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/ibis/util.py
--rw-r--r--   0        0        0    18419 2024-03-22 20:15:42.687352 turntable_spoonbill-9.0.4/pyproject.toml
--rw-r--r--   0        0        0    15934 1970-01-01 00:00:00.000000 turntable_spoonbill-9.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11346 2024-03-30 19:28:49.772058 turntable_spoonbill-9.0.5/LICENSE.txt
+-rw-r--r--   0        0        0    11115 2024-03-30 19:28:49.772058 turntable_spoonbill-9.0.5/README.md
+-rw-r--r--   0        0        0     4167 2024-03-30 19:28:49.884059 turntable_spoonbill-9.0.5/ibis/__init__.py
+-rw-r--r--   0        0        0    39475 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/__init__.py
+-rw-r--r--   0        0        0    43203 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/__init__.py
+-rw-r--r--   0        0        0     6319 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/client.py
+-rw-r--r--   0        0        0    27701 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/compiler.py
+-rw-r--r--   0        0        0      466 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/converter.py
+-rw-r--r--   0        0        0     2473 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/datatypes.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/__init__.py
+-rw-r--r--   0        0        0    10849 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/__init__.py
+-rw-r--r--   0        0        0     3206 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/conftest.py
+-rw-r--r--   0        0        0      146 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/snapshots/test_client/test_cross_project_query/out.sql
+-rw-r--r--   0        0        0      173 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/snapshots/test_client/test_multiple_project_queries/out.sql
+-rw-r--r--   0        0        0      155 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/snapshots/test_client/test_multiple_project_queries_database_api/out.sql
+-rw-r--r--   0        0        0      408 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/snapshots/test_client/test_subquery_scalar_params/out.sql
+-rw-r--r--   0        0        0    13227 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/test_client.py
+-rw-r--r--   0        0        0     6609 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/test_connect.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/udf/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/udf/snapshots/test_udf_execute/test_udf_with_struct/out.sql
+-rw-r--r--   0        0        0     4701 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/udf/test_udf_execute.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/__init__.py
+-rw-r--r--   0        0        0      196 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_approx/filter-approx_median/out.sql
+-rw-r--r--   0        0        0      166 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_approx/filter-approx_nunique/out.sql
+-rw-r--r--   0        0        0      122 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_approx/no_filter-approx_median/out.sql
+-rw-r--r--   0        0        0      120 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_approx/no_filter-approx_nunique/out.sql
+-rw-r--r--   0        0        0       77 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_binary/out.sql
+-rw-r--r--   0        0        0      143 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/filter-bit_and/out.sql
+-rw-r--r--   0        0        0      141 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/filter-bit_or/out.sql
+-rw-r--r--   0        0        0      143 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/filter-bit_xor/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/no_filter-bit_and/out.sql
+-rw-r--r--   0        0        0       85 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/no_filter-bit_or/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bit/no_filter-bit_xor/out.sql
+-rw-r--r--   0        0        0       98 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bool_reducers/mean/out.sql
+-rw-r--r--   0        0        0       97 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bool_reducers/sum/out.sql
+-rw-r--r--   0        0        0      253 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bool_reducers_where_conj/out.sql
+-rw-r--r--   0        0        0      144 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bool_reducers_where_simple/out.sql
+-rw-r--r--   0        0        0      249 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_bucket/out.sql
+-rw-r--r--   0        0        0      111 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_cast_float_to_int/out.sql
+-rw-r--r--   0        0        0       55 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_compile_toplevel/out.sql
+-rw-r--r--   0        0        0      130 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_cov/pop/out.sql
+-rw-r--r--   0        0        0      131 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_cov/sample/out.sql
+-rw-r--r--   0        0        0      106 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/date/index.sql
+-rw-r--r--   0        0        0      107 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/date/name.sql
+-rw-r--r--   0        0        0      136 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/datetime/index.sql
+-rw-r--r--   0        0        0      137 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/datetime/name.sql
+-rw-r--r--   0        0        0      106 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/string_date/index.sql
+-rw-r--r--   0        0        0      107 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/string_date/name.sql
+-rw-r--r--   0        0        0      136 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/string_timestamp/index.sql
+-rw-r--r--   0        0        0      137 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/string_timestamp/name.sql
+-rw-r--r--   0        0        0      136 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/timestamp/index.sql
+-rw-r--r--   0        0        0      137 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/timestamp/name.sql
+-rw-r--r--   0        0        0      106 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/timestamp_date/index.sql
+-rw-r--r--   0        0        0      107 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_day_of_week/timestamp_date/name.sql
+-rw-r--r--   0        0        0      130 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_divide_by_zero/floordiv/out.sql
+-rw-r--r--   0        0        0      103 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_divide_by_zero/truediv/out.sql
+-rw-r--r--   0        0        0       50 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_extract_temporal_from_timestamp/date/out.sql
+-rw-r--r--   0        0        0       50 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_extract_temporal_from_timestamp/time/out.sql
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_azimuth/out.sql
+-rw-r--r--   0        0        0       74 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/contains/out.sql
+-rw-r--r--   0        0        0       75 2024-03-30 19:28:49.888059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/covered_by/out.sql
+-rw-r--r--   0        0        0       72 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/covers/out.sql
+-rw-r--r--   0        0        0       78 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/d_within/out.sql
+-rw-r--r--   0        0        0       76 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/difference/out.sql
+-rw-r--r--   0        0        0       74 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/disjoint/out.sql
+-rw-r--r--   0        0        0       74 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/distance/out.sql
+-rw-r--r--   0        0        0       72 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/geo_equals/out.sql
+-rw-r--r--   0        0        0       78 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/intersection/out.sql
+-rw-r--r--   0        0        0       76 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/intersects/out.sql
+-rw-r--r--   0        0        0       77 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/max_distance/out.sql
+-rw-r--r--   0        0        0       73 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/touches/out.sql
+-rw-r--r--   0        0        0       71 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/union/out.sql
+-rw-r--r--   0        0        0       72 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_binary/within/out.sql
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_minmax/x_max/out.sql
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_minmax/x_min/out.sql
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_minmax/y_max/out.sql
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_minmax/y_min/out.sql
+-rw-r--r--   0        0        0       71 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_point/out.sql
+-rw-r--r--   0        0        0       64 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_simplify/out.sql
+-rw-r--r--   0        0        0       55 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/aread/out.sql
+-rw-r--r--   0        0        0       59 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/as_binary/out.sql
+-rw-r--r--   0        0        0       57 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/as_text/out.sql
+-rw-r--r--   0        0        0       62 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/buffer/out.sql
+-rw-r--r--   0        0        0       59 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/centroid/out.sql
+-rw-r--r--   0        0        0       59 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/end_point/out.sql
+-rw-r--r--   0        0        0       63 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/geometry_type/out.sql
+-rw-r--r--   0        0        0       57 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/length/out.sql
+-rw-r--r--   0        0        0       60 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/npoints/out.sql
+-rw-r--r--   0        0        0       60 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/perimeter/out.sql
+-rw-r--r--   0        0        0       60 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/point_n/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary/start_point/out.sql
+-rw-r--r--   0        0        0       60 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_unary_union/out.sql
+-rw-r--r--   0        0        0       50 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_xy/x/out.sql
+-rw-r--r--   0        0        0       50 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_geospatial_xy/y/out.sql
+-rw-r--r--   0        0        0      107 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hash/binary/out.sql
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hash/string/out.sql
+-rw-r--r--   0        0        0       69 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/md5-test-binary/out.sql
+-rw-r--r--   0        0        0       37 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/md5-test-string/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha1-test-binary/out.sql
+-rw-r--r--   0        0        0       29 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha1-test-string/out.sql
+-rw-r--r--   0        0        0       64 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha256-test-binary/out.sql
+-rw-r--r--   0        0        0       32 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha256-test-string/out.sql
+-rw-r--r--   0        0        0       64 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha512-test-binary/out.sql
+-rw-r--r--   0        0        0       32 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_hashbytes/sha512-test-string/out.sql
+-rw-r--r--   0        0        0      404 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_identical_to/out.sql
+-rw-r--r--   0        0        0       46 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_integer_to_timestamp/ms/out.sql
+-rw-r--r--   0        0        0       78 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_integer_to_timestamp/ns/out.sql
+-rw-r--r--   0        0        0       46 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_integer_to_timestamp/s/out.sql
+-rw-r--r--   0        0        0       45 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_integer_to_timestamp/us/out.sql
+-rw-r--r--   0        0        0       71 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_string/escape_ascii_sequences/out.sql
+-rw-r--r--   0        0        0       31 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_string/escape_backslash/out.sql
+-rw-r--r--   0        0        0       31 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_string/escape_quote/out.sql
+-rw-r--r--   0        0        0       63 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_string/not_escape_special_characters/out.sql
+-rw-r--r--   0        0        0       68 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/datetime/out.sql
+-rw-r--r--   0        0        0       52 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/string_time/out.sql
+-rw-r--r--   0        0        0       68 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/string_timestamp/out.sql
+-rw-r--r--   0        0        0       52 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/time/out.sql
+-rw-r--r--   0        0        0       68 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_timestamp_or_time/timestamp/out.sql
+-rw-r--r--   0        0        0       86 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/date/out.sql
+-rw-r--r--   0        0        0      116 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/datetime/out.sql
+-rw-r--r--   0        0        0       86 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/string_date/out.sql
+-rw-r--r--   0        0        0      116 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/string_timestamp/out.sql
+-rw-r--r--   0        0        0      116 2024-03-30 19:28:49.892059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/timestamp/out.sql
+-rw-r--r--   0        0        0       86 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_literal_year/timestamp_date/out.sql
+-rw-r--r--   0        0        0       46 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_now/out.sql
+-rw-r--r--   0        0        0      417 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_projection_fusion_only_peeks_at_immediate_parent/out.sql
+-rw-r--r--   0        0        0      443 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_range_window_function/prec_foll/out.sql
+-rw-r--r--   0        0        0      451 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_range_window_function/prec_prec/out.sql
+-rw-r--r--   0        0        0      122 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_set_operation/difference/out.sql
+-rw-r--r--   0        0        0      125 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_set_operation/intersect/out.sql
+-rw-r--r--   0        0        0      116 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_set_operation/union_all/out.sql
+-rw-r--r--   0        0        0      121 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_set_operation/union_distinct/out.sql
+-rw-r--r--   0        0        0      148 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_substring/out.sql
+-rw-r--r--   0        0        0       60 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/day-date/out.sql
+-rw-r--r--   0        0        0       65 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/day-timestamp/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/hour-time/out.sql
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/hour-timestamp/out.sql
+-rw-r--r--   0        0        0       68 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/micros-time/out.sql
+-rw-r--r--   0        0        0       73 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/micros-timestamp/out.sql
+-rw-r--r--   0        0        0       68 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/millis-time/out.sql
+-rw-r--r--   0        0        0       73 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/millis-timestamp/out.sql
+-rw-r--r--   0        0        0       63 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/minute-time/out.sql
+-rw-r--r--   0        0        0       68 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/minute-timestamp/out.sql
+-rw-r--r--   0        0        0       62 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/month-date/out.sql
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/month-timestamp/out.sql
+-rw-r--r--   0        0        0       64 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/quarter-date/out.sql
+-rw-r--r--   0        0        0       69 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/quarter-timestamp/out.sql
+-rw-r--r--   0        0        0       63 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/second-time/out.sql
+-rw-r--r--   0        0        0       68 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/second-timestamp/out.sql
+-rw-r--r--   0        0        0       69 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/week-date/out.sql
+-rw-r--r--   0        0        0       74 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/week-timestamp/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/year-date/out.sql
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_temporal_truncate/year-timestamp/out.sql
+-rw-r--r--   0        0        0      141 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_to_timestamp_no_timezone/out.sql
+-rw-r--r--   0        0        0      173 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_to_timestamp_timezone/out.sql
+-rw-r--r--   0        0        0      448 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/days/out.sql
+-rw-r--r--   0        0        0      420 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/five/out.sql
+-rw-r--r--   0        0        0      450 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/hours/out.sql
+-rw-r--r--   0        0        0      464 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/micros/out.sql
+-rw-r--r--   0        0        0      454 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/minutes/out.sql
+-rw-r--r--   0        0        0      416 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/nanos/out.sql
+-rw-r--r--   0        0        0      454 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/seconds/out.sql
+-rw-r--r--   0        0        0      485 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/two_days/out.sql
+-rw-r--r--   0        0        0      450 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/week/out.sql
+-rw-r--r--   0        0        0      237 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_trailing_range_window/years/out.sql
+-rw-r--r--   0        0        0      397 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union/False/out.sql
+-rw-r--r--   0        0        0      402 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union/True/out.sql
+-rw-r--r--   0        0        0      476 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union_cte/False-False/out.sql
+-rw-r--r--   0        0        0      481 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union_cte/False-True/out.sql
+-rw-r--r--   0        0        0      481 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union_cte/True-False/out.sql
+-rw-r--r--   0        0        0      486 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_union_cte/True-True/out.sql
+-rw-r--r--   0        0        0      490 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_unnest/out_one_unnest.sql
+-rw-r--r--   0        0        0      905 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_unnest/out_two_unnests.sql
+-rw-r--r--   0        0        0      444 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_function/current_foll/out.sql
+-rw-r--r--   0        0        0      444 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_function/prec_current/out.sql
+-rw-r--r--   0        0        0      444 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_function/prec_prec/out.sql
+-rw-r--r--   0        0        0      104 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_unbounded/following/out.sql
+-rw-r--r--   0        0        0      104 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_window_unbounded/preceding/out.sql
+-rw-r--r--   0        0        0      955 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/test_client.py
+-rw-r--r--   0        0        0    20048 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/test_compiler.py
+-rw-r--r--   0        0        0     2954 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/test_datatypes.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/__init__.py
+-rw-r--r--   0        0        0       58 2024-03-30 19:28:49.896059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_builtin/test_bqutil_fn_from_hex/out.sql
+-rw-r--r--   0        0        0      124 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_builtin/test_farm_fingerprint/out.sql
+-rw-r--r--   0        0        0       76 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_assign/out.js
+-rw-r--r--   0        0        0       42 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_binary_operators/add/out.js
+-rw-r--r--   0        0        0       42 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_binary_operators/div/out.js
+-rw-r--r--   0        0        0       42 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_binary_operators/mul/out.js
+-rw-r--r--   0        0        0       42 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_binary_operators/sub/out.js
+-rw-r--r--   0        0        0      178 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_class/out.js
+-rw-r--r--   0        0        0      125 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_class_with_properties/out.js
+-rw-r--r--   0        0        0      139 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_continue/out.js
+-rw-r--r--   0        0        0      154 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_delete/out.js
+-rw-r--r--   0        0        0       64 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_dict/out.js
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_floordiv/out.js
+-rw-r--r--   0        0        0       40 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_function_def/out.js
+-rw-r--r--   0        0        0      249 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_lambda_with_splat/out.js
+-rw-r--r--   0        0        0       44 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_len_rewrite/out.js
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_list_comp/out.js
+-rw-r--r--   0        0        0       80 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_logical_not/out.js
+-rw-r--r--   0        0        0       56 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_missing_vararg/out.js
+-rw-r--r--   0        0        0       58 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_pow/out.js
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_scope_with_while/out.js
+-rw-r--r--   0        0        0       85 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_set_to_object/out.js
+-rw-r--r--   0        0        0       78 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_setitem/out.js
+-rw-r--r--   0        0        0      134 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_splat/out.js
+-rw-r--r--   0        0        0       49 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_str/out.js
+-rw-r--r--   0        0        0      106 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_true_false_none/out.js
+-rw-r--r--   0        0        0       59 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_tuple/out.js
+-rw-r--r--   0        0        0       48 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_unary_minus/out.js
+-rw-r--r--   0        0        0       48 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_unary_plus/out.js
+-rw-r--r--   0        0        0       48 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_varargs/out.js
+-rw-r--r--   0        0        0       51 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_variable_declaration/out.js
+-rw-r--r--   0        0        0       40 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_yield/out.js
+-rw-r--r--   0        0        0       40 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/snapshots/test_core/test_yield_from/out.js
+-rw-r--r--   0        0        0      798 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/test_builtin.py
+-rw-r--r--   0        0        0     6533 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/test_core.py
+-rw-r--r--   0        0        0     2002 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/test_find.py
+-rw-r--r--   0        0        0     1926 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/test_usage.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/udf/__init__.py
+-rw-r--r--   0        0        0    17057 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/udf/core.py
+-rw-r--r--   0        0        0     1599 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/udf/find.py
+-rw-r--r--   0        0        0     1255 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/bigquery/udf/rewrite.py
+-rw-r--r--   0        0        0    24527 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/__init__.py
+-rw-r--r--   0        0        0    22408 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/compiler.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/__init__.py
+-rw-r--r--   0        0        0     3415 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/conftest.py
+-rw-r--r--   0        0        0      139 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/count/out.sql
+-rw-r--r--   0        0        0      135 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/max/out.sql
+-rw-r--r--   0        0        0      136 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/mean/out.sql
+-rw-r--r--   0        0        0      135 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/min/out.sql
+-rw-r--r--   0        0        0      150 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/std/out.sql
+-rw-r--r--   0        0        0      135 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/sum/out.sql
+-rw-r--r--   0        0        0      144 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_reduction_where/var/out.sql
+-rw-r--r--   0        0        0      149 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_std_var_pop/std/out.sql
+-rw-r--r--   0        0        0      143 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_aggregations/test_std_var_pop/var/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/float/out.sql
+-rw-r--r--   0        0        0      119 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/float32/out.sql
+-rw-r--r--   0        0        0      110 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/float64/out.sql
+-rw-r--r--   0        0        0      115 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/int16/out.sql
+-rw-r--r--   0        0        0      113 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_double_col/int8/out.sql
+-rw-r--r--   0        0        0      113 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/date/out.sql
+-rw-r--r--   0        0        0      115 2024-03-30 19:28:49.900059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/int16/out.sql
+-rw-r--r--   0        0        0      113 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/int8/out.sql
+-rw-r--r--   0        0        0      142 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/mapstring_int64/out.sql
+-rw-r--r--   0        0        0      108 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/string/out.sql
+-rw-r--r--   0        0        0      167 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/structa_string_b_int64/out.sql
+-rw-r--r--   0        0        0      122 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_cast_string_col/timestamp/out.sql
+-rw-r--r--   0        0        0      317 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_column_regexp_extract/out.sql
+-rw-r--r--   0        0        0      142 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_column_regexp_replace/out.sql
+-rw-r--r--   0        0        0       88 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_greatest_least/out1.sql
+-rw-r--r--   0        0        0      103 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_greatest_least/out2.sql
+-rw-r--r--   0        0        0       82 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_greatest_least/out3.sql
+-rw-r--r--   0        0        0       97 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_greatest_least/out4.sql
+-rw-r--r--   0        0        0      211 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_group_concat/comma_none/out.sql
+-rw-r--r--   0        0        0      278 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_group_concat/comma_zero/out.sql
+-rw-r--r--   0        0        0      211 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_group_concat/minus_none/out.sql
+-rw-r--r--   0        0        0       94 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_hash/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/bigint_col/out.sql
+-rw-r--r--   0        0        0       59 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/bool_col/out.sql
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/date_string_col/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/double_col/out.sql
+-rw-r--r--   0        0        0       60 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/float_col/out.sql
+-rw-r--r--   0        0        0       53 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/id/out.sql
+-rw-r--r--   0        0        0        5 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/index/out.sql
+-rw-r--r--   0        0        0       58 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/int_col/out.sql
+-rw-r--r--   0        0        0       56 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/month/out.sql
+-rw-r--r--   0        0        0       63 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/smallint_col/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/string_col/out.sql
+-rw-r--r--   0        0        0       64 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/timestamp_col/out.sql
+-rw-r--r--   0        0        0       62 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/tinyint_col/out.sql
+-rw-r--r--   0        0        0       55 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_noop_cast/year/out.sql
+-rw-r--r--   0        0        0      111 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_find/out1.sql
+-rw-r--r--   0        0        0      132 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_find/out2.sql
+-rw-r--r--   0        0        0      118 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_find_in_set/out.sql
+-rw-r--r--   0        0        0      112 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_like/out1.sql
+-rw-r--r--   0        0        0      184 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_like/out2.sql
+-rw-r--r--   0        0        0      218 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_substring/out1.sql
+-rw-r--r--   0        0        0      227 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_string_column_substring/out2.sql
+-rw-r--r--   0        0        0      119 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_cast/out1.sql
+-rw-r--r--   0        0        0      107 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_cast/out2.sql
+-rw-r--r--   0        0        0      110 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_from_integer/out.sql
+-rw-r--r--   0        0        0       34 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_now/out.sql
+-rw-r--r--   0        0        0      135 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/d/out.sql
+-rw-r--r--   0        0        0      143 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/h/out.sql
+-rw-r--r--   0        0        0      147 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/m/out.sql
+-rw-r--r--   0        0        0      147 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/minute/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/w/out.sql
+-rw-r--r--   0        0        0      143 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_timestamp_truncate/y/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/abs/out.sql
+-rw-r--r--   0        0        0      114 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/ceil/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/exp/out.sql
+-rw-r--r--   0        0        0       86 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/log/out.sql
+-rw-r--r--   0        0        0       91 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/log10/out.sql
+-rw-r--r--   0        0        0       89 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/log2/out.sql
+-rw-r--r--   0        0        0       91 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/round/out.sql
+-rw-r--r--   0        0        0       97 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/round_0/out.sql
+-rw-r--r--   0        0        0       97 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/round_2/out.sql
+-rw-r--r--   0        0        0      121 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/sign/out.sql
+-rw-r--r--   0        0        0       89 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_functions/test_translate_math_functions/sqrt/out.sql
+-rw-r--r--   0        0        0      122 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_fine_grained_timestamp_literals/micros/out.sql
+-rw-r--r--   0        0        0      151 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_fine_grained_timestamp_literals/micros_tz/out.sql
+-rw-r--r--   0        0        0      122 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_fine_grained_timestamp_literals/millis/out.sql
+-rw-r--r--   0        0        0      151 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_fine_grained_timestamp_literals/millis_tz/out.sql
+-rw-r--r--   0        0        0       10 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_literals/nested_quote/out.sql
+-rw-r--r--   0        0        0       13 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_literals/nested_token/out.sql
+-rw-r--r--   0        0        0        8 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_literals/simple/out.sql
+-rw-r--r--   0        0        0       25 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/false/out.sql
+-rw-r--r--   0        0        0       21 2024-03-30 19:28:49.904060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/float/out.sql
+-rw-r--r--   0        0        0       17 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/int/out.sql
+-rw-r--r--   0        0        0       36 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/nested_quote/out.sql
+-rw-r--r--   0        0        0       43 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/nested_token/out.sql
+-rw-r--r--   0        0        0       31 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/simple/out.sql
+-rw-r--r--   0        0        0       23 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_string_numeric_boolean_literals/true/out.sql
+-rw-r--r--   0        0        0      102 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_timestamp_literals/expr0/out.sql
+-rw-r--r--   0        0        0      102 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_timestamp_literals/expr1/out.sql
+-rw-r--r--   0        0        0      102 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_literals/test_timestamp_literals/expr2/out.sql
+-rw-r--r--   0        0        0      104 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_between/out.sql
+-rw-r--r--   0        0        0      110 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/add/out.sql
+-rw-r--r--   0        0        0      113 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/eq/out.sql
+-rw-r--r--   0        0        0      120 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/ge/out.sql
+-rw-r--r--   0        0        0      114 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/gt/out.sql
+-rw-r--r--   0        0        0      117 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/le/out.sql
+-rw-r--r--   0        0        0      111 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/lt/out.sql
+-rw-r--r--   0        0        0      115 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/mul/out.sql
+-rw-r--r--   0        0        0      117 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/ne/out.sql
+-rw-r--r--   0        0        0      118 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/pow/out.sql
+-rw-r--r--   0        0        0      115 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/sub/out.sql
+-rw-r--r--   0        0        0      113 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_operators/truediv/out.sql
+-rw-r--r--   0        0        0      157 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_parenthesization/lambda0/out.sql
+-rw-r--r--   0        0        0      117 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_parenthesization/lambda1/out.sql
+-rw-r--r--   0        0        0      166 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_binary_infix_parenthesization/lambda2/out.sql
+-rw-r--r--   0        0        0       92 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_negate/bool_col/out.sql
+-rw-r--r--   0        0        0       94 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_negate/float_col/out.sql
+-rw-r--r--   0        0        0       90 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_negate/int_col/out.sql
+-rw-r--r--   0        0        0      198 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_search_case/out.sql
+-rw-r--r--   0        0        0      168 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_operators/test_simple_case/out.sql
+-rw-r--r--   0        0        0      136 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_array_join_in_subquery/out.sql
+-rw-r--r--   0        0        0      227 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_complex_array_expr_projection/out.sql
+-rw-r--r--   0        0        0      256 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_complex_join/out.sql
+-rw-r--r--   0        0        0      150 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_count_name/out.sql
+-rw-r--r--   0        0        0      177 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_ifelse_use_if/out.sql
+-rw-r--r--   0        0        0      343 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_isin_notin_in_select/out1.sql
+-rw-r--r--   0        0        0      357 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_isin_notin_in_select/out2.sql
+-rw-r--r--   0        0        0      145 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_isnull_case_expr_rewrite_failure/out.sql
+-rw-r--r--   0        0        0      367 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_join_self_reference/out.sql
+-rw-r--r--   0        0        0      216 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_named_from_filter_groupby/out1.sql
+-rw-r--r--   0        0        0      216 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_named_from_filter_groupby/out2.sql
+-rw-r--r--   0        0        0       37 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_physical_table_reference_translate/out.sql
+-rw-r--r--   0        0        0       29 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_scalar_exprs_no_table_refs/add/out.sql
+-rw-r--r--   0        0        0       34 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_scalar_exprs_no_table_refs/now/out.sql
+-rw-r--r--   0        0        0       45 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_self_reference_simple/out.sql
+-rw-r--r--   0        0        0      409 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-awardID-any_inner_join/out.sql
+-rw-r--r--   0        0        0      414 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-awardID-any_left_join/out.sql
+-rw-r--r--   0        0        0      411 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-awardID-inner_join/out.sql
+-rw-r--r--   0        0        0      416 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-awardID-left_join/out.sql
+-rw-r--r--   0        0        0      410 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-playerID-any_inner_join/out.sql
+-rw-r--r--   0        0        0      415 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-playerID-any_left_join/out.sql
+-rw-r--r--   0        0        0      412 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-playerID-inner_join/out.sql
+-rw-r--r--   0        0        0      417 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_joins/playerID-playerID-left_join/out.sql
+-rw-r--r--   0        0        0      428 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_simple_scalar_aggregates/out.sql
+-rw-r--r--   0        0        0      561 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_table_column_unbox/out.sql
+-rw-r--r--   0        0        0      307 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_timestamp_extract_field/out.sql
+-rw-r--r--   0        0        0      380 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_where_simple_comparisons/out.sql
+-rw-r--r--   0        0        0      363 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_where_with_between/out.sql
+-rw-r--r--   0        0        0      119 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_where_with_timestamp/out.sql
+-rw-r--r--   0        0        0     5069 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_aggregations.py
+-rw-r--r--   0        0        0     9060 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_client.py
+-rw-r--r--   0        0        0     9902 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_datatypes.py
+-rw-r--r--   0        0        0    14466 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_functions.py
+-rw-r--r--   0        0        0     1931 2024-03-30 19:28:49.908059 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_literals.py
+-rw-r--r--   0        0        0     7328 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_operators.py
+-rw-r--r--   0        0        0    11840 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_select.py
+-rw-r--r--   0        0        0    21760 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/conftest.py
+-rw-r--r--   0        0        0     6116 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/__init__.py
+-rw-r--r--   0        0        0     3022 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/convert.py
+-rw-r--r--   0        0        0    14114 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/executor.py
+-rw-r--r--   0        0        0     6623 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/helpers.py
+-rw-r--r--   0        0        0     1876 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/kernels.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/__init__.py
+-rw-r--r--   0        0        0    11178 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/conftest.py
+-rw-r--r--   0        0        0     5854 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_arrays.py
+-rw-r--r--   0        0        0     5242 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_cast.py
+-rw-r--r--   0        0        0     3483 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_client.py
+-rw-r--r--   0        0        0     1049 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_core.py
+-rw-r--r--   0        0        0     5782 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_functions.py
+-rw-r--r--   0        0        0    12016 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_join.py
+-rw-r--r--   0        0        0     2609 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_maps.py
+-rw-r--r--   0        0        0    28046 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_operations.py
+-rw-r--r--   0        0        0     3860 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_strings.py
+-rw-r--r--   0        0        0     2548 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_structs.py
+-rw-r--r--   0        0        0     6771 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_temporal.py
+-rw-r--r--   0        0        0    10915 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_udf.py
+-rw-r--r--   0        0        0    16722 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_window.py
+-rw-r--r--   0        0        0    21597 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/datafusion/__init__.py
+-rw-r--r--   0        0        0    17397 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/datafusion/compiler.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/__init__.py
+-rw-r--r--   0        0        0     1303 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/conftest.py
+-rw-r--r--   0        0        0     1091 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/test_connect.py
+-rw-r--r--   0        0        0     1214 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/test_register.py
+-rw-r--r--   0        0        0      799 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/test_select.py
+-rw-r--r--   0        0        0      177 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/test_string.py
+-rw-r--r--   0        0        0      760 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/test_temporal.py
+-rw-r--r--   0        0        0     2060 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/test_udf.py
+-rw-r--r--   0        0        0     3603 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/datafusion/udfs.py
+-rw-r--r--   0        0        0     5602 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/druid/__init__.py
+-rw-r--r--   0        0        0     6259 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/druid/compiler.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/druid/tests/__init__.py
+-rw-r--r--   0        0        0     4793 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/druid/tests/conftest.py
+-rw-r--r--   0        0        0    49168 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/__init__.py
+-rw-r--r--   0        0        0    14608 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/compiler.py
+-rw-r--r--   0        0        0      240 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/converter.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/__init__.py
+-rw-r--r--   0        0        0     3987 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/conftest.py
+-rw-r--r--   0        0        0       37 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_client/test_to_other_sql/out.sql
+-rw-r--r--   0        0        0       54 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_to_floating_point_type/float32/out.sql
+-rw-r--r--   0        0        0       56 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_to_floating_point_type/float64/out.sql
+-rw-r--r--   0        0        0       74 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_uints/uint16/out.sql
+-rw-r--r--   0        0        0       73 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_uints/uint32/out.sql
+-rw-r--r--   0        0        0       72 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_uints/uint64/out.sql
+-rw-r--r--   0        0        0       72 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_datatypes/test_cast_uints/uint8/out.sql
+-rw-r--r--   0        0        0       92 2024-03-30 19:28:49.912060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_geospatial_dwithin/out.sql
+-rw-r--r--   0        0        0       57 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_geospatial_unary_snapshot/as_text/out.sql
+-rw-r--r--   0        0        0       58 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_geospatial_unary_snapshot/n_points/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr0/out.sql
+-rw-r--r--   0        0        0       83 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr0-POINT_1_0/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr1/out.sql
+-rw-r--r--   0        0        0      102 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp0-0_0/out.sql
+-rw-r--r--   0        0        0      102 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp1-1_1/out.sql
+-rw-r--r--   0        0        0      102 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp2-2_2/out.sql
+-rw-r--r--   0        0        0      117 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp3-0_0_1_1_2_2/out.sql
+-rw-r--r--   0        0        0      117 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp4-2_2_1_1_0_0/out.sql
+-rw-r--r--   0        0        0      121 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp5-0_0_1_1_2_2_0_0/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp6-0_0_1_1_2_2_0_0/out.sql
+-rw-r--r--   0        0        0      141 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp7-0_0_1_1_2_2_2_2_1_1_0_0/out.sql
+-rw-r--r--   0        0        0      123 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp8-0_0_1_1_2_2/out.sql
+-rw-r--r--   0        0        0     8259 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/test_client.py
+-rw-r--r--   0        0        0     3612 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/test_datatypes.py
+-rw-r--r--   0        0        0    11219 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/test_geospatial.py
+-rw-r--r--   0        0        0    14798 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/test_register.py
+-rw-r--r--   0        0        0     2171 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/test_udf.py
+-rw-r--r--   0        0        0    14804 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/exasol/__init__.py
+-rw-r--r--   0        0        0     6805 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/exasol/compiler.py
+-rw-r--r--   0        0        0     1260 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/exasol/converter.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/exasol/tests/__init__.py
+-rw-r--r--   0        0        0     3524 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/exasol/tests/conftest.py
+-rw-r--r--   0        0        0    33390 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/__init__.py
+-rw-r--r--   0        0        0    19772 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/compiler.py
+-rw-r--r--   0        0        0     6885 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/datatypes.py
+-rw-r--r--   0        0        0    10797 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/ddl.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/__init__.py
+-rw-r--r--   0        0        0     5368 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/conftest.py
+-rw-r--r--   0        0        0      237 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_complex_filtered_agg/out.sql
+-rw-r--r--   0        0        0      246 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_complex_groupby_aggregation/out.sql
+-rw-r--r--   0        0        0      220 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_complex_projections/out.sql
+-rw-r--r--   0        0        0       92 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_count_star/out.sql
+-rw-r--r--   0        0        0       65 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/day/out.sql
+-rw-r--r--   0        0        0       58 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/day_of_year/out.sql
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/hour/out.sql
+-rw-r--r--   0        0        0       68 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/minute/out.sql
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/month/out.sql
+-rw-r--r--   0        0        0       69 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/quarter/out.sql
+-rw-r--r--   0        0        0       68 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/second/out.sql
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/week_of_year/out.sql
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_extract_fields/year/out.sql
+-rw-r--r--   0        0        0      260 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_filter/out.sql
+-rw-r--r--   0        0        0      225 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_having/out.sql
+-rw-r--r--   0        0        0      132 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_simple_filtered_agg/out.sql
+-rw-r--r--   0        0        0       55 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_sum/out.sql
+-rw-r--r--   0        0        0      117 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_timestamp_from_unix/timestamp_ms/out.sql
+-rw-r--r--   0        0        0      112 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_timestamp_from_unix/timestamp_s/out.sql
+-rw-r--r--   0        0        0      202 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_value_counts/out.sql
+-rw-r--r--   0        0        0      275 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_window_aggregation/out.sql
+-rw-r--r--   0        0        0      719 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_window_topn/out.sql
+-rw-r--r--   0        0        0      129 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_windowing_tvf/cumulate_window/out.sql
+-rw-r--r--   0        0        0      124 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_windowing_tvf/hop_window/out.sql
+-rw-r--r--   0        0        0       99 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_windowing_tvf/tumble_window/out.sql
+-rw-r--r--   0        0        0      160 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_window/test_range_window/out.sql
+-rw-r--r--   0        0        0      139 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_window/test_rows_window/out.sql
+-rw-r--r--   0        0        0     4962 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/test_compiler.py
+-rw-r--r--   0        0        0     1181 2024-03-30 19:28:49.916060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/test_datatypes.py
+-rw-r--r--   0        0        0    16229 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/test_ddl.py
+-rw-r--r--   0        0        0     4795 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/test_join.py
+-rw-r--r--   0        0        0      632 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/test_udf.py
+-rw-r--r--   0        0        0     1975 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/flink/tests/test_window.py
+-rw-r--r--   0        0        0    11772 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/flink/utils.py
+-rw-r--r--   0        0        0    40475 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/__init__.py
+-rw-r--r--   0        0        0    10149 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/client.py
+-rw-r--r--   0        0        0    12545 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/compiler.py
+-rw-r--r--   0        0        0    17678 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/ddl.py
+-rw-r--r--   0        0        0     8596 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/metadata.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/__init__.py
+-rw-r--r--   0        0        0     6735 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/conftest.py
+-rw-r--r--   0        0        0      212 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/mocks.py
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/first/out.sql
+-rw-r--r--   0        0        0      129 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lag_arg/out.sql
+-rw-r--r--   0        0        0      123 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lag_default/out.sql
+-rw-r--r--   0        0        0      132 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lag_explicit_default/out.sql
+-rw-r--r--   0        0        0      136 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/last/out.sql
+-rw-r--r--   0        0        0      131 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lead_arg/out.sql
+-rw-r--r--   0        0        0      125 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lead_default/out.sql
+-rw-r--r--   0        0        0      134 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/lead_explicit_default/out.sql
+-rw-r--r--   0        0        0      119 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/ntile/out.sql
+-rw-r--r--   0        0        0      126 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_analytic_functions/test_analytic_exprs/percent_rank/out.sql
+-rw-r--r--   0        0        0      695 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_assign_labels/out.sql
+-rw-r--r--   0        0        0      331 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/close_extreme_false/out.sql
+-rw-r--r--   0        0        0      331 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/close_extreme_false_closed_right/out.sql
+-rw-r--r--   0        0        0      399 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/close_extreme_false_include_under_include_over/out.sql
+-rw-r--r--   0        0        0      332 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/closed_right/out.sql
+-rw-r--r--   0        0        0      365 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/closed_right_close_extreme_false_include_under/out.sql
+-rw-r--r--   0        0        0      158 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/closed_right_include_over_include_under/out.sql
+-rw-r--r--   0        0        0      332 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/default/out.sql
+-rw-r--r--   0        0        0      158 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_over_include_under0/out.sql
+-rw-r--r--   0        0        0      184 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_over_include_under1/out.sql
+-rw-r--r--   0        0        0      189 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_over_include_under2/out.sql
+-rw-r--r--   0        0        0      365 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_under/out.sql
+-rw-r--r--   0        0        0      399 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_to_case/include_under_include_over/out.sql
+-rw-r--r--   0        0        0       89 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_case_exprs/test_decimal_fillna_cast_arg/fillna_l_extendedprice/out.sql
+-rw-r--r--   0        0        0       91 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_case_exprs/test_decimal_fillna_cast_arg/fillna_l_extendedprice_double/out.sql
+-rw-r--r--   0        0        0       84 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_case_exprs/test_decimal_fillna_cast_arg/fillna_l_quantity/out.sql
+-rw-r--r--   0        0        0      110 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_case_exprs/test_identical_to/out.sql
+-rw-r--r--   0        0        0       80 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_case_exprs/test_identical_to_special_case/out.sql
+-rw-r--r--   0        0        0      102 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_case_exprs/test_ifelse_use_if/out.sql
+-rw-r--r--   0        0        0       88 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_case_exprs/test_isnull_1_0/out1.sql
+-rw-r--r--   0        0        0       98 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_case_exprs/test_isnull_1_0/out2.sql
+-rw-r--r--   0        0        0      148 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_case_exprs/test_nullif_ifnull/nullif_boolean/out.sql
+-rw-r--r--   0        0        0      118 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_case_exprs/test_nullif_ifnull/nullif_input/out.sql
+-rw-r--r--   0        0        0      152 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_case_exprs/test_nullif_ifnull/nullif_negate_boolean/out.sql
+-rw-r--r--   0        0        0      198 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_case_exprs/test_search_case/out.sql
+-rw-r--r--   0        0        0      139 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_case_exprs/test_simple_case/out.sql
+-rw-r--r--   0        0        0      103 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/coalesce_columns/out.sql
+-rw-r--r--   0        0        0       94 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/coalesce_scalar/out.sql
+-rw-r--r--   0        0        0      103 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/greatest_columns/out.sql
+-rw-r--r--   0        0        0       94 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/greatest_scalar/out.sql
+-rw-r--r--   0        0        0       97 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/least_columns/out.sql
+-rw-r--r--   0        0        0       88 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_coalesce_greater_least/test_varargs_functions/least_scalar/out.sql
+-rw-r--r--   0        0        0       50 2024-03-30 19:28:49.920060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_add_partition/out.sql
+-rw-r--r--   0        0        0       48 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_add_partition_string_key/out.sql
+-rw-r--r--   0        0        0       80 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_add_partition_with_props/out.sql
+-rw-r--r--   0        0        0       80 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_partition_properties/out1.sql
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_partition_properties/out2.sql
+-rw-r--r--   0        0        0       93 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_partition_properties/out3.sql
+-rw-r--r--   0        0        0       82 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_partition_properties/out4.sql
+-rw-r--r--   0        0        0       80 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_table_properties/out1.sql
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_table_properties/out2.sql
+-rw-r--r--   0        0        0       93 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_table_properties/out3.sql
+-rw-r--r--   0        0        0       82 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_alter_table_properties/out4.sql
+-rw-r--r--   0        0        0       90 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_avro_other_formats/out.sql
+-rw-r--r--   0        0        0       47 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_cache_table_pool_name/out1.sql
+-rw-r--r--   0        0        0       47 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_cache_table_pool_name/out2.sql
+-rw-r--r--   0        0        0      114 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_external_table_as/out.sql
+-rw-r--r--   0        0        0      491 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_external_table_avro/out.sql
+-rw-r--r--   0        0        0      241 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_delimited/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_like_parquet/out.sql
+-rw-r--r--   0        0        0      382 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_parquet/out.sql
+-rw-r--r--   0        0        0      106 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_parquet_like_other/out.sql
+-rw-r--r--   0        0        0      140 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_parquet_with_schema/out.sql
+-rw-r--r--   0        0        0      126 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_create_table_with_location_compile/out.sql
+-rw-r--r--   0        0        0       51 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_drop_partition/out.sql
+-rw-r--r--   0        0        0       22 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_drop_table_compile/out1.sql
+-rw-r--r--   0        0        0       32 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_drop_table_compile/out2.sql
+-rw-r--r--   0        0        0      102 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_load_data_partitioned/out1.sql
+-rw-r--r--   0        0        0      112 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_load_data_partitioned/out2.sql
+-rw-r--r--   0        0        0       71 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_load_data_unpartitioned/out1.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_load_data_unpartitioned/out2.sql
+-rw-r--r--   0        0        0      385 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_no_overwrite/out.sql
+-rw-r--r--   0        0        0       88 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_select_basics/out1.sql
+-rw-r--r--   0        0        0       93 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_ddl_compilation/test_select_basics/out2.sql
+-rw-r--r--   0        0        0      266 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_exprs/test_filter_with_analytic/out.sql
+-rw-r--r--   0        0        0      207 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_exprs/test_named_from_filter_group_by/abc.sql
+-rw-r--r--   0        0        0      207 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_exprs/test_named_from_filter_group_by/foo.sql
+-rw-r--r--   0        0        0      134 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_exprs/test_nunique_where/out.sql
+-rw-r--r--   0        0        0      117 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_exprs/test_where_with_timestamp/out.sql
+-rw-r--r--   0        0        0       83 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_in_not_in/test_field_in_literals/isin/out.sql
+-rw-r--r--   0        0        0      102 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_in_not_in/test_field_in_literals/notin/out.sql
+-rw-r--r--   0        0        0      196 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_in_not_in/test_isin_notin_in_select/isin/out.sql
+-rw-r--r--   0        0        0      210 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_in_not_in/test_isin_notin_in_select/notin/out.sql
+-rw-r--r--   0        0        0       85 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_in_not_in/test_literal_in_fields/isin/out.sql
+-rw-r--r--   0        0        0      104 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_in_not_in/test_literal_in_fields/notin/out.sql
+-rw-r--r--   0        0        0      169 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_group_by_with_window_preserves_range/out.sql
+-rw-r--r--   0        0        0      114 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_is_parens/isnull/out.sql
+-rw-r--r--   0        0        0      102 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_is_parens/notnull/out.sql
+-rw-r--r--   0        0        0      130 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_is_parens_identical_to/out.sql
+-rw-r--r--   0        0        0     1165 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_join_aliasing/out.sql
+-rw-r--r--   0        0        0     1971 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_join_key_name/out.sql
+-rw-r--r--   0        0        0      921 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_join_key_name2/out.sql
+-rw-r--r--   0        0        0      111 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_join_no_predicates_for_impala/cross_join/out.sql
+-rw-r--r--   0        0        0      121 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_join_no_predicates_for_impala/inner_join/out.sql
+-rw-r--r--   0        0        0      126 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_join_no_predicates_for_impala/left_join/out.sql
+-rw-r--r--   0        0        0      126 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_join_no_predicates_for_impala/outer_join/out.sql
+-rw-r--r--   0        0        0      183 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_join_with_nested_or_condition/out.sql
+-rw-r--r--   0        0        0      241 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_join_with_nested_xor_condition/out.sql
+-rw-r--r--   0        0        0      397 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_limit_cte_extract/out.sql
+-rw-r--r--   0        0        0       93 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_logically_negate_complex_boolean_expr/out.sql
+-rw-r--r--   0        0        0      268 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_multiple_filters/out.sql
+-rw-r--r--   0        0        0      289 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_multiple_filters2/out.sql
+-rw-r--r--   0        0        0      337 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_nested_join_base/out.sql
+-rw-r--r--   0        0        0      914 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_nested_join_multiple_ctes/out.sql
+-rw-r--r--   0        0        0      557 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_nested_joins_single_cte/out.sql
+-rw-r--r--   0        0        0       71 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_relabel_projection/out.sql
+-rw-r--r--   0        0        0      148 2024-03-30 19:28:49.924060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_find/out.sql
+-rw-r--r--   0        0        0       97 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/ascii_str/out.sql
+-rw-r--r--   0        0        0      532 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/capitalize/out.sql
+-rw-r--r--   0        0        0      109 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/extract_host/out.sql
+-rw-r--r--   0        0        0      111 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/find/out.sql
+-rw-r--r--   0        0        0      131 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/find_in_set_multiple/out.sql
+-rw-r--r--   0        0        0      126 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/find_in_set_single/out.sql
+-rw-r--r--   0        0        0      121 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/find_with_offset/out.sql
+-rw-r--r--   0        0        0       99 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/length/out.sql
+-rw-r--r--   0        0        0      112 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/like/out.sql
+-rw-r--r--   0        0        0      184 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/like_multiple/out.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/lower/out.sql
+-rw-r--r--   0        0        0      105 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/lpad_char/out.sql
+-rw-r--r--   0        0        0      107 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/lpad_default/out.sql
+-rw-r--r--   0        0        0       92 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/lstrip/out.sql
+-rw-r--r--   0        0        0      133 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/re_extract/out.sql
+-rw-r--r--   0        0        0      141 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/re_replace/out.sql
+-rw-r--r--   0        0        0      115 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/re_search/out.sql
+-rw-r--r--   0        0        0       99 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/repeat/out.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/reverse/out.sql
+-rw-r--r--   0        0        0      115 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/rlike/out.sql
+-rw-r--r--   0        0        0      105 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/rpad_char/out.sql
+-rw-r--r--   0        0        0      107 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/rpad_default/out.sql
+-rw-r--r--   0        0        0       92 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/rstrip/out.sql
+-rw-r--r--   0        0        0       90 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/strip/out.sql
+-rw-r--r--   0        0        0      146 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/strright/out.sql
+-rw-r--r--   0        0        0      229 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/substr_0_3/out.sql
+-rw-r--r--   0        0        0      220 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/substr_2/out.sql
+-rw-r--r--   0        0        0      119 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/translate/out.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/upper/out.sql
+-rw-r--r--   0        0        0       54 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_join/out.sql
+-rw-r--r--   0        0        0      171 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_create_uda/False/out.sql
+-rw-r--r--   0        0        0      196 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_create_uda/True/out.sql
+-rw-r--r--   0        0        0       99 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_create_udf/out.sql
+-rw-r--r--   0        0        0      115 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_create_udf_type_conversions/out.sql
+-rw-r--r--   0        0        0       51 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_delete_udf_aggregate/out.sql
+-rw-r--r--   0        0        0       48 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_delete_udf_db/out.sql
+-rw-r--r--   0        0        0       51 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_delete_udf_if_exists/out.sql
+-rw-r--r--   0        0        0       41 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_delete_udf_simple/out.sql
+-rw-r--r--   0        0        0       32 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_list_udafs/out.sql
+-rw-r--r--   0        0        0       48 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_list_udafs_like/out.sql
+-rw-r--r--   0        0        0       22 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_list_udf/out.sql
+-rw-r--r--   0        0        0       38 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_list_udfs_like/out.sql
+-rw-r--r--   0        0        0       75 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_sql_generation/out.sql
+-rw-r--r--   0        0        0       54 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_udf/test_sql_generation_from_infoclass/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_hash/out.sql
+-rw-r--r--   0        0        0       93 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/log_with_base/out.sql
+-rw-r--r--   0        0        0      124 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/round_expr/out.sql
+-rw-r--r--   0        0        0      107 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/round_no_args/out.sql
+-rw-r--r--   0        0        0       97 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/round_two/out.sql
+-rw-r--r--   0        0        0       97 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/round_zero/out.sql
+-rw-r--r--   0        0        0      105 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/sign_double/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/sign_float/out.sql
+-rw-r--r--   0        0        0      108 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric/sign_tinyint/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-abs/out.sql
+-rw-r--r--   0        0        0      104 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-approx_median/out.sql
+-rw-r--r--   0        0        0      103 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-approx_nunique/out.sql
+-rw-r--r--   0        0        0      105 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-ceil/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-exp/out.sql
+-rw-r--r--   0        0        0      107 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-floor/out.sql
+-rw-r--r--   0        0        0       85 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-ln/out.sql
+-rw-r--r--   0        0        0       86 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-log/out.sql
+-rw-r--r--   0        0        0       91 2024-03-30 19:28:49.928060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-log10/out.sql
+-rw-r--r--   0        0        0       89 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-log2/out.sql
+-rw-r--r--   0        0        0       99 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-nullif_zero/out.sql
+-rw-r--r--   0        0        0       23 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-nullifzero/out.sql
+-rw-r--r--   0        0        0       89 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-sqrt/out.sql
+-rw-r--r--   0        0        0       90 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-zero_ifnull/out.sql
+-rw-r--r--   0        0        0       25 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/double_col-zeroifnull/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-abs/out.sql
+-rw-r--r--   0        0        0       98 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-approx_median/out.sql
+-rw-r--r--   0        0        0       97 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-approx_nunique/out.sql
+-rw-r--r--   0        0        0       99 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-ceil/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-exp/out.sql
+-rw-r--r--   0        0        0      101 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-floor/out.sql
+-rw-r--r--   0        0        0       79 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-ln/out.sql
+-rw-r--r--   0        0        0       80 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-log/out.sql
+-rw-r--r--   0        0        0       85 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-log10/out.sql
+-rw-r--r--   0        0        0       83 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-log2/out.sql
+-rw-r--r--   0        0        0       93 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-nullif_zero/out.sql
+-rw-r--r--   0        0        0       20 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-nullifzero/out.sql
+-rw-r--r--   0        0        0       83 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-sqrt/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-zero_ifnull/out.sql
+-rw-r--r--   0        0        0       22 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_numeric_unary_builtins/int_col-zeroifnull/out.sql
+-rw-r--r--   0        0        0      144 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/avg/out.sql
+-rw-r--r--   0        0        0      147 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/count/out.sql
+-rw-r--r--   0        0        0      143 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/max/out.sql
+-rw-r--r--   0        0        0      143 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/min/out.sql
+-rw-r--r--   0        0        0      158 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/stddev_pop/out.sql
+-rw-r--r--   0        0        0      159 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/stddev_samp/out.sql
+-rw-r--r--   0        0        0      143 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/sum/out.sql
+-rw-r--r--   0        0        0      157 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/var_pop/out.sql
+-rw-r--r--   0        0        0      153 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_unary_builtins/test_reduction_where/var_samp/out.sql
+-rw-r--r--   0        0        0       73 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_any_all/all/out.sql
+-rw-r--r--   0        0        0       73 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_any_all/any/out.sql
+-rw-r--r--   0        0        0       92 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_any_all/not_all/out.sql
+-rw-r--r--   0        0        0       92 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_any_all/not_any/out.sql
+-rw-r--r--   0        0        0       79 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_between/out.sql
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/add/out.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/and/out.sql
+-rw-r--r--   0        0        0       70 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/div/out.sql
+-rw-r--r--   0        0        0       70 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/eq/out.sql
+-rw-r--r--   0        0        0       77 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/ge/out.sql
+-rw-r--r--   0        0        0       71 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/gt/out.sql
+-rw-r--r--   0        0        0       74 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/le/out.sql
+-rw-r--r--   0        0        0       68 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/lt/out.sql
+-rw-r--r--   0        0        0       72 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/mul/out.sql
+-rw-r--r--   0        0        0       74 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/ne/out.sql
+-rw-r--r--   0        0        0       93 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/or/out.sql
+-rw-r--r--   0        0        0       75 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/pow/out.sql
+-rw-r--r--   0        0        0       72 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/sub/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_operators/xor/out.sql
+-rw-r--r--   0        0        0       76 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_parenthesization/function_call/out.sql
+-rw-r--r--   0        0        0      105 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_parenthesization/negation/out.sql
+-rw-r--r--   0        0        0       96 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_binary_infix_parenthesization/parens_left/out.sql
+-rw-r--r--   0        0        0       79 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/a-int16/out.sql
+-rw-r--r--   0        0        0       74 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/a-int32/out.sql
+-rw-r--r--   0        0        0       77 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/a-int64/out.sql
+-rw-r--r--   0        0        0       78 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/a-string/out.sql
+-rw-r--r--   0        0        0       77 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/d-int8/out.sql
+-rw-r--r--   0        0        0       79 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/g-double/out.sql
+-rw-r--r--   0        0        0       84 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_casts/g-timestamp/out.sql
+-rw-r--r--   0        0        0       15 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_correlated_predicate_subquery/out.sql
+-rw-r--r--   0        0        0      189 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_correlated_predicate_subquery/out1.sql
+-rw-r--r--   0        0        0      189 2024-03-30 19:28:49.932060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_correlated_predicate_subquery/out2.sql
+-rw-r--r--   0        0        0       94 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_decimal_casts/column/out.sql
+-rw-r--r--   0        0        0       83 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_decimal_casts/literal/out.sql
+-rw-r--r--   0        0        0       93 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_isnull_notnull/compound_isnull/out.sql
+-rw-r--r--   0        0        0       64 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_isnull_notnull/isnull/out.sql
+-rw-r--r--   0        0        0       69 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_isnull_notnull/notnull/out.sql
+-rw-r--r--   0        0        0       41 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/embedded_double_quote/out.sql
+-rw-r--r--   0        0        0       34 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/embedded_single_quote/out.sql
+-rw-r--r--   0        0        0       25 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/false/out.sql
+-rw-r--r--   0        0        0       21 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/float/out.sql
+-rw-r--r--   0        0        0       17 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/int/out.sql
+-rw-r--r--   0        0        0       31 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/simple/out.sql
+-rw-r--r--   0        0        0       23 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_literals/true/out.sql
+-rw-r--r--   0        0        0       70 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_misc_conditionals/out.sql
+-rw-r--r--   0        0        0       68 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_named_expressions/cast/out.sql
+-rw-r--r--   0        0        0       83 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_named_expressions/compound_expr/out.sql
+-rw-r--r--   0        0        0       58 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_named_expressions/spaces/out.sql
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_negate/a/out.sql
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_negate/f/out.sql
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_negate/h/out.sql
+-rw-r--r--   0        0        0      152 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_sql_extract/out.sql
+-rw-r--r--   0        0        0       99 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_day_of_week/full_name/out.sql
+-rw-r--r--   0        0        0      115 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_day_of_week/index/out.sql
+-rw-r--r--   0        0        0      121 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/days/out1.sql
+-rw-r--r--   0        0        0       83 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/days/out2.sql
+-rw-r--r--   0        0        0      122 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/hours/out1.sql
+-rw-r--r--   0        0        0       84 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/hours/out2.sql
+-rw-r--r--   0        0        0      124 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/minutes/out1.sql
+-rw-r--r--   0        0        0       86 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/minutes/out2.sql
+-rw-r--r--   0        0        0      123 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/months/out1.sql
+-rw-r--r--   0        0        0       85 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/months/out2.sql
+-rw-r--r--   0        0        0      124 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/seconds/out1.sql
+-rw-r--r--   0        0        0       86 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/seconds/out2.sql
+-rw-r--r--   0        0        0      122 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/weeks/out1.sql
+-rw-r--r--   0        0        0       84 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/weeks/out2.sql
+-rw-r--r--   0        0        0      122 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/years/out1.sql
+-rw-r--r--   0        0        0       84 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_deltas/years/out2.sql
+-rw-r--r--   0        0        0       78 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/day/out.sql
+-rw-r--r--   0        0        0       80 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/hour/out.sql
+-rw-r--r--   0        0        0      104 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/microsecond/out.sql
+-rw-r--r--   0        0        0      101 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/millisecond/out.sql
+-rw-r--r--   0        0        0       84 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/minute/out.sql
+-rw-r--r--   0        0        0       82 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/month/out.sql
+-rw-r--r--   0        0        0       84 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/second/out.sql
+-rw-r--r--   0        0        0       80 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_extract_field/year/out.sql
+-rw-r--r--   0        0        0      122 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_from_integer/default/out.sql
+-rw-r--r--   0        0        0      147 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_from_integer/ms/out.sql
+-rw-r--r--   0        0        0      150 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_from_integer/us/out.sql
+-rw-r--r--   0        0        0       77 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_literals/pd_timestamp/out.sql
+-rw-r--r--   0        0        0       77 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_literals/pydatetime/out.sql
+-rw-r--r--   0        0        0       77 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_literals/timestamp_function/out.sql
+-rw-r--r--   0        0        0       48 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_value_exprs/test_timestamp_now/out.sql
+-rw-r--r--   0        0        0      621 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_add_default_order_by/out.sql
+-rw-r--r--   0        0        0      239 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_aggregate_in_projection/out.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/max/out1.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/max/out2.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/mean/out1.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/mean/out2.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/min/out1.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/min/out2.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/sum/out1.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_cumulative_functions/sum/out2.sql
+-rw-r--r--   0        0        0      180 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_multiple_windows/out.sql
+-rw-r--r--   0        0        0      151 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_nested_analytic_function/out.sql
+-rw-r--r--   0        0        0      104 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_order_by_desc/out1.sql
+-rw-r--r--   0        0        0      188 2024-03-30 19:28:49.936060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_order_by_desc/out2.sql
+-rw-r--r--   0        0        0      203 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_propagate_nested_windows/out.sql
+-rw-r--r--   0        0        0      177 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_rank_functions/out.sql
+-rw-r--r--   0        0        0      244 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_row_number_does_not_require_order_by/out1.sql
+-rw-r--r--   0        0        0      252 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_row_number_does_not_require_order_by/out2.sql
+-rw-r--r--   0        0        0      244 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_row_number_properly_composes_with_arithmetic/out.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/cumulative/out.sql
+-rw-r--r--   0        0        0       95 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_0/out.sql
+-rw-r--r--   0        0        0      137 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_10_5/out.sql
+-rw-r--r--   0        0        0      144 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_2/out.sql
+-rw-r--r--   0        0        0      136 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_2_prec_0/out.sql
+-rw-r--r--   0        0        0      137 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/foll_5_10/out.sql
+-rw-r--r--   0        0        0      144 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/prec_0/out.sql
+-rw-r--r--   0        0        0      144 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/prec_5/out.sql
+-rw-r--r--   0        0        0      136 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/prec_5_foll_0/out.sql
+-rw-r--r--   0        0        0      136 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/prec_5_foll_2/out.sql
+-rw-r--r--   0        0        0      137 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_window_frame_specs/trailing_10/out.sql
+-rw-r--r--   0        0        0     1215 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_analytic_functions.py
+-rw-r--r--   0        0        0     2861 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_bucket_histogram.py
+-rw-r--r--   0        0        0     2846 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_case_exprs.py
+-rw-r--r--   0        0        0     6938 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_client.py
+-rw-r--r--   0        0        0     1076 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_coalesce_greater_least.py
+-rw-r--r--   0        0        0     8439 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_ddl.py
+-rw-r--r--   0        0        0     8913 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_ddl_compilation.py
+-rw-r--r--   0        0        0    19387 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_exprs.py
+-rw-r--r--   0        0        0     1135 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_in_not_in.py
+-rw-r--r--   0        0        0     3857 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_metadata.py
+-rw-r--r--   0        0        0     2486 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_parquet_ddl.py
+-rw-r--r--   0        0        0     7271 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_partition.py
+-rw-r--r--   0        0        0     1704 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_patched.py
+-rw-r--r--   0        0        0     9252 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_sql.py
+-rw-r--r--   0        0        0     2586 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_string_builtins.py
+-rw-r--r--   0        0        0    16540 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_udf.py
+-rw-r--r--   0        0        0     3800 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_unary_builtins.py
+-rw-r--r--   0        0        0     7357 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_value_exprs.py
+-rw-r--r--   0        0        0     4311 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_window.py
+-rw-r--r--   0        0        0     7085 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/impala/udf.py
+-rw-r--r--   0        0        0    16984 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/mssql/__init__.py
+-rw-r--r--   0        0        0    15609 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/mssql/compiler.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/mssql/tests/__init__.py
+-rw-r--r--   0        0        0     1707 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/mssql/tests/conftest.py
+-rw-r--r--   0        0        0     3394 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/mssql/tests/test_client.py
+-rw-r--r--   0        0        0    15883 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/mysql/__init__.py
+-rw-r--r--   0        0        0    12174 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/mysql/compiler.py
+-rw-r--r--   0        0        0      855 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/mysql/converter.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/mysql/tests/__init__.py
+-rw-r--r--   0        0        0     2508 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/mysql/tests/conftest.py
+-rw-r--r--   0        0        0     6291 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/mysql/tests/test_client.py
+-rw-r--r--   0        0        0    18423 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/oracle/__init__.py
+-rw-r--r--   0        0        0    16558 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/oracle/compiler.py
+-rw-r--r--   0        0        0      451 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/oracle/converter.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/oracle/tests/__init__.py
+-rw-r--r--   0        0        0     5014 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/oracle/tests/conftest.py
+-rw-r--r--   0        0        0     1575 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/oracle/tests/test_client.py
+-rw-r--r--   0        0        0      672 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/oracle/tests/test_datatypes.py
+-rw-r--r--   0        0        0    10502 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/__init__.py
+-rw-r--r--   0        0        0     3122 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/convert.py
+-rw-r--r--   0        0        0    26760 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/executor.py
+-rw-r--r--   0        0        0     7176 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/helpers.py
+-rw-r--r--   0        0        0    16143 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/kernels.py
+-rw-r--r--   0        0        0    10393 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/rewrites.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/__init__.py
+-rw-r--r--   0        0        0     9098 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/conftest.py
+-rw-r--r--   0        0        0     6431 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_arrays.py
+-rw-r--r--   0        0        0     5603 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_cast.py
+-rw-r--r--   0        0        0     2288 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_client.py
+-rw-r--r--   0        0        0     1763 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_core.py
+-rw-r--r--   0        0        0     8621 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_functions.py
+-rw-r--r--   0        0        0     1943 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_helpers.py
+-rw-r--r--   0        0        0    21442 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_join.py
+-rw-r--r--   0        0        0     2813 2024-03-30 19:28:49.940060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_maps.py
+-rw-r--r--   0        0        0    25980 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_operations.py
+-rw-r--r--   0        0        0     5619 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_strings.py
+-rw-r--r--   0        0        0     2386 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_structs.py
+-rw-r--r--   0        0        0     5977 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_temporal.py
+-rw-r--r--   0        0        0    12258 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_udf.py
+-rw-r--r--   0        0        0    20161 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_window.py
+-rw-r--r--   0        0        0      741 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/pandas/udf.py
+-rw-r--r--   0        0        0    17597 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/polars/__init__.py
+-rw-r--r--   0        0        0    37062 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/polars/compiler.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/polars/tests/__init__.py
+-rw-r--r--   0        0        0     1688 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/polars/tests/conftest.py
+-rw-r--r--   0        0        0      724 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/polars/tests/test_join.py
+-rw-r--r--   0        0        0     3257 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/polars/tests/test_udf.py
+-rw-r--r--   0        0        0    24072 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/__init__.py
+-rw-r--r--   0        0        0    18588 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/compiler.py
+-rw-r--r--   0        0        0      615 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/converter.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/__init__.py
+-rw-r--r--   0        0        0     2890 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/conftest.py
+-rw-r--r--   0        0        0       56 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_client/test_compile_toplevel/out.sql
+-rw-r--r--   0        0        0      246 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_client/test_timezone_from_column/out.sql
+-rw-r--r--   0        0        0      668 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_functions/test_analytic_functions/out.sql
+-rw-r--r--   0        0        0      108 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_functions/test_cast/double_to_int16/out.sql
+-rw-r--r--   0        0        0      107 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_functions/test_cast/double_to_int8/out.sql
+-rw-r--r--   0        0        0      109 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_functions/test_cast/string_to_decimal_no_params/out.sql
+-rw-r--r--   0        0        0      121 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_functions/test_cast/string_to_decimal_params/out.sql
+-rw-r--r--   0        0        0      118 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_functions/test_cast/string_to_double/out.sql
+-rw-r--r--   0        0        0      106 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_functions/test_cast/string_to_float/out.sql
+-rw-r--r--   0        0        0      113 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_functions/test_date_cast/out.sql
+-rw-r--r--   0        0        0       64 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_functions/test_timestamp_cast_noop/out1.sql
+-rw-r--r--   0        0        0      102 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_functions/test_timestamp_cast_noop/out2.sql
+-rw-r--r--   0        0        0      364 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_functions/test_union_cte/False/out.sql
+-rw-r--r--   0        0        0      356 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_functions/test_union_cte/True/out.sql
+-rw-r--r--   0        0        0      338 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_equals/out1.sql
+-rw-r--r--   0        0        0       97 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_equals/out2.sql
+-rw-r--r--   0        0        0       82 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_equals/out3.sql
+-rw-r--r--   0        0        0      229 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/linestring-geography/out.sql
+-rw-r--r--   0        0        0      229 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/linestring-geometry/out.sql
+-rw-r--r--   0        0        0      223 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/linestring-none/out.sql
+-rw-r--r--   0        0        0      229 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/linestring-srid/out.sql
+-rw-r--r--   0        0        0      377 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multilinestring-geography/out.sql
+-rw-r--r--   0        0        0      377 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multilinestring-geometry/out.sql
+-rw-r--r--   0        0        0      371 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multilinestring-none/out.sql
+-rw-r--r--   0        0        0      377 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multilinestring-srid/out.sql
+-rw-r--r--   0        0        0      257 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipoint-geography/out.sql
+-rw-r--r--   0        0        0      257 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipoint-geometry/out.sql
+-rw-r--r--   0        0        0      251 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipoint-none/out.sql
+-rw-r--r--   0        0        0      257 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipoint-srid/out.sql
+-rw-r--r--   0        0        0      486 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipolygon-geography/out.sql
+-rw-r--r--   0        0        0      486 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipolygon-geometry/out.sql
+-rw-r--r--   0        0        0      474 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipolygon-none/out.sql
+-rw-r--r--   0        0        0      486 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/multipolygon-srid/out.sql
+-rw-r--r--   0        0        0      153 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/point-geography/out.sql
+-rw-r--r--   0        0        0      153 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/point-geometry/out.sql
+-rw-r--r--   0        0        0      147 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/point-none/out.sql
+-rw-r--r--   0        0        0      153 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/point-srid/out.sql
+-rw-r--r--   0        0        0      441 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon-geography/out.sql
+-rw-r--r--   0        0        0      441 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon-geometry/out.sql
+-rw-r--r--   0        0        0      429 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon-none/out.sql
+-rw-r--r--   0        0        0      441 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon-srid/out.sql
+-rw-r--r--   0        0        0      281 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon_single-geography/out.sql
+-rw-r--r--   0        0        0      281 2024-03-30 19:28:49.944060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon_single-geometry/out.sql
+-rw-r--r--   0        0        0      275 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon_single-none/out.sql
+-rw-r--r--   0        0        0      281 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_literals_smoke/polygon_single-srid/out.sql
+-rw-r--r--   0        0        0      124 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/linestring_contains/out.sql
+-rw-r--r--   0        0        0      106 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/linestring_end_point/out.sql
+-rw-r--r--   0        0        0       91 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/linestring_length/out.sql
+-rw-r--r--   0        0        0      110 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/linestring_start_point/out.sql
+-rw-r--r--   0        0        0       97 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/multipolygon_n_points/out.sql
+-rw-r--r--   0        0        0      106 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/point_set_srid/out.sql
+-rw-r--r--   0        0        0       77 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/point_srid/out.sql
+-rw-r--r--   0        0        0       71 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/point_x/out.sql
+-rw-r--r--   0        0        0       71 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/point_y/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/polygon_area/out.sql
+-rw-r--r--   0        0        0       91 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_geo_ops_smoke/polygon_perimeter/out.sql
+-rw-r--r--   0        0        0      103 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr0/out.sql
+-rw-r--r--   0        0        0      109 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr1/out.sql
+-rw-r--r--   0        0        0      109 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr2/out.sql
+-rw-r--r--   0        0        0      109 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr3/out.sql
+-rw-r--r--   0        0        0      109 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr4/out.sql
+-rw-r--r--   0        0        0      109 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr5/out.sql
+-rw-r--r--   0        0        0      109 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr6/out.sql
+-rw-r--r--   0        0        0      109 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_explicit/expr7/out.sql
+-rw-r--r--   0        0        0      139 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp0/out.sql
+-rw-r--r--   0        0        0      139 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp1/out.sql
+-rw-r--r--   0        0        0      139 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp2/out.sql
+-rw-r--r--   0        0        0      199 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp3/out.sql
+-rw-r--r--   0        0        0      199 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp4/out.sql
+-rw-r--r--   0        0        0      215 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp5/out.sql
+-rw-r--r--   0        0        0      243 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp6/out.sql
+-rw-r--r--   0        0        0      295 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp7/out.sql
+-rw-r--r--   0        0        0      199 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_geospatial/test_literal_geospatial_inferred/shp8/out.sql
+-rw-r--r--   0        0        0       80 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_postgis/test_select_linestring_geodata/out.sql
+-rw-r--r--   0        0        0       84 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_postgis/test_select_multipolygon_geodata/out.sql
+-rw-r--r--   0        0        0       70 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_postgis/test_select_point_geodata/out.sql
+-rw-r--r--   0        0        0       74 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_postgis/test_select_polygon_geodata/out.sql
+-rw-r--r--   0        0        0     7544 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/test_client.py
+-rw-r--r--   0        0        0    38740 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/test_functions.py
+-rw-r--r--   0        0        0    17043 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/test_geospatial.py
+-rw-r--r--   0        0        0      416 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/test_json.py
+-rw-r--r--   0        0        0     9321 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/test_postgis.py
+-rw-r--r--   0        0        0      488 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/test_string.py
+-rw-r--r--   0        0        0     5188 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/test_udf.py
+-rw-r--r--   0        0        0    24362 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/pyspark/__init__.py
+-rw-r--r--   0        0        0    16406 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/pyspark/compiler.py
+-rw-r--r--   0        0        0     1263 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/pyspark/converter.py
+-rw-r--r--   0        0        0     4491 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/pyspark/datatypes.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/__init__.py
+-rw-r--r--   0        0        0    11767 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/conftest.py
+-rw-r--r--   0        0        0      665 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/test_aggregation.py
+-rw-r--r--   0        0        0     4658 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/test_array.py
+-rw-r--r--   0        0        0     3805 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/test_basic.py
+-rw-r--r--   0        0        0     4895 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/test_ddl.py
+-rw-r--r--   0        0        0      801 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/test_null.py
+-rw-r--r--   0        0        0     2340 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/test_window.py
+-rw-r--r--   0        0        0     8473 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/risingwave/__init__.py
+-rw-r--r--   0        0        0     2747 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/risingwave/compiler.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/risingwave/tests/__init__.py
+-rw-r--r--   0        0        0     2386 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/risingwave/tests/conftest.py
+-rw-r--r--   0        0        0       56 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/risingwave/tests/snapshots/test_client/test_compile_toplevel/out.sql
+-rw-r--r--   0        0        0      349 2024-03-30 19:28:49.948060 turntable_spoonbill-9.0.5/ibis/backends/risingwave/tests/snapshots/test_functions/test_analytic_functions/out.sql
+-rw-r--r--   0        0        0      364 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/risingwave/tests/snapshots/test_functions/test_union_cte/False/out.sql
+-rw-r--r--   0        0        0      356 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/risingwave/tests/snapshots/test_functions/test_union_cte/True/out.sql
+-rw-r--r--   0        0        0     3511 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/risingwave/tests/test_client.py
+-rw-r--r--   0        0        0    25860 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/risingwave/tests/test_functions.py
+-rw-r--r--   0        0        0      416 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/risingwave/tests/test_json.py
+-rw-r--r--   0        0        0    37436 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/snowflake/__init__.py
+-rw-r--r--   0        0        0    21366 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/snowflake/compiler.py
+-rw-r--r--   0        0        0     2914 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/snowflake/converter.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/snowflake/tests/__init__.py
+-rw-r--r--   0        0        0     6274 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/snowflake/tests/conftest.py
+-rw-r--r--   0        0        0     8646 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/snowflake/tests/test_client.py
+-rw-r--r--   0        0        0     3971 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/snowflake/tests/test_datatypes.py
+-rw-r--r--   0        0        0     4165 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/snowflake/tests/test_udf.py
+-rw-r--r--   0        0        0    12441 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sql/__init__.py
+-rw-r--r--   0        0        0    46975 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sql/compiler.py
+-rw-r--r--   0        0        0    35564 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sql/datatypes.py
+-rw-r--r--   0        0        0     3520 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sql/ddl.py
+-rw-r--r--   0        0        0     9985 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sql/dialects.py
+-rw-r--r--   0        0        0     9852 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sql/rewrites.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sql/tests/__init__.py
+-rw-r--r--   0        0        0      550 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sql/tests/test_compiler.py
+-rw-r--r--   0        0        0     2565 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sql/tests/test_datatypes.py
+-rw-r--r--   0        0        0    18080 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sqlite/__init__.py
+-rw-r--r--   0        0        0    15477 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sqlite/compiler.py
+-rw-r--r--   0        0        0      751 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sqlite/converter.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sqlite/tests/__init__.py
+-rw-r--r--   0        0        0     2608 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sqlite/tests/conftest.py
+-rw-r--r--   0        0        0     2059 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sqlite/tests/test_client.py
+-rw-r--r--   0        0        0     3053 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sqlite/tests/test_types.py
+-rw-r--r--   0        0        0     9750 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/sqlite/udf.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/__init__.py
+-rw-r--r--   0        0        0    12682 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/base.py
+-rw-r--r--   0        0        0     2637 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/data.py
+-rw-r--r--   0        0        0     4954 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/errors.py
+-rw-r--r--   0        0        0      600 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/bigquery/out.sql
+-rw-r--r--   0        0        0      714 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/clickhouse/out.sql
+-rw-r--r--   0        0        0      714 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/datafusion/out.sql
+-rw-r--r--   0        0        0      714 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/druid/out.sql
+-rw-r--r--   0        0        0      748 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/duckdb/out.sql
+-rw-r--r--   0        0        0      600 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/exasol/out.sql
+-rw-r--r--   0        0        0      622 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/flink/out.sql
+-rw-r--r--   0        0        0      622 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/impala/out.sql
+-rw-r--r--   0        0        0      765 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/mssql/out.sql
+-rw-r--r--   0        0        0      702 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/mysql/out.sql
+-rw-r--r--   0        0        0      598 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/oracle/out.sql
+-rw-r--r--   0        0        0      714 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/postgres/out.sql
+-rw-r--r--   0        0        0      622 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/pyspark/out.sql
+-rw-r--r--   0        0        0      714 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/risingwave/out.sql
+-rw-r--r--   0        0        0      600 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/snowflake/out.sql
+-rw-r--r--   0        0        0      736 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/sqlite/out.sql
+-rw-r--r--   0        0        0      714 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/trino/out.sql
+-rw-r--r--   0        0        0      111 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/bigquery/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/clickhouse/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/datafusion/out.sql
+-rw-r--r--   0        0        0      111 2024-03-30 19:28:49.952060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/druid/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/duckdb/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/exasol/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/flink/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/impala/out.sql
+-rw-r--r--   0        0        0      174 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/mssql/out.sql
+-rw-r--r--   0        0        0       99 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/mysql/out.sql
+-rw-r--r--   0        0        0      112 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/oracle/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/postgres/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/pyspark/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/risingwave/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/snowflake/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/sqlite/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_default_limit/trino/out.sql
+-rw-r--r--   0        0        0      111 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/bigquery/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/clickhouse/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/datafusion/out.sql
+-rw-r--r--   0        0        0      111 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/druid/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/duckdb/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/exasol/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/flink/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/impala/out.sql
+-rw-r--r--   0        0        0      174 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/mssql/out.sql
+-rw-r--r--   0        0        0       99 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/mysql/out.sql
+-rw-r--r--   0        0        0      112 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/oracle/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/postgres/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/pyspark/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/risingwave/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/snowflake/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/sqlite/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_disable_query_limit/trino/out.sql
+-rw-r--r--   0        0        0      116 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/bigquery/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/clickhouse/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/datafusion/out.sql
+-rw-r--r--   0        0        0      452 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/druid/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/duckdb/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/exasol/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/flink/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/impala/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/mssql/out.sql
+-rw-r--r--   0        0        0      417 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/mysql/out.sql
+-rw-r--r--   0        0        0      411 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/oracle/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/postgres/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/pyspark/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/risingwave/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/snowflake/out.sql
+-rw-r--r--   0        0        0      399 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/sqlite/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_interactive_execute_on_repr/trino/out.sql
+-rw-r--r--   0        0        0      158 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/bigquery/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/clickhouse/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/datafusion/out.sql
+-rw-r--r--   0        0        0      162 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/druid/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/duckdb/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/exasol/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/flink/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/impala/out.sql
+-rw-r--r--   0        0        0      229 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/mssql/out.sql
+-rw-r--r--   0        0        0      146 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/mysql/out.sql
+-rw-r--r--   0        0        0      172 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/oracle/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/postgres/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/pyspark/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/risingwave/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/snowflake/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.956060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/sqlite/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_interactive/test_respect_set_limit/trino/out.sql
+-rw-r--r--   0        0        0      324 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_join/test_complex_join_agg/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/bigquery/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/clickhouse/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/datafusion/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/druid/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/duckdb/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/exasol/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/flink/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/impala/out.sql
+-rw-r--r--   0        0        0      356 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/mssql/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/mysql/out.sql
+-rw-r--r--   0        0        0      305 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/oracle/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/postgres/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/pyspark/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/risingwave/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/snowflake/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/sqlite/out.sql
+-rw-r--r--   0        0        0      323 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_cte_refs_in_topo_order/trino/out.sql
+-rw-r--r--   0        0        0      395 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/bigquery/out.sql
+-rw-r--r--   0        0        0      691 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/clickhouse/out.sql
+-rw-r--r--   0        0        0      514 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/datafusion/out.sql
+-rw-r--r--   0        0        0      395 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/druid/out.sql
+-rw-r--r--   0        0        0      395 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/duckdb/out.sql
+-rw-r--r--   0        0        0      395 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/exasol/out.sql
+-rw-r--r--   0        0        0      691 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/flink/out.sql
+-rw-r--r--   0        0        0      395 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/impala/out.sql
+-rw-r--r--   0        0        0      691 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/mssql/out.sql
+-rw-r--r--   0        0        0      395 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/mysql/out.sql
+-rw-r--r--   0        0        0      688 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/oracle/out.sql
+-rw-r--r--   0        0        0      395 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/postgres/out.sql
+-rw-r--r--   0        0        0      395 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/pyspark/out.sql
+-rw-r--r--   0        0        0      395 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/risingwave/out.sql
+-rw-r--r--   0        0        0      395 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/snowflake/out.sql
+-rw-r--r--   0        0        0      395 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/sqlite/out.sql
+-rw-r--r--   0        0        0      395 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/trino/out.sql
+-rw-r--r--   0        0        0      137 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/bigquery/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/clickhouse/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/datafusion/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/druid/out.sql
+-rw-r--r--   0        0        0      155 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/duckdb/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/exasol/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/flink/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/impala/out.sql
+-rw-r--r--   0        0        0      177 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/mssql/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/mysql/out.sql
+-rw-r--r--   0        0        0      132 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/oracle/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/postgres/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/pyspark/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/risingwave/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/snowflake/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/sqlite/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_isin_bug/trino/out.sql
+-rw-r--r--   0        0        0     6419 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/bigquery/out.sql
+-rw-r--r--   0        0        0     3435 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/clickhouse/out.sql
+-rw-r--r--   0        0        0     2512 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/duckdb/out.sql
+-rw-r--r--   0        0        0     2850 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/postgres/out.sql
+-rw-r--r--   0        0        0     3024 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/pyspark/out.sql
+-rw-r--r--   0        0        0     2850 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/risingwave/out.sql
+-rw-r--r--   0        0        0     7590 2024-03-30 19:28:49.960060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/trino/out.sql
+-rw-r--r--   0        0        0       55 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/bigquery-date/out.sql
+-rw-r--r--   0        0        0       98 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/bigquery-timestamp/out.sql
+-rw-r--r--   0        0        0       60 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/clickhouse-date/out.sql
+-rw-r--r--   0        0        0      119 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/clickhouse-timestamp/out.sql
+-rw-r--r--   0        0        0       71 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/datafusion-date/out.sql
+-rw-r--r--   0        0        0      133 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/datafusion-timestamp/out.sql
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/druid-date/out.sql
+-rw-r--r--   0        0        0      108 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/druid-timestamp/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/duckdb-date/out.sql
+-rw-r--r--   0        0        0      103 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/duckdb-timestamp/out.sql
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/exasol-date/out.sql
+-rw-r--r--   0        0        0      105 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/exasol-timestamp/out.sql
+-rw-r--r--   0        0        0       52 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/impala-date/out.sql
+-rw-r--r--   0        0        0       89 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/impala-timestamp/out.sql
+-rw-r--r--   0        0        0       65 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/mssql-date/out.sql
+-rw-r--r--   0        0        0      111 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/mssql-timestamp/out.sql
+-rw-r--r--   0        0        0       58 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/mysql-date/out.sql
+-rw-r--r--   0        0        0      100 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/mysql-timestamp/out.sql
+-rw-r--r--   0        0        0       77 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/oracle-date/out.sql
+-rw-r--r--   0        0        0      134 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/oracle-timestamp/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/postgres-date/out.sql
+-rw-r--r--   0        0        0      108 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/postgres-timestamp/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/pyspark-date/out.sql
+-rw-r--r--   0        0        0      108 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/pyspark-timestamp/out.sql
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/risingwave-date/out.sql
+-rw-r--r--   0        0        0      108 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/risingwave-timestamp/out.sql
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/snowflake-date/out.sql
+-rw-r--r--   0        0        0      113 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/snowflake-timestamp/out.sql
+-rw-r--r--   0        0        0       52 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/sqlite-date/out.sql
+-rw-r--r--   0        0        0       89 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/sqlite-timestamp/out.sql
+-rw-r--r--   0        0        0       71 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/trino-date/out.sql
+-rw-r--r--   0        0        0      132 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_temporal_literal_sql/trino-timestamp/out.sql
+-rw-r--r--   0        0        0       49 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-bigquery/out.sql
+-rw-r--r--   0        0        0       71 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-clickhouse/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-datafusion/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-druid/out.sql
+-rw-r--r--   0        0        0       57 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-duckdb/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-exasol/out.sql
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-impala/out.sql
+-rw-r--r--   0        0        0       65 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-mssql/out.sql
+-rw-r--r--   0        0        0       56 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-mysql/out.sql
+-rw-r--r--   0        0        0       92 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-oracle/out.sql
+-rw-r--r--   0        0        0      109 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-postgres/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-risingwave/out.sql
+-rw-r--r--   0        0        0       64 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-snowflake/out.sql
+-rw-r--r--   0        0        0       47 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-sqlite/out.sql
+-rw-r--r--   0        0        0       61 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/0-trino/out.sql
+-rw-r--r--   0        0        0       57 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-bigquery/out.sql
+-rw-r--r--   0        0        0       86 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-clickhouse/out.sql
+-rw-r--r--   0        0        0       76 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-datafusion/out.sql
+-rw-r--r--   0        0        0       76 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-druid/out.sql
+-rw-r--r--   0        0        0       70 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-duckdb/out.sql
+-rw-r--r--   0        0        0       76 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-exasol/out.sql
+-rw-r--r--   0        0        0       81 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-impala/out.sql
+-rw-r--r--   0        0        0       73 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-mssql/out.sql
+-rw-r--r--   0        0        0       69 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-mysql/out.sql
+-rw-r--r--   0        0        0      107 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-oracle/out.sql
+-rw-r--r--   0        0        0      122 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-postgres/out.sql
+-rw-r--r--   0        0        0       76 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-risingwave/out.sql
+-rw-r--r--   0        0        0       80 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-snowflake/out.sql
+-rw-r--r--   0        0        0       62 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-sqlite/out.sql
+-rw-r--r--   0        0        0       76 2024-03-30 19:28:49.964060 turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_temporal/test_time_literal_sql/234567-trino/out.sql
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/__init__.py
+-rw-r--r--   0        0        0     4714 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/conftest.py
+-rw-r--r--   0        0        0      335 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_agg_and_non_agg_filter/out.sql
+-rw-r--r--   0        0        0      372 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_agg_filter/out.sql
+-rw-r--r--   0        0        0      372 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_agg_filter_with_alias/out.sql
+-rw-r--r--   0        0        0      582 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_column_distinct/decompiled.py
+-rw-r--r--   0        0        0      104 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_column_distinct/out.sql
+-rw-r--r--   0        0        0      128 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_column_expr_default_name/decompiled.py
+-rw-r--r--   0        0        0       94 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_column_expr_default_name/out.sql
+-rw-r--r--   0        0        0      142 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_column_expr_retains_name/decompiled.py
+-rw-r--r--   0        0        0       82 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_column_expr_retains_name/out.sql
+-rw-r--r--   0        0        0      649 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_count_distinct/decompiled.py
+-rw-r--r--   0        0        0      484 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_count_distinct/out.sql
+-rw-r--r--   0        0        0      898 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_difference_project_column/decompiled.py
+-rw-r--r--   0        0        0      475 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_difference_project_column/out.sql
+-rw-r--r--   0        0        0      236 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_having_from_filter/decompiled.py
+-rw-r--r--   0        0        0      304 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_having_from_filter/out.sql
+-rw-r--r--   0        0        0      320 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_having_size/out.sql
+-rw-r--r--   0        0        0      903 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_intersect_project_column/decompiled.py
+-rw-r--r--   0        0        0      478 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_intersect_project_column/out.sql
+-rw-r--r--   0        0        0      737 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_multiple_count_distinct/decompiled.py
+-rw-r--r--   0        0        0      180 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_multiple_count_distinct/out.sql
+-rw-r--r--   0        0        0      377 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_pushdown_with_or/out.sql
+-rw-r--r--   0        0        0      314 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_simple_agg_filter/out.sql
+-rw-r--r--   0        0        0      407 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_subquery_where_location/decompiled.py
+-rw-r--r--   0        0        0      378 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_subquery_where_location/out.sql
+-rw-r--r--   0        0        0      851 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_table_difference/decompiled.py
+-rw-r--r--   0        0        0      491 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_table_difference/out.sql
+-rw-r--r--   0        0        0      617 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_table_distinct/decompiled.py
+-rw-r--r--   0        0        0      124 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_table_distinct/out.sql
+-rw-r--r--   0        0        0      446 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_table_drop_with_filter/decompiled.py
+-rw-r--r--   0        0        0      355 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_table_drop_with_filter/out.sql
+-rw-r--r--   0        0        0      850 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_table_intersect/decompiled.py
+-rw-r--r--   0        0        0      494 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_table_intersect/out.sql
+-rw-r--r--   0        0        0      846 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_union/decompiled.py
+-rw-r--r--   0        0        0      490 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_union/out.sql
+-rw-r--r--   0        0        0      124 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_union_order_by/decompiled.py
+-rw-r--r--   0        0        0      228 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_union_order_by/out.sql
+-rw-r--r--   0        0        0      857 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_union_project_column/decompiled.py
+-rw-r--r--   0        0        0      478 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_union_project_column/out.sql
+-rw-r--r--   0        0        0      661 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_count_joined/decompiled.py
+-rw-r--r--   0        0        0      290 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_count_joined/out.sql
+-rw-r--r--   0        0        0      195 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_having/explicit.sql
+-rw-r--r--   0        0        0      243 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_having/inline.sql
+-rw-r--r--   0        0        0      267 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_projection_alias_bug/out.sql
+-rw-r--r--   0        0        0      366 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_projection_subquery/agg_filtered.sql
+-rw-r--r--   0        0        0      405 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_projection_subquery/agg_filtered2.sql
+-rw-r--r--   0        0        0      252 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_projection_subquery/filtered.sql
+-rw-r--r--   0        0        0      231 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_projection_subquery/proj.sql
+-rw-r--r--   0        0        0      369 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_anti_join/decompiled.py
+-rw-r--r--   0        0        0      145 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_anti_join/out.sql
+-rw-r--r--   0        0        0      197 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_bool_bool/decompiled.py
+-rw-r--r--   0        0        0      154 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_bool_bool/out.sql
+-rw-r--r--   0        0        0      574 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_bug_duplicated_where/out.sql
+-rw-r--r--   0        0        0     1096 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_bug_project_multiple_times/out.sql
+-rw-r--r--   0        0        0      930 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_case_in_projection/decompiled.py
+-rw-r--r--   0        0        0      388 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_case_in_projection/out.sql
+-rw-r--r--   0        0        0      611 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_chain_limit_doesnt_collapse/result.sql
+-rw-r--r--   0        0        0      384 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_complex_union/result.sql
+-rw-r--r--   0        0        0      374 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_double_nested_subquery_no_aliases/out.sql
+-rw-r--r--   0        0        0      202 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_endswith/decompiled.py
+-rw-r--r--   0        0        0       67 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_endswith/out.sql
+-rw-r--r--   0        0        0      173 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_exists_subquery/out.sql
+-rw-r--r--   0        0        0      245 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_filter_inside_exists/out.sql
+-rw-r--r--   0        0        0      172 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_filter_predicates/out.sql
+-rw-r--r--   0        0        0      513 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_filter_self_join_analysis_bug/result.sql
+-rw-r--r--   0        0        0      379 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_filter_subquery_derived_reduction/expr3.sql
+-rw-r--r--   0        0        0      440 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_filter_subquery_derived_reduction/expr4.sql
+-rw-r--r--   0        0        0      242 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_fuse_projections/decompiled.py
+-rw-r--r--   0        0        0      148 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_fuse_projections/project.sql
+-rw-r--r--   0        0        0      190 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_fuse_projections/project_filter.sql
+-rw-r--r--   0        0        0       79 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_identifier_quoting/out.sql
+-rw-r--r--   0        0        0      131 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_incorrect_predicate_pushdown/result.sql
+-rw-r--r--   0        0        0       99 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_incorrect_predicate_pushdown_with_literal/result.sql
+-rw-r--r--   0        0        0     1188 2024-03-30 19:28:49.968060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_between_joins/decompiled.py
+-rw-r--r--   0        0        0      403 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_between_joins/out.sql
+-rw-r--r--   0        0        0      637 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_filtered_tables_no_pushdown/out.sql
+-rw-r--r--   0        0        0     1369 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_just_materialized/decompiled.py
+-rw-r--r--   0        0        0      490 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_just_materialized/out.sql
+-rw-r--r--   0        0        0      430 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_projection_subquery_bug/out.sql
+-rw-r--r--   0        0        0      565 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_with_conditional_aggregate/result.sql
+-rw-r--r--   0        0        0      192 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_with_limited_table/out.sql
+-rw-r--r--   0        0        0      397 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_limit_cte_extract/out.sql
+-rw-r--r--   0        0        0     1981 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_limit_with_self_join/decompiled.py
+-rw-r--r--   0        0        0     1051 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_limit_with_self_join/out.sql
+-rw-r--r--   0        0        0      429 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_loj_subquery_filter_handling/out.sql
+-rw-r--r--   0        0        0      540 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_multiple_joins/decompiled.py
+-rw-r--r--   0        0        0      247 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_multiple_joins/out.sql
+-rw-r--r--   0        0        0      552 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_multiple_limits/decompiled.py
+-rw-r--r--   0        0        0       99 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_multiple_limits/out.sql
+-rw-r--r--   0        0        0       72 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_nameless_table/decompiled.py
+-rw-r--r--   0        0        0       23 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_nameless_table/out.sql
+-rw-r--r--   0        0        0      696 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_order_by_on_limit_yield_subquery/decompiled.py
+-rw-r--r--   0        0        0      212 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_order_by_on_limit_yield_subquery/out.sql
+-rw-r--r--   0        0        0       98 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_projection_filter_fuse/out.sql
+-rw-r--r--   0        0        0      174 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_scalar_subquery_different_table/out.sql
+-rw-r--r--   0        0        0      213 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/agg_explicit_column/decompiled.py
+-rw-r--r--   0        0        0       84 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/agg_explicit_column/out.sql
+-rw-r--r--   0        0        0      227 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/agg_string_columns/decompiled.py
+-rw-r--r--   0        0        0      106 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/agg_string_columns/out.sql
+-rw-r--r--   0        0        0      161 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/aggregate_table_count_metric/decompiled.py
+-rw-r--r--   0        0        0       60 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/aggregate_table_count_metric/out.sql
+-rw-r--r--   0        0        0      183 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/filter_then_limit/decompiled.py
+-rw-r--r--   0        0        0      131 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/filter_then_limit/out.sql
+-rw-r--r--   0        0        0      163 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/limit_simple/decompiled.py
+-rw-r--r--   0        0        0       40 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/limit_simple/out.sql
+-rw-r--r--   0        0        0      197 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/limit_then_filter/decompiled.py
+-rw-r--r--   0        0        0      167 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/limit_then_filter/out.sql
+-rw-r--r--   0        0        0      166 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/limit_with_offset/decompiled.py
+-rw-r--r--   0        0        0       49 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/limit_with_offset/out.sql
+-rw-r--r--   0        0        0      195 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/mixed_columns_ascending/decompiled.py
+-rw-r--r--   0        0        0       58 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/mixed_columns_ascending/out.sql
+-rw-r--r--   0        0        0      138 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/self_reference_simple/decompiled.py
+-rw-r--r--   0        0        0       34 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/self_reference_simple/out.sql
+-rw-r--r--   0        0        0      177 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/single_column/decompiled.py
+-rw-r--r--   0        0        0      108 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/single_column/out.sql
+-rw-r--r--   0        0        0      328 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/test_physical_table_reference_translate/decompiled.py
+-rw-r--r--   0        0        0       26 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_select_sql/test_physical_table_reference_translate/out.sql
+-rw-r--r--   0        0        0      485 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_self_join_subquery_distinct_equal/out.sql
+-rw-r--r--   0        0        0      369 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_semi_join/decompiled.py
+-rw-r--r--   0        0        0      145 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_semi_join/out.sql
+-rw-r--r--   0        0        0      402 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_simple_joins/decompiled.py
+-rw-r--r--   0        0        0      146 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_simple_joins/inner.sql
+-rw-r--r--   0        0        0      180 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_simple_joins/inner_two_preds.sql
+-rw-r--r--   0        0        0      151 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_simple_joins/left.sql
+-rw-r--r--   0        0        0      151 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_simple_joins/outer.sql
+-rw-r--r--   0        0        0      141 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_sort_then_group_by_propagates_keys/result1.sql
+-rw-r--r--   0        0        0      141 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_sort_then_group_by_propagates_keys/result2.sql
+-rw-r--r--   0        0        0      204 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_startswith/decompiled.py
+-rw-r--r--   0        0        0       72 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_startswith/out.sql
+-rw-r--r--   0        0        0     1991 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_factor_correlated_subquery/out.sql
+-rw-r--r--   0        0        0      178 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_in_filter_predicate/expr.sql
+-rw-r--r--   0        0        0      341 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_in_filter_predicate/expr2.sql
+-rw-r--r--   0        0        0      629 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_in_union/decompiled.py
+-rw-r--r--   0        0        0      420 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_in_union/out.sql
+-rw-r--r--   0        0        0      512 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_used_for_self_join/out.sql
+-rw-r--r--   0        0        0      656 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_analysis_bug/out.sql
+-rw-r--r--   0        0        0      369 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_operation/e1.sql
+-rw-r--r--   0        0        0      382 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_operation/e2.sql
+-rw-r--r--   0        0        0     1178 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_predicate_pushdown_bug/out.sql
+-rw-r--r--   0        0        0      223 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_to_aggregate/out.sql
+-rw-r--r--   0        0        0      841 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_tpch_self_join_failure/out.sql
+-rw-r--r--   0        0        0      728 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_analyze_scalar_op/decompiled.py
+-rw-r--r--   0        0        0      591 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_analyze_scalar_op/out.sql
+-rw-r--r--   0        0        0      458 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_no_pushdown_possible/decompiled.py
+-rw-r--r--   0        0        0      339 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_no_pushdown_possible/out.sql
+-rw-r--r--   0        0        0      438 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_with_between/decompiled.py
+-rw-r--r--   0        0        0      264 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_with_between/out.sql
+-rw-r--r--   0        0        0      469 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_with_join/decompiled.py
+-rw-r--r--   0        0        0      396 2024-03-30 19:28:49.972060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_with_join/out.sql
+-rw-r--r--   0        0        0      243 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_aggregate/having_count/out.sql
+-rw-r--r--   0        0        0      195 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_aggregate/having_sum/out.sql
+-rw-r--r--   0        0        0       84 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_aggregate/single/out.sql
+-rw-r--r--   0        0        0      106 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_aggregate/two/out.sql
+-rw-r--r--   0        0        0      121 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_between/out.sql
+-rw-r--r--   0        0        0      156 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_boolean_conjunction/and/out.sql
+-rw-r--r--   0        0        0      155 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_boolean_conjunction/or/out.sql
+-rw-r--r--   0        0        0      211 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_coalesce/out.sql
+-rw-r--r--   0        0        0       91 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_comparisons/eq/out.sql
+-rw-r--r--   0        0        0       92 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_comparisons/ge/out.sql
+-rw-r--r--   0        0        0       91 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_comparisons/gt/out.sql
+-rw-r--r--   0        0        0       92 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_comparisons/le/out.sql
+-rw-r--r--   0        0        0       91 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_comparisons/lt/out.sql
+-rw-r--r--   0        0        0       92 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_comparisons/ne/out.sql
+-rw-r--r--   0        0        0      291 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_cte_factor_distinct_but_equal/out.sql
+-rw-r--r--   0        0        0       87 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_distinct/count_distinct/out.sql
+-rw-r--r--   0        0        0      121 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_distinct/group_by_count_distinct/out.sql
+-rw-r--r--   0        0        0      124 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_distinct/projection_distinct/out.sql
+-rw-r--r--   0        0        0      104 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_distinct/single_column_projection_distinct/out.sql
+-rw-r--r--   0        0        0       54 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_distinct/table_distinct/out.sql
+-rw-r--r--   0        0        0      179 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_exists/e1.sql
+-rw-r--r--   0        0        0      239 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_exists/e2.sql
+-rw-r--r--   0        0        0      217 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_filter_group_by_agg_with_same_name/out.sql
+-rw-r--r--   0        0        0      704 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_gh_1045/out.sql
+-rw-r--r--   0        0        0       78 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_isnull_notnull/isnull/out.sql
+-rw-r--r--   0        0        0       82 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_isnull_notnull/notnull/out.sql
+-rw-r--r--   0        0        0      490 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_join_just_materialized/out.sql
+-rw-r--r--   0        0        0      250 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_joins/inner/out.sql
+-rw-r--r--   0        0        0      191 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_joins/inner_select/out.sql
+-rw-r--r--   0        0        0      255 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_joins/left/out.sql
+-rw-r--r--   0        0        0      196 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_joins/left_select/out.sql
+-rw-r--r--   0        0        0      255 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_joins/outer/out.sql
+-rw-r--r--   0        0        0      196 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_joins/outer_select/out.sql
+-rw-r--r--   0        0        0       40 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_limit/expr_fn0/out.sql
+-rw-r--r--   0        0        0       49 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_limit/expr_fn1/out.sql
+-rw-r--r--   0        0        0      131 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_limit_filter/out.sql
+-rw-r--r--   0        0        0      167 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_limit_subquery/out.sql
+-rw-r--r--   0        0        0      512 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_lower_projection_sort_key/decompiled.py
+-rw-r--r--   0        0        0      405 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_lower_projection_sort_key/out.sql
+-rw-r--r--   0        0        0      330 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_multi_join/out.sql
+-rw-r--r--   0        0        0      100 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_mutate_filter_join_no_cross_join/out.sql
+-rw-r--r--   0        0        0       91 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_named_expr/out.sql
+-rw-r--r--   0        0        0      105 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_negate/out.sql
+-rw-r--r--   0        0        0      986 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_no_cart_join/out.sql
+-rw-r--r--   0        0        0     1517 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_no_cartesian_join/out.sql
+-rw-r--r--   0        0        0      319 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_no_cross_join/out.sql
+-rw-r--r--   0        0        0      205 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_not_exists/out.sql
+-rw-r--r--   0        0        0      108 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_order_by/column/out.sql
+-rw-r--r--   0        0        0      108 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_order_by/random/out.sql
+-rw-r--r--   0        0        0      115 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_order_by_expr/out.sql
+-rw-r--r--   0        0        0      238 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_searched_case/out.sql
+-rw-r--r--   0        0        0      457 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_self_reference_in_not_exists/anti.sql
+-rw-r--r--   0        0        0      431 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_self_reference_in_not_exists/semi.sql
+-rw-r--r--   0        0        0      146 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_self_reference_join/out.sql
+-rw-r--r--   0        0        0      118 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_simple_case/out.sql
+-rw-r--r--   0        0        0      206 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_sort_aggregation_translation_failure/out.sql
+-rw-r--r--   0        0        0      231 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_subquery_aliased/out.sql
+-rw-r--r--   0        0        0      349 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_where_correlated_subquery/out.sql
+-rw-r--r--   0        0        0      699 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_where_correlated_subquery_with_join/out.sql
+-rw-r--r--   0        0        0      198 2024-03-30 19:28:49.976060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_where_simple_comparisons/decompiled.py
+-rw-r--r--   0        0        0      177 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_where_simple_comparisons/out.sql
+-rw-r--r--   0        0        0      162 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_where_uncorrelated_subquery/out.sql
+-rw-r--r--   0        0        0       94 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_aggregate/having_count/out.sql
+-rw-r--r--   0        0        0       94 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_aggregate/having_sum/out.sql
+-rw-r--r--   0        0        0       70 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_aggregate/single/out.sql
+-rw-r--r--   0        0        0       88 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_aggregate/two/out.sql
+-rw-r--r--   0        0        0       77 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_between/out.sql
+-rw-r--r--   0        0        0       86 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_boolean_conjunction/and/out.sql
+-rw-r--r--   0        0        0       85 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_boolean_conjunction/or/out.sql
+-rw-r--r--   0        0        0      168 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_coalesce/out.sql
+-rw-r--r--   0        0        0       64 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_comparisons/eq/out.sql
+-rw-r--r--   0        0        0       65 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_comparisons/ge/out.sql
+-rw-r--r--   0        0        0       64 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_comparisons/gt/out.sql
+-rw-r--r--   0        0        0       65 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_comparisons/le/out.sql
+-rw-r--r--   0        0        0       64 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_comparisons/lt/out.sql
+-rw-r--r--   0        0        0       65 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_comparisons/ne/out.sql
+-rw-r--r--   0        0        0      167 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_cte_factor_distinct_but_equal/out.sql
+-rw-r--r--   0        0        0       77 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_distinct/count_distinct/out.sql
+-rw-r--r--   0        0        0      107 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_distinct/group_by_count_distinct/out.sql
+-rw-r--r--   0        0        0       76 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_distinct/projection_distinct/out.sql
+-rw-r--r--   0        0        0       62 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_distinct/single_column_projection_distinct/out.sql
+-rw-r--r--   0        0        0      252 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_distinct/table_distinct/out.sql
+-rw-r--r--   0        0        0      161 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_exists/e1.sql
+-rw-r--r--   0        0        0      181 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_exists/e2.sql
+-rw-r--r--   0        0        0      183 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_filter_group_by_agg_with_same_name/out.sql
+-rw-r--r--   0        0        0      631 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_gh_1045/out.sql
+-rw-r--r--   0        0        0       68 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_isnull_notnull/isnull/out.sql
+-rw-r--r--   0        0        0       72 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_isnull_notnull/notnull/out.sql
+-rw-r--r--   0        0        0      390 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_join_just_materialized/out.sql
+-rw-r--r--   0        0        0      200 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_joins/inner/out.sql
+-rw-r--r--   0        0        0      153 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_joins/inner_select/out.sql
+-rw-r--r--   0        0        0      211 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_joins/left/out.sql
+-rw-r--r--   0        0        0      164 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_joins/left_select/out.sql
+-rw-r--r--   0        0        0      211 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_joins/outer/out.sql
+-rw-r--r--   0        0        0      164 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_joins/outer_select/out.sql
+-rw-r--r--   0        0        0       73 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_limit/expr_fn0/out.sql
+-rw-r--r--   0        0        0       82 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_limit/expr_fn1/out.sql
+-rw-r--r--   0        0        0       90 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_limit_filter/out.sql
+-rw-r--r--   0        0        0      197 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_limit_subquery/out.sql
+-rw-r--r--   0        0        0      489 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_lower_projection_sort_key/decompiled.py
+-rw-r--r--   0        0        0      459 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_lower_projection_sort_key/out.sql
+-rw-r--r--   0        0        0      252 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_multi_join/out.sql
+-rw-r--r--   0        0        0      173 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_mutate_filter_join_no_cross_join/out.sql
+-rw-r--r--   0        0        0       64 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_named_expr/out.sql
+-rw-r--r--   0        0        0       65 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_negate/out.sql
+-rw-r--r--   0        0        0      592 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_no_cart_join/out.sql
+-rw-r--r--   0        0        0      237 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_no_cross_join/out.sql
+-rw-r--r--   0        0        0      187 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_not_exists/out.sql
+-rw-r--r--   0        0        0       96 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_order_by/column/out.sql
+-rw-r--r--   0        0        0      100 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_order_by/random/out.sql
+-rw-r--r--   0        0        0      155 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_order_by_expr/out.sql
+-rw-r--r--   0        0        0      176 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_searched_case/out.sql
+-rw-r--r--   0        0        0      399 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_self_reference_in_not_exists/anti.sql
+-rw-r--r--   0        0        0      373 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_self_reference_in_not_exists/semi.sql
+-rw-r--r--   0        0        0      108 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_self_reference_join/out.sql
+-rw-r--r--   0        0        0      108 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_simple_case/out.sql
+-rw-r--r--   0        0        0      192 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_sort_aggregation_translation_failure/out.sql
+-rw-r--r--   0        0        0      203 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_subquery_aliased/out.sql
+-rw-r--r--   0        0        0      840 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_tpc_h11/out.sql
+-rw-r--r--   0        0        0      344 2024-03-30 19:28:49.980060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_tpc_h17/out.sql
+-rw-r--r--   0        0        0      183 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_where_correlated_subquery/out.sql
+-rw-r--r--   0        0        0      767 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_where_correlated_subquery_with_join/out.sql
+-rw-r--r--   0        0        0      200 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_where_simple_comparisons/decompiled.py
+-rw-r--r--   0        0        0      101 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_where_simple_comparisons/out.sql
+-rw-r--r--   0        0        0      130 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_where_uncorrelated_subquery/out.sql
+-rw-r--r--   0        0        0     7554 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/test_compiler.py
+-rw-r--r--   0        0        0    26440 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/test_select_sql.py
+-rw-r--r--   0        0        0    16629 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/sql/test_sql.py
+-rw-r--r--   0        0        0    53832 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_aggregation.py
+-rw-r--r--   0        0        0     3980 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_api.py
+-rw-r--r--   0        0        0    39186 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_array.py
+-rw-r--r--   0        0        0     4261 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_asof_join.py
+-rw-r--r--   0        0        0      982 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_binary.py
+-rw-r--r--   0        0        0    48297 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_client.py
+-rw-r--r--   0        0        0     1126 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_column.py
+-rw-r--r--   0        0        0     3916 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_dataframe_interchange.py
+-rw-r--r--   0        0        0    10230 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_dot_sql.py
+-rw-r--r--   0        0        0     1439 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_examples.py
+-rw-r--r--   0        0        0    16675 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_export.py
+-rw-r--r--   0        0        0    57186 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_generic.py
+-rw-r--r--   0        0        0     2960 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_interactive.py
+-rw-r--r--   0        0        0    12333 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_join.py
+-rw-r--r--   0        0        0     2759 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_json.py
+-rw-r--r--   0        0        0    10926 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_map.py
+-rw-r--r--   0        0        0     1541 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_markers.py
+-rw-r--r--   0        0        0     4046 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_network.py
+-rw-r--r--   0        0        0    52300 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_numeric.py
+-rw-r--r--   0        0        0     6498 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_param.py
+-rw-r--r--   0        0        0    14141 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_register.py
+-rw-r--r--   0        0        0     8795 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_set_ops.py
+-rw-r--r--   0        0        0     5635 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_sql.py
+-rw-r--r--   0        0        0    34670 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_string.py
+-rw-r--r--   0        0        0     4840 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_struct.py
+-rw-r--r--   0        0        0    82007 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_temporal.py
+-rw-r--r--   0        0        0     4372 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_timecontext.py
+-rw-r--r--   0        0        0     5122 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_udf.py
+-rw-r--r--   0        0        0     1844 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_uuid.py
+-rw-r--r--   0        0        0    25106 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_vectorized_udf.py
+-rw-r--r--   0        0        0    40444 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/test_window.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/__init__.py
+-rw-r--r--   0        0        0     4113 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/conftest.py
+-rw-r--r--   0        0        0      545 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h01.sql
+-rw-r--r--   0        0        0      841 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h02.sql
+-rw-r--r--   0        0        0      468 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h03.sql
+-rw-r--r--   0        0        0      408 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h04.sql
+-rw-r--r--   0        0        0      522 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h05.sql
+-rw-r--r--   0        0        0      243 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h06.sql
+-rw-r--r--   0        0        0      954 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h07.sql
+-rw-r--r--   0        0        0      950 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h08.sql
+-rw-r--r--   0        0        0      678 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h09.sql
+-rw-r--r--   0        0        0      580 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h10.sql
+-rw-r--r--   0        0        0      582 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h11.sql
+-rw-r--r--   0        0        0      704 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h12.sql
+-rw-r--r--   0        0        0      366 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h13.sql
+-rw-r--r--   0        0        0      364 2024-03-30 19:28:49.984060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h14.sql
+-rw-r--r--   0        0        0      951 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h15.sql
+-rw-r--r--   0        0        0      553 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h16.sql
+-rw-r--r--   0        0        0      329 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h17.sql
+-rw-r--r--   0        0        0      555 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h18.sql
+-rw-r--r--   0        0        0     1043 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h19.sql
+-rw-r--r--   0        0        0      909 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h20.sql
+-rw-r--r--   0        0        0      803 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h21.sql
+-rw-r--r--   0        0        0      807 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h22.sql
+-rw-r--r--   0        0        0     1470 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h01/test_tpc_h01/duckdb/h01.sql
+-rw-r--r--   0        0        0     1728 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h01/test_tpc_h01/snowflake/h01.sql
+-rw-r--r--   0        0        0     1607 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h01/test_tpc_h01/trino/h01.sql
+-rw-r--r--   0        0        0     3009 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h02/test_tpc_h02/duckdb/h02.sql
+-rw-r--r--   0        0        0     5688 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h02/test_tpc_h02/snowflake/h02.sql
+-rw-r--r--   0        0        0     5022 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h02/test_tpc_h02/trino/h02.sql
+-rw-r--r--   0        0        0     2552 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h03/test_tpc_h03/duckdb/h03.sql
+-rw-r--r--   0        0        0     4324 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h03/test_tpc_h03/snowflake/h03.sql
+-rw-r--r--   0        0        0     3967 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h03/test_tpc_h03/trino/h03.sql
+-rw-r--r--   0        0        0      854 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h04/test_tpc_h04/duckdb/h04.sql
+-rw-r--r--   0        0        0     1382 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h04/test_tpc_h04/snowflake/h04.sql
+-rw-r--r--   0        0        0     1243 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h04/test_tpc_h04/trino/h04.sql
+-rw-r--r--   0        0        0     3449 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h05/test_tpc_h05/duckdb/h05.sql
+-rw-r--r--   0        0        0     6105 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h05/test_tpc_h05/snowflake/h05.sql
+-rw-r--r--   0        0        0     5531 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h05/test_tpc_h05/trino/h05.sql
+-rw-r--r--   0        0        0      733 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h06/test_tpc_h06/duckdb/h06.sql
+-rw-r--r--   0        0        0      999 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h06/test_tpc_h06/snowflake/h06.sql
+-rw-r--r--   0        0        0      962 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h06/test_tpc_h06/trino/h06.sql
+-rw-r--r--   0        0        0     1785 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h07/test_tpc_h07/duckdb/h07.sql
+-rw-r--r--   0        0        0     4153 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h07/test_tpc_h07/snowflake/h07.sql
+-rw-r--r--   0        0        0     3651 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h07/test_tpc_h07/trino/h07.sql
+-rw-r--r--   0        0        0     1611 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h08/test_tpc_h08/duckdb/h08.sql
+-rw-r--r--   0        0        0     4614 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h08/test_tpc_h08/snowflake/h08.sql
+-rw-r--r--   0        0        0     3963 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h08/test_tpc_h08/trino/h08.sql
+-rw-r--r--   0        0        0     1257 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h09/test_tpc_h09/duckdb/h09.sql
+-rw-r--r--   0        0        0     3990 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h09/test_tpc_h09/snowflake/h09.sql
+-rw-r--r--   0        0        0     3410 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h09/test_tpc_h09/trino/h09.sql
+-rw-r--r--   0        0        0     2981 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h10/test_tpc_h10/duckdb/h10.sql
+-rw-r--r--   0        0        0     5069 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h10/test_tpc_h10/snowflake/h10.sql
+-rw-r--r--   0        0        0     4641 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h10/test_tpc_h10/trino/h10.sql
+-rw-r--r--   0        0        0     2806 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h11/test_tpc_h11/duckdb/h11.sql
+-rw-r--r--   0        0        0     4797 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h11/test_tpc_h11/snowflake/h11.sql
+-rw-r--r--   0        0        0     4370 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h11/test_tpc_h11/trino/h11.sql
+-rw-r--r--   0        0        0     2413 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h12/test_tpc_h12/duckdb/h12.sql
+-rw-r--r--   0        0        0     3560 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h12/test_tpc_h12/snowflake/h12.sql
+-rw-r--r--   0        0        0     3314 2024-03-30 19:28:49.988060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h12/test_tpc_h12/trino/h12.sql
+-rw-r--r--   0        0        0     1003 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h13/test_tpc_h13/duckdb/h13.sql
+-rw-r--r--   0        0        0     1954 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h13/test_tpc_h13/snowflake/h13.sql
+-rw-r--r--   0        0        0     1705 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h13/test_tpc_h13/trino/h13.sql
+-rw-r--r--   0        0        0     1800 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h14/test_tpc_h14/duckdb/h14.sql
+-rw-r--r--   0        0        0     2906 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h14/test_tpc_h14/snowflake/h14.sql
+-rw-r--r--   0        0        0     2702 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h14/test_tpc_h14/trino/h14.sql
+-rw-r--r--   0        0        0     2656 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h15/test_tpc_h15/duckdb/h15.sql
+-rw-r--r--   0        0        0     3962 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h15/test_tpc_h15/snowflake/h15.sql
+-rw-r--r--   0        0        0     3568 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h15/test_tpc_h15/trino/h15.sql
+-rw-r--r--   0        0        0     1759 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h16/test_tpc_h16/duckdb/h16.sql
+-rw-r--r--   0        0        0     2457 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h16/test_tpc_h16/snowflake/h16.sql
+-rw-r--r--   0        0        0     2255 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h16/test_tpc_h16/trino/h16.sql
+-rw-r--r--   0        0        0     2301 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h17/test_tpc_h17/duckdb/h17.sql
+-rw-r--r--   0        0        0     3785 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h17/test_tpc_h17/snowflake/h17.sql
+-rw-r--r--   0        0        0     3466 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h17/test_tpc_h17/trino/h17.sql
+-rw-r--r--   0        0        0     2788 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h18/test_tpc_h18/duckdb/h18.sql
+-rw-r--r--   0        0        0     4477 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h18/test_tpc_h18/snowflake/h18.sql
+-rw-r--r--   0        0        0     4114 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h18/test_tpc_h18/trino/h18.sql
+-rw-r--r--   0        0        0     3630 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h19/test_tpc_h19/duckdb/h19.sql
+-rw-r--r--   0        0        0     4622 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h19/test_tpc_h19/snowflake/h19.sql
+-rw-r--r--   0        0        0     4396 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h19/test_tpc_h19/trino/h19.sql
+-rw-r--r--   0        0        0     1769 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h20/test_tpc_h20/duckdb/h20.sql
+-rw-r--r--   0        0        0     2984 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h20/test_tpc_h20/snowflake/h20.sql
+-rw-r--r--   0        0        0     2644 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h20/test_tpc_h20/trino/h20.sql
+-rw-r--r--   0        0        0     1773 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h21/test_tpc_h21/duckdb/h21.sql
+-rw-r--r--   0        0        0     3652 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h21/test_tpc_h21/snowflake/h21.sql
+-rw-r--r--   0        0        0     3229 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h21/test_tpc_h21/trino/h21.sql
+-rw-r--r--   0        0        0     1976 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h22/test_tpc_h22/duckdb/h22.sql
+-rw-r--r--   0        0        0     2252 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h22/test_tpc_h22/snowflake/h22.sql
+-rw-r--r--   0        0        0     2076 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h22/test_tpc_h22/trino/h22.sql
+-rw-r--r--   0        0        0     1445 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h01.py
+-rw-r--r--   0        0        0     1417 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h02.py
+-rw-r--r--   0        0        0      778 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h03.py
+-rw-r--r--   0        0        0      663 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h04.py
+-rw-r--r--   0        0        0     1046 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h05.py
+-rw-r--r--   0        0        0      666 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h06.py
+-rw-r--r--   0        0        0     1413 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h07.py
+-rw-r--r--   0        0        0     1516 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h08.py
+-rw-r--r--   0        0        0     1100 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h09.py
+-rw-r--r--   0        0        0     1019 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h10.py
+-rw-r--r--   0        0        0      908 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h11.py
+-rw-r--r--   0        0        0     1337 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h12.py
+-rw-r--r--   0        0        0      775 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h13.py
+-rw-r--r--   0        0        0      689 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h14.py
+-rw-r--r--   0        0        0      986 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h15.py
+-rw-r--r--   0        0        0     1098 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h16.py
+-rw-r--r--   0        0        0      850 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h17.py
+-rw-r--r--   0        0        0     1025 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h18.py
+-rw-r--r--   0        0        0     1758 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h19.py
+-rw-r--r--   0        0        0     1161 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h20.py
+-rw-r--r--   0        0        0     1451 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h21.py
+-rw-r--r--   0        0        0     1085 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h22.py
+-rw-r--r--   0        0        0    17392 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/trino/__init__.py
+-rw-r--r--   0        0        0    15984 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/trino/compiler.py
+-rw-r--r--   0        0        0      754 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/trino/converter.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/trino/tests/__init__.py
+-rw-r--r--   0        0        0     5875 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/trino/tests/conftest.py
+-rw-r--r--   0        0        0      174 2024-03-30 19:28:49.992060 turntable_spoonbill-9.0.5/ibis/backends/trino/tests/snapshots/test_client/test_builtin_scalar_udf/result.txt
+-rw-r--r--   0        0        0     4524 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/backends/trino/tests/test_client.py
+-rw-r--r--   0        0        0     2239 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/backends/trino/tests/test_datatypes.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/__init__.py
+-rw-r--r--   0        0        0    19763 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/annotations.py
+-rw-r--r--   0        0        0     7859 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/bases.py
+-rw-r--r--   0        0        0     4706 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/caching.py
+-rw-r--r--   0        0        0    10691 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/collections.py
+-rw-r--r--   0        0        0    18211 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/deferred.py
+-rw-r--r--   0        0        0     7283 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/dispatch.py
+-rw-r--r--   0        0        0    25639 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/egraph.py
+-rw-r--r--   0        0        0     4225 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/exceptions.py
+-rw-r--r--   0        0        0    22452 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/graph.py
+-rw-r--r--   0        0        0     8146 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/grounds.py
+-rw-r--r--   0        0        0     1395 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/numeric.py
+-rw-r--r--   0        0        0    49056 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/patterns.py
+-rw-r--r--   0        0        0     6684 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/temporal.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/__init__.py
+-rw-r--r--   0        0        0      161 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/conftest.py
+-rw-r--r--   0        0        0       96 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/snapshots/test_annotations/test_annotated_function_without_decoration/error.txt
+-rw-r--r--   0        0        0      114 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/snapshots/test_annotations/test_signature_from_callable_with_keyword_only_arguments/too_many_positional_arguments.txt
+-rw-r--r--   0        0        0      131 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/snapshots/test_annotations/test_signature_from_callable_with_positional_only_arguments/parameter_is_positional_only.txt
+-rw-r--r--   0        0        0      375 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/snapshots/test_grounds/test_error_message/error_message.txt
+-rw-r--r--   0        0        0      385 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/snapshots/test_grounds/test_error_message/error_message_py311.txt
+-rw-r--r--   0        0        0    13351 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_annotations.py
+-rw-r--r--   0        0        0     7544 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_bases.py
+-rw-r--r--   0        0        0    12557 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_collections.py
+-rw-r--r--   0        0        0    15334 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_deferred.py
+-rw-r--r--   0        0        0     4578 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_dispatch.py
+-rw-r--r--   0        0        0    12986 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_egraph.py
+-rw-r--r--   0        0        0    11228 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_graph.py
+-rw-r--r--   0        0        0     1405 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_graph_benchmarks.py
+-rw-r--r--   0        0        0    26781 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_grounds.py
+-rw-r--r--   0        0        0      937 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_grounds_benchmarks.py
+-rw-r--r--   0        0        0     1011 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_grounds_py310.py
+-rw-r--r--   0        0        0     2314 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_numeric.py
+-rw-r--r--   0        0        0    39898 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_patterns.py
+-rw-r--r--   0        0        0     8384 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_temporal.py
+-rw-r--r--   0        0        0     3698 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/tests/test_typing.py
+-rw-r--r--   0        0        0     6963 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/common/typing.py
+-rw-r--r--   0        0        0     6038 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/config.py
+-rw-r--r--   0        0        0     1356 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/conftest.py
+-rw-r--r--   0        0        0      758 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/examples/CITATIONS.md
+-rw-r--r--   0        0        0     4689 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/examples/__init__.py
+-rw-r--r--   0        0        0    38919 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/examples/metadata.json
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/examples/tests/__init__.py
+-rw-r--r--   0        0        0     2358 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/examples/tests/test_examples.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/expr/__init__.py
+-rw-r--r--   0        0        0      896 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/expr/analysis.py
+-rw-r--r--   0        0        0    65639 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/expr/api.py
+-rw-r--r--   0        0        0    11712 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/expr/builders.py
+-rw-r--r--   0        0        0     1327 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/expr/datashape.py
+-rw-r--r--   0        0        0      523 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/expr/datatypes/__init__.py
+-rw-r--r--   0        0        0     5036 2024-03-30 19:28:49.996060 turntable_spoonbill-9.0.5/ibis/expr/datatypes/cast.py
+-rw-r--r--   0        0        0    29349 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/datatypes/core.py
+-rw-r--r--   0        0        0     5992 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/datatypes/parse.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/datatypes/tests/__init__.py
+-rw-r--r--   0        0        0     3110 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/datatypes/tests/test_cast.py
+-rw-r--r--   0        0        0    17967 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/datatypes/tests/test_core.py
+-rw-r--r--   0        0        0     8028 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/datatypes/tests/test_parse.py
+-rw-r--r--   0        0        0    13969 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/datatypes/tests/test_value.py
+-rw-r--r--   0        0        0    11347 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/datatypes/value.py
+-rw-r--r--   0        0        0    12321 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/decompile.py
+-rw-r--r--   0        0        0    10822 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/format.py
+-rw-r--r--   0        0        0     1247 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/__init__.py
+-rw-r--r--   0        0        0     1610 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/analytic.py
+-rw-r--r--   0        0        0     4265 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/arrays.py
+-rw-r--r--   0        0        0     5188 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/core.py
+-rw-r--r--   0        0        0     6029 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/generic.py
+-rw-r--r--   0        0        0    10593 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/geospatial.py
+-rw-r--r--   0        0        0     1427 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/histograms.py
+-rw-r--r--   0        0        0      579 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/json.py
+-rw-r--r--   0        0        0     3220 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/logical.py
+-rw-r--r--   0        0        0     1523 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/maps.py
+-rw-r--r--   0        0        0     5933 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/numeric.py
+-rw-r--r--   0        0        0     7152 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/reductions.py
+-rw-r--r--   0        0        0    10131 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/relations.py
+-rw-r--r--   0        0        0     1270 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/sortkeys.py
+-rw-r--r--   0        0        0     5352 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/strings.py
+-rw-r--r--   0        0        0     1229 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/structs.py
+-rw-r--r--   0        0        0     1832 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/subqueries.py
+-rw-r--r--   0        0        0     6658 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/temporal.py
+-rw-r--r--   0        0        0     1997 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/temporal_windows.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/__init__.py
+-rw-r--r--   0        0        0      158 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/conftest.py
+-rw-r--r--   0        0        0      166 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/snapshots/test_generic/test_error_message_when_constructing_literal/call0-missing_a_required_argument/missing_a_required_argument.txt
+-rw-r--r--   0        0        0      187 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/snapshots/test_generic/test_error_message_when_constructing_literal/call1-too_many_positional_arguments/too_many_positional_arguments.txt
+-rw-r--r--   0        0        0      204 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/snapshots/test_generic/test_error_message_when_constructing_literal/call2-got_an_unexpected_keyword/got_an_unexpected_keyword.txt
+-rw-r--r--   0        0        0      215 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/snapshots/test_generic/test_error_message_when_constructing_literal/call3-multiple_values_for_argument/multiple_values_for_argument.txt
+-rw-r--r--   0        0        0      216 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/snapshots/test_generic/test_error_message_when_constructing_literal/call4-invalid_dtype/invalid_dtype.txt
+-rw-r--r--   0        0        0       46 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/snapshots/test_generic/test_error_message_when_constructing_literal/call5-unable_to_normalize/unable_to_normalize.txt
+-rw-r--r--   0        0        0     5645 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/test_core.py
+-rw-r--r--   0        0        0      789 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/test_core_py310.py
+-rw-r--r--   0        0        0     5054 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/test_generic.py
+-rw-r--r--   0        0        0     3058 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/test_rewrites.py
+-rw-r--r--   0        0        0      432 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/test_sortkeys.py
+-rw-r--r--   0        0        0      909 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/tests/test_structs.py
+-rw-r--r--   0        0        0    16316 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/udf.py
+-rw-r--r--   0        0        0     1138 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/vectorized.py
+-rw-r--r--   0        0        0     3790 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/operations/window.py
+-rw-r--r--   0        0        0     8966 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/rewrites.py
+-rw-r--r--   0        0        0     4393 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/rules.py
+-rw-r--r--   0        0        0     8490 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/schema.py
+-rw-r--r--   0        0        0    10410 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/sql.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/__init__.py
+-rw-r--r--   0        0        0    11451 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/conftest.py
+-rw-r--r--   0        0        0      254 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_aggregate_arg_names/repr.txt
+-rw-r--r--   0        0        0      116 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_argument_repr_shows_name/repr.txt
+-rw-r--r--   0        0        0      396 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_asof_join/repr.txt
+-rw-r--r--   0        0        0      206 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_complex_repr/repr.txt
+-rw-r--r--   0        0        0      394 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_destruct_selection/repr.txt
+-rw-r--r--   0        0        0       79 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_fillna/fillna_dict_repr.txt
+-rw-r--r--   0        0        0      105 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_fillna/fillna_int_repr.txt
+-rw-r--r--   0        0        0      109 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_fillna/fillna_str_repr.txt
+-rw-r--r--   0        0        0       28 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_format_dummy_table/repr.txt
+-rw-r--r--   0        0        0      153 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_format_in_memory_table/repr.txt
+-rw-r--r--   0        0        0      478 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_format_multiple_join_with_projection/repr.txt
+-rw-r--r--   0        0        0      479 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_format_new_relational_operation/repr.txt
+-rw-r--r--   0        0        0      204 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_format_projection/repr.txt
+-rw-r--r--   0        0        0      155 2024-03-30 19:28:50.000060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_format_table_column/repr.txt
+-rw-r--r--   0        0        0       32 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_format_table_with_empty_schema/repr.txt
+-rw-r--r--   0        0        0      315 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_memoize_filtered_table/repr.txt
+-rw-r--r--   0        0        0      455 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_memoize_filtered_tables_in_join/repr.txt
+-rw-r--r--   0        0        0      172 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_named_value_expr_show_name/repr.txt
+-rw-r--r--   0        0        0      161 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_named_value_expr_show_name/repr2.txt
+-rw-r--r--   0        0        0      153 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_repr_exact/repr.txt
+-rw-r--r--   0        0        0       88 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_same_column_multiple_aliases/repr.txt
+-rw-r--r--   0        0        0       26 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_schema_truncation/repr1.txt
+-rw-r--r--   0        0        0      116 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_schema_truncation/repr8.txt
+-rw-r--r--   0        0        0      235 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_schema_truncation/repr_all.txt
+-rw-r--r--   0        0        0       74 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_table_count_expr/cnt_repr.txt
+-rw-r--r--   0        0        0      242 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_table_count_expr/join_repr.txt
+-rw-r--r--   0        0        0      194 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_table_count_expr/union_repr.txt
+-rw-r--r--   0        0        0      168 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_table_type_output/repr.txt
+-rw-r--r--   0        0        0      489 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_two_inner_joins/repr.txt
+-rw-r--r--   0        0        0      134 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_window_group_by/repr.txt
+-rw-r--r--   0        0        0      164 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_format/test_window_no_group_by/repr.txt
+-rw-r--r--   0        0        0     1041 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_aggregation_with_multiple_joins/decompiled.py
+-rw-r--r--   0        0        0      341 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_aggregation/decompiled.py
+-rw-r--r--   0        0        0      726 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_aggregation_with_join/decompiled.py
+-rw-r--r--   0        0        0      885 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_join/inner/decompiled.py
+-rw-r--r--   0        0        0      884 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_join/left/decompiled.py
+-rw-r--r--   0        0        0      885 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_join/right/decompiled.py
+-rw-r--r--   0        0        0      280 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_projection/decompiled.py
+-rw-r--r--   0        0        0      423 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_in_clause/decompiled.py
+-rw-r--r--   0        0        0      884 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_join_with_filter/decompiled.py
+-rw-r--r--   0        0        0      920 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_multiple_joins/decompiled.py
+-rw-r--r--   0        0        0      531 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_scalar_subquery/decompiled.py
+-rw-r--r--   0        0        0      309 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_simple_reduction/decompiled.py
+-rw-r--r--   0        0        0      210 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_simple_select_count/decompiled.py
+-rw-r--r--   0        0        0      133 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_table_alias/decompiled.py
+-rw-r--r--   0        0        0     4616 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/test_api.py
+-rw-r--r--   0        0        0     2006 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/test_datashape.py
+-rw-r--r--   0        0        0     2288 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/test_decompile.py
+-rw-r--r--   0        0        0     1023 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/test_dereference.py
+-rw-r--r--   0        0        0    11559 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/test_format.py
+-rw-r--r--   0        0        0    47733 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/test_newrels.py
+-rw-r--r--   0        0        0     3216 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/test_reductions.py
+-rw-r--r--   0        0        0     2721 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/test_rewrites.py
+-rw-r--r--   0        0        0    13287 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/test_schema.py
+-rw-r--r--   0        0        0     4095 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/test_sql.py
+-rw-r--r--   0        0        0     4676 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/tests/test_visualize.py
+-rw-r--r--   0        0        0      931 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/types/__init__.py
+-rw-r--r--   0        0        0    50191 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/types/arrays.py
+-rw-r--r--   0        0        0      819 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/types/binary.py
+-rw-r--r--   0        0        0      271 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/types/collections.py
+-rw-r--r--   0        0        0    23300 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/types/core.py
+-rw-r--r--   0        0        0     5402 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/types/dataframe_interchange.py
+-rw-r--r--   0        0        0    76495 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/types/generic.py
+-rw-r--r--   0        0        0    66172 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/types/geospatial.py
+-rw-r--r--   0        0        0    11482 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/types/groupby.py
+-rw-r--r--   0        0        0      446 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/types/inet.py
+-rw-r--r--   0        0        0    18273 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/types/joins.py
+-rw-r--r--   0        0        0     5142 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/types/json.py
+-rw-r--r--   0        0        0    20054 2024-03-30 19:28:50.004060 turntable_spoonbill-9.0.5/ibis/expr/types/logical.py
+-rw-r--r--   0        0        0    17251 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/expr/types/maps.py
+-rw-r--r--   0        0        0    37520 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/expr/types/numeric.py
+-rw-r--r--   0        0        0    12899 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/expr/types/pretty.py
+-rw-r--r--   0        0        0   243607 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/expr/types/relations.py
+-rw-r--r--   0        0        0    57776 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/expr/types/strings.py
+-rw-r--r--   0        0        0    14388 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/expr/types/structs.py
+-rw-r--r--   0        0        0    31164 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/expr/types/temporal.py
+-rw-r--r--   0        0        0     4743 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/expr/types/temporal_windows.py
+-rw-r--r--   0        0        0      173 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/expr/types/typing.py
+-rw-r--r--   0        0        0      276 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/expr/types/uuid.py
+-rw-r--r--   0        0        0     7259 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/expr/visualize.py
+-rw-r--r--   0        0        0     6772 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/formats/__init__.py
+-rw-r--r--   0        0        0     3551 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/formats/numpy.py
+-rw-r--r--   0        0        0    13701 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/formats/pandas.py
+-rw-r--r--   0        0        0     5896 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/formats/polars.py
+-rw-r--r--   0        0        0     9661 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/formats/pyarrow.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/formats/tests/__init__.py
+-rw-r--r--   0        0        0     4370 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/formats/tests/test_numpy.py
+-rw-r--r--   0        0        0    14006 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/formats/tests/test_pandas.py
+-rw-r--r--   0        0        0     4787 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/formats/tests/test_polars.py
+-rw-r--r--   0        0        0     6829 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/formats/tests/test_pyarrow.py
+-rw-r--r--   0        0        0      235 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/interactive.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/legacy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/legacy/udf/__init__.py
+-rw-r--r--   0        0        0     2149 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/legacy/udf/validate.py
+-rw-r--r--   0        0        0    11957 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/legacy/udf/vectorized.py
+-rw-r--r--   0        0        0    24142 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/selectors.py
+-rw-r--r--   0        0        0     2236 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/streamlit/__init__.py
+-rw-r--r--   0        0        0      609 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/benchmarks/__init__.py
+-rw-r--r--   0        0        0    21311 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/benchmarks/test_benchmarks.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/__init__.py
+-rw-r--r--   0        0        0     1729 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/conftest.py
+-rw-r--r--   0        0        0     2962 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/mocks.py
+-rw-r--r--   0        0        0     1984 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/snapshots/test_format_sql_operations/test_format_sql_query_result/repr.txt
+-rw-r--r--   0        0        0      421 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/snapshots/test_format_sql_operations/test_memoize_database_table/repr.txt
+-rw-r--r--   0        0        0     1276 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/snapshots/test_format_sql_operations/test_memoize_insert_sort_key/repr.txt
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/snapshots/test_interactive/test_default_limit/out.sql
+-rw-r--r--   0        0        0       66 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/snapshots/test_interactive/test_disable_query_limit/out.sql
+-rw-r--r--   0        0        0      105 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/snapshots/test_interactive/test_respect_set_limit/out.sql
+-rw-r--r--   0        0        0     8899 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_analysis.py
+-rw-r--r--   0        0        0     2844 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_analytics.py
+-rw-r--r--   0        0        0     4470 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_case.py
+-rw-r--r--   0        0        0     4125 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_decimal.py
+-rw-r--r--   0        0        0     1643 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_format_sql_operations.py
+-rw-r--r--   0        0        0      769 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_geospatial.py
+-rw-r--r--   0        0        0     5008 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_literal.py
+-rw-r--r--   0        0        0     1599 2024-03-30 19:28:50.008060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_pipe.py
+-rw-r--r--   0        0        0     6127 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_pretty_repr.py
+-rw-r--r--   0        0        0     3250 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_relocate.py
+-rw-r--r--   0        0        0    14328 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_selectors.py
+-rw-r--r--   0        0        0     1243 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_set_operations.py
+-rw-r--r--   0        0        0     6326 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_sql_builtins.py
+-rw-r--r--   0        0        0     3549 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_string.py
+-rw-r--r--   0        0        0     2641 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_struct.py
+-rw-r--r--   0        0        0    60536 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_table.py
+-rw-r--r--   0        0        0    26786 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_temporal.py
+-rw-r--r--   0        0        0     2703 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_temporal_windows.py
+-rw-r--r--   0        0        0     5714 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_timestamp.py
+-rw-r--r--   0        0        0     4482 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_udf.py
+-rw-r--r--   0        0        0      181 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_uuid.py
+-rw-r--r--   0        0        0    49864 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_value_exprs.py
+-rw-r--r--   0        0        0    16910 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_window_frames.py
+-rw-r--r--   0        0        0     2008 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/expr/test_window_functions.py
+-rw-r--r--   0        0        0     7581 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/strategies.py
+-rw-r--r--   0        0        0     2029 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/test_api.py
+-rw-r--r--   0        0        0      401 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/test_config.py
+-rw-r--r--   0        0        0     5025 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/test_strategies.py
+-rw-r--r--   0        0        0     3741 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/test_util.py
+-rw-r--r--   0        0        0      226 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/test_version.py
+-rw-r--r--   0        0        0     1898 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/tests/util.py
+-rw-r--r--   0        0        0    17130 2024-03-30 19:28:50.012060 turntable_spoonbill-9.0.5/ibis/util.py
+-rw-r--r--   0        0        0    18419 2024-03-30 19:28:50.016060 turntable_spoonbill-9.0.5/pyproject.toml
+-rw-r--r--   0        0        0    15934 1970-01-01 00:00:00.000000 turntable_spoonbill-9.0.5/PKG-INFO
```

### Comparing `turntable_spoonbill-9.0.4/LICENSE.txt` & `turntable_spoonbill-9.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/README.md` & `turntable_spoonbill-9.0.5/README.md`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/__init__.py` & `turntable_spoonbill-9.0.5/ibis/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/client.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/datatypes.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/datatypes.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/test_connect.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/test_connect.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/system/udf/test_udf_execute.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/system/udf/test_udf_execute.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_unnest/out_two_unnests.sql` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/snapshots/test_compiler/test_unnest/out_two_unnests.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/test_compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/test_compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/test_datatypes.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/test_builtin.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/test_builtin.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/test_core.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/test_core.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/test_find.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/test_find.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/tests/unit/udf/test_usage.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/tests/unit/udf/test_usage.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/udf/core.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/udf/core.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/udf/find.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/udf/find.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/bigquery/udf/rewrite.py` & `turntable_spoonbill-9.0.5/ibis/backends/bigquery/udf/rewrite.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/clickhouse/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/clickhouse/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/clickhouse/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/snapshots/test_select/test_table_column_unbox/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/snapshots/test_select/test_table_column_unbox/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_aggregations.py` & `turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_datatypes.py` & `turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_functions.py` & `turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_literals.py` & `turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_literals.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_operators.py` & `turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/clickhouse/tests/test_select.py` & `turntable_spoonbill-9.0.5/ibis/backends/clickhouse/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/convert.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/convert.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/executor.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/executor.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/helpers.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/helpers.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/kernels.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/kernels.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_arrays.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_cast.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_cast.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_core.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_functions.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_join.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_maps.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_operations.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_strings.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_structs.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_temporal.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_temporal.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/dask/tests/test_window.py` & `turntable_spoonbill-9.0.5/ibis/backends/dask/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/datafusion/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/datafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/datafusion/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/datafusion/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/test_connect.py` & `turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/test_register.py` & `turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/test_select.py` & `turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/test_temporal.py` & `turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/test_temporal.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/datafusion/tests/test_udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/datafusion/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/datafusion/udfs.py` & `turntable_spoonbill-9.0.5/ibis/backends/datafusion/udfs.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/druid/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/druid/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/druid/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/druid/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/druid/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/druid/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/duckdb/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/duckdb/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/duckdb/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/test_datatypes.py` & `turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/test_geospatial.py` & `turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/test_geospatial.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/test_register.py` & `turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/duckdb/tests/test_udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/duckdb/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/exasol/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/exasol/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/exasol/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/exasol/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/exasol/converter.py` & `turntable_spoonbill-9.0.5/ibis/backends/exasol/converter.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/exasol/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/exasol/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/flink/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/flink/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/flink/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/flink/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/flink/datatypes.py` & `turntable_spoonbill-9.0.5/ibis/backends/flink/datatypes.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/flink/ddl.py` & `turntable_spoonbill-9.0.5/ibis/backends/flink/ddl.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/flink/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/flink/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/flink/tests/snapshots/test_compiler/test_window_topn/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/flink/tests/snapshots/test_compiler/test_window_topn/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/flink/tests/test_compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/flink/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/flink/tests/test_datatypes.py` & `turntable_spoonbill-9.0.5/ibis/backends/flink/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/flink/tests/test_ddl.py` & `turntable_spoonbill-9.0.5/ibis/backends/flink/tests/test_ddl.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/flink/tests/test_join.py` & `turntable_spoonbill-9.0.5/ibis/backends/flink/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/flink/tests/test_udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/flink/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/flink/tests/test_window.py` & `turntable_spoonbill-9.0.5/ibis/backends/flink/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/flink/utils.py` & `turntable_spoonbill-9.0.5/ibis/backends/flink/utils.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/client.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/ddl.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/ddl.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/metadata.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/metadata.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_assign_labels/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_bucket_histogram/test_bucket_assign_labels/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_join_aliasing/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_join_aliasing/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_join_key_name/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_join_key_name/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_join_key_name2/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_join_key_name2/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_nested_join_multiple_ctes/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_nested_join_multiple_ctes/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_sql/test_nested_joins_single_cte/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_sql/test_nested_joins_single_cte/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/capitalize/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_string_builtins/test_string_builtins/capitalize/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/snapshots/test_window/test_add_default_order_by/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/snapshots/test_window/test_add_default_order_by/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_analytic_functions.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_analytic_functions.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_bucket_histogram.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_bucket_histogram.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_case_exprs.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_case_exprs.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_coalesce_greater_least.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_coalesce_greater_least.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_ddl.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_ddl.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_ddl_compilation.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_ddl_compilation.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_exprs.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_exprs.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_in_not_in.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_in_not_in.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_metadata.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_parquet_ddl.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_parquet_ddl.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_partition.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_patched.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_patched.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_sql.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_string_builtins.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_string_builtins.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_unary_builtins.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_unary_builtins.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_value_exprs.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_value_exprs.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/tests/test_window.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/impala/udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/impala/udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/mssql/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/mssql/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/mssql/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/mssql/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/mssql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/mssql/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/mssql/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/mysql/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/mysql/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/mysql/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/mysql/converter.py` & `turntable_spoonbill-9.0.5/ibis/backends/mysql/converter.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/mysql/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/mysql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/mysql/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/mysql/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/oracle/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/oracle/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/oracle/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/oracle/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/oracle/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/oracle/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/oracle/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/oracle/tests/test_datatypes.py` & `turntable_spoonbill-9.0.5/ibis/backends/oracle/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/convert.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/convert.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/executor.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/executor.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/helpers.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/helpers.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/kernels.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/kernels.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/rewrites.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/rewrites.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_arrays.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_cast.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_cast.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_core.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_functions.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_helpers.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_join.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_maps.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_operations.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_strings.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_structs.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_temporal.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_temporal.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/tests/test_window.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pandas/udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/pandas/udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/polars/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/polars/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/polars/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/polars/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/polars/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/polars/tests/test_join.py` & `turntable_spoonbill-9.0.5/ibis/backends/polars/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/polars/tests/test_udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/polars/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/postgres/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/postgres/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/postgres/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/postgres/converter.py` & `turntable_spoonbill-9.0.5/ibis/backends/postgres/converter.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/snapshots/test_functions/test_analytic_functions/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/snapshots/test_functions/test_analytic_functions/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/test_functions.py` & `turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/test_geospatial.py` & `turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/test_geospatial.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/test_postgis.py` & `turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/test_postgis.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/postgres/tests/test_udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/postgres/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pyspark/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pyspark/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/pyspark/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pyspark/converter.py` & `turntable_spoonbill-9.0.5/ibis/backends/pyspark/converter.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pyspark/datatypes.py` & `turntable_spoonbill-9.0.5/ibis/backends/pyspark/datatypes.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/test_aggregation.py` & `turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/test_array.py` & `turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/test_basic.py` & `turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/test_ddl.py` & `turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/test_ddl.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/test_null.py` & `turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/test_null.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/pyspark/tests/test_window.py` & `turntable_spoonbill-9.0.5/ibis/backends/pyspark/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/risingwave/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/risingwave/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/risingwave/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/risingwave/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/risingwave/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/risingwave/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/risingwave/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/risingwave/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/risingwave/tests/test_functions.py` & `turntable_spoonbill-9.0.5/ibis/backends/risingwave/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/snowflake/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/snowflake/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/snowflake/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/snowflake/converter.py` & `turntable_spoonbill-9.0.5/ibis/backends/snowflake/converter.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/snowflake/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/snowflake/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/snowflake/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/snowflake/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/snowflake/tests/test_datatypes.py` & `turntable_spoonbill-9.0.5/ibis/backends/snowflake/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/snowflake/tests/test_udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/snowflake/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sql/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sql/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/sql/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sql/datatypes.py` & `turntable_spoonbill-9.0.5/ibis/backends/sql/datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 _from_sqlglot_types = {
     typecode.BIGDECIMAL: partial(dt.Decimal, 76, 38),
     typecode.BIGINT: dt.Int64,
     typecode.BINARY: dt.Binary,
     typecode.BOOLEAN: dt.Boolean,
     typecode.CHAR: dt.String,
     typecode.DATE: dt.Date,
+    typecode.DATETIME: dt.Timestamp,
+    typecode.DATETIME64: dt.Timestamp,
     typecode.DOUBLE: dt.Float64,
     typecode.ENUM: dt.String,
     typecode.ENUM8: dt.String,
     typecode.ENUM16: dt.String,
     typecode.FLOAT: dt.Float32,
     typecode.FIXEDSTRING: dt.String,
     typecode.GEOMETRY: partial(dt.GeoSpatial, geotype="geometry"),
```

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sql/ddl.py` & `turntable_spoonbill-9.0.5/ibis/backends/sql/ddl.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sql/dialects.py` & `turntable_spoonbill-9.0.5/ibis/backends/sql/dialects.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sql/rewrites.py` & `turntable_spoonbill-9.0.5/ibis/backends/sql/rewrites.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sql/tests/test_compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/sql/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sql/tests/test_datatypes.py` & `turntable_spoonbill-9.0.5/ibis/backends/sql/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sqlite/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sqlite/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/sqlite/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sqlite/converter.py` & `turntable_spoonbill-9.0.5/ibis/backends/sqlite/converter.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sqlite/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/sqlite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sqlite/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/sqlite/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sqlite/tests/test_types.py` & `turntable_spoonbill-9.0.5/ibis/backends/sqlite/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/sqlite/udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/sqlite/udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/base.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/base.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/data.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/data.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/errors.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/errors.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/bigquery/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/bigquery/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/clickhouse/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/clickhouse/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/datafusion/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/datafusion/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/druid/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/druid/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/duckdb/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/duckdb/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/exasol/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/exasol/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/flink/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/flink/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/impala/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/impala/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/mssql/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/mssql/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/mysql/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/mysql/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/oracle/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/oracle/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/postgres/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/postgres/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/pyspark/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/pyspark/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/risingwave/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/risingwave/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/snowflake/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/snowflake/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/sqlite/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/sqlite/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/trino/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_generic/test_many_subqueries/trino/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/clickhouse/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/clickhouse/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/datafusion/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/datafusion/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/flink/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/flink/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/mssql/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/mssql/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/oracle/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_group_by_has_index/oracle/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/bigquery/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/bigquery/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/clickhouse/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/clickhouse/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/duckdb/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/duckdb/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/postgres/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/postgres/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/pyspark/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/pyspark/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/risingwave/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/risingwave/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/trino/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/snapshots/test_sql/test_union_aliasing/trino/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_column_distinct/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_column_distinct/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_count_distinct/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_count_distinct/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_difference_project_column/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_difference_project_column/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_intersect_project_column/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_intersect_project_column/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_multiple_count_distinct/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_multiple_count_distinct/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_table_difference/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_table_difference/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_table_distinct/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_table_distinct/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_table_intersect/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_table_intersect/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_union/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_union/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_compiler/test_union_project_column/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_compiler/test_union_project_column/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_count_joined/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_aggregate_count_joined/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_bug_duplicated_where/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_bug_duplicated_where/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_bug_project_multiple_times/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_bug_project_multiple_times/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_case_in_projection/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_case_in_projection/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_chain_limit_doesnt_collapse/result.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_chain_limit_doesnt_collapse/result.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_filter_self_join_analysis_bug/result.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_filter_self_join_analysis_bug/result.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_between_joins/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_between_joins/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_filtered_tables_no_pushdown/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_filtered_tables_no_pushdown/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_just_materialized/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_just_materialized/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_with_conditional_aggregate/result.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_join_with_conditional_aggregate/result.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_limit_with_self_join/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_limit_with_self_join/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_limit_with_self_join/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_limit_with_self_join/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_multiple_joins/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_multiple_joins/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_multiple_limits/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_multiple_limits/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_order_by_on_limit_yield_subquery/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_order_by_on_limit_yield_subquery/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_factor_correlated_subquery/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_factor_correlated_subquery/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_in_union/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_in_union/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_used_for_self_join/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_subquery_used_for_self_join/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_analysis_bug/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_analysis_bug/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_predicate_pushdown_bug/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_topk_predicate_pushdown_bug/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_tpch_self_join_failure/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_tpch_self_join_failure/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_analyze_scalar_op/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_analyze_scalar_op/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_analyze_scalar_op/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_select_sql/test_where_analyze_scalar_op/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_gh_1045/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_gh_1045/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_lower_projection_sort_key/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_lower_projection_sort_key/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_no_cart_join/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_no_cart_join/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_no_cartesian_join/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_no_cartesian_join/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sql/test_where_correlated_subquery_with_join/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sql/test_where_correlated_subquery_with_join/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_gh_1045/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_gh_1045/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_no_cart_join/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_no_cart_join/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_tpc_h11/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_tpc_h11/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_where_correlated_subquery_with_join/out.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/snapshots/test_sqlalchemy/test_where_correlated_subquery_with_join/out.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/test_compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/test_compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/test_select_sql.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/test_select_sql.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/sql/test_sql.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/sql/test_sql.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_aggregation.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_api.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_array.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_asof_join.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_asof_join.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_binary.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_column.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_column.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_dataframe_interchange.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_dataframe_interchange.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_dot_sql.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_dot_sql.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_examples.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_export.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_generic.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_interactive.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_join.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_json.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_map.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_markers.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_markers.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_network.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_numeric.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_numeric.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_param.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_param.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_register.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_set_ops.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_set_ops.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_sql.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_string.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_struct.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_temporal.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_temporal.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_timecontext.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_timecontext.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_uuid.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_uuid.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_vectorized_udf.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_vectorized_udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/test_window.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h01.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h01.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h02.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h02.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h05.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h05.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h07.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h07.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h08.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h08.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h09.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h09.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h10.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h10.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h11.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h11.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h12.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h12.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h15.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h15.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h16.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h16.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h18.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h18.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h19.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h19.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h20.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h20.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h21.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h21.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/queries/duckdb/h22.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/queries/duckdb/h22.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h01/test_tpc_h01/duckdb/h01.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h01/test_tpc_h01/duckdb/h01.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h01/test_tpc_h01/snowflake/h01.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h01/test_tpc_h01/snowflake/h01.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h01/test_tpc_h01/trino/h01.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h01/test_tpc_h01/trino/h01.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h02/test_tpc_h02/duckdb/h02.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h02/test_tpc_h02/duckdb/h02.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h02/test_tpc_h02/snowflake/h02.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h02/test_tpc_h02/snowflake/h02.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h02/test_tpc_h02/trino/h02.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h02/test_tpc_h02/trino/h02.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h03/test_tpc_h03/duckdb/h03.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h03/test_tpc_h03/duckdb/h03.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h03/test_tpc_h03/snowflake/h03.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h03/test_tpc_h03/snowflake/h03.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h03/test_tpc_h03/trino/h03.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h03/test_tpc_h03/trino/h03.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h04/test_tpc_h04/duckdb/h04.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h04/test_tpc_h04/duckdb/h04.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h04/test_tpc_h04/snowflake/h04.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h04/test_tpc_h04/snowflake/h04.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h04/test_tpc_h04/trino/h04.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h04/test_tpc_h04/trino/h04.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h05/test_tpc_h05/duckdb/h05.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h05/test_tpc_h05/duckdb/h05.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h05/test_tpc_h05/snowflake/h05.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h05/test_tpc_h05/snowflake/h05.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h05/test_tpc_h05/trino/h05.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h05/test_tpc_h05/trino/h05.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h06/test_tpc_h06/duckdb/h06.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h06/test_tpc_h06/duckdb/h06.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h06/test_tpc_h06/snowflake/h06.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h06/test_tpc_h06/snowflake/h06.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h06/test_tpc_h06/trino/h06.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h06/test_tpc_h06/trino/h06.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h07/test_tpc_h07/duckdb/h07.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h07/test_tpc_h07/duckdb/h07.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h07/test_tpc_h07/snowflake/h07.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h07/test_tpc_h07/snowflake/h07.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h07/test_tpc_h07/trino/h07.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h07/test_tpc_h07/trino/h07.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h08/test_tpc_h08/duckdb/h08.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h08/test_tpc_h08/duckdb/h08.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h08/test_tpc_h08/snowflake/h08.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h08/test_tpc_h08/snowflake/h08.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h08/test_tpc_h08/trino/h08.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h08/test_tpc_h08/trino/h08.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h09/test_tpc_h09/duckdb/h09.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h09/test_tpc_h09/duckdb/h09.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h09/test_tpc_h09/snowflake/h09.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h09/test_tpc_h09/snowflake/h09.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h09/test_tpc_h09/trino/h09.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h09/test_tpc_h09/trino/h09.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h10/test_tpc_h10/duckdb/h10.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h10/test_tpc_h10/duckdb/h10.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h10/test_tpc_h10/snowflake/h10.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h10/test_tpc_h10/snowflake/h10.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h10/test_tpc_h10/trino/h10.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h10/test_tpc_h10/trino/h10.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h11/test_tpc_h11/duckdb/h11.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h11/test_tpc_h11/duckdb/h11.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h11/test_tpc_h11/snowflake/h11.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h11/test_tpc_h11/snowflake/h11.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h11/test_tpc_h11/trino/h11.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h11/test_tpc_h11/trino/h11.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h12/test_tpc_h12/duckdb/h12.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h12/test_tpc_h12/duckdb/h12.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h12/test_tpc_h12/snowflake/h12.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h12/test_tpc_h12/snowflake/h12.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h12/test_tpc_h12/trino/h12.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h12/test_tpc_h12/trino/h12.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h13/test_tpc_h13/duckdb/h13.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h13/test_tpc_h13/duckdb/h13.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h13/test_tpc_h13/snowflake/h13.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h13/test_tpc_h13/snowflake/h13.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h13/test_tpc_h13/trino/h13.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h13/test_tpc_h13/trino/h13.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h14/test_tpc_h14/duckdb/h14.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h14/test_tpc_h14/duckdb/h14.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h14/test_tpc_h14/snowflake/h14.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h14/test_tpc_h14/snowflake/h14.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h14/test_tpc_h14/trino/h14.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h14/test_tpc_h14/trino/h14.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h15/test_tpc_h15/duckdb/h15.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h15/test_tpc_h15/duckdb/h15.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h15/test_tpc_h15/snowflake/h15.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h15/test_tpc_h15/snowflake/h15.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h15/test_tpc_h15/trino/h15.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h15/test_tpc_h15/trino/h15.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h16/test_tpc_h16/duckdb/h16.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h16/test_tpc_h16/duckdb/h16.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h16/test_tpc_h16/snowflake/h16.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h16/test_tpc_h16/snowflake/h16.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h16/test_tpc_h16/trino/h16.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h16/test_tpc_h16/trino/h16.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h17/test_tpc_h17/duckdb/h17.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h17/test_tpc_h17/duckdb/h17.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h17/test_tpc_h17/snowflake/h17.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h17/test_tpc_h17/snowflake/h17.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h17/test_tpc_h17/trino/h17.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h17/test_tpc_h17/trino/h17.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h18/test_tpc_h18/duckdb/h18.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h18/test_tpc_h18/duckdb/h18.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h18/test_tpc_h18/snowflake/h18.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h18/test_tpc_h18/snowflake/h18.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h18/test_tpc_h18/trino/h18.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h18/test_tpc_h18/trino/h18.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h19/test_tpc_h19/duckdb/h19.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h19/test_tpc_h19/duckdb/h19.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h19/test_tpc_h19/snowflake/h19.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h19/test_tpc_h19/snowflake/h19.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h19/test_tpc_h19/trino/h19.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h19/test_tpc_h19/trino/h19.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h20/test_tpc_h20/duckdb/h20.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h20/test_tpc_h20/duckdb/h20.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h20/test_tpc_h20/snowflake/h20.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h20/test_tpc_h20/snowflake/h20.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h20/test_tpc_h20/trino/h20.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h20/test_tpc_h20/trino/h20.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h21/test_tpc_h21/duckdb/h21.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h21/test_tpc_h21/duckdb/h21.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h21/test_tpc_h21/snowflake/h21.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h21/test_tpc_h21/snowflake/h21.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h21/test_tpc_h21/trino/h21.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h21/test_tpc_h21/trino/h21.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h22/test_tpc_h22/duckdb/h22.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h22/test_tpc_h22/duckdb/h22.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h22/test_tpc_h22/snowflake/h22.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h22/test_tpc_h22/snowflake/h22.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/snapshots/test_h22/test_tpc_h22/trino/h22.sql` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/snapshots/test_h22/test_tpc_h22/trino/h22.sql`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h01.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h01.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h02.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h02.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h03.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h03.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h04.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h04.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h05.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h05.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h06.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h06.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h07.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h07.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h08.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h08.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h09.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h09.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h10.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h10.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h11.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h11.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h12.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h12.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h13.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h13.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h14.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h14.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h15.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h15.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h16.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h16.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h17.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h17.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h18.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h18.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h19.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h19.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h20.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h20.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h21.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h21.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/tests/tpch/test_h22.py` & `turntable_spoonbill-9.0.5/ibis/backends/tests/tpch/test_h22.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/trino/__init__.py` & `turntable_spoonbill-9.0.5/ibis/backends/trino/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/trino/compiler.py` & `turntable_spoonbill-9.0.5/ibis/backends/trino/compiler.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/trino/converter.py` & `turntable_spoonbill-9.0.5/ibis/backends/trino/converter.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/trino/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/backends/trino/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/trino/tests/test_client.py` & `turntable_spoonbill-9.0.5/ibis/backends/trino/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/backends/trino/tests/test_datatypes.py` & `turntable_spoonbill-9.0.5/ibis/backends/trino/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/annotations.py` & `turntable_spoonbill-9.0.5/ibis/common/annotations.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/bases.py` & `turntable_spoonbill-9.0.5/ibis/common/bases.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/caching.py` & `turntable_spoonbill-9.0.5/ibis/common/caching.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/collections.py` & `turntable_spoonbill-9.0.5/ibis/common/collections.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/deferred.py` & `turntable_spoonbill-9.0.5/ibis/common/deferred.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/dispatch.py` & `turntable_spoonbill-9.0.5/ibis/common/dispatch.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/egraph.py` & `turntable_spoonbill-9.0.5/ibis/common/egraph.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/exceptions.py` & `turntable_spoonbill-9.0.5/ibis/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/graph.py` & `turntable_spoonbill-9.0.5/ibis/common/graph.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/grounds.py` & `turntable_spoonbill-9.0.5/ibis/common/grounds.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/numeric.py` & `turntable_spoonbill-9.0.5/ibis/common/numeric.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/patterns.py` & `turntable_spoonbill-9.0.5/ibis/common/patterns.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/temporal.py` & `turntable_spoonbill-9.0.5/ibis/common/temporal.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_annotations.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_bases.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_bases.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_collections.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_deferred.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_deferred.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_dispatch.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_egraph.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_egraph.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_graph.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_graph_benchmarks.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_graph_benchmarks.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_grounds.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_grounds.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_grounds_benchmarks.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_grounds_benchmarks.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_grounds_py310.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_grounds_py310.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_numeric.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_numeric.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_patterns.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_temporal.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_temporal.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/tests/test_typing.py` & `turntable_spoonbill-9.0.5/ibis/common/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/common/typing.py` & `turntable_spoonbill-9.0.5/ibis/common/typing.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/config.py` & `turntable_spoonbill-9.0.5/ibis/config.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/conftest.py` & `turntable_spoonbill-9.0.5/ibis/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/examples/CITATIONS.md` & `turntable_spoonbill-9.0.5/ibis/examples/CITATIONS.md`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/examples/__init__.py` & `turntable_spoonbill-9.0.5/ibis/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/examples/metadata.json` & `turntable_spoonbill-9.0.5/ibis/examples/metadata.json`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/examples/tests/test_examples.py` & `turntable_spoonbill-9.0.5/ibis/examples/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/analysis.py` & `turntable_spoonbill-9.0.5/ibis/expr/analysis.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/api.py` & `turntable_spoonbill-9.0.5/ibis/expr/api.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/builders.py` & `turntable_spoonbill-9.0.5/ibis/expr/builders.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/datashape.py` & `turntable_spoonbill-9.0.5/ibis/expr/datashape.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/datatypes/__init__.py` & `turntable_spoonbill-9.0.5/ibis/expr/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/datatypes/cast.py` & `turntable_spoonbill-9.0.5/ibis/expr/datatypes/cast.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/datatypes/core.py` & `turntable_spoonbill-9.0.5/ibis/expr/datatypes/core.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/datatypes/parse.py` & `turntable_spoonbill-9.0.5/ibis/expr/datatypes/parse.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/datatypes/tests/test_cast.py` & `turntable_spoonbill-9.0.5/ibis/expr/datatypes/tests/test_cast.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/datatypes/tests/test_core.py` & `turntable_spoonbill-9.0.5/ibis/expr/datatypes/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/datatypes/tests/test_parse.py` & `turntable_spoonbill-9.0.5/ibis/expr/datatypes/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/datatypes/tests/test_value.py` & `turntable_spoonbill-9.0.5/ibis/expr/datatypes/tests/test_value.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/datatypes/value.py` & `turntable_spoonbill-9.0.5/ibis/expr/datatypes/value.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/decompile.py` & `turntable_spoonbill-9.0.5/ibis/expr/decompile.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/format.py` & `turntable_spoonbill-9.0.5/ibis/expr/format.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/__init__.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/analytic.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/analytic.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/arrays.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/arrays.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/core.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/core.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/generic.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/generic.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/geospatial.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/geospatial.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/histograms.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/histograms.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/json.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/json.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/logical.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/logical.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/maps.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/maps.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/numeric.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/numeric.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/reductions.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/reductions.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/relations.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/relations.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,16 +80,15 @@
 
     shape = ds.columnar
 
     def __init__(self, rel, name):
         if name not in rel.schema:
             columns_formatted = ", ".join(map(repr, rel.schema.names))
             raise IbisTypeError(
-                f"Column {name!r} is not found in table. "
-                f"Existing columns: {columns_formatted}."
+                f"Column {name!r} is not found in table. \nExisting columns: {columns_formatted}."
             )
         super().__init__(rel=rel, name=name)
 
     @attribute
     def dtype(self):
         return self.rel.schema[self.name]
```

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/sortkeys.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/sortkeys.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/strings.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/strings.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/structs.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/structs.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/subqueries.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/subqueries.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/temporal.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/temporal.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/temporal_windows.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/temporal_windows.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/tests/test_core.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/tests/test_core_py310.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/tests/test_core_py310.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/tests/test_generic.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/tests/test_rewrites.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/tests/test_rewrites.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/tests/test_structs.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/udf.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/vectorized.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/vectorized.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/operations/window.py` & `turntable_spoonbill-9.0.5/ibis/expr/operations/window.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/rewrites.py` & `turntable_spoonbill-9.0.5/ibis/expr/rewrites.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/rules.py` & `turntable_spoonbill-9.0.5/ibis/expr/rules.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/schema.py` & `turntable_spoonbill-9.0.5/ibis/expr/schema.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/sql.py` & `turntable_spoonbill-9.0.5/ibis/expr/sql.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/conftest.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_aggregation_with_multiple_joins/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_aggregation_with_multiple_joins/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_aggregation_with_join/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_aggregation_with_join/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_join/inner/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_join/inner/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_join/left/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_join/left/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_join/right/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_basic_join/right/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_join_with_filter/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_join_with_filter/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_multiple_joins/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_multiple_joins/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/snapshots/test_sql/test_parse_sql_scalar_subquery/decompiled.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/snapshots/test_sql/test_parse_sql_scalar_subquery/decompiled.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/test_api.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/test_datashape.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/test_datashape.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/test_decompile.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/test_decompile.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/test_dereference.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/test_dereference.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/test_format.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/test_newrels.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/test_newrels.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/test_reductions.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/test_reductions.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/test_rewrites.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/test_rewrites.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/test_schema.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/test_sql.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/tests/test_visualize.py` & `turntable_spoonbill-9.0.5/ibis/expr/tests/test_visualize.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/__init__.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/arrays.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/arrays.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/binary.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/binary.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/core.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/core.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/dataframe_interchange.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/dataframe_interchange.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/generic.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/generic.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/geospatial.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/geospatial.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/groupby.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/groupby.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/joins.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/joins.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/json.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/json.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/logical.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/logical.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/maps.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/maps.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/numeric.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/numeric.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/pretty.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/pretty.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/relations.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/relations.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/strings.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/strings.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/structs.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/structs.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/temporal.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/temporal.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/types/temporal_windows.py` & `turntable_spoonbill-9.0.5/ibis/expr/types/temporal_windows.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/expr/visualize.py` & `turntable_spoonbill-9.0.5/ibis/expr/visualize.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/formats/__init__.py` & `turntable_spoonbill-9.0.5/ibis/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/formats/numpy.py` & `turntable_spoonbill-9.0.5/ibis/formats/numpy.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/formats/pandas.py` & `turntable_spoonbill-9.0.5/ibis/formats/pandas.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/formats/polars.py` & `turntable_spoonbill-9.0.5/ibis/formats/polars.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/formats/pyarrow.py` & `turntable_spoonbill-9.0.5/ibis/formats/pyarrow.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/formats/tests/test_numpy.py` & `turntable_spoonbill-9.0.5/ibis/formats/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/formats/tests/test_pandas.py` & `turntable_spoonbill-9.0.5/ibis/formats/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/formats/tests/test_polars.py` & `turntable_spoonbill-9.0.5/ibis/formats/tests/test_polars.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/formats/tests/test_pyarrow.py` & `turntable_spoonbill-9.0.5/ibis/formats/tests/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/legacy/udf/validate.py` & `turntable_spoonbill-9.0.5/ibis/legacy/udf/validate.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/legacy/udf/vectorized.py` & `turntable_spoonbill-9.0.5/ibis/legacy/udf/vectorized.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/selectors.py` & `turntable_spoonbill-9.0.5/ibis/selectors.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/streamlit/__init__.py` & `turntable_spoonbill-9.0.5/ibis/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/__init__.py` & `turntable_spoonbill-9.0.5/ibis/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/benchmarks/test_benchmarks.py` & `turntable_spoonbill-9.0.5/ibis/tests/benchmarks/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/conftest.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/conftest.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/mocks.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/mocks.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/snapshots/test_format_sql_operations/test_format_sql_query_result/repr.txt` & `turntable_spoonbill-9.0.5/ibis/tests/expr/snapshots/test_format_sql_operations/test_format_sql_query_result/repr.txt`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/snapshots/test_format_sql_operations/test_memoize_insert_sort_key/repr.txt` & `turntable_spoonbill-9.0.5/ibis/tests/expr/snapshots/test_format_sql_operations/test_memoize_insert_sort_key/repr.txt`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_analysis.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_analysis.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_analytics.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_analytics.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_case.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_case.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_decimal.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_decimal.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_format_sql_operations.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_format_sql_operations.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_geospatial.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_geospatial.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_literal.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_literal.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_pipe.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_pipe.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_pretty_repr.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_pretty_repr.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_relocate.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_relocate.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_selectors.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_selectors.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_set_operations.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_set_operations.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_sql_builtins.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_sql_builtins.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_string.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_string.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_struct.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_struct.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_table.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_table.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_temporal.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_temporal.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_temporal_windows.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_temporal_windows.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_timestamp.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_udf.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_udf.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_value_exprs.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_value_exprs.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_window_frames.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_window_frames.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/expr/test_window_functions.py` & `turntable_spoonbill-9.0.5/ibis/tests/expr/test_window_functions.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/strategies.py` & `turntable_spoonbill-9.0.5/ibis/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/test_api.py` & `turntable_spoonbill-9.0.5/ibis/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/test_strategies.py` & `turntable_spoonbill-9.0.5/ibis/tests/test_strategies.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/test_util.py` & `turntable_spoonbill-9.0.5/ibis/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/tests/util.py` & `turntable_spoonbill-9.0.5/ibis/tests/util.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/ibis/util.py` & `turntable_spoonbill-9.0.5/ibis/util.py`

 * *Files identical despite different names*

### Comparing `turntable_spoonbill-9.0.4/pyproject.toml` & `turntable_spoonbill-9.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turntable-spoonbill"
-version = "9.0.4"
+version = "9.0.5"
 packages = [{ include = "ibis" }]
 include = ["ibis/examples/metadata.json", "ibis/examples/CITATIONS.md"]
 exclude = [
   "ibis/examples/gen_examples.R",
   "ibis/examples/gen_registry.py",
   "ibis/examples/data",
   "ibis/examples/descriptions",
```

### Comparing `turntable_spoonbill-9.0.4/PKG-INFO` & `turntable_spoonbill-9.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turntable-spoonbill
-Version: 9.0.4
+Version: 9.0.5
 Summary: Productivity-centric Python Big Data Framework
 Home-page: https://ibis-project.org
 License: Apache-2.0
 Author: Turntable Team
 Author-email: team@turntable.so
 Maintainer: Ibis Maintainers
 Maintainer-email: maintainers@ibis-project.org
```

