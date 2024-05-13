# Comparing `tmp/fastapi_xroad_soap-0.4.4.tar.gz` & `tmp/fastapi_xroad_soap-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_xroad_soap-0.4.4.tar", max compression
+gzip compressed data, was "fastapi_xroad_soap-0.4.5.tar", max compression
```

## Comparing `fastapi_xroad_soap-0.4.4.tar` & `fastapi_xroad_soap-0.4.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0    13831 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/LICENSE
--rw-r--r--   0        0        0     6684 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/README.md
--rw-r--r--   0        0        0      524 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/__init__.py
--rw-r--r--   0        0        0      574 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/elements.py
--rw-r--r--   0        0        0      431 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/faults.py
--rw-r--r--   0        0        0      340 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/__init__.py
--rw-r--r--   0        0        0      666 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/__init__.py
--rw-r--r--   0        0        0     2953 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/base_element_spec.py
--rw-r--r--   0        0        0     1194 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/composite_meta.py
--rw-r--r--   0        0        0      988 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/dynamic_spec.py
--rw-r--r--   0        0        0     4392 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/message_body.py
--rw-r--r--   0        0        0     2705 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/validators.py
--rw-r--r--   0        0        0     1067 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/constants.py
--rw-r--r--   0        0        0      486 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/__init__.py
--rw-r--r--   0        0        0     1061 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/__init__.py
--rw-r--r--   0        0        0     1479 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/boolean.py
--rw-r--r--   0        0        0     1195 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/date.py
--rw-r--r--   0        0        0     1243 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/datetime.py
--rw-r--r--   0        0        0     1180 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/float.py
--rw-r--r--   0        0        0     1223 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/integer.py
--rw-r--r--   0        0        0     1247 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/netres.py
--rw-r--r--   0        0        0     1284 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/string.py
--rw-r--r--   0        0        0     6437 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/swaref.py
--rw-r--r--   0        0        0     1195 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/time.py
--rw-r--r--   0        0        0     2125 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/numeric_type_spec.py
--rw-r--r--   0        0        0     2276 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/string_type_spec.py
--rw-r--r--   0        0        0     3767 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/validators.py
--rw-r--r--   0        0        0      679 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/__init__.py
--rw-r--r--   0        0        0     2836 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/factory.py
--rw-r--r--   0        0        0     1425 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/generics.py
--rw-r--r--   0        0        0     1912 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/header.py
--rw-r--r--   0        0        0     2020 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/file_size.py
--rw-r--r--   0        0        0      742 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/__init__.py
--rw-r--r--   0        0        0     2608 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/bodypart.py
--rw-r--r--   0        0        0     1898 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/decoder.py
--rw-r--r--   0        0        0     2493 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/encoder.py
--rw-r--r--   0        0        0     1020 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/errors.py
--rw-r--r--   0        0        0      955 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/__init__.py
--rw-r--r--   0        0        0     5257 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/action.py
--rw-r--r--   0        0        0     5223 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/faults.py
--rw-r--r--   0        0        0     1654 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/response.py
--rw-r--r--   0        0        0     5632 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/service.py
--rw-r--r--   0        0        0     2312 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/service.pyi
--rw-r--r--   0        0        0     2004 2024-05-06 12:38:16.953684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/validators.py
--rw-r--r--   0        0        0     5172 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/storage.py
--rw-r--r--   0        0        0     3249 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/uid_gen.py
--rw-r--r--   0        0        0     1068 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/__init__.py
--rw-r--r--   0        0        0     3057 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/content_utils.py
--rw-r--r--   0        0        0     2673 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/path_utils.py
--rw-r--r--   0        0        0      851 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/route_utils.py
--rw-r--r--   0        0        0      397 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/__init__.py
--rw-r--r--   0        0        0     5471 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/generator.py
--rw-r--r--   0        0        0     4274 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/helpers.py
--rw-r--r--   0        0        0     2050 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/__init__.py
--rw-r--r--   0        0        0     2864 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/binding.py
--rw-r--r--   0        0        0     1270 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/conditions.py
--rw-r--r--   0        0        0     1360 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/definitions.py
--rw-r--r--   0        0        0     1698 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/port_type.py
--rw-r--r--   0        0        0     1315 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/restrictions.py
--rw-r--r--   0        0        0     2139 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/schema.py
--rw-r--r--   0        0        0     1361 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/service.py
--rw-r--r--   0        0        0      561 2024-05-06 12:38:16.957684 fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/utils.py
--rw-r--r--   0        0        0     2587 2024-05-06 12:38:17.049684 fastapi_xroad_soap-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     8405 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    13831 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/LICENSE
+-rw-r--r--   0        0        0     6684 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/README.md
+-rw-r--r--   0        0        0      524 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/__init__.py
+-rw-r--r--   0        0        0      574 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/elements.py
+-rw-r--r--   0        0        0      431 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/faults.py
+-rw-r--r--   0        0        0      340 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/__init__.py
+-rw-r--r--   0        0        0      666 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/base/__init__.py
+-rw-r--r--   0        0        0     2953 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/base/base_element_spec.py
+-rw-r--r--   0        0        0     1194 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/base/composite_meta.py
+-rw-r--r--   0        0        0      988 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/base/dynamic_spec.py
+-rw-r--r--   0        0        0     4392 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/base/message_body.py
+-rw-r--r--   0        0        0     2705 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/base/validators.py
+-rw-r--r--   0        0        0     1067 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/constants.py
+-rw-r--r--   0        0        0      486 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/__init__.py
+-rw-r--r--   0        0        0     1061 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/__init__.py
+-rw-r--r--   0        0        0     1479 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/boolean.py
+-rw-r--r--   0        0        0     1195 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/date.py
+-rw-r--r--   0        0        0     1243 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/datetime.py
+-rw-r--r--   0        0        0     1180 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/float.py
+-rw-r--r--   0        0        0     1223 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/integer.py
+-rw-r--r--   0        0        0     1247 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/netres.py
+-rw-r--r--   0        0        0     1284 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/string.py
+-rw-r--r--   0        0        0     6437 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/swaref.py
+-rw-r--r--   0        0        0     1195 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/time.py
+-rw-r--r--   0        0        0     2125 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/numeric_type_spec.py
+-rw-r--r--   0        0        0     2276 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/string_type_spec.py
+-rw-r--r--   0        0        0     3767 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/validators.py
+-rw-r--r--   0        0        0      679 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/envelope/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/envelope/factory.py
+-rw-r--r--   0        0        0     1425 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/envelope/generics.py
+-rw-r--r--   0        0        0     1912 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/envelope/header.py
+-rw-r--r--   0        0        0     2020 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/file_size.py
+-rw-r--r--   0        0        0      742 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/multipart/__init__.py
+-rw-r--r--   0        0        0     2608 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/multipart/bodypart.py
+-rw-r--r--   0        0        0     1898 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/multipart/decoder.py
+-rw-r--r--   0        0        0     2493 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/multipart/encoder.py
+-rw-r--r--   0        0        0     1020 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/multipart/errors.py
+-rw-r--r--   0        0        0      955 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/__init__.py
+-rw-r--r--   0        0        0     5257 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/action.py
+-rw-r--r--   0        0        0     5223 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/faults.py
+-rw-r--r--   0        0        0     1654 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/response.py
+-rw-r--r--   0        0        0     5654 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/service.py
+-rw-r--r--   0        0        0     2312 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/service.pyi
+-rw-r--r--   0        0        0     2004 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/validators.py
+-rw-r--r--   0        0        0     5172 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/storage.py
+-rw-r--r--   0        0        0     3249 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/uid_gen.py
+-rw-r--r--   0        0        0     1068 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/utils/__init__.py
+-rw-r--r--   0        0        0     3057 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/utils/content_utils.py
+-rw-r--r--   0        0        0     2673 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/utils/path_utils.py
+-rw-r--r--   0        0        0      851 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/utils/route_utils.py
+-rw-r--r--   0        0        0      397 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/__init__.py
+-rw-r--r--   0        0        0     5471 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/generator.py
+-rw-r--r--   0        0        0     4274 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/helpers.py
+-rw-r--r--   0        0        0     2050 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/__init__.py
+-rw-r--r--   0        0        0     2864 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/binding.py
+-rw-r--r--   0        0        0     1270 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/conditions.py
+-rw-r--r--   0        0        0     1360 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/definitions.py
+-rw-r--r--   0        0        0     1698 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/port_type.py
+-rw-r--r--   0        0        0     1315 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/restrictions.py
+-rw-r--r--   0        0        0     2139 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/schema.py
+-rw-r--r--   0        0        0     1361 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/service.py
+-rw-r--r--   0        0        0      561 2024-05-13 15:17:50.284031 fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/utils.py
+-rw-r--r--   0        0        0     2588 2024-05-13 15:17:50.380031 fastapi_xroad_soap-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     8406 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.4.5/PKG-INFO
```

### Comparing `fastapi_xroad_soap-0.4.4/LICENSE` & `fastapi_xroad_soap-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/README.md` & `fastapi_xroad_soap-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/__init__.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/elements.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/elements.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/__init__.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/base/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/base_element_spec.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/base/base_element_spec.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/composite_meta.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/base/composite_meta.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/dynamic_spec.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/base/dynamic_spec.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/message_body.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/base/message_body.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/base/validators.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/base/validators.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/constants.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/constants.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/__init__.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/boolean.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/boolean.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/date.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/date.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/datetime.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/datetime.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/float.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/float.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/integer.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/integer.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/netres.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/netres.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/string.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/string.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/swaref.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/swaref.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/models/time.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/models/time.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/numeric_type_spec.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/numeric_type_spec.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/string_type_spec.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/string_type_spec.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/elements/validators.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/elements/validators.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/__init__.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/envelope/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/factory.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/envelope/factory.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/generics.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/envelope/generics.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/envelope/header.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/envelope/header.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/file_size.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/file_size.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/__init__.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/multipart/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/bodypart.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/multipart/bodypart.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/decoder.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/multipart/decoder.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/encoder.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/multipart/encoder.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/multipart/errors.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/multipart/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/__init__.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/action.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/action.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/faults.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/faults.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/response.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/response.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/service.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 		app.add_middleware(
 			middleware_class=SoapMiddleware,
 			dispatch=self._soap_middleware
 		)
 
 	async def _soap_middleware(self, http_request: Request, _: t.Callable) -> t.Optional[Response]:
 		try:
-			if http_request.url.path != self._path:
+			if self._path != '/' and http_request.url.path != self._path:
 				return Response(status_code=404)
 			elif "wsdl" in http_request.query_params:
 				if self._wsdl_response is None:
 					self.regenerate_wsdl()
 				return self._wsdl_response
 			elif http_request.method != "POST":
 				raise f.InvalidMethodFault(http_request.method)
```

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/service.pyi` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/service.pyi`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/soap/validators.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/soap/validators.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/storage.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/uid_gen.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/uid_gen.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/__init__.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/content_utils.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/utils/content_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/path_utils.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/utils/route_utils.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/utils/route_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/generator.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/generator.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/helpers.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/helpers.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/__init__.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/binding.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/binding.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/conditions.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/conditions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/definitions.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/definitions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/port_type.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/port_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/restrictions.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/restrictions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/schema.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/internal/wsdl/models/service.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/internal/wsdl/models/service.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/fastapi_xroad_soap/utils.py` & `fastapi_xroad_soap-0.4.5/fastapi_xroad_soap/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.4/pyproject.toml` & `fastapi_xroad_soap-0.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-xroad-soap"
-version = "0.4.4"
+version = "0.4.5"
 description = "FastAPI Extension for X-Road SOAP"
 authors = ["Zero Reports Team <zero.dev@rik.ee>"]
 license = "EUPL-1.2"
 readme = "README.md"
 keywords = ["fastapi", "xroad", "soap"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -33,30 +33,30 @@
 [tool.poetry.urls]
 "Repository" = "https://github.com/rik-ee/fastapi-xroad-soap"
 "Documentation" = "https://github.com/rik-ee/fastapi-xroad-soap/wiki"
 "Bug Tracker" = "https://github.com/rik-ee/fastapi-xroad-soap/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = "^2.7.0"
-pydantic-xml = "^2.9.1"
+pydantic = "^2.7.1"
+pydantic-xml = "^2.11.0"
 fastapi = "^0.110.0"
-lxml = "^5.2.1"
+lxml = "^5.2.2"
 chardet = "^5.2.0"
 inflection = "^0.5.1"
 charset-normalizer = "^3.3.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-coverage = "^7.4.4"
+coverage = "^7.5.1"
 uvicorn = "^0.29.0"
-pyright = "^1.1.359"
-pytest = "^8.1.1"
+pyright = "^1.1.362"
+pytest = "^8.2.0"
 pytest-cov = "^5.0.0"
 pytest-asyncio = "^0.23.6"
 pytest-pyright = "^0.0.6"
 devtools-cli = "^0.13.3"
 types-lxml = "^2024.4.14"
 httpx = "^0.27.0"
```

### Comparing `fastapi_xroad_soap-0.4.4/PKG-INFO` & `fastapi_xroad_soap-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-xroad-soap
-Version: 0.4.4
+Version: 0.4.5
 Summary: FastAPI Extension for X-Road SOAP
 License: EUPL-1.2
 Keywords: fastapi,xroad,soap
 Author: Zero Reports Team
 Author-email: zero.dev@rik.ee
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -26,17 +26,17 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: charset-normalizer (>=3.3.2,<4.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
-Requires-Dist: lxml (>=5.2.1,<6.0.0)
-Requires-Dist: pydantic (>=2.7.0,<3.0.0)
-Requires-Dist: pydantic-xml (>=2.9.1,<3.0.0)
+Requires-Dist: lxml (>=5.2.2,<6.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
+Requires-Dist: pydantic-xml (>=2.11.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/rik-ee/fastapi-xroad-soap/issues
 Project-URL: Documentation, https://github.com/rik-ee/fastapi-xroad-soap/wiki
 Project-URL: Repository, https://github.com/rik-ee/fastapi-xroad-soap
 Description-Content-Type: text/markdown
 
 # FastAPI X-Road SOAP
```

