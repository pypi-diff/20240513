# Comparing `tmp/odin-2.8.1.tar.gz` & `tmp/odin-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odin-2.8.1.tar", max compression
+gzip compressed data, was "odin-2.9.0.tar", max compression
```

## Comparing `odin-2.8.1.tar` & `odin-2.9.0.tar`

### file list

```diff
@@ -1,122 +1,122 @@
--rw-r--r--   0        0        0     1539 2023-06-15 23:41:28.830387 odin-2.8.1/LICENSE
--rw-r--r--   0        0        0     7879 2023-06-15 23:41:28.830387 odin-2.8.1/README.rst
--rw-r--r--   0        0        0     2491 2023-06-15 23:41:28.834387 odin-2.8.1/pyproject.toml
--rw-r--r--   0        0        0      718 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/__init__.py
--rw-r--r--   0        0        0     5356 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/adapters.py
--rw-r--r--   0        0        0     7306 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/annotated_resource/__init__.py
--rw-r--r--   0        0        0      518 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/annotated_resource/special_fields.py
--rw-r--r--   0        0        0      791 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/annotated_resource/type_aliases.py
--rw-r--r--   0        0        0     8701 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/annotated_resource/type_resolution.py
--rw-r--r--   0        0        0      376 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/bases.py
--rw-r--r--   0        0        0        0 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/__init__.py
--rw-r--r--   0        0        0    10541 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/csv_codec.py
--rw-r--r--   0        0        0     2480 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/dict_codec.py
--rw-r--r--   0        0        0     4547 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/json_codec.py
--rw-r--r--   0        0        0     4264 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/msgpack_codec.py
--rw-r--r--   0        0        0     5899 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/toml_codec.py
--rw-r--r--   0        0        0     3115 2023-06-15 23:41:28.834387 odin-2.8.1/src/odin/codecs/xml_codec.py
--rw-r--r--   0        0        0     3970 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/codecs/yaml_codec.py
--rw-r--r--   0        0        0     1249 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/compatibility.py
--rw-r--r--   0        0        0        0 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/__init__.py
--rw-r--r--   0        0        0      503 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/arrow/__init__.py
--rw-r--r--   0        0        0     1791 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/arrow/fields.py
--rw-r--r--   0        0        0      146 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/geo/__init__.py
--rw-r--r--   0        0        0     3765 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/geo/datatypes.py
--rw-r--r--   0        0        0     2370 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/geo/fields.py
--rw-r--r--   0        0        0     6371 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/json_schema/__init__.py
--rw-r--r--   0        0        0      115 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/money/__init__.py
--rw-r--r--   0        0        0    18131 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/money/datatypes.py
--rw-r--r--   0        0        0     1585 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/money/fields.py
--rw-r--r--   0        0        0      222 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/pint/__init__.py
--rw-r--r--   0        0        0     2182 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/pint/fields.py
--rw-r--r--   0        0        0      245 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/pint/units.py
--rw-r--r--   0        0        0       80 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/rich/__init__.py
--rw-r--r--   0        0        0      631 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/rich/theme.py
--rw-r--r--   0        0        0     1662 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/rich/validation_tree.py
--rw-r--r--   0        0        0     6787 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/sphinx/__init__.py
--rw-r--r--   0        0        0     1309 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/contrib/swagger/__init__.py
--rw-r--r--   0        0        0     1183 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/datastructures.py
--rw-r--r--   0        0        0    10233 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/datetimeutil.py
--rw-r--r--   0        0        0     1624 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/decorators.py
--rw-r--r--   0        0        0     4800 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/exceptions.py
--rw-r--r--   0        0        0    33799 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/fields/__init__.py
--rw-r--r--   0        0        0     2078 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/fields/base.py
--rw-r--r--   0        0        0     8102 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/fields/composite.py
--rw-r--r--   0        0        0     4479 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/fields/virtual.py
--rw-r--r--   0        0        0     4426 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/filtering.py
--rw-r--r--   0        0        0     1849 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/helpers.py
--rw-r--r--   0        0        0    34236 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/mapping/__init__.py
--rw-r--r--   0        0        0     2359 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/mapping/helpers.py
--rw-r--r--   0        0        0     8940 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/proxy.py
--rw-r--r--   0        0        0        0 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/py.typed
--rw-r--r--   0        0        0     5383 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/registration.py
--rw-r--r--   0        0        0    27572 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/resources.py
--rw-r--r--   0        0        0     1562 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/serializers.py
--rw-r--r--   0        0        0     9572 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/traversal.py
--rw-r--r--   0        0        0     8910 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/utils/__init__.py
--rw-r--r--   0        0        0     3725 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/utils/ipv6.py
--rw-r--r--   0        0        0    10342 2023-06-15 23:41:28.838387 odin-2.8.1/src/odin/validators.py
--rw-r--r--   0        0        0        0 2023-06-15 23:41:28.838387 odin-2.8.1/tests/__init__.py
--rw-r--r--   0        0        0      582 2023-06-15 23:41:28.838387 odin-2.8.1/tests/_helpers.py
--rw-r--r--   0        0        0        0 2023-06-15 23:41:28.838387 odin-2.8.1/tests/annotated_resources/__init__.py
--rw-r--r--   0        0        0    12091 2023-06-15 23:41:28.838387 odin-2.8.1/tests/annotated_resources/test_type_resolution.py
--rw-r--r--   0        0        0      429 2023-06-15 23:41:28.838387 odin-2.8.1/tests/conftest.py
--rw-r--r--   0        0        0     1779 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_arrow_fields.py
--rw-r--r--   0        0        0     6023 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_geo_datatypes.py
--rw-r--r--   0        0        0     2797 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_geo_fields.py
--rw-r--r--   0        0        0     2293 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_geo_serialisation.py
--rw-r--r--   0        0        0     3323 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_money_datatypes.py
--rw-r--r--   0        0        0      733 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_money_fields.py
--rw-r--r--   0        0        0      911 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_money_serialisation.py
--rw-r--r--   0        0        0     1216 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_pint_fields.py
--rw-r--r--   0        0        0      433 2023-06-15 23:41:28.838387 odin-2.8.1/tests/contrib/test_sphinx.py
--rw-r--r--   0        0        0      301 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-incorrect.toml
--rw-r--r--   0        0        0      720 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-invalid.json
--rw-r--r--   0        0        0      303 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-invalid.toml
--rw-r--r--   0        0        0      354 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-invalid.yaml
--rw-r--r--   0        0        0      642 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-valid.json
--rw-r--r--   0        0        0      325 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-valid.toml
--rw-r--r--   0        0        0      453 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-valid.xml
--rw-r--r--   0        0        0      357 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/book-valid.yaml
--rw-r--r--   0        0        0      469 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-header-alt-order.csv
--rw-r--r--   0        0        0     2503 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-invalid-nested.json
--rw-r--r--   0        0        0      442 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-invalid.csv
--rw-r--r--   0        0        0      441 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-last-bad.csv
--rw-r--r--   0        0        0      441 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-lower-header.csv
--rw-r--r--   0        0        0      389 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-no-header.csv
--rw-r--r--   0        0        0      441 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library-valid.csv
--rw-r--r--   0        0        0     2543 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library.json
--rw-r--r--   0        0        0     1948 2023-06-15 23:41:28.838387 odin-2.8.1/tests/fixtures/library.yaml
--rw-r--r--   0        0        0     6147 2023-06-15 23:41:28.838387 odin-2.8.1/tests/resources.py
--rw-r--r--   0        0        0     2339 2023-06-15 23:41:28.838387 odin-2.8.1/tests/resources_annotated.py
--rw-r--r--   0        0        0     3922 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_adapters.py
--rw-r--r--   0        0        0     3124 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_annotated_resources.py
--rw-r--r--   0        0        0     7033 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_csv.py
--rw-r--r--   0        0        0     3018 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_dict.py
--rw-r--r--   0        0        0     2673 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_json.py
--rw-r--r--   0        0        0     2689 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_msgpack.py
--rw-r--r--   0        0        0     6256 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_toml.py
--rw-r--r--   0        0        0     2157 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_xml.py
--rw-r--r--   0        0        0     2228 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_codec_yaml.py
--rw-r--r--   0        0        0     1143 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_compatibility.py
--rw-r--r--   0        0        0     1793 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_datastructures.py
--rw-r--r--   0        0        0    11627 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_datetimeutil.py
--rw-r--r--   0        0        0     1070 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_decorators.py
--rw-r--r--   0        0        0     2072 2023-06-15 23:41:28.838387 odin-2.8.1/tests/test_exceptions.py
--rw-r--r--   0        0        0    48478 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_fields.py
--rw-r--r--   0        0        0     9825 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_fields_composite.py
--rw-r--r--   0        0        0     1028 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_fields_virtual.py
--rw-r--r--   0        0        0     4564 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_filtering.py
--rw-r--r--   0        0        0     1735 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_helpers.py
--rw-r--r--   0        0        0     3176 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_kitchensink.py
--rw-r--r--   0        0        0    20443 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_mapping.py
--rw-r--r--   0        0        0      963 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_mapping_helpers.py
--rw-r--r--   0        0        0     1374 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_polymorphic.py
--rw-r--r--   0        0        0     5058 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_proxy.py
--rw-r--r--   0        0        0     2904 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_resource_base.py
--rw-r--r--   0        0        0    11513 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_resources.py
--rw-r--r--   0        0        0     2206 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_serializers.py
--rw-r--r--   0        0        0    10433 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_traversal.py
--rw-r--r--   0        0        0     5860 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_utils.py
--rw-r--r--   0        0        0     7619 2023-06-15 23:41:28.842387 odin-2.8.1/tests/test_validators.py
--rw-r--r--   0        0        0     9538 1970-01-01 00:00:00.000000 odin-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1539 2023-09-27 13:51:12.538876 odin-2.9.0/LICENSE
+-rw-r--r--   0        0        0     7879 2023-09-27 13:51:12.538876 odin-2.9.0/README.rst
+-rw-r--r--   0        0        0     2491 2023-09-27 13:51:12.538876 odin-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0      718 2023-09-27 13:51:12.538876 odin-2.9.0/src/odin/__init__.py
+-rw-r--r--   0        0        0     5356 2023-09-27 13:51:12.538876 odin-2.9.0/src/odin/adapters.py
+-rw-r--r--   0        0        0     7306 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/annotated_resource/__init__.py
+-rw-r--r--   0        0        0      518 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/annotated_resource/special_fields.py
+-rw-r--r--   0        0        0      791 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/annotated_resource/type_aliases.py
+-rw-r--r--   0        0        0     8701 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/annotated_resource/type_resolution.py
+-rw-r--r--   0        0        0      376 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/bases.py
+-rw-r--r--   0        0        0        0 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/codecs/__init__.py
+-rw-r--r--   0        0        0    10541 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/codecs/csv_codec.py
+-rw-r--r--   0        0        0     2480 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/codecs/dict_codec.py
+-rw-r--r--   0        0        0     4547 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/codecs/json_codec.py
+-rw-r--r--   0        0        0     4264 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/codecs/msgpack_codec.py
+-rw-r--r--   0        0        0     5899 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/codecs/toml_codec.py
+-rw-r--r--   0        0        0     3115 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/codecs/xml_codec.py
+-rw-r--r--   0        0        0     3970 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/codecs/yaml_codec.py
+-rw-r--r--   0        0        0     1249 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/compatibility.py
+-rw-r--r--   0        0        0        0 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/__init__.py
+-rw-r--r--   0        0        0      503 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/arrow/__init__.py
+-rw-r--r--   0        0        0     1791 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/arrow/fields.py
+-rw-r--r--   0        0        0      146 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/geo/__init__.py
+-rw-r--r--   0        0        0     3765 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/geo/datatypes.py
+-rw-r--r--   0        0        0     2370 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/geo/fields.py
+-rw-r--r--   0        0        0     6675 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/json_schema/__init__.py
+-rw-r--r--   0        0        0      115 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/money/__init__.py
+-rw-r--r--   0        0        0    18131 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/money/datatypes.py
+-rw-r--r--   0        0        0     1585 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/money/fields.py
+-rw-r--r--   0        0        0      222 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/pint/__init__.py
+-rw-r--r--   0        0        0     2182 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/pint/fields.py
+-rw-r--r--   0        0        0      245 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/pint/units.py
+-rw-r--r--   0        0        0       80 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/rich/__init__.py
+-rw-r--r--   0        0        0      631 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/rich/theme.py
+-rw-r--r--   0        0        0     1662 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/rich/validation_tree.py
+-rw-r--r--   0        0        0     6787 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/sphinx/__init__.py
+-rw-r--r--   0        0        0     1309 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/contrib/swagger/__init__.py
+-rw-r--r--   0        0        0     1183 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/datastructures.py
+-rw-r--r--   0        0        0    10233 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/datetimeutil.py
+-rw-r--r--   0        0        0     1624 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/decorators.py
+-rw-r--r--   0        0        0     4800 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/exceptions.py
+-rw-r--r--   0        0        0    33799 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/fields/__init__.py
+-rw-r--r--   0        0        0     2078 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/fields/base.py
+-rw-r--r--   0        0        0     9348 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/fields/composite.py
+-rw-r--r--   0        0        0     4479 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/fields/virtual.py
+-rw-r--r--   0        0        0     4426 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/filtering.py
+-rw-r--r--   0        0        0     1849 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/helpers.py
+-rw-r--r--   0        0        0    34236 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/mapping/__init__.py
+-rw-r--r--   0        0        0     2359 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/mapping/helpers.py
+-rw-r--r--   0        0        0     8940 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/proxy.py
+-rw-r--r--   0        0        0        0 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/py.typed
+-rw-r--r--   0        0        0     5383 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/registration.py
+-rw-r--r--   0        0        0    27572 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/resources.py
+-rw-r--r--   0        0        0     1562 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/serializers.py
+-rw-r--r--   0        0        0     9572 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/traversal.py
+-rw-r--r--   0        0        0     8910 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/utils/__init__.py
+-rw-r--r--   0        0        0     3725 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/utils/ipv6.py
+-rw-r--r--   0        0        0    10342 2023-09-27 13:51:12.542876 odin-2.9.0/src/odin/validators.py
+-rw-r--r--   0        0        0        0 2023-09-27 13:51:12.542876 odin-2.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      582 2023-09-27 13:51:12.542876 odin-2.9.0/tests/_helpers.py
+-rw-r--r--   0        0        0        0 2023-09-27 13:51:12.542876 odin-2.9.0/tests/annotated_resources/__init__.py
+-rw-r--r--   0        0        0    12091 2023-09-27 13:51:12.542876 odin-2.9.0/tests/annotated_resources/test_type_resolution.py
+-rw-r--r--   0        0        0      429 2023-09-27 13:51:12.542876 odin-2.9.0/tests/conftest.py
+-rw-r--r--   0        0        0     1779 2023-09-27 13:51:12.542876 odin-2.9.0/tests/contrib/test_arrow_fields.py
+-rw-r--r--   0        0        0     6023 2023-09-27 13:51:12.542876 odin-2.9.0/tests/contrib/test_geo_datatypes.py
+-rw-r--r--   0        0        0     2797 2023-09-27 13:51:12.542876 odin-2.9.0/tests/contrib/test_geo_fields.py
+-rw-r--r--   0        0        0     2293 2023-09-27 13:51:12.542876 odin-2.9.0/tests/contrib/test_geo_serialisation.py
+-rw-r--r--   0        0        0     3323 2023-09-27 13:51:12.542876 odin-2.9.0/tests/contrib/test_money_datatypes.py
+-rw-r--r--   0        0        0      733 2023-09-27 13:51:12.542876 odin-2.9.0/tests/contrib/test_money_fields.py
+-rw-r--r--   0        0        0      911 2023-09-27 13:51:12.542876 odin-2.9.0/tests/contrib/test_money_serialisation.py
+-rw-r--r--   0        0        0     1216 2023-09-27 13:51:12.542876 odin-2.9.0/tests/contrib/test_pint_fields.py
+-rw-r--r--   0        0        0      433 2023-09-27 13:51:12.542876 odin-2.9.0/tests/contrib/test_sphinx.py
+-rw-r--r--   0        0        0      301 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/book-incorrect.toml
+-rw-r--r--   0        0        0      720 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/book-invalid.json
+-rw-r--r--   0        0        0      303 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/book-invalid.toml
+-rw-r--r--   0        0        0      354 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/book-invalid.yaml
+-rw-r--r--   0        0        0      642 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/book-valid.json
+-rw-r--r--   0        0        0      325 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/book-valid.toml
+-rw-r--r--   0        0        0      453 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/book-valid.xml
+-rw-r--r--   0        0        0      357 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/book-valid.yaml
+-rw-r--r--   0        0        0      469 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/library-header-alt-order.csv
+-rw-r--r--   0        0        0     2503 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/library-invalid-nested.json
+-rw-r--r--   0        0        0      442 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/library-invalid.csv
+-rw-r--r--   0        0        0      441 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/library-last-bad.csv
+-rw-r--r--   0        0        0      441 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/library-lower-header.csv
+-rw-r--r--   0        0        0      389 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/library-no-header.csv
+-rw-r--r--   0        0        0      441 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/library-valid.csv
+-rw-r--r--   0        0        0     2543 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/library.json
+-rw-r--r--   0        0        0     1948 2023-09-27 13:51:12.542876 odin-2.9.0/tests/fixtures/library.yaml
+-rw-r--r--   0        0        0     6147 2023-09-27 13:51:12.542876 odin-2.9.0/tests/resources.py
+-rw-r--r--   0        0        0     2339 2023-09-27 13:51:12.542876 odin-2.9.0/tests/resources_annotated.py
+-rw-r--r--   0        0        0     3922 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_adapters.py
+-rw-r--r--   0        0        0     3124 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_annotated_resources.py
+-rw-r--r--   0        0        0     7033 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_codec_csv.py
+-rw-r--r--   0        0        0     3018 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_codec_dict.py
+-rw-r--r--   0        0        0     2673 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_codec_json.py
+-rw-r--r--   0        0        0     2689 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_codec_msgpack.py
+-rw-r--r--   0        0        0     6256 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_codec_toml.py
+-rw-r--r--   0        0        0     2157 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_codec_xml.py
+-rw-r--r--   0        0        0     2228 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_codec_yaml.py
+-rw-r--r--   0        0        0     1143 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_compatibility.py
+-rw-r--r--   0        0        0     1793 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_datastructures.py
+-rw-r--r--   0        0        0    11627 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_datetimeutil.py
+-rw-r--r--   0        0        0     1070 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_decorators.py
+-rw-r--r--   0        0        0     2072 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0    48478 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_fields.py
+-rw-r--r--   0        0        0    10297 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_fields_composite.py
+-rw-r--r--   0        0        0     1028 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_fields_virtual.py
+-rw-r--r--   0        0        0     4564 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_filtering.py
+-rw-r--r--   0        0        0     1735 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_helpers.py
+-rw-r--r--   0        0        0     3176 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_kitchensink.py
+-rw-r--r--   0        0        0    20443 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_mapping.py
+-rw-r--r--   0        0        0      963 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_mapping_helpers.py
+-rw-r--r--   0        0        0     1374 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_polymorphic.py
+-rw-r--r--   0        0        0     5058 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_proxy.py
+-rw-r--r--   0        0        0     2904 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_resource_base.py
+-rw-r--r--   0        0        0    11513 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_resources.py
+-rw-r--r--   0        0        0     2206 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_serializers.py
+-rw-r--r--   0        0        0    10433 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_traversal.py
+-rw-r--r--   0        0        0     5860 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_utils.py
+-rw-r--r--   0        0        0     7619 2023-09-27 13:51:12.546876 odin-2.9.0/tests/test_validators.py
+-rw-r--r--   0        0        0     9538 1970-01-01 00:00:00.000000 odin-2.9.0/PKG-INFO
```

### Comparing `odin-2.8.1/LICENSE` & `odin-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/README.rst` & `odin-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/pyproject.toml` & `odin-2.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "odin"
-version = "2.8.1"
+version = "2.9.0"
 description = "Data-structure definition/validation/traversal, mapping and serialisation toolkit for Python"
 authors = ["Tim Savage <tim@savage.company>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 repository = "https://github.com/python-odin/odin"
 documentation = "https://odin.readthedocs.org"
 keywords = ["data-structure", "validation", "data-mapping"]
```

### Comparing `odin-2.8.1/src/odin/__init__.py` & `odin-2.9.0/src/odin/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/adapters.py` & `odin-2.9.0/src/odin/adapters.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/annotated_resource/__init__.py` & `odin-2.9.0/src/odin/annotated_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/annotated_resource/special_fields.py` & `odin-2.9.0/src/odin/annotated_resource/special_fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/annotated_resource/type_aliases.py` & `odin-2.9.0/src/odin/annotated_resource/type_aliases.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/annotated_resource/type_resolution.py` & `odin-2.9.0/src/odin/annotated_resource/type_resolution.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/codecs/csv_codec.py` & `odin-2.9.0/src/odin/codecs/csv_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/codecs/dict_codec.py` & `odin-2.9.0/src/odin/codecs/dict_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/codecs/json_codec.py` & `odin-2.9.0/src/odin/codecs/json_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/codecs/msgpack_codec.py` & `odin-2.9.0/src/odin/codecs/msgpack_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/codecs/toml_codec.py` & `odin-2.9.0/src/odin/codecs/toml_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/codecs/xml_codec.py` & `odin-2.9.0/src/odin/codecs/xml_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/codecs/yaml_codec.py` & `odin-2.9.0/src/odin/codecs/yaml_codec.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/compatibility.py` & `odin-2.9.0/src/odin/compatibility.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/contrib/arrow/fields.py` & `odin-2.9.0/src/odin/contrib/arrow/fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/contrib/geo/datatypes.py` & `odin-2.9.0/src/odin/contrib/geo/datatypes.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/contrib/geo/fields.py` & `odin-2.9.0/src/odin/contrib/geo/fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/contrib/json_schema/__init__.py` & `odin-2.9.0/src/odin/contrib/json_schema/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 VALIDATOR_SCHEMAS = {
     odin.validators.MaxValueValidator: {},
     odin.validators.MinValueValidator: {},
     odin.validators.LengthValidator: {},
     odin.validators.MaxLengthValidator: {},
     odin.validators.MinLengthValidator: {},
 }
+JSON_SCHEMA_METHOD: Final[str] = "as_json_schema"
 
 
 class JSONSchema:
     """JSON Schema representation of an Odin resource."""
 
     def __init__(
         self, resource: Type[ResourceBase], *, require_type_field: bool = True
@@ -104,15 +105,19 @@
 
     def _field_type(
         self, field: odin.Field
     ) -> Tuple[Union[str, List[str]], Dict[str, Any]]:
         """Get the type of a field."""
 
         field_type = type(field)
-        if field_type in FIELD_SCHEMAS:
+
+        if method := getattr(field, JSON_SCHEMA_METHOD, None):
+            type_name, schema = method()
+
+        elif field_type in FIELD_SCHEMAS:
             type_name, schema = FIELD_SCHEMAS[field_type]
 
         elif isinstance(field, odin.EnumField):
             type_name = "string"
             schema = {"enum": tuple(str(item.value) for item in field.enum_type)}
 
         elif isinstance(field, odin.TypedListField):
@@ -136,20 +141,23 @@
 
     def _composite_field_to_schema(self, field: odin.CompositeField) -> Dict[str, Any]:
         """Convert a composite field to a JSON schema."""
 
         # Handle abstract resources
         child_resources = get_child_resources(field.of)
         if child_resources:
-            schema = {
-                "oneOf": [
-                    self._schema_def(child_resource)
-                    for child_resource in child_resources
-                ]
-            }
+            if len(child_resources) == 1:
+                schema = self._schema_def(child_resources[0])
+            else:
+                schema = {
+                    "oneOf": [
+                        self._schema_def(child_resource)
+                        for child_resource in child_resources
+                    ]
+                }
         else:
             schema = self._schema_def(field.of)
 
         if isinstance(field, odin.ListOf):
             schema = {"type": "array", "items": schema}
 
         elif isinstance(field, odin.DictOf):
```

### Comparing `odin-2.8.1/src/odin/contrib/money/datatypes.py` & `odin-2.9.0/src/odin/contrib/money/datatypes.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/contrib/money/fields.py` & `odin-2.9.0/src/odin/contrib/money/fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/contrib/pint/fields.py` & `odin-2.9.0/src/odin/contrib/pint/fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/contrib/rich/theme.py` & `odin-2.9.0/src/odin/contrib/rich/theme.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/contrib/rich/validation_tree.py` & `odin-2.9.0/src/odin/contrib/rich/validation_tree.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/contrib/sphinx/__init__.py` & `odin-2.9.0/src/odin/contrib/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/contrib/swagger/__init__.py` & `odin-2.9.0/src/odin/contrib/swagger/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/datastructures.py` & `odin-2.9.0/src/odin/datastructures.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/datetimeutil.py` & `odin-2.9.0/src/odin/datetimeutil.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/decorators.py` & `odin-2.9.0/src/odin/decorators.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/exceptions.py` & `odin-2.9.0/src/odin/exceptions.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/fields/__init__.py` & `odin-2.9.0/src/odin/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/fields/base.py` & `odin-2.9.0/src/odin/fields/base.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/fields/composite.py` & `odin-2.9.0/src/odin/fields/composite.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from typing import Any, Iterator, Tuple
+"""Composite fields for handling collections of resources."""
+import abc
+from functools import cached_property
+from typing import Any, Callable, Iterator, Tuple
 
 from odin import bases, exceptions
 from odin.fields import Field
 from odin.resources import create_resource_from_dict
 from odin.utils import value_in_choices
 from odin.validators import EMPTY_VALUES
 
@@ -12,40 +15,77 @@
     "ObjectAs",
     "ListOf",
     "ArrayOf",
     "DictOf",
 )
 
 
-class CompositeField(Field):
-    """
-    The base class for composite (or fields that contain other resources) eg DictAs/ListOf fields.
-    """
+class CompositeField(Field, metaclass=abc.ABCMeta):
+    """The base class for composite.
+
+    Fields that contain other resources eg DictAs/ListOf fields."""
+
+    @classmethod
+    def delayed(cls, resource_callable: Callable[[], Any], **options):
+        """Create a delayed resource field.
+
+        This is used in the case of tree structures where a resource may reference itself.
+
+        This should be used with a lambda function to avoid referencing an incomplete type.
+
+        .. code-block:: python
+
+            class Category(odin.Resource):
+                name = odin.StringField()
+                child_categories = odin.DictAs.delayed(lambda: Category)
 
-    def __init__(self, resource, use_container=False, **options):
         """
-        Initialisation of a CompositeField.
+        return cls(resource_callable, **options)
+
+    def __init__(self, resource, use_container=False, **options):
+        """Initialisation of a CompositeField.
 
         :param resource:
         :param use_container: Special flag for codecs that support containers or just multiple instances of a
             sub element (ie XML).
         :param empty: This collection can be empty
         :param options: Additional options passed to :py:class:`odin.fields.Field` super class.
 
         """
+
         if not hasattr(resource, "_meta"):
-            raise TypeError(f"{resource!r} is not a valid type for a related field.")
-        self.of = resource
+            if callable(resource):
+                # Delayed resolution of the resource type.
+                self._of = resource
+            else:
+                # Keep this pattern so old behaviour remains.
+                raise TypeError(
+                    f"{resource!r} is not a valid type for a related field."
+                )
+        else:
+            self._of = resource
         self.use_container = use_container
 
         if not options.get("null", False):
-            options.setdefault("default", lambda: resource())
+            options.setdefault("default", lambda: self.of())
 
         super().__init__(**options)
 
+    @cached_property
+    def of(self):
+        """Return the resource type."""
+        resource = self._of
+        if not hasattr(resource, "_meta") and callable(resource):
+            resource = resource()
+            if not hasattr(resource, "_meta"):
+                raise TypeError(
+                    f"{resource!r} is not a valid type for a related field."
+                )
+        return resource
+
     def to_python(self, value):
         """Convert raw value to a python value."""
         if value is None:
             return None
         if isinstance(value, self.of):
             return value
         if isinstance(value, dict):
@@ -55,32 +95,24 @@
 
     def validate(self, value):
         """Validate the value."""
         super().validate(value)
         if value not in EMPTY_VALUES:
             value.full_clean()
 
+    @abc.abstractmethod
     def item_iter_from_object(self, obj):
-        """
-        Return an iterator of items (resource, idx) from composite field.
+        """Return an iterator of items (resource, idx) from composite field.
 
         For single items (eg ``DictAs`` will return a list a single item (resource, None))
-
-        :param obj:
-        :return:
         """
-        raise NotImplementedError()
 
+    @abc.abstractmethod
     def key_to_python(self, key):
-        """
-        A to python method for the key value.
-        :param key:
-        :return:
-        """
-        raise NotImplementedError()
+        """A to python method for the key value."""
 
 
 class DictAs(CompositeField):
     """Treat a dictionary as a Resource."""
 
     default_error_messages = {
         "invalid": "Must be a dict of type ``%r``.",
@@ -239,15 +271,15 @@
             super_validate = super().validate
             self._process_dict(value, super_validate)
 
         if (value is not None) and (not value) and (not self.empty):
             raise exceptions.ValidationError(self.error_messages["empty"], code="empty")
 
     def __iter__(self):
-        # This does nothing but it does prevent inspections from complaining.
+        # This does nothing, it does prevent inspections from complaining.
         return None  # NoQA
 
     def item_iter_from_object(self, obj) -> Iterator[Tuple[str, Any]]:
         """Iterate object returning key/value pairs"""
         resources = self.value_from_object(obj)
         if resources:
             for key in sorted(resources):
```

### Comparing `odin-2.8.1/src/odin/fields/virtual.py` & `odin-2.9.0/src/odin/fields/virtual.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/filtering.py` & `odin-2.9.0/src/odin/filtering.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/helpers.py` & `odin-2.9.0/src/odin/helpers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/mapping/__init__.py` & `odin-2.9.0/src/odin/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/mapping/helpers.py` & `odin-2.9.0/src/odin/mapping/helpers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/proxy.py` & `odin-2.9.0/src/odin/proxy.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/registration.py` & `odin-2.9.0/src/odin/registration.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/resources.py` & `odin-2.9.0/src/odin/resources.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/serializers.py` & `odin-2.9.0/src/odin/serializers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/traversal.py` & `odin-2.9.0/src/odin/traversal.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/utils/__init__.py` & `odin-2.9.0/src/odin/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/utils/ipv6.py` & `odin-2.9.0/src/odin/utils/ipv6.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/src/odin/validators.py` & `odin-2.9.0/src/odin/validators.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/_helpers.py` & `odin-2.9.0/tests/_helpers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/annotated_resources/test_type_resolution.py` & `odin-2.9.0/tests/annotated_resources/test_type_resolution.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/contrib/test_arrow_fields.py` & `odin-2.9.0/tests/contrib/test_arrow_fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/contrib/test_geo_datatypes.py` & `odin-2.9.0/tests/contrib/test_geo_datatypes.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/contrib/test_geo_fields.py` & `odin-2.9.0/tests/contrib/test_geo_fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/contrib/test_geo_serialisation.py` & `odin-2.9.0/tests/contrib/test_geo_serialisation.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/contrib/test_money_datatypes.py` & `odin-2.9.0/tests/contrib/test_money_datatypes.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/contrib/test_money_fields.py` & `odin-2.9.0/tests/contrib/test_money_fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/contrib/test_money_serialisation.py` & `odin-2.9.0/tests/contrib/test_money_serialisation.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/contrib/test_pint_fields.py` & `odin-2.9.0/tests/contrib/test_pint_fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/fixtures/book-invalid.json` & `odin-2.9.0/tests/fixtures/book-invalid.json`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/fixtures/book-valid.json` & `odin-2.9.0/tests/fixtures/book-valid.json`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/fixtures/library-invalid-nested.json` & `odin-2.9.0/tests/fixtures/library-invalid-nested.json`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/fixtures/library.json` & `odin-2.9.0/tests/fixtures/library.json`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/fixtures/library.yaml` & `odin-2.9.0/tests/fixtures/library.yaml`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/resources.py` & `odin-2.9.0/tests/resources.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/resources_annotated.py` & `odin-2.9.0/tests/resources_annotated.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_adapters.py` & `odin-2.9.0/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_annotated_resources.py` & `odin-2.9.0/tests/test_annotated_resources.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_codec_csv.py` & `odin-2.9.0/tests/test_codec_csv.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_codec_dict.py` & `odin-2.9.0/tests/test_codec_dict.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_codec_json.py` & `odin-2.9.0/tests/test_codec_json.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_codec_msgpack.py` & `odin-2.9.0/tests/test_codec_msgpack.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_codec_toml.py` & `odin-2.9.0/tests/test_codec_toml.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_codec_xml.py` & `odin-2.9.0/tests/test_codec_xml.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_codec_yaml.py` & `odin-2.9.0/tests/test_codec_yaml.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_compatibility.py` & `odin-2.9.0/tests/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_datastructures.py` & `odin-2.9.0/tests/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_datetimeutil.py` & `odin-2.9.0/tests/test_datetimeutil.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_decorators.py` & `odin-2.9.0/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_exceptions.py` & `odin-2.9.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_fields.py` & `odin-2.9.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_fields_composite.py` & `odin-2.9.0/tests/test_fields_composite.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,32 @@
         if len(first) != len(second):
             raise AssertionError("Dicts are different lengths")
         for key in first.keys():
             self.assertResourceEqual(first[key], second[key])
 
     # DictAs ##################################################################
 
-    def test_dictas_ensure_is_resource(self):
+    def test_dictas__where_a_resource_is_not_supplied(self):
         with pytest.raises(TypeError):
             DictAs("an item")
 
+    def test_dictas__where_resource_resolution_is_delayed(self):
+        target = DictAs.delayed(lambda: ExampleResource, null=True)
+
+        assert target.of is ExampleResource
+        assert target.null is True
+
+    def test_dictas__where_resource_resolution_is_delayed_but_a_resource_is_not_supplied(
+        self,
+    ):
+        target = DictAs.delayed(lambda: "an item", null=True)
+
+        with pytest.raises(TypeError):
+            assert target.of
+
     def test_dictas_1(self):
         f = DictAs(ExampleResource)
         pytest.raises(ValidationError, f.clean, None)
         pytest.raises(ValidationError, f.clean, "abc")
         pytest.raises(ValidationError, f.clean, 123)
         pytest.raises(ValidationError, f.clean, {})
         pytest.raises(
```

### Comparing `odin-2.8.1/tests/test_fields_virtual.py` & `odin-2.9.0/tests/test_fields_virtual.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_filtering.py` & `odin-2.9.0/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_helpers.py` & `odin-2.9.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_kitchensink.py` & `odin-2.9.0/tests/test_kitchensink.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_mapping.py` & `odin-2.9.0/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_mapping_helpers.py` & `odin-2.9.0/tests/test_mapping_helpers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_polymorphic.py` & `odin-2.9.0/tests/test_polymorphic.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_proxy.py` & `odin-2.9.0/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_resource_base.py` & `odin-2.9.0/tests/test_resource_base.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_resources.py` & `odin-2.9.0/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_serializers.py` & `odin-2.9.0/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_traversal.py` & `odin-2.9.0/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_utils.py` & `odin-2.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/tests/test_validators.py` & `odin-2.9.0/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `odin-2.8.1/PKG-INFO` & `odin-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odin
-Version: 2.8.1
+Version: 2.9.0
 Summary: Data-structure definition/validation/traversal, mapping and serialisation toolkit for Python
 Home-page: https://github.com/python-odin/odin
 License: BSD-3-Clause
 Keywords: data-structure,validation,data-mapping
 Author: Tim Savage
 Author-email: tim@savage.company
 Requires-Python: >=3.8,<4.0
```

