# Comparing `tmp/bacpypes3-0.0.93.tar.gz` & `tmp/bacpypes3-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacpypes3-0.0.93.tar", last modified: Mon Apr 15 02:45:34 2024, max compression
+gzip compressed data, was "bacpypes3-0.0.94.tar", last modified: Mon May 13 04:40:55 2024, max compression
```

## Comparing `bacpypes3-0.0.93.tar` & `bacpypes3-0.0.94.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.281255 bacpypes3-0.0.93/
--rw-r--r--   0 joel      (1000) joel      (1000)      666 2024-04-15 02:45:34.281255 bacpypes3-0.0.93/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)      346 2023-03-09 18:20:30.000000 bacpypes3-0.0.93/README.md
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.265254 bacpypes3-0.0.93/bacpypes3/
--rw-rw-r--   0 joel      (1000) joel      (1000)     1391 2024-04-15 02:44:37.000000 bacpypes3-0.0.93/bacpypes3/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    25537 2023-10-23 02:32:34.000000 bacpypes3-0.0.93/bacpypes3/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    56670 2023-10-23 02:32:34.000000 bacpypes3-0.0.93/bacpypes3/apdu.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    34748 2024-03-21 12:00:37.000000 bacpypes3-0.0.93/bacpypes3/app.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    65965 2023-10-31 15:46:12.000000 bacpypes3-0.0.93/bacpypes3/appservice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    21688 2024-03-31 21:04:35.000000 bacpypes3-0.0.93/bacpypes3/argparse.py
--rw-rw-r--   0 joel      (1000) joel      (1000)   103597 2024-03-31 21:04:35.000000 bacpypes3-0.0.93/bacpypes3/basetypes.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16296 2023-10-14 01:56:06.000000 bacpypes3-0.0.93/bacpypes3/cmd.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     7934 2022-11-21 19:40:26.000000 bacpypes3-0.0.93/bacpypes3/comm.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     7128 2023-01-24 05:27:28.000000 bacpypes3-0.0.93/bacpypes3/console.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    64628 2023-10-23 02:32:34.000000 bacpypes3-0.0.93/bacpypes3/constructeddata.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10659 2023-06-29 13:02:40.000000 bacpypes3-0.0.93/bacpypes3/debugging.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     9685 2023-02-08 13:29:16.000000 bacpypes3-0.0.93/bacpypes3/errors.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.269254 bacpypes3-0.0.93/bacpypes3/ipv4/
--rw-rw-r--   0 joel      (1000) joel      (1000)     9911 2024-01-20 06:39:19.000000 bacpypes3-0.0.93/bacpypes3/ipv4/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8238 2023-04-22 03:23:44.000000 bacpypes3-0.0.93/bacpypes3/ipv4/app.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    25882 2023-04-21 19:42:07.000000 bacpypes3-0.0.93/bacpypes3/ipv4/bvll.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4119 2023-02-12 01:55:32.000000 bacpypes3-0.0.93/bacpypes3/ipv4/link.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    61699 2023-04-21 19:25:10.000000 bacpypes3-0.0.93/bacpypes3/ipv4/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.269254 bacpypes3-0.0.93/bacpypes3/ipv6/
--rw-rw-r--   0 joel      (1000) joel      (1000)     6919 2024-01-20 06:39:19.000000 bacpypes3-0.0.93/bacpypes3/ipv6/__init__.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    32041 2023-01-24 14:48:16.000000 bacpypes3-0.0.93/bacpypes3/ipv6/bvll.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    57488 2023-02-01 12:39:44.000000 bacpypes3-0.0.93/bacpypes3/ipv6/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.269254 bacpypes3-0.0.93/bacpypes3/json/
--rw-rw-r--   0 joel      (1000) joel      (1000)      102 2023-01-24 13:54:53.000000 bacpypes3-0.0.93/bacpypes3/json/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      132 2022-09-06 15:15:46.000000 bacpypes3-0.0.93/bacpypes3/json/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16743 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/bacpypes3/json/util.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.269254 bacpypes3-0.0.93/bacpypes3/lib/
--rw-rw-r--   0 joel      (1000) joel      (1000)       41 2023-01-24 05:27:28.000000 bacpypes3-0.0.93/bacpypes3/lib/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    15883 2023-11-13 00:20:14.000000 bacpypes3-0.0.93/bacpypes3/lib/batchread.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.273254 bacpypes3-0.0.93/bacpypes3/local/
--rw-rw-r--   0 joel      (1000) joel      (1000)      463 2023-10-23 02:32:34.000000 bacpypes3-0.0.93/bacpypes3/local/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5836 2024-03-21 05:28:34.000000 bacpypes3-0.0.93/bacpypes3/local/analog.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4696 2024-03-21 05:28:34.000000 bacpypes3-0.0.93/bacpypes3/local/binary.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     6059 2023-06-20 12:14:17.000000 bacpypes3-0.0.93/bacpypes3/local/cmd.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18826 2023-06-20 12:14:17.000000 bacpypes3-0.0.93/bacpypes3/local/cov.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5769 2023-01-24 13:31:42.000000 bacpypes3-0.0.93/bacpypes3/local/device.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    89092 2024-03-31 21:04:35.000000 bacpypes3-0.0.93/bacpypes3/local/event.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    14523 2023-06-21 18:50:45.000000 bacpypes3-0.0.93/bacpypes3/local/fault.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1998 2024-03-21 05:28:34.000000 bacpypes3-0.0.93/bacpypes3/local/multistate.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5022 2023-07-01 17:57:36.000000 bacpypes3-0.0.93/bacpypes3/local/networkport.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    23309 2023-06-21 18:50:45.000000 bacpypes3-0.0.93/bacpypes3/local/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1046 2023-01-03 14:48:04.000000 bacpypes3-0.0.93/bacpypes3/local/oos.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    24849 2023-10-23 02:32:34.000000 bacpypes3-0.0.93/bacpypes3/local/schedule.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    82059 2024-03-31 21:04:35.000000 bacpypes3-0.0.93/bacpypes3/netservice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    28240 2023-01-24 05:27:28.000000 bacpypes3-0.0.93/bacpypes3/npdu.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    91152 2024-03-21 05:28:34.000000 bacpypes3-0.0.93/bacpypes3/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    66217 2024-03-31 21:04:35.000000 bacpypes3-0.0.93/bacpypes3/pdu.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    93478 2024-04-15 02:44:37.000000 bacpypes3-0.0.93/bacpypes3/primitivedata.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.273254 bacpypes3-0.0.93/bacpypes3/rdf/
--rw-rw-r--   0 joel      (1000) joel      (1000)      353 2023-01-24 13:54:37.000000 bacpypes3-0.0.93/bacpypes3/rdf/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      130 2022-08-22 23:43:00.000000 bacpypes3-0.0.93/bacpypes3/rdf/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10764 2024-04-02 15:17:43.000000 bacpypes3-0.0.93/bacpypes3/rdf/core.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    19634 2023-12-11 01:30:51.000000 bacpypes3-0.0.93/bacpypes3/rdf/util.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.273254 bacpypes3-0.0.93/bacpypes3/sc/
--rw-rw-r--   0 joel      (1000) joel      (1000)       65 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/bacpypes3/sc/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    33859 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/bacpypes3/sc/bvll.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18081 2023-02-27 03:52:18.000000 bacpypes3-0.0.93/bacpypes3/sc/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.273254 bacpypes3-0.0.93/bacpypes3/service/
--rw-rw-r--   0 joel      (1000) joel      (1000)       78 2023-01-24 13:55:00.000000 bacpypes3-0.0.93/bacpypes3/service/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    22864 2023-10-31 15:28:33.000000 bacpypes3-0.0.93/bacpypes3/service/cov.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    23249 2023-09-15 04:35:23.000000 bacpypes3-0.0.93/bacpypes3/service/device.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    40398 2024-03-21 12:00:37.000000 bacpypes3-0.0.93/bacpypes3/service/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3869 2023-05-31 11:51:39.000000 bacpypes3-0.0.93/bacpypes3/settings.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3854 2023-10-23 02:32:34.000000 bacpypes3-0.0.93/bacpypes3/vendor.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.273254 bacpypes3-0.0.93/bacpypes3/vlan/
--rw-rw-r--   0 joel      (1000) joel      (1000)    11838 2023-07-01 17:57:36.000000 bacpypes3-0.0.93/bacpypes3/vlan/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1692 2023-07-01 17:57:36.000000 bacpypes3-0.0.93/bacpypes3/vlan/link.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.281255 bacpypes3-0.0.93/bacpypes3.egg-info/
--rw-r--r--   0 joel      (1000) joel      (1000)      666 2024-04-15 02:45:34.000000 bacpypes3-0.0.93/bacpypes3.egg-info/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)     3099 2024-04-15 02:45:34.000000 bacpypes3-0.0.93/bacpypes3.egg-info/SOURCES.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2024-04-15 02:45:34.000000 bacpypes3-0.0.93/bacpypes3.egg-info/dependency_links.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2021-06-28 12:41:48.000000 bacpypes3-0.0.93/bacpypes3.egg-info/not-zip-safe
--rw-rw-r--   0 joel      (1000) joel      (1000)       16 2024-04-15 02:45:34.000000 bacpypes3-0.0.93/bacpypes3.egg-info/top_level.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)      101 2023-10-23 02:32:34.000000 bacpypes3-0.0.93/pyproject.toml
--rw-rw-r--   0 joel      (1000) joel      (1000)       38 2024-04-15 02:45:34.281255 bacpypes3-0.0.93/setup.cfg
--rw-rw-r--   0 joel      (1000) joel      (1000)     1219 2023-05-04 14:51:12.000000 bacpypes3-0.0.93/setup.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.273254 bacpypes3-0.0.93/tests/
--rw-rw-r--   0 joel      (1000) joel      (1000)      351 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2298 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/clocked_test.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      372 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/conftest.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    49924 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/state_machine.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      644 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_1.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3054 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test__template.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.277254 bacpypes3-0.0.93/tests/test_constructed_data/
--rw-rw-r--   0 joel      (1000) joel      (1000)      247 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_constructed_data/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2616 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_constructed_data/test_any.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2526 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_constructed_data/test_array.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2894 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_constructed_data/test_choice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2071 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_constructed_data/test_list.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4013 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_constructed_data/test_read_property_multiple.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10217 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_constructed_data/test_sequence.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8422 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_constructed_data/test_sequence_of.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.277254 bacpypes3-0.0.93/tests/test_pdu/
--rw-rw-r--   0 joel      (1000) joel      (1000)      126 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_pdu/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16956 2024-03-31 21:04:35.000000 bacpypes3-0.0.93/tests/test_pdu/test_address.py
--rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_pdu/test_pci.py
--rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_pdu/test_pdu.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.281255 bacpypes3-0.0.93/tests/test_primitive_data/
--rw-rw-r--   0 joel      (1000) joel      (1000)      456 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_primitive_data/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3309 2023-01-09 14:29:42.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_bit_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2629 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_boolean.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3204 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_character_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3406 2024-04-15 02:44:37.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_date.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2794 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_double.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3266 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_enumerated.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2632 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_integer.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2363 2022-10-03 15:42:31.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_null.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3739 2021-07-22 21:59:33.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_object_identifier.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2775 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_octet_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2785 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_real.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4262 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_tag.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2546 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_time.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3588 2021-06-28 12:37:49.000000 bacpypes3-0.0.93/tests/test_primitive_data/test_unsigned.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.281255 bacpypes3-0.0.93/tests/test_utilities/
--rw-rw-r--   0 joel      (1000) joel      (1000)      130 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_utilities/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18594 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_utilities/test_state_machine.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-04-15 02:45:34.281255 bacpypes3-0.0.93/tests/test_vlan/
--rw-rw-r--   0 joel      (1000) joel      (1000)      200 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_vlan/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8287 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_vlan/test_ipv4_network.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     6304 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_vlan/test_ipv4_router.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8904 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/test_vlan/test_network.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    12098 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/trapped_classes.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1397 2023-01-26 13:59:48.000000 bacpypes3-0.0.93/tests/utilities.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.627399 bacpypes3-0.0.94/
+-rw-r--r--   0 joel      (1000) joel      (1000)      666 2024-05-13 04:40:55.627399 bacpypes3-0.0.94/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)      346 2023-03-09 18:20:30.000000 bacpypes3-0.0.94/README.md
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.615399 bacpypes3-0.0.94/bacpypes3/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1391 2024-04-22 04:44:28.000000 bacpypes3-0.0.94/bacpypes3/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    25537 2023-10-23 02:32:34.000000 bacpypes3-0.0.94/bacpypes3/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    56670 2023-10-23 02:32:34.000000 bacpypes3-0.0.94/bacpypes3/apdu.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    34748 2024-03-21 12:00:37.000000 bacpypes3-0.0.94/bacpypes3/app.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    65965 2023-10-31 15:46:12.000000 bacpypes3-0.0.94/bacpypes3/appservice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    21688 2024-03-31 21:04:35.000000 bacpypes3-0.0.94/bacpypes3/argparse.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)   105875 2024-04-22 04:44:28.000000 bacpypes3-0.0.94/bacpypes3/basetypes.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16296 2023-10-14 01:56:06.000000 bacpypes3-0.0.94/bacpypes3/cmd.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     7934 2022-11-21 19:40:26.000000 bacpypes3-0.0.94/bacpypes3/comm.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     7128 2023-01-24 05:27:28.000000 bacpypes3-0.0.94/bacpypes3/console.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    64628 2023-10-23 02:32:34.000000 bacpypes3-0.0.94/bacpypes3/constructeddata.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10659 2023-06-29 13:02:40.000000 bacpypes3-0.0.94/bacpypes3/debugging.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     9685 2023-02-08 13:29:16.000000 bacpypes3-0.0.94/bacpypes3/errors.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.619399 bacpypes3-0.0.94/bacpypes3/ipv4/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     9911 2024-01-20 06:39:19.000000 bacpypes3-0.0.94/bacpypes3/ipv4/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8238 2023-04-22 03:23:44.000000 bacpypes3-0.0.94/bacpypes3/ipv4/app.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    25882 2023-04-21 19:42:07.000000 bacpypes3-0.0.94/bacpypes3/ipv4/bvll.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4119 2023-02-12 01:55:32.000000 bacpypes3-0.0.94/bacpypes3/ipv4/link.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    61699 2023-04-21 19:25:10.000000 bacpypes3-0.0.94/bacpypes3/ipv4/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.619399 bacpypes3-0.0.94/bacpypes3/ipv6/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6919 2024-01-20 06:39:19.000000 bacpypes3-0.0.94/bacpypes3/ipv6/__init__.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    32041 2023-01-24 14:48:16.000000 bacpypes3-0.0.94/bacpypes3/ipv6/bvll.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    57488 2023-02-01 12:39:44.000000 bacpypes3-0.0.94/bacpypes3/ipv6/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.619399 bacpypes3-0.0.94/bacpypes3/json/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      102 2023-01-24 13:54:53.000000 bacpypes3-0.0.94/bacpypes3/json/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      132 2022-09-06 15:15:46.000000 bacpypes3-0.0.94/bacpypes3/json/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16743 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/bacpypes3/json/util.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.619399 bacpypes3-0.0.94/bacpypes3/lib/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       41 2023-01-24 05:27:28.000000 bacpypes3-0.0.94/bacpypes3/lib/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    15883 2023-11-13 00:20:14.000000 bacpypes3-0.0.94/bacpypes3/lib/batchread.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.619399 bacpypes3-0.0.94/bacpypes3/local/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      463 2023-10-23 02:32:34.000000 bacpypes3-0.0.94/bacpypes3/local/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5836 2024-03-21 05:28:34.000000 bacpypes3-0.0.94/bacpypes3/local/analog.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4696 2024-03-21 05:28:34.000000 bacpypes3-0.0.94/bacpypes3/local/binary.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6059 2023-06-20 12:14:17.000000 bacpypes3-0.0.94/bacpypes3/local/cmd.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18826 2023-06-20 12:14:17.000000 bacpypes3-0.0.94/bacpypes3/local/cov.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5769 2023-01-24 13:31:42.000000 bacpypes3-0.0.94/bacpypes3/local/device.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    89092 2024-03-31 21:04:35.000000 bacpypes3-0.0.94/bacpypes3/local/event.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    14523 2023-06-21 18:50:45.000000 bacpypes3-0.0.94/bacpypes3/local/fault.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1998 2024-03-21 05:28:34.000000 bacpypes3-0.0.94/bacpypes3/local/multistate.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5022 2023-07-01 17:57:36.000000 bacpypes3-0.0.94/bacpypes3/local/networkport.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    23309 2023-06-21 18:50:45.000000 bacpypes3-0.0.94/bacpypes3/local/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1046 2023-01-03 14:48:04.000000 bacpypes3-0.0.94/bacpypes3/local/oos.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    24849 2023-10-23 02:32:34.000000 bacpypes3-0.0.94/bacpypes3/local/schedule.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    82059 2024-03-31 21:04:35.000000 bacpypes3-0.0.94/bacpypes3/netservice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    28240 2023-01-24 05:27:28.000000 bacpypes3-0.0.94/bacpypes3/npdu.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    91152 2024-03-21 05:28:34.000000 bacpypes3-0.0.94/bacpypes3/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    66217 2024-03-31 21:04:35.000000 bacpypes3-0.0.94/bacpypes3/pdu.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    95071 2024-04-22 04:44:28.000000 bacpypes3-0.0.94/bacpypes3/primitivedata.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.623399 bacpypes3-0.0.94/bacpypes3/rdf/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      353 2023-01-24 13:54:37.000000 bacpypes3-0.0.94/bacpypes3/rdf/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      130 2022-08-22 23:43:00.000000 bacpypes3-0.0.94/bacpypes3/rdf/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10764 2024-04-02 15:17:43.000000 bacpypes3-0.0.94/bacpypes3/rdf/core.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    19657 2024-04-22 04:44:28.000000 bacpypes3-0.0.94/bacpypes3/rdf/util.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.623399 bacpypes3-0.0.94/bacpypes3/sc/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       65 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/bacpypes3/sc/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    33859 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/bacpypes3/sc/bvll.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18081 2023-02-27 03:52:18.000000 bacpypes3-0.0.94/bacpypes3/sc/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.623399 bacpypes3-0.0.94/bacpypes3/service/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       78 2023-01-24 13:55:00.000000 bacpypes3-0.0.94/bacpypes3/service/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    22864 2023-10-31 15:28:33.000000 bacpypes3-0.0.94/bacpypes3/service/cov.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    23249 2023-09-15 04:35:23.000000 bacpypes3-0.0.94/bacpypes3/service/device.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    40398 2024-03-21 12:00:37.000000 bacpypes3-0.0.94/bacpypes3/service/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3869 2023-05-31 11:51:39.000000 bacpypes3-0.0.94/bacpypes3/settings.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3854 2023-10-23 02:32:34.000000 bacpypes3-0.0.94/bacpypes3/vendor.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.623399 bacpypes3-0.0.94/bacpypes3/vlan/
+-rw-rw-r--   0 joel      (1000) joel      (1000)    11838 2023-07-01 17:57:36.000000 bacpypes3-0.0.94/bacpypes3/vlan/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1692 2023-07-01 17:57:36.000000 bacpypes3-0.0.94/bacpypes3/vlan/link.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.627399 bacpypes3-0.0.94/bacpypes3.egg-info/
+-rw-r--r--   0 joel      (1000) joel      (1000)      666 2024-05-13 04:40:55.000000 bacpypes3-0.0.94/bacpypes3.egg-info/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3099 2024-05-13 04:40:55.000000 bacpypes3-0.0.94/bacpypes3.egg-info/SOURCES.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2024-05-13 04:40:55.000000 bacpypes3-0.0.94/bacpypes3.egg-info/dependency_links.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2021-06-28 12:41:48.000000 bacpypes3-0.0.94/bacpypes3.egg-info/not-zip-safe
+-rw-rw-r--   0 joel      (1000) joel      (1000)       16 2024-05-13 04:40:55.000000 bacpypes3-0.0.94/bacpypes3.egg-info/top_level.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)      101 2023-10-23 02:32:34.000000 bacpypes3-0.0.94/pyproject.toml
+-rw-rw-r--   0 joel      (1000) joel      (1000)       38 2024-05-13 04:40:55.627399 bacpypes3-0.0.94/setup.cfg
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1219 2023-05-04 14:51:12.000000 bacpypes3-0.0.94/setup.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.623399 bacpypes3-0.0.94/tests/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      351 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2298 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/clocked_test.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      372 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/conftest.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    49924 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/state_machine.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      644 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_1.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3054 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test__template.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.623399 bacpypes3-0.0.94/tests/test_constructed_data/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      247 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_constructed_data/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2616 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_constructed_data/test_any.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2526 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_constructed_data/test_array.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2894 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_constructed_data/test_choice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2071 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_constructed_data/test_list.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4013 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_constructed_data/test_read_property_multiple.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10217 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_constructed_data/test_sequence.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8422 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_constructed_data/test_sequence_of.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.627399 bacpypes3-0.0.94/tests/test_pdu/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      126 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_pdu/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16956 2024-03-31 21:04:35.000000 bacpypes3-0.0.94/tests/test_pdu/test_address.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_pdu/test_pci.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_pdu/test_pdu.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.627399 bacpypes3-0.0.94/tests/test_primitive_data/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      456 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_primitive_data/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3309 2023-01-09 14:29:42.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_bit_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2629 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_boolean.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3204 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_character_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4503 2024-04-22 04:44:28.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_date.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2794 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_double.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3266 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_enumerated.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2632 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_integer.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2363 2022-10-03 15:42:31.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_null.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3739 2021-07-22 21:59:33.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_object_identifier.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2775 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_octet_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2785 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_real.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4262 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_tag.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3648 2024-04-22 04:44:28.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_time.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3588 2021-06-28 12:37:49.000000 bacpypes3-0.0.94/tests/test_primitive_data/test_unsigned.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.627399 bacpypes3-0.0.94/tests/test_utilities/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      130 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_utilities/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18594 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_utilities/test_state_machine.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-13 04:40:55.627399 bacpypes3-0.0.94/tests/test_vlan/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      200 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_vlan/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8287 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_vlan/test_ipv4_network.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6304 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_vlan/test_ipv4_router.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8904 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/test_vlan/test_network.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    12098 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/trapped_classes.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1397 2023-01-26 13:59:48.000000 bacpypes3-0.0.94/tests/utilities.py
```

### Comparing `bacpypes3-0.0.93/PKG-INFO` & `bacpypes3-0.0.94/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacpypes3
-Version: 0.0.93
+Version: 0.0.94
 Summary: BACnet Communications Library
 Home-page: https://github.com/JoelBender/bacpypes3
 Author: Joel Bender
 Author-email: joel@carrickbender.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bacpypes3-0.0.93/bacpypes3/__init__.py` & `bacpypes3-0.0.94/bacpypes3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 if _sys.platform not in _supported_platforms:
     _warnings.warn("unsupported platform", RuntimeWarning)
 
 #
 #   Project Metadata
 #
 
-__version__ = "0.0.93"
+__version__ = "0.0.94"
 __author__ = "Joel Bender"
 __email__ = "joel@carrickbender.com"
 
 #
 #   Settings and Debugging
 #
```

### Comparing `bacpypes3-0.0.93/bacpypes3/__main__.py` & `bacpypes3-0.0.94/bacpypes3/__main__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/apdu.py` & `bacpypes3-0.0.94/bacpypes3/apdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/app.py` & `bacpypes3-0.0.94/bacpypes3/app.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/appservice.py` & `bacpypes3-0.0.94/bacpypes3/appservice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/argparse.py` & `bacpypes3-0.0.94/bacpypes3/argparse.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/basetypes.py` & `bacpypes3-0.0.94/bacpypes3/basetypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # mypy: ignore-errors
 
 from __future__ import annotations
 
 import re
 import struct
 import time
+import datetime
 
 from typing import (
     Union,
     cast,
     Any as _Any,
     Optional,
     Union,
@@ -1841,25 +1842,103 @@
 
 
 class DateTime(Sequence):
     _order = ("date", "time")
     date = Date
     time = Time
 
+    def __init__(
+        self,
+        arg: Optional[datetime.datetime] = None,
+        **kwargs,
+    ) -> None:
+        if arg is None:
+            pass
+        elif isinstance(arg, DateTime):
+            kwargs["date"] = arg.date
+            kwargs["time"] = arg.time
+        elif isinstance(arg, datetime.datetime):
+            date_value = (
+                arg.year - 1900,
+                arg.month,
+                arg.day,
+                arg.weekday() + 1,
+            )
+            time_value = (
+                arg.hour,
+                arg.minute,
+                arg.second,
+                arg.microsecond // 10000,
+            )
+
+            kwargs["date"] = date_value
+            kwargs["time"] = time_value
+
+        super().__init__(**kwargs)
+
     @classmethod
     def now(cls: type, when: Optional[float] = None) -> DateTime:
         """
         Return the current date and time.
         """
         if when is None:
             when = time.time()
 
         # return an instance
         return cast(DateTime, cls(date=Date.now(when), time=Time.now(when)))
 
+    @property
+    def is_special(self) -> bool:
+        return self.date.is_special or self.time.is_special
+
+    @property
+    def datetime(self) -> datetime.datetime:
+        """Return the value as a datetime.datetime object."""
+        if self.is_special:
+            raise ValueError("datetime contains special values")
+
+        year, month, day, day_of_week = self.date
+        hour, minute, second, hundredth = self.time
+        return datetime.datetime(
+            year + 1900, month, day, hour, minute, second, hundredth * 10000
+        )
+
+    def isoformat(self) -> str:
+        return self.datetime.isoformat()
+
+    @classmethod
+    def fromisoformat(cls: type, datetime_string: str) -> Date:
+        datetime_value = datetime.datetime.fromisoformat(datetime_string)
+
+        date_value = (
+            datetime_value.year - 1900,
+            datetime_value.month,
+            datetime_value.day,
+            datetime_value.weekday() + 1,
+        )
+        time_value = (
+            datetime_value.hour,
+            datetime_value.minute,
+            datetime_value.second,
+            datetime_value.microsecond // 10000,
+        )
+
+        # return an instance
+        return cast(Date, cls(date=date_value, time=time_value))
+
+    @classmethod
+    def cast(cls, arg):
+        if _debug:
+            HostAddress._debug("DeviceAddress.cast %r", arg)
+
+        if isinstance(arg, (DateTime, datetime.datetime)):
+            return arg
+        else:
+            raise TypeError(type(arg))
+
     def __str__(self) -> str:
         return f"{self.date} {self.time}"
 
 
 class TimeValue(Sequence):
     _order = ("time", "value")
     time = Time()
```

### Comparing `bacpypes3-0.0.93/bacpypes3/cmd.py` & `bacpypes3-0.0.94/bacpypes3/cmd.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/comm.py` & `bacpypes3-0.0.94/bacpypes3/comm.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/console.py` & `bacpypes3-0.0.94/bacpypes3/console.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/constructeddata.py` & `bacpypes3-0.0.94/bacpypes3/constructeddata.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/debugging.py` & `bacpypes3-0.0.94/bacpypes3/debugging.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/errors.py` & `bacpypes3-0.0.94/bacpypes3/errors.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/ipv4/__init__.py` & `bacpypes3-0.0.94/bacpypes3/ipv4/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/ipv4/app.py` & `bacpypes3-0.0.94/bacpypes3/ipv4/app.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/ipv4/bvll.py` & `bacpypes3-0.0.94/bacpypes3/ipv4/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/ipv4/link.py` & `bacpypes3-0.0.94/bacpypes3/ipv4/link.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/ipv4/service.py` & `bacpypes3-0.0.94/bacpypes3/ipv4/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/ipv6/__init__.py` & `bacpypes3-0.0.94/bacpypes3/ipv6/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/ipv6/bvll.py` & `bacpypes3-0.0.94/bacpypes3/ipv6/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/ipv6/service.py` & `bacpypes3-0.0.94/bacpypes3/ipv6/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/json/util.py` & `bacpypes3-0.0.94/bacpypes3/json/util.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/lib/batchread.py` & `bacpypes3-0.0.94/bacpypes3/lib/batchread.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/local/analog.py` & `bacpypes3-0.0.94/bacpypes3/local/analog.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/local/binary.py` & `bacpypes3-0.0.94/bacpypes3/local/binary.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/local/cmd.py` & `bacpypes3-0.0.94/bacpypes3/local/cmd.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/local/cov.py` & `bacpypes3-0.0.94/bacpypes3/local/cov.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/local/device.py` & `bacpypes3-0.0.94/bacpypes3/local/device.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/local/event.py` & `bacpypes3-0.0.94/bacpypes3/local/event.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/local/fault.py` & `bacpypes3-0.0.94/bacpypes3/local/fault.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/local/multistate.py` & `bacpypes3-0.0.94/bacpypes3/local/multistate.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/local/networkport.py` & `bacpypes3-0.0.94/bacpypes3/local/networkport.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/local/object.py` & `bacpypes3-0.0.94/bacpypes3/local/object.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/local/oos.py` & `bacpypes3-0.0.94/bacpypes3/local/oos.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/local/schedule.py` & `bacpypes3-0.0.94/bacpypes3/local/schedule.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/netservice.py` & `bacpypes3-0.0.94/bacpypes3/netservice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/npdu.py` & `bacpypes3-0.0.94/bacpypes3/npdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/object.py` & `bacpypes3-0.0.94/bacpypes3/object.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/pdu.py` & `bacpypes3-0.0.94/bacpypes3/pdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/primitivedata.py` & `bacpypes3-0.0.94/bacpypes3/primitivedata.py`

 * *Files 4% similar despite different names*

```diff
@@ -2139,15 +2139,17 @@
                 if not day_of_week:
                     day_of_week = 255
             elif day in _special_day_inv:
                 if not day_of_week:
                     day_of_week = 255
             elif not day_of_week:
                 try:
-                    day_of_week = datetime.datetime(year + 1900, month, day).weekday() + 1
+                    day_of_week = (
+                        datetime.datetime(year + 1900, month, day).weekday() + 1
+                    )
                 except OverflowError:
                     pass
 
             # save the value
             arg = (year, month, day, day_of_week)
 
         else:
@@ -2179,14 +2181,42 @@
         return (
             (year == 255)
             or (month in _special_mon_inv)
             or (day in _special_day_inv)
             or (day_of_week == 255)
         )
 
+    @property
+    def date(self) -> datetime.date:
+        """Return the value as a datetime.date object."""
+        if self.is_special:
+            raise ValueError("date contains special values")
+
+        # rip it apart
+        year, month, day, day_of_week = self
+
+        return datetime.date(year + 1900, month, day)
+
+    def isoformat(self) -> str:
+        return self.date.isoformat()
+
+    @classmethod
+    def fromisoformat(cls: type, date_string: str) -> Date:
+        date_value = datetime.date.fromisoformat(date_string)
+
+        value = (
+            date_value.year - 1900,
+            date_value.month,
+            date_value.day,
+            date_value.weekday() + 1,
+        )
+
+        # return an instance
+        return cast(Date, cls(value))
+
     def __str__(self) -> str:
         """String representation of the date."""
         # rip it apart
         year, month, day, day_of_week = self
 
         if year == 255:
             year = "*"
@@ -2334,14 +2364,41 @@
     def is_special(self) -> bool:
         """Date has wildcard values."""
         # rip it apart
         hour, minute, second, hundredth = self
 
         return (hour == 255) or (minute == 255) or (second == 255) or (hundredth == 255)
 
+    @property
+    def time(self) -> datetime.time:
+        """Return the value as a datetime.time object."""
+        if self.is_special:
+            raise ValueError("time contains special values")
+        # rip it apart
+        hour, minute, second, hundredth = self
+
+        return datetime.time(hour, minute, second, hundredth * 10000)
+
+    def isoformat(self) -> str:
+        return self.time.isoformat()
+
+    @classmethod
+    def fromisoformat(cls: type, time_string: str) -> Time:
+        time_value = datetime.time.fromisoformat(time_string)
+
+        value = (
+            time_value.hour,
+            time_value.minute,
+            time_value.second,
+            time_value.microsecond // 10000,
+        )
+
+        # return an instance
+        return cast(Time, cls(value))
+
     def __str__(self) -> str:
         # rip it apart
         hour, minute, second, hundredth = self
 
         rslt = ""
         if hour == 255:
             rslt += "*:"
```

### Comparing `bacpypes3-0.0.93/bacpypes3/rdf/core.py` & `bacpypes3-0.0.94/bacpypes3/rdf/core.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/rdf/util.py` & `bacpypes3-0.0.94/bacpypes3/rdf/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -282,41 +282,39 @@
         return class_(uri_value[1])
 
     raise NotImplementedError("enumeraeted_decode")
 
 
 def date_encode(graph: Graph, value):
     if value.is_special:
-        return Literal(str(value), datatype=BACnetNS.Date)
+        return Literal(str(value), datatype=BACnetNS.datePattern)
     else:
-        date_string = "{:04d}-{:02d}-{:02d}".format(value[0] + 1900, value[1], value[2])
-        return Literal(date_string, datatype=XSD.date, normalize=False)
+        return Literal(value.date)
 
 
 def date_decode(graph: Graph, value):
     assert isinstance(value, Literal)
-    if value.datatype == BACnetNS.Date:
+    if value.datatype == BACnetNS.datePattern:
         return Date(str(value))
     elif value.datatype == XSD.date:
         return Date(value.value)
     else:
         raise TypeError(value.datatype)
 
 
 def time_encode(graph: Graph, value):
-    time_string = str(value)
     if value.is_special:
-        return Literal(time_string, datatype=BACnetNS.Time)
+        return Literal(str(value), datatype=BACnetNS.timePattern)
     else:
-        return Literal(time_string, datatype=XSD.time, normalize=False)
+        return Literal(value.time)  # normalize=False?
 
 
 def time_decode(graph: Graph, value):
     assert isinstance(value, Literal)
-    if value.datatype == BACnetNS.Time:
+    if value.datatype == BACnetNS.timePattern:
         return Time(str(value))
     elif value.datatype == XSD.time:
         return Time(value.value)
     else:
         raise TypeError(value.datatype)
 
 
@@ -329,14 +327,31 @@
 
 def objectidentifier_decode(graph: Graph, value):
     # alternate (value.datatype == BACnetNS.ObjectIdentifier)
     assert isinstance(value, Literal) and (value.datatype is None)
     return ObjectIdentifier(str(value))
 
 
+def datetime_encode(graph: Graph, value):
+    if value.is_special:
+        return Literal(str(value), datatype=BACnetNS.dateTimePattern)
+    else:
+        return Literal(value.datetime)  # normalize=False?
+
+
+def datetime_decode(graph: Graph, value):
+    assert isinstance(value, Literal)
+    if value.datatype == BACnetNS.dateTimePattern:
+        return DateTime(str(value))
+    elif value.datatype == XSD.dateTime:
+        return DateTime(value.value)
+    else:
+        raise TypeError(value.datatype)
+
+
 #
 #
 #
 
 
 def atomic_encode(graph: Graph, value) -> Literal:
     if isinstance(value, Null):
@@ -361,14 +376,16 @@
         literal = enumerated_encode(graph, value)
     elif isinstance(value, Date):
         literal = date_encode(graph, value)
     elif isinstance(value, Time):
         literal = time_encode(graph, value)
     elif isinstance(value, ObjectIdentifier):
         literal = objectidentifier_encode(graph, value)
+    elif isinstance(value, DateTime):
+        literal = datetime_encode(graph, value)
     else:
         raise TypeError("atomic element expected: " + str(type(value)))
 
     return literal
 
 
 def atomic_decode(graph: Graph, literal, class_) -> Atomic:
@@ -394,14 +411,16 @@
         value = enumerated_decode(graph, literal, class_)
     elif issubclass(class_, Date):
         value = date_decode(graph, literal)
     elif issubclass(class_, Time):
         value = time_decode(graph, literal)
     elif issubclass(class_, ObjectIdentifier):
         value = objectidentifier_decode(graph, literal)
+    elif issubclass(class_, DateTime):
+        value = datetime_decode(graph, literal)
     else:
         raise TypeError("not an atomic element")
 
     return value
 
 
 #
@@ -429,27 +448,26 @@
         if _debug:
             sequence_to_graph._debug(f"    - {attr}, {element}: {value}")
         if value is None:
             continue
 
         if isinstance(value, Atomic):
             literal = atomic_encode(graph, value)
+        elif isinstance(value, DateTime):
+            literal = datetime_encode(graph, value)
         elif isinstance(value, Sequence):
             literal = BNode()
             sequence_to_graph(value, literal, graph)
         elif isinstance(value, ExtendedList):
             extendedlist_to_graph(value, node, attr_to_predicate(attr), graph)
             continue
         elif isinstance(value, (AnyAtomic, AnyAtomicExtended)):
             value = value.get_value()
             if isinstance(value, Atomic):
                 literal = atomic_encode(graph, value)
-            elif isinstance(value, DateTime):
-                literal = BNode()
-                sequence_to_graph(value, literal, graph)
         else:
             raise TypeError(value)
 
         graph.add((node, attr_to_predicate(attr), literal))
 
     return graph
 
@@ -472,33 +490,23 @@
         if _debug:
             Sequence._debug("    - literal: %r", literal)
         if literal is None:
             continue
 
         if issubclass(element, Atomic):
             value = atomic_decode(graph, literal, element)
+        elif issubclass(element, DateTime):
+            value = datetime_decode(graph, literal)
         elif issubclass(element, Sequence):
             value = graph_to_sequence(graph, literal, element)
         elif issubclass(element, ExtendedList):
             value = graph_to_extendedlist(graph, node, attr_to_predicate(attr), element)
         elif issubclass(element, (AnyAtomic, AnyAtomicExtended)):
             if literal == BACnetNS.Null:
                 value = Null(())
-
-            elif isinstance(literal, (BNode, URIRef)):
-                date_literal = graph.value(subject=literal, predicate=BACnetNS["date"])
-                time_literal = graph.value(subject=literal, predicate=BACnetNS["time"])
-                if (date_literal is not None) and (time_literal is not None):
-                    value = DateTime(
-                        date=date_decode(graph, date_literal),
-                        time=time_decode(graph, time_literal),
-                    )
-                else:
-                    raise ValueError("DateTime expected")
-
             elif isinstance(literal, Literal):
                 if literal.datatype == XSD.boolean:
                     value = boolean_decode(graph, literal)
                 elif literal.datatype == XSD.nonNegativeInteger:
                     value = unsigned_decode(graph, literal)
                 elif literal.datatype == XSD.integer:
                     value = integer_decode(graph, literal)
@@ -510,17 +518,17 @@
                     value = octetstring_decode(graph, literal)
                 elif literal.datatype == XSD.hexBinary:
                     value = octetstring_decode(graph, literal)
                 elif literal.datatype is None:
                     value = characterstring_decode(graph, literal)
                 elif literal.datatype == BACnetNS.BitString:
                     value = bitstring_decode(graph, literal)
-                elif literal.datatype in (BACnetNS.Date, XSD.date):
+                elif literal.datatype in (BACnetNS.datePattern, XSD.date):
                     value = date_decode(graph, literal)
-                elif literal.datatype in (BACnetNS.Time, XSD.time):
+                elif literal.datatype in (BACnetNS.timePattern, XSD.time):
                     value = time_decode(graph, literal)
                 elif literal.datatype == BACnetNS.ObjectIdentifier:
                     value = objectidentifier_decode(graph, literal)
                 else:
                     raise ValueError(literal.datatype)
             else:
                 raise ValueError(literal)
```

### Comparing `bacpypes3-0.0.93/bacpypes3/sc/bvll.py` & `bacpypes3-0.0.94/bacpypes3/sc/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/sc/service.py` & `bacpypes3-0.0.94/bacpypes3/sc/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/service/cov.py` & `bacpypes3-0.0.94/bacpypes3/service/cov.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/service/device.py` & `bacpypes3-0.0.94/bacpypes3/service/device.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/service/object.py` & `bacpypes3-0.0.94/bacpypes3/service/object.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/settings.py` & `bacpypes3-0.0.94/bacpypes3/settings.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/vendor.py` & `bacpypes3-0.0.94/bacpypes3/vendor.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/vlan/__init__.py` & `bacpypes3-0.0.94/bacpypes3/vlan/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3/vlan/link.py` & `bacpypes3-0.0.94/bacpypes3/vlan/link.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/bacpypes3.egg-info/PKG-INFO` & `bacpypes3-0.0.94/bacpypes3.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacpypes3
-Version: 0.0.93
+Version: 0.0.94
 Summary: BACnet Communications Library
 Home-page: https://github.com/JoelBender/bacpypes3
 Author: Joel Bender
 Author-email: joel@carrickbender.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bacpypes3-0.0.93/bacpypes3.egg-info/SOURCES.txt` & `bacpypes3-0.0.94/bacpypes3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/setup.py` & `bacpypes3-0.0.94/setup.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/clocked_test.py` & `bacpypes3-0.0.94/tests/clocked_test.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/state_machine.py` & `bacpypes3-0.0.94/tests/state_machine.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_1.py` & `bacpypes3-0.0.94/tests/test_1.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test__template.py` & `bacpypes3-0.0.94/tests/test__template.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_constructed_data/test_any.py` & `bacpypes3-0.0.94/tests/test_constructed_data/test_any.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_constructed_data/test_array.py` & `bacpypes3-0.0.94/tests/test_constructed_data/test_array.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_constructed_data/test_choice.py` & `bacpypes3-0.0.94/tests/test_constructed_data/test_choice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_constructed_data/test_list.py` & `bacpypes3-0.0.94/tests/test_constructed_data/test_list.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_constructed_data/test_read_property_multiple.py` & `bacpypes3-0.0.94/tests/test_constructed_data/test_read_property_multiple.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_constructed_data/test_sequence.py` & `bacpypes3-0.0.94/tests/test_constructed_data/test_sequence.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_constructed_data/test_sequence_of.py` & `bacpypes3-0.0.94/tests/test_constructed_data/test_sequence_of.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_pdu/test_address.py` & `bacpypes3-0.0.94/tests/test_pdu/test_address.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_primitive_data/test_bit_string.py` & `bacpypes3-0.0.94/tests/test_primitive_data/test_bit_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_primitive_data/test_boolean.py` & `bacpypes3-0.0.94/tests/test_primitive_data/test_boolean.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_primitive_data/test_character_string.py` & `bacpypes3-0.0.94/tests/test_primitive_data/test_character_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_primitive_data/test_date.py` & `bacpypes3-0.0.94/tests/test_primitive_data/test_time.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,143 +1,152 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """
-Test Date
+Test Time
 ---------
 """
 
 import unittest
 import pytest
 
 from bacpypes3.debugging import bacpypes_debugging, ModuleLogger, xtob
-from bacpypes3.primitivedata import Tag, TagClass, TagNumber, TagList, Date
+from bacpypes3.primitivedata import Tag, TagClass, TagNumber, TagList, Time
+from bacpypes3.rdf.util import (
+    time_encode as rdf_time_encode,
+    time_decode as rdf_time_decode,
+)
 
 # some debugging
 _debug = 0
 _log = ModuleLogger(globals())
 
 
 @bacpypes_debugging
-def date_tag(x):
+def time_tag(x):
     """Convert a hex string to a real application tag."""
     if _debug:
-        date_tag._debug("date_tag %r", x)
+        time_tag._debug("time_tag %r", x)
 
     b = xtob(x)
-    tag = Tag(TagClass.application, TagNumber.date, len(b), b)
+    tag = Tag(TagClass.application, TagNumber.time, len(b), b)
     if _debug:
-        date_tag._debug("    - tag: %r", tag)
+        time_tag._debug("    - tag: %r", tag)
 
     return tag
 
 
 @bacpypes_debugging
-def date_encode(obj):
-    """Encode a Date object into a tag."""
+def time_encode(obj):
+    """Encode a Time object into a tag."""
     if _debug:
-        date_encode._debug("date_encode %r", obj)
+        time_encode._debug("time_encode %r", obj)
 
     tag = obj.encode()[0]
     if _debug:
-        date_encode._debug("    - tag: %r", tag)
+        time_encode._debug("    - tag: %r", tag)
 
     return tag
 
 
 @bacpypes_debugging
-def date_decode(tag):
-    """Decode a Date from a tag."""
+def time_decode(tag):
+    """Decode a Time from a tag."""
     if _debug:
-        date_decode._debug("date_decode %r", tag)
+        time_decode._debug("time_decode %r", tag)
 
-    obj = Date.decode(TagList([tag]))
+    obj = Time.decode(TagList([tag]))
     if _debug:
-        date_decode._debug("    - obj: %r", obj)
+        time_decode._debug("    - obj: %r", obj)
 
     return obj
 
 
 @bacpypes_debugging
-def date_endec(v, x):
-    """Pass the value to Date, construct a tag from the hex string,
+def time_endec(v, x):
+    """Pass the value to Time, construct a tag from the hex string,
     and compare results of encoding and decoding."""
     if _debug:
-        date_endec._debug("date_endec %r %r", v, x)
+        time_endec._debug("time_endec %r %r", v, x)
 
-    obj = Date(v)
+    obj = Time(v)
     if _debug:
-        date_endec._debug("    - obj: %r", obj)
+        time_endec._debug("    - obj: %r", obj)
 
-    tag = date_tag(x)
+    tag = time_tag(x)
     if _debug:
-        date_endec._debug("    - tag: %r", tag)
+        time_endec._debug("    - tag: %r", tag)
         tag.debug_contents()
 
-    assert date_encode(obj) == tag
-    assert date_decode(tag) == obj
+    assert time_encode(obj) == tag
+    assert time_decode(tag) == obj
 
 
 @bacpypes_debugging
-class TestDate(unittest.TestCase):
-    def test_date_error(self):
+class TestTime(unittest.TestCase):
+    def test_time(self):
         if _debug:
-            TestDate._debug("test_date_error")
+            TestTime._debug("test_time")
+
+        obj = Time((255, 255, 255, 255))
+        assert obj == (255, 255, 255, 255)
 
         with pytest.raises(TypeError):
-            Date(1.5)
+            Time(1.5)
         with pytest.raises(ValueError):
-            Date("some string")
+            Time("some string")
 
-    def test_date_tuple(self):
+    def test_time_tuple(self):
         if _debug:
-            TestDate._debug("test_date_tuple")
+            TestTime._debug("test_time_tuple")
 
-        obj = Date((1, 2, 3, 4))
+        obj = Time((1, 2, 3, 4))
         assert obj == (1, 2, 3, 4)
-        assert str(obj) == "1901-2-3 thu"
+        assert str(obj) == "01:02:03.04"
 
-        obj = Date((2001, 3, 4, 5))
-        assert obj == (101, 3, 4, 5)
-        assert str(obj) == "2001-3-4 fri"
+    def test_time_copy(self):
+        if _debug:
+            TestTime._debug("test_time_copy")
 
-    def test_date_string(self):
+        obj1 = Time((5, 6, 7, 8))
+        obj2 = Time(obj1)
+        assert obj1 == obj2
+
+    def test_time_endec(self):
         if _debug:
-            TestDate._debug("test_date_string")
+            TestTime._debug("test_time_endec")
 
-        # calulate DOW
-        obj = Date("1901-2-3")
-        assert obj == (1, 2, 3, 7)
-        assert str(obj) == "1901-2-3 sun"
+        time_endec((1, 2, 3, 4), "01020304")
 
-        # provide a wrong DOW, but accept it
-        obj = Date("1901-2-3 thu")
-        assert obj == (1, 2, 3, 4)
-        assert str(obj) == "1901-2-3 thu"
+    def test_time_isoformat(self):
+        if _debug:
+            TestTime._debug("test_time_isoformat")
 
-        # specific date, explicit wildcard DOW
-        obj = Date("1901-2-3 *")
-        assert obj == (1, 2, 3, 255)
+        obj1 = Time("01:02:03.04")
+        obj1_string = obj1.isoformat()
+        if _debug:
+            TestTime._debug("    - obj1_string: %r", obj1_string)
 
-        # any day in 1901, implicit wildcard DOW
-        obj = Date("1901-*-*")
-        assert obj == (1, 255, 255, 255)
-        assert str(obj) == "1901-*-* *"
+        obj2 = Time.fromisoformat(obj1_string)
+        assert obj1 == obj2
 
-        # any Monday in 1901
-        obj = Date("1901-*-* mon")
-        assert obj == (1, 255, 255, 1)
-        assert str(obj) == "1901-*-* mon"
+    def test_time_literal(self):
+        if _debug:
+            TestTime._debug("test_time_literal")
 
-    def test_date_copy(self):
+        # specific time
+        obj1 = Time("01:02:03.04")
+        obj1_literal = rdf_time_encode(None, obj1)
         if _debug:
-            TestDate._debug("test_date_copy")
+            TestTime._debug("    - obj1_literal: %r", obj1_literal)
 
-        obj1 = Date((5, 6, 7, 8))
-        obj2 = Date(obj1)
+        obj2 = rdf_time_decode(None, obj1_literal)
         assert obj1 == obj2
 
-    def test_date_endec(self):
+        # time pattern
+        obj3 = Time("01:02:*")
+        obj3_literal = rdf_time_encode(None, obj3)
         if _debug:
-            TestDate._debug("test_date_endec")
+            TestTime._debug("    - obj3_literal: %r", obj3_literal)
 
-        date_endec((1, 2, 3, 4), "01020304")
+        obj4 = rdf_time_decode(None, obj3_literal)
+        assert obj3 == obj4
```

### Comparing `bacpypes3-0.0.93/tests/test_primitive_data/test_double.py` & `bacpypes3-0.0.94/tests/test_primitive_data/test_double.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_primitive_data/test_enumerated.py` & `bacpypes3-0.0.94/tests/test_primitive_data/test_enumerated.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_primitive_data/test_integer.py` & `bacpypes3-0.0.94/tests/test_primitive_data/test_integer.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_primitive_data/test_null.py` & `bacpypes3-0.0.94/tests/test_primitive_data/test_null.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_primitive_data/test_object_identifier.py` & `bacpypes3-0.0.94/tests/test_primitive_data/test_object_identifier.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_primitive_data/test_octet_string.py` & `bacpypes3-0.0.94/tests/test_primitive_data/test_octet_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_primitive_data/test_real.py` & `bacpypes3-0.0.94/tests/test_primitive_data/test_real.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_primitive_data/test_tag.py` & `bacpypes3-0.0.94/tests/test_primitive_data/test_tag.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_primitive_data/test_unsigned.py` & `bacpypes3-0.0.94/tests/test_primitive_data/test_unsigned.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_utilities/test_state_machine.py` & `bacpypes3-0.0.94/tests/test_utilities/test_state_machine.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_vlan/test_ipv4_network.py` & `bacpypes3-0.0.94/tests/test_vlan/test_ipv4_network.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_vlan/test_ipv4_router.py` & `bacpypes3-0.0.94/tests/test_vlan/test_ipv4_router.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/test_vlan/test_network.py` & `bacpypes3-0.0.94/tests/test_vlan/test_network.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/trapped_classes.py` & `bacpypes3-0.0.94/tests/trapped_classes.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.93/tests/utilities.py` & `bacpypes3-0.0.94/tests/utilities.py`

 * *Files identical despite different names*

