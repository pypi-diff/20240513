# Comparing `tmp/scottbrian_utils-3.0.0.tar.gz` & `tmp/scottbrian_utils-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scottbrian_utils-3.0.0.tar", last modified: Sat Dec  2 18:20:19 2023, max compression
+gzip compressed data, was "scottbrian_utils-4.0.0.tar", last modified: Mon May 13 00:36:01 2024, max compression
```

## Comparing `scottbrian_utils-3.0.0.tar` & `scottbrian_utils-4.0.0.tar`

### file list

```diff
@@ -1,101 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.547577 scottbrian_utils-3.0.0/
--rw-rw-rw-   0        0        0     2054 2023-11-24 16:34:06.000000 scottbrian_utils-3.0.0/.gitignore
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.454555 scottbrian_utils-3.0.0/.idea/
--rw-rw-rw-   0        0        0      184 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/.idea/.gitignore
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.455556 scottbrian_utils-3.0.0/.idea/codeStyles/
--rw-rw-rw-   0        0        0      153 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/.idea/codeStyles/codeStyleConfig.xml
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.457556 scottbrian_utils-3.0.0/.idea/dictionaries/
--rw-rw-rw-   0        0        0       86 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/.idea/dictionaries/Tiger.xml
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.458557 scottbrian_utils-3.0.0/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      234 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      426 2023-11-23 15:37:03.000000 scottbrian_utils-3.0.0/.idea/misc.xml
--rw-rw-rw-   0        0        0      291 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/.idea/modules.xml
--rw-rw-rw-   0        0        0      191 2022-01-25 18:21:47.000000 scottbrian_utils-3.0.0/.idea/other.xml
--rw-rw-rw-   0        0        0     1265 2023-11-22 18:32:15.000000 scottbrian_utils-3.0.0/.idea/scottbrian_utils.iml
--rw-rw-rw-   0        0        0      185 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/.idea/vcs.xml
--rw-rw-rw-   0        0        0      636 2022-01-25 18:57:49.000000 scottbrian_utils-3.0.0/.readthedocs.yml
--rw-rw-rw-   0        0        0     1092 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      609 2023-11-24 17:53:09.000000 scottbrian_utils-3.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7088 2023-12-02 18:20:19.546576 scottbrian_utils-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4879 2023-11-26 18:28:54.000000 scottbrian_utils-3.0.0/README.rst
--rw-rw-rw-   0        0        0     4336 2023-11-30 15:47:35.000000 scottbrian_utils-3.0.0/conftest.py
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.459557 scottbrian_utils-3.0.0/docs/
--rw-rw-rw-   0        0        0       50 2022-01-25 18:21:47.000000 scottbrian_utils-3.0.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.482562 scottbrian_utils-3.0.0/docs/source/
--rw-rw-rw-   0        0        0    83406 2023-10-14 18:15:17.000000 scottbrian_utils-3.0.0/docs/source/UniqueTS_UseCase1.svg
--rw-rw-rw-   0        0        0        0 2022-01-14 00:08:20.000000 scottbrian_utils-3.0.0/docs/source/_static
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.485562 scottbrian_utils-3.0.0/docs/source/adjust_sphinx/
--rw-rw-rw-   0        0        0        0 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/docs/source/adjust_sphinx/__init__.py
--rw-rw-rw-   0        0        0     2425 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/docs/source/adjust_sphinx/adjust_sphinx.py
--rw-rw-rw-   0        0        0     2377 2023-11-22 18:11:03.000000 scottbrian_utils-3.0.0/docs/source/conf.py
--rw-rw-rw-   0        0        0       38 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/docs/source/diag_msg_link.rst
--rw-rw-rw-   0        0        0       41 2023-11-22 18:45:05.000000 scottbrian_utils-3.0.0/docs/source/doc_checker_link.rst
--rw-rw-rw-   0        0        0       42 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/docs/source/file_catalog_link.rst
--rw-rw-rw-   0        0        0       40 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/docs/source/flower_box_link.rst
--rw-rw-rw-   0        0        0      781 2023-11-22 18:48:24.000000 scottbrian_utils-3.0.0/docs/source/index.rst
--rw-rw-rw-   0        0        0       42 2022-01-25 18:21:47.000000 scottbrian_utils-3.0.0/docs/source/log_verifier_link.rst
--rw-rw-rw-   0        0        0       34 2022-01-25 18:21:47.000000 scottbrian_utils-3.0.0/docs/source/msgs_link.rst
--rw-rw-rw-   0        0        0       36 2022-02-23 01:02:07.000000 scottbrian_utils-3.0.0/docs/source/pauser_link.rst
--rw-rw-rw-   0        0        0      306 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/docs/source/setup.py
--rw-rw-rw-   0        0        0       40 2022-01-25 18:21:47.000000 scottbrian_utils-3.0.0/docs/source/stop_watch_link.rst
--rw-rw-rw-   0        0        0       38 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/docs/source/time_hdr_link.rst
--rw-rw-rw-   0        0        0       35 2022-01-25 18:21:47.000000 scottbrian_utils-3.0.0/docs/source/timer_link.rst
--rw-rw-rw-   0        0        0       39 2023-10-14 19:36:48.000000 scottbrian_utils-3.0.0/docs/source/unique_ts_link.rst
--rw-rw-rw-   0        0        0      229 2023-11-24 00:01:05.000000 scottbrian_utils-3.0.0/mypy.ini
--rw-rw-rw-   0        0        0     1148 2023-11-25 00:21:35.000000 scottbrian_utils-3.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      846 2023-11-28 15:25:57.000000 scottbrian_utils-3.0.0/pytest.ini
--rw-rw-rw-   0        0        0       42 2023-12-02 18:20:19.548577 scottbrian_utils-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      192 2023-11-22 18:11:03.000000 scottbrian_utils-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.486562 scottbrian_utils-3.0.0/src/
--rw-rw-rw-   0        0        0     5191 2022-01-25 18:21:47.000000 scottbrian_utils-3.0.0/src/conftest.py
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.507567 scottbrian_utils-3.0.0/src/scottbrian_utils/
--rw-rw-rw-   0        0        0      139 2023-11-22 18:11:03.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/__init__.py
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/__init__.pyi
--rw-rw-rw-   0        0        0    12890 2023-11-24 00:13:36.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/diag_msg.py
--rw-rw-rw-   0        0        0     8201 2023-11-30 17:05:18.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/doc_checker.py
--rw-rw-rw-   0        0        0    15198 2023-11-24 00:13:02.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/file_catalog.py
--rw-rw-rw-   0        0        0     1833 2022-01-25 18:21:47.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/flower_box.py
--rw-rw-rw-   0        0        0    22177 2023-11-28 14:37:00.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/log_verifier.py
--rw-rw-rw-   0        0        0     7606 2022-01-25 18:21:47.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/msgs.py
--rw-rw-rw-   0        0        0    20415 2023-11-24 00:11:58.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/pauser.py
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/py.typed
--rw-rw-rw-   0        0        0     6792 2023-01-26 16:36:30.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/stop_watch.py
--rw-rw-rw-   0        0        0    17926 2022-01-25 18:21:47.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/time_hdr.py
--rw-rw-rw-   0        0        0    24423 2023-04-11 22:05:38.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/timer.py
--rw-rw-rw-   0        0        0     2322 2023-10-14 23:15:12.000000 scottbrian_utils-3.0.0/src/scottbrian_utils/unique_ts.py
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.544575 scottbrian_utils-3.0.0/src/scottbrian_utils.egg-info/
--rw-rw-rw-   0        0        0     7088 2023-12-02 18:20:19.000000 scottbrian_utils-3.0.0/src/scottbrian_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2521 2023-12-02 18:20:19.000000 scottbrian_utils-3.0.0/src/scottbrian_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-02 18:20:19.000000 scottbrian_utils-3.0.0/src/scottbrian_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-12-02 18:20:19.000000 scottbrian_utils-3.0.0/src/scottbrian_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-12-02 18:20:19.000000 scottbrian_utils-3.0.0/src/scottbrian_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.427549 scottbrian_utils-3.0.0/tests/
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.533573 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/
--rw-rw-rw-   0        0        0       38 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/__init__.py
--rw-rw-rw-   0        0        0     8171 2023-11-24 21:49:34.000000 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/adjust_diag_msg_tcode.py
--rw-rw-rw-   0        0        0     5469 2023-07-01 17:34:46.000000 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/conftest.py
--rw-rw-rw-   0        0        0   493189 2023-11-24 21:49:35.000000 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_diag_msg.py
--rw-rw-rw-   0        0        0    17147 2023-11-24 00:16:31.000000 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_file_catalog.py
--rw-rw-rw-   0        0        0     7704 2023-07-01 17:34:46.000000 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_flower_box.py
--rw-rw-rw-   0        0        0    59161 2023-11-29 23:52:45.000000 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_log_verifier.py
--rw-rw-rw-   0        0        0    16651 2023-07-01 17:34:46.000000 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_msgs.py
--rw-rw-rw-   0        0        0    36592 2023-11-24 00:15:56.000000 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_pauser.py
--rw-rw-rw-   0        0        0    17642 2023-07-01 17:34:46.000000 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_stop_watch.py
--rw-rw-rw-   0        0        0    73026 2023-11-24 00:15:18.000000 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_time_hdr.py
--rw-rw-rw-   0        0        0    40767 2023-11-23 15:44:47.000000 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_timer.py
--rw-rw-rw-   0        0        0     5972 2023-11-25 00:12:19.000000 scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_unique_ts.py
--rw-rw-rw-   0        0        0     6348 2023-11-29 23:53:35.000000 scottbrian_utils-3.0.0/tox.ini
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.428549 scottbrian_utils-3.0.0/type_stubs/
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.535574 scottbrian_utils-3.0.0/type_stubs/mypywrapt/
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.537574 scottbrian_utils-3.0.0/type_stubs/mypywrapt/adjust_src/
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/type_stubs/mypywrapt/adjust_src/__init__.pyi
--rw-rw-rw-   0        0        0     1292 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/type_stubs/mypywrapt/adjust_src/adjust_src.py
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.429550 scottbrian_utils-3.0.0/type_stubs/mypywrapt/build/
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.429550 scottbrian_utils-3.0.0/type_stubs/mypywrapt/build/lib/
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.540574 scottbrian_utils-3.0.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/__init__.pyi
--rw-rw-rw-   0        0        0      329 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/decorators.pyi
--rw-rw-rw-   0        0        0      388 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/type_stubs/mypywrapt/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-02 18:20:19.543575 scottbrian_utils-3.0.0/type_stubs/mypywrapt/wrapt-stubs/
--rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/type_stubs/mypywrapt/wrapt-stubs/__init__.pyi
--rw-rw-rw-   0        0        0      329 2021-12-29 18:20:23.000000 scottbrian_utils-3.0.0/type_stubs/mypywrapt/wrapt-stubs/decorators.pyi
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.795690 scottbrian_utils-4.0.0/
+-rw-rw-rw-   0        0        0     2054 2023-11-24 16:34:06.000000 scottbrian_utils-4.0.0/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.703669 scottbrian_utils-4.0.0/.idea/
+-rw-rw-rw-   0        0        0      184 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/.idea/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.704670 scottbrian_utils-4.0.0/.idea/codeStyles/
+-rw-rw-rw-   0        0        0      153 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/.idea/codeStyles/codeStyleConfig.xml
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.705670 scottbrian_utils-4.0.0/.idea/dictionaries/
+-rw-rw-rw-   0        0        0       86 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/.idea/dictionaries/Tiger.xml
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.707670 scottbrian_utils-4.0.0/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      234 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      426 2023-11-23 15:37:03.000000 scottbrian_utils-4.0.0/.idea/misc.xml
+-rw-rw-rw-   0        0        0      291 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/.idea/modules.xml
+-rw-rw-rw-   0        0        0      191 2022-01-25 18:21:47.000000 scottbrian_utils-4.0.0/.idea/other.xml
+-rw-rw-rw-   0        0        0     1265 2023-11-22 18:32:15.000000 scottbrian_utils-4.0.0/.idea/scottbrian_utils.iml
+-rw-rw-rw-   0        0        0      185 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/.idea/vcs.xml
+-rw-rw-rw-   0        0        0      701 2023-12-02 22:36:11.000000 scottbrian_utils-4.0.0/.readthedocs.yml
+-rw-rw-rw-   0        0        0     1092 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      609 2023-11-24 17:53:09.000000 scottbrian_utils-4.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7678 2024-05-13 00:36:01.793689 scottbrian_utils-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5392 2024-05-11 18:57:18.000000 scottbrian_utils-4.0.0/README.rst
+-rw-rw-rw-   0        0        0     4338 2024-04-21 18:34:57.000000 scottbrian_utils-4.0.0/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.708670 scottbrian_utils-4.0.0/docs/
+-rw-rw-rw-   0        0        0       57 2023-12-02 22:55:23.000000 scottbrian_utils-4.0.0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.730675 scottbrian_utils-4.0.0/docs/source/
+-rw-rw-rw-   0        0        0    83406 2023-10-14 18:15:17.000000 scottbrian_utils-4.0.0/docs/source/UniqueTS_UseCase1.svg
+-rw-rw-rw-   0        0        0        0 2022-01-14 00:08:20.000000 scottbrian_utils-4.0.0/docs/source/_static
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.733676 scottbrian_utils-4.0.0/docs/source/adjust_sphinx/
+-rw-rw-rw-   0        0        0        0 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/docs/source/adjust_sphinx/__init__.py
+-rw-rw-rw-   0        0        0     2425 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/docs/source/adjust_sphinx/adjust_sphinx.py
+-rw-rw-rw-   0        0        0     2356 2024-04-09 16:58:14.000000 scottbrian_utils-4.0.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0      107 2024-03-31 17:44:01.000000 scottbrian_utils-4.0.0/docs/source/diag_msg_link.rst
+-rw-rw-rw-   0        0        0       41 2024-03-31 01:45:20.000000 scottbrian_utils-4.0.0/docs/source/doc_checker_link.rst
+-rw-rw-rw-   0        0        0       41 2024-04-21 18:48:29.000000 scottbrian_utils-4.0.0/docs/source/entry_trace_link.rst
+-rw-rw-rw-   0        0        0       54 2024-03-31 17:05:54.000000 scottbrian_utils-4.0.0/docs/source/file_catalog_link.rst
+-rw-rw-rw-   0        0        0       40 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/docs/source/flower_box_link.rst
+-rw-rw-rw-   0        0        0      835 2024-04-21 18:48:29.000000 scottbrian_utils-4.0.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0       49 2024-03-31 01:41:28.000000 scottbrian_utils-4.0.0/docs/source/log_verifier_link.rst
+-rw-rw-rw-   0        0        0       39 2024-03-31 01:41:28.000000 scottbrian_utils-4.0.0/docs/source/msgs_link.rst
+-rw-rw-rw-   0        0        0       58 2024-03-31 17:11:13.000000 scottbrian_utils-4.0.0/docs/source/pauser_link.rst
+-rw-rw-rw-   0        0        0      306 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/docs/source/setup.py
+-rw-rw-rw-   0        0        0       50 2024-03-31 17:12:31.000000 scottbrian_utils-4.0.0/docs/source/stop_watch_link.rst
+-rw-rw-rw-   0        0        0       74 2024-03-31 17:15:52.000000 scottbrian_utils-4.0.0/docs/source/time_hdr_link.rst
+-rw-rw-rw-   0        0        0       41 2024-03-31 17:15:52.000000 scottbrian_utils-4.0.0/docs/source/timer_link.rst
+-rw-rw-rw-   0        0        0       48 2024-03-31 17:15:52.000000 scottbrian_utils-4.0.0/docs/source/unique_ts_link.rst
+-rw-rw-rw-   0        0        0      266 2024-04-24 17:55:01.000000 scottbrian_utils-4.0.0/mypy.ini
+-rw-rw-rw-   0        0        0     1207 2024-04-24 15:49:06.000000 scottbrian_utils-4.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      886 2024-04-23 02:16:03.000000 scottbrian_utils-4.0.0/pytest.ini
+-rw-rw-rw-   0        0        0       42 2024-05-13 00:36:01.795690 scottbrian_utils-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      192 2023-11-22 18:11:03.000000 scottbrian_utils-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.734676 scottbrian_utils-4.0.0/src/
+-rw-rw-rw-   0        0        0     5191 2022-01-25 18:21:47.000000 scottbrian_utils-4.0.0/src/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.754681 scottbrian_utils-4.0.0/src/scottbrian_utils/
+-rw-rw-rw-   0        0        0      141 2024-04-09 16:58:14.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/__init__.py
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/__init__.pyi
+-rw-rw-rw-   0        0        0    12890 2023-11-24 00:13:36.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/diag_msg.py
+-rw-rw-rw-   0        0        0     8201 2023-11-30 17:05:18.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/doc_checker.py
+-rw-rw-rw-   0        0        0    13327 2024-05-12 01:24:29.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/entry_trace.py
+-rw-rw-rw-   0        0        0    15194 2024-03-31 01:49:03.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/file_catalog.py
+-rw-rw-rw-   0        0        0     1833 2022-01-25 18:21:47.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/flower_box.py
+-rw-rw-rw-   0        0        0    48973 2024-05-10 18:26:16.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/log_verifier.py
+-rw-rw-rw-   0        0        0     7606 2022-01-25 18:21:47.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/msgs.py
+-rw-rw-rw-   0        0        0    20415 2023-11-24 00:11:58.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/pauser.py
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/py.typed
+-rw-rw-rw-   0        0        0     6792 2023-01-26 16:36:30.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/stop_watch.py
+-rw-rw-rw-   0        0        0    18522 2024-04-14 23:53:31.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/time_hdr.py
+-rw-rw-rw-   0        0        0    24423 2023-04-11 22:05:38.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/timer.py
+-rw-rw-rw-   0        0        0     2322 2023-10-14 23:15:12.000000 scottbrian_utils-4.0.0/src/scottbrian_utils/unique_ts.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.792688 scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/
+-rw-rw-rw-   0        0        0     7678 2024-05-13 00:36:01.000000 scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2638 2024-05-13 00:36:01.000000 scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 00:36:01.000000 scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-13 00:36:01.000000 scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-13 00:36:01.000000 scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.678663 scottbrian_utils-4.0.0/tests/
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.781687 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/
+-rw-rw-rw-   0        0        0       38 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/__init__.py
+-rw-rw-rw-   0        0        0     8171 2023-11-24 21:49:34.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/adjust_diag_msg_tcode.py
+-rw-rw-rw-   0        0        0     5699 2024-04-24 20:25:46.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/conftest.py
+-rw-rw-rw-   0        0        0   493189 2023-11-24 21:49:35.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_diag_msg.py
+-rw-rw-rw-   0        0        0   106995 2024-05-12 19:26:02.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_entry_trace.py
+-rw-rw-rw-   0        0        0    17147 2023-11-24 00:16:31.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_file_catalog.py
+-rw-rw-rw-   0        0        0     7704 2023-07-01 17:34:46.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_flower_box.py
+-rw-rw-rw-   0        0        0   152540 2024-05-10 20:20:22.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_log_verifier.py
+-rw-rw-rw-   0        0        0    15938 2024-05-08 01:06:25.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_msgs.py
+-rw-rw-rw-   0        0        0    36592 2023-11-24 00:15:56.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_pauser.py
+-rw-rw-rw-   0        0        0    17642 2023-07-01 17:34:46.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_stop_watch.py
+-rw-rw-rw-   0        0        0    77560 2024-04-22 00:08:46.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_time_hdr.py
+-rw-rw-rw-   0        0        0    40767 2023-11-23 15:44:47.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_timer.py
+-rw-rw-rw-   0        0        0     5972 2023-11-25 00:12:19.000000 scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_unique_ts.py
+-rw-rw-rw-   0        0        0     6635 2024-05-03 14:48:19.000000 scottbrian_utils-4.0.0/tox.ini
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.679664 scottbrian_utils-4.0.0/type_stubs/
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.783687 scottbrian_utils-4.0.0/type_stubs/mypywrapt/
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.785687 scottbrian_utils-4.0.0/type_stubs/mypywrapt/adjust_src/
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/adjust_src/__init__.pyi
+-rw-rw-rw-   0        0        0     1292 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/adjust_src/adjust_src.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.680663 scottbrian_utils-4.0.0/type_stubs/mypywrapt/build/
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.680663 scottbrian_utils-4.0.0/type_stubs/mypywrapt/build/lib/
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.788689 scottbrian_utils-4.0.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/__init__.pyi
+-rw-rw-rw-   0        0        0      329 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/build/lib/wrapt-stubs/decorators.pyi
+-rw-rw-rw-   0        0        0      388 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 00:36:01.791689 scottbrian_utils-4.0.0/type_stubs/mypywrapt/wrapt-stubs/
+-rw-rw-rw-   0        0        0      121 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/wrapt-stubs/__init__.pyi
+-rw-rw-rw-   0        0        0      329 2021-12-29 18:20:23.000000 scottbrian_utils-4.0.0/type_stubs/mypywrapt/wrapt-stubs/decorators.pyi
```

### Comparing `scottbrian_utils-3.0.0/.gitignore` & `scottbrian_utils-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/.idea/scottbrian_utils.iml` & `scottbrian_utils-4.0.0/.idea/scottbrian_utils.iml`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/LICENSE.txt` & `scottbrian_utils-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/MANIFEST.in` & `scottbrian_utils-4.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/PKG-INFO` & `scottbrian_utils-4.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scottbrian_utils
-Version: 3.0.0
+Version: 4.0.0
 Summary: Miscellaneous utilities
 Author-email: Scott Tuttle <sbtuttle@outlook.com>
 License: MIT License
         
         Copyright (c) [2020] [Scott Tuttle]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,40 +32,44 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Recovery Tools
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Requires-Python: >=3.12
+Requires-Python: ~=3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: typing_extensions
-Requires-Dist: wrapt
+Requires-Dist: more-itertools~=10.2
+Requires-Dist: pandas~=2.2
+Requires-Dist: typing_extensions~=4.11
+Requires-Dist: wrapt~=1.16
 
 ================
 scottbrian-utils
 ================
 
 Intro
 =====
 
 This is a collection of generally useful functions for use with any application.
 
 1. The diag_msg function allows you to print a message with the time and caller sequence added for you.
-2. The FileCatalog item allows you to map file names to their paths.
-3. The @time_box decorator allows you to print start, stop, and execution times.
-4. The print_flower_box_msg function allows you to print text in a flower box (i.e., surrounded by asterisks).
-5. The log_verifier allows you to verify that expected log messages have been issued.
-6. The msgs item is a simple facility you can use to send messages between threads.
-7. The stop_watch item is a simple timing function that you can use in test cases.
-8. The timer item provides a way to keep track of time to determine when a function has timed out.
-9. The Pauser class provides a pause function similar to the python sleep function, but with improved accuracy.
-10. The UniqueTS class provides a way to obtain a unique timestamp.
-11. The doc_checker module provides an easy way to do doctest.
+2. The doc_checker module provides an easy way to do a doctest.
+3. The etrace decorator provide entry and exit tracing including passed args and returned values.
+4. The FileCatalog item allows you to map file names to their paths.
+5. The print_flower_box_msg function allows you to print text in a flower box (i.e., surrounded by asterisks).
+6. The log_verifier allows you to verify that expected log messages have been issued.
+7. The msgs item is a simple facility you can use in test cases to send messages between threads.
+8. The Pauser class provides a pause function similar to the python sleep function, but with improved accuracy.
+9. The stop_watch item is a simple timing function that you can use in test cases.
+10. The @time_box decorator allows you to print start, stop, and execution times.
+11. The timer item provides a way to keep track of time to determine when a function has timed out.
+12. The UniqueTS class provides a way to obtain a unique timestamp.
+
 
 Examples:
 =========
 
 With **diag_msg** you can print messages with the time and caller info added automatically.
 
 :Example: print a diagnostic message (<input> appears as the module name when run from the console)
@@ -183,14 +187,24 @@
 
 * 3.0.0
     * added unique_ts
     * added doc_checker
     * support python 3.12
     * drop support python < 3.12
 
+* 4.0.0
+    * added timedelta_match_string to time_hdr.py
+    * added entry_trace.py
+    * restructured log_verifier:
+        * performance improvements
+        * changes to clarify that regex patterns are used
+        * changed report format
+        * method add_pattern replaces deprecated method add_msg
+        * method verify_match_results replaces deprecated verify_log_results
+
 
 Meta
 ====
 
 Scott Tuttle
 
 Distributed under the MIT license. See ``LICENSE`` for more information.
```

### Comparing `scottbrian_utils-3.0.0/README.rst` & `scottbrian_utils-4.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 
 Intro
 =====
 
 This is a collection of generally useful functions for use with any application.
 
 1. The diag_msg function allows you to print a message with the time and caller sequence added for you.
-2. The FileCatalog item allows you to map file names to their paths.
-3. The @time_box decorator allows you to print start, stop, and execution times.
-4. The print_flower_box_msg function allows you to print text in a flower box (i.e., surrounded by asterisks).
-5. The log_verifier allows you to verify that expected log messages have been issued.
-6. The msgs item is a simple facility you can use to send messages between threads.
-7. The stop_watch item is a simple timing function that you can use in test cases.
-8. The timer item provides a way to keep track of time to determine when a function has timed out.
-9. The Pauser class provides a pause function similar to the python sleep function, but with improved accuracy.
-10. The UniqueTS class provides a way to obtain a unique timestamp.
-11. The doc_checker module provides an easy way to do doctest.
+2. The doc_checker module provides an easy way to do a doctest.
+3. The etrace decorator provide entry and exit tracing including passed args and returned values.
+4. The FileCatalog item allows you to map file names to their paths.
+5. The print_flower_box_msg function allows you to print text in a flower box (i.e., surrounded by asterisks).
+6. The log_verifier allows you to verify that expected log messages have been issued.
+7. The msgs item is a simple facility you can use in test cases to send messages between threads.
+8. The Pauser class provides a pause function similar to the python sleep function, but with improved accuracy.
+9. The stop_watch item is a simple timing function that you can use in test cases.
+10. The @time_box decorator allows you to print start, stop, and execution times.
+11. The timer item provides a way to keep track of time to determine when a function has timed out.
+12. The UniqueTS class provides a way to obtain a unique timestamp.
+
 
 Examples:
 =========
 
 With **diag_msg** you can print messages with the time and caller info added automatically.
 
 :Example: print a diagnostic message (<input> appears as the module name when run from the console)
@@ -139,14 +141,24 @@
 
 * 3.0.0
     * added unique_ts
     * added doc_checker
     * support python 3.12
     * drop support python < 3.12
 
+* 4.0.0
+    * added timedelta_match_string to time_hdr.py
+    * added entry_trace.py
+    * restructured log_verifier:
+        * performance improvements
+        * changes to clarify that regex patterns are used
+        * changed report format
+        * method add_pattern replaces deprecated method add_msg
+        * method verify_match_results replaces deprecated verify_log_results
+
 
 Meta
 ====
 
 Scott Tuttle
 
 Distributed under the MIT license. See ``LICENSE`` for more information.
```

### Comparing `scottbrian_utils-3.0.0/conftest.py` & `scottbrian_utils-4.0.0/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,17 +64,17 @@
 
                 match_re = re.compile(match_str)
                 found_items = match_re.finditer(got)
                 want = match_re.sub(repl_dt, want)
 
             # match_str = "<.+?>"
             if self.mod_name == "diag_msg":
-                match_str = "diag_msg.py\[0\]>"
+                match_str = r"diag_msg.py\[0\]>"
             else:
-                match_str = "README.rst\[0\]>"
+                match_str = r"README.rst\[0\]>"
             replacement = "<input>"
             got = re.sub(match_str, replacement, got)
 
         if self.mod_name == "pauser":
             match_str = "pauser.min_interval_secs=0.0[0-9]{1,2}"
 
             found_item = re.match(match_str, got)
```

### Comparing `scottbrian_utils-3.0.0/docs/source/UniqueTS_UseCase1.svg` & `scottbrian_utils-4.0.0/docs/source/UniqueTS_UseCase1.svg`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/docs/source/adjust_sphinx/adjust_sphinx.py` & `scottbrian_utils-4.0.0/docs/source/adjust_sphinx/adjust_sphinx.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/docs/source/conf.py` & `scottbrian_utils-4.0.0/docs/source/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,54 +13,56 @@
 
 from os import fspath
 import sys
 from pathlib import Path
 
 proj_dir = Path.cwd().resolve().parents[1]  # back two directories
 sys.path.insert(0, fspath(proj_dir))
-sys.path.insert(0, fspath(proj_dir / 'src'))
-sys.path.insert(0, fspath(proj_dir / 'src/scottbrian_utils'))
+sys.path.insert(0, fspath(proj_dir / "src"))
+sys.path.insert(0, fspath(proj_dir / "src/scottbrian_utils"))
 
 
 # -- Project information -----------------------------------------------------
 
-project = 'scottbrian_utils'
-copyright = '2020, 2023, Scott Tuttle'
-author = 'Scott Tuttle'
+project = "scottbrian_utils"
+copyright = "2020, 2023, Scott Tuttle"
+author = "Scott Tuttle"
 
 # The full version, including alpha/beta/rc tags
-release = '3.0.0'
+release = "4.0.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ['sphinx.ext.autodoc',
-              'sphinx.ext.napoleon',
-              'sphinx_autodoc_typehints',
-              'sphinx_rtd_theme']
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.napoleon",
+    "sphinx_autodoc_typehints",
+    "sphinx_rtd_theme",
+]
 
-autoclass_content = 'both'
-autodoc_member_order = 'groupwise'
+autoclass_content = "both"
+autodoc_member_order = "groupwise"
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = []
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_rtd_theme"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
```

### Comparing `scottbrian_utils-3.0.0/docs/source/index.rst` & `scottbrian_utils-4.0.0/docs/source/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,23 @@
    contain the root `toctree` directive.
 
 
 .. include:: ../../README.rst
 
 .. toctree::
    :maxdepth: 2
+   :titlesonly:
    :caption: API Reference:
 
    diag_msg <diag_msg_link>
 
    doc_checker <doc_checker_link>
 
+   entry_trace <entry_trace_link>
+
    file_catalog <file_catalog_link>
 
    flower_box <flower_box_link>
 
    log_verifier <log_verifier_link>
 
    msgs <msgs_link>
```

### Comparing `scottbrian_utils-3.0.0/pyproject.toml` & `scottbrian_utils-4.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 [project]
 name = "scottbrian_utils"
-version = "3.0.0"
+version = "4.0.0"
 description = "Miscellaneous utilities"
 readme = "README.rst"
-requires-python = ">=3.12"
+requires-python = "~=3.12"
 license = {file = "LICENSE.txt"}
 keywords = ["utilities"]
 authors = [{name = "Scott Tuttle", email = "sbtuttle@outlook.com"}]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Recovery Tools",
     "Topic :: Utilities",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.12",
     "Operating System :: Microsoft :: Windows :: Windows 10"]
 dependencies = [
-    "typing_extensions",
-    "wrapt",
+    "more-itertools ~=10.2",
+    "pandas ~=2.2",
+    "typing_extensions ~=4.11",
+    "wrapt ~=1.16",
 ]
 
 [tool.setuptools]
 packages = ["scottbrian_utils"]
 package-dir = {"" = "src"}
 
 [project.urls]
 Documentation = "https://scottbrian-utils.readthedocs.io/en/latest/"
 Source = "https://github.com/ScottBrian/scottbrian_utils.git"
 
 [build-system]
 requires = [
-    "setuptools >= 69.0.0",
-    "wheel >= 0.41.3"
+    "setuptools ~=69.5",
+    "wheel ~=0.43"
 ]
 build-backend = 'setuptools.build_meta'
```

### Comparing `scottbrian_utils-3.0.0/pytest.ini` & `scottbrian_utils-4.0.0/pytest.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [pytest]
 addopts = -rsxX -l --tb=short --strict-markers --strict-config -p no:doctest
 xfail_strict = true
-log_cli = 1
+log_cli = 0
 log_cli_level = DEBUG
 #  log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
-log_cli_format ='%(asctime)s %(msecs)03d [%(levelname)8s] %(filename)20s: %(funcName)s: %(lineno)d %(message)s')
+log_cli_format ='%(asctime)s %(msecs)03d [%(levelname)8s] %(name)s %(filename)20s: %(funcName)s: %(lineno)d %(message)s')
 # log_cli_date_format = %Y-%m-%d %H:%M:%S
 log_cli_date_format = %H:%M:%S
 
 markers =
     cover: mark a test as a coverage test.
     cover2: mark test as a coverage test.
     seltest: mark test as selected for pytest run.
 
+filterwarnings =
+    error
+
 # for sybil (see above addopts where I put it to avoid duplicate tag)
 # addopts = -p no:doctest
 
 # log_file = MyLogFile.log
 # log_file_format =%(asctime)s [%(levelname)8s] %(filename)20s: %(funcName)s: %(lineno)d %(message)s')
 # log_file_date_format = %H:%M:%S
 ;
```

### Comparing `scottbrian_utils-3.0.0/src/conftest.py` & `scottbrian_utils-4.0.0/src/conftest.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/src/scottbrian_utils/diag_msg.py` & `scottbrian_utils-4.0.0/src/scottbrian_utils/diag_msg.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/src/scottbrian_utils/doc_checker.py` & `scottbrian_utils-4.0.0/src/scottbrian_utils/doc_checker.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/src/scottbrian_utils/file_catalog.py` & `scottbrian_utils-4.0.0/src/scottbrian_utils/file_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module file_catalog.
 
-============
-file_catalog
-============
+===========
+FileCatalog
+===========
 
 With **file_catalog**, you can set up a mapping of file names to their
 paths. An application can then use the catalog to retrieve the paths
 based on the file name. By keeping different catalogs with the same file
 names but different paths, different runs of the application can use
 each of the different catalogs as appropriate. For example, one catalog
 could be used for testing purposes and another for normal production.
@@ -49,14 +49,15 @@
 
        a. FileNameNotFound
        b. FileSpecIncorrect
        c. IllegalAddAttempt
        d. IllegalDelAtempt
 
 """
+
 import csv
 from pathlib import Path
 from typing import Dict, List, Optional, Type, TYPE_CHECKING
 
 FileSpecs = Dict[str, Path]
 
 
@@ -225,15 +226,15 @@
         '/run/media/file2.pdf'
 
         """
         try:
             return self.catalog[file_name]
         except KeyError:
             raise FileNameNotFound(
-                "Catalog does not have an entry for" f"file name: {file_name}"
+                "Catalog does not have an entry for file name: {file_name}"
             )
 
     def add_paths(self, file_specs: FileSpecs) -> None:
         """Add one or more paths to the catalog.
 
         Args:
             file_specs: A dictionary of one or more entries. The key is
```

### Comparing `scottbrian_utils-3.0.0/src/scottbrian_utils/flower_box.py` & `scottbrian_utils-4.0.0/src/scottbrian_utils/flower_box.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/src/scottbrian_utils/msgs.py` & `scottbrian_utils-4.0.0/src/scottbrian_utils/msgs.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/src/scottbrian_utils/pauser.py` & `scottbrian_utils-4.0.0/src/scottbrian_utils/pauser.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/src/scottbrian_utils/stop_watch.py` & `scottbrian_utils-4.0.0/src/scottbrian_utils/stop_watch.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/src/scottbrian_utils/time_hdr.py` & `scottbrian_utils-4.0.0/src/scottbrian_utils/time_hdr.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,22 +35,22 @@
        (see flower_box module in scottbrian_utils package).
     2) a time_box decorator that wraps a function and uses the
        StartStopHeader to print the starting and ending time messages.
 
 time_box imports functools, sys, datetime, wrapt, and types from typing
 
 """
+
 ########################################################################
 # Standard Library
 ########################################################################
 import functools
 from datetime import datetime
 import re
-from typing import (Any, Callable, cast, NewType, Optional,
-                    TypeVar, Union)
+from typing import Any, Callable, cast, NewType, Optional, TypeVar, Union
 
 from typing import overload
 
 ########################################################################
 # Third Party
 ########################################################################
 from wrapt.decorators import decorator
@@ -63,15 +63,33 @@
 ########################################################################
 # type aliases
 ########################################################################
 
 ########################################################################
 # NewType
 ########################################################################
-DT_Format = NewType('DT_Format', str)
+DT_Format = NewType("DT_Format", str)
+
+
+########################################################################
+# timedelta regex match string
+########################################################################
+match_str_days = "(-?1 day, |-?[2-9] days, |-?[1-9][0-9]{1,8} days, |)"
+match_str_hours = "([0-9]|1[0-9]|2[0-3])"
+match_str_mins = "[0-5][0-9]"
+match_str_secs = "[0-5][0-9]"
+match_str_usecs = r"(\.[0-9]{6}|)"
+
+timedelta_match_string = (
+    f"{match_str_days}"
+    f"{match_str_hours}:"
+    f"{match_str_mins}:"
+    f"{match_str_secs}"
+    f"{match_str_usecs}"
+)
 
 
 ########################################################################
 # StartStopHeader
 ########################################################################
 class StartStopHeader:
     """Provide support for the time_box decorator.
@@ -84,50 +102,52 @@
         3) method print_end_msg to print the end trailer with end time
            and elapsed time
 
     While there might be some standalone uses for this class and its
     methods, its intended use is by the time_box decorator described
     later in this module.
     """
-    default_dt_format: DT_Format = DT_Format('%a %b %d %Y %H:%M:%S')
+
+    default_dt_format: DT_Format = DT_Format("%a %b %d %Y %H:%M:%S")
 
     def __init__(self, func_name: str) -> None:
         """Store func_name and set the start and end times to None.
 
         Args:
             func_name: The name of the function to appear in the start
                          and stop messages
         """
         self.func_name = func_name
         self.start_DT: datetime = datetime.max
         self.end_DT: datetime = datetime.min
 
-    def print_end_msg(self, dt_format: DT_Format = default_dt_format,
-                      **kwargs: Any) -> None:
+    def print_end_msg(
+        self, dt_format: DT_Format = default_dt_format, **kwargs: Any
+    ) -> None:
         """Issue end time message in a flower box.
 
         The end message includes the current datetime and elapsed time
         (calculated as the difference between the end time and the saved
         start time - see the *print_start_msg* method).
 
         Args:
             dt_format: Specifies the datetime format to use in the end
                          time message. The default is
                          StartStopHeader.default_dt_format.
             kwargs: Specifies the print arguments to use on the print
                       statement, such as *end*, *file*, or *flush*.
         """
         self.end_DT = datetime.now()
-        msg1 = 'Ending ' + self.func_name + ' on ' \
-               + self.end_DT.strftime(dt_format)
-        msg2 = 'Elapsed time: ' + str(self.end_DT - self.start_DT)
+        msg1 = "Ending " + self.func_name + " on " + self.end_DT.strftime(dt_format)
+        msg2 = "Elapsed time: " + str(self.end_DT - self.start_DT)
         print_flower_box_msg([msg1, msg2], **kwargs)
 
-    def print_start_msg(self, dt_format: DT_Format = default_dt_format,
-                        **kwargs: Any) -> None:
+    def print_start_msg(
+        self, dt_format: DT_Format = default_dt_format, **kwargs: Any
+    ) -> None:
         """Issue start time message in a flower box.
 
         The start message includes the current datetime which is also
         saved to be used later to calculate the elapsed time for the
         *print_end_msg* invocation.
 
         Args:
@@ -157,42 +177,49 @@
         ********************************************
         * Ending func3 on Mon Jun 29 2020 18:22:50 *
         * Elapsed time: 0:00:00.001842             *
         ********************************************
 
         """
         self.start_DT = datetime.now()
-        msg = 'Starting ' + self.func_name + ' on ' \
-              + self.start_DT.strftime(dt_format)
+        msg = "Starting " + self.func_name + " on " + self.start_DT.strftime(dt_format)
         print_flower_box_msg([msg], **kwargs)
 
 
-F = TypeVar('F', bound=Callable[..., Any])
+F = TypeVar("F", bound=Callable[..., Any])
 
 
 @overload
-def time_box(wrapped: F, *,
-             dt_format: DT_Format = StartStopHeader.default_dt_format,
-             time_box_enabled: Union[bool, Callable[..., bool]] = True,
-             **kwargs: Any) -> F:
+def time_box(
+    wrapped: F,
+    *,
+    dt_format: DT_Format = StartStopHeader.default_dt_format,
+    time_box_enabled: Union[bool, Callable[..., bool]] = True,
+    **kwargs: Any,
+) -> F:
     pass
 
 
 @overload
-def time_box(*,
-             dt_format: DT_Format = StartStopHeader.default_dt_format,
-             time_box_enabled: Union[bool, Callable[..., bool]] = True,
-             **kwargs: Any) -> Callable[[F], F]:
+def time_box(
+    *,
+    dt_format: DT_Format = StartStopHeader.default_dt_format,
+    time_box_enabled: Union[bool, Callable[..., bool]] = True,
+    **kwargs: Any,
+) -> Callable[[F], F]:
     pass
 
 
-def time_box(wrapped: Optional[F] = None, *,
-             dt_format: DT_Format = StartStopHeader.default_dt_format,
-             time_box_enabled: Union[bool, Callable[..., bool]] = True,
-             **kwargs: Any) -> F:
+def time_box(
+    wrapped: Optional[F] = None,
+    *,
+    dt_format: DT_Format = StartStopHeader.default_dt_format,
+    time_box_enabled: Union[bool, Callable[..., bool]] = True,
+    **kwargs: Any,
+) -> F:
     """Decorator to wrap a function in start time and end time messages.
 
     The time_box decorator can be invoked with or without arguments, and
     the function being wrapped can optionally take arguments and
     optionally return a value. The wrapt.decorator is used to preserve
     the wrapped function introspection capabilities, and
     functools.partial is used to handle the case where decorator
@@ -355,22 +382,31 @@
     #     One other complication is that we are also using the
     #     wrapt.decorator for the inner wrapper function which does some
     #     more smoke and mirrors to ensure introspection will work as
     #     expected.
     # ==================================================================
 
     if wrapped is None:
-        return cast(F, functools.partial(time_box, dt_format=dt_format,
-                                         time_box_enabled=time_box_enabled,
-                                         **kwargs))
+        return cast(
+            F,
+            functools.partial(
+                time_box,
+                dt_format=dt_format,
+                time_box_enabled=time_box_enabled,
+                **kwargs,
+            ),
+        )
 
     @decorator(enabled=time_box_enabled)  # type: ignore
-    def wrapper(func_to_wrap: F, instance: Optional[Any],
-                args: tuple[Any, ...],
-                kwargs2: dict[str, Any]) -> Any:
+    def wrapper(
+        func_to_wrap: F,
+        instance: Optional[Any],
+        args: tuple[Any, ...],
+        kwargs2: dict[str, Any],
+    ) -> Any:
         header = StartStopHeader(func_to_wrap.__name__)
         header.print_start_msg(dt_format=dt_format, **kwargs)
 
         ret_value = func_to_wrap(*args, **kwargs2)
 
         header.print_end_msg(dt_format=dt_format, **kwargs)
 
@@ -378,78 +414,85 @@
 
     return cast(F, wrapper(wrapped))
 
 
 ########################################################################
 # get_datetime_match_string
 ########################################################################
-def get_datetime_match_string(format: str) -> str:
+def get_datetime_match_string(format_str: str) -> str:
     """Return a regex string to match a datetime string.
 
     Args:
-        format: string used to format a datetime that is to be used to
-                  create a match string
+        format_str: string used to format a datetime that is to be used
+            to create a match string
+
+    .. versionchanged:: 3.0.0
+           *format* keyword changed to *format_str*
 
     Returns:
         string that is to be used in a regex expression to match a
         datetime string
 
     """
-    match_str_a = r'(Sun|Mon|Tue|Wed|Thu|Fri|Sat)'
-    match_str_A = r'(Sunday|Monday|Tuesday|Wednesday|Thursday|Friday|Saturday)'
-    match_str_d = r'([0-2][0-9]|3[0-1])'
-    match_str_b = r'(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)'
-    match_str_B = (r'(January|February|March|April|May|June|July|August'
-                   r'|September|October|November|December)')
-    match_str_m = r'(0[1-9]|1[0-2])'
-    match_str_w = r'[0-6]'
-    match_str_y = r'[0-9]{2,2}'
-    match_str_Y = r'[1-9][0-9]{3,3}'
-
-    match_str_H = r'([0-1][0-9]|2[0-3])'
-    match_str_I = r'(0[1-9]|1[0-2])'
-    match_str_p = r'(AM|PM)'
-    match_str_M = r'[0-5][0-9]'
-    match_str_S = r'[0-5][0-9]'
-    match_str_f = r'[0-9]{6,6}'
-    match_str_z = r'[+-]' + f'{match_str_H}{match_str_M}'
-    match_str_Z = r'(UTC|GMT)([+-]' + f'({match_str_H}:{match_str_M}))*'
-    match_str_j = r'[0-3][0-9]{2,2}'
-    match_str_U = r'[0-5][0-9]'
-    match_str_W = r'[0-5][0-9]'
-    match_str_c = (f'{match_str_a} {match_str_b} ( [1-9]|[0-2][0-9]|3[0-1]) '
-                   f'{match_str_H}:{match_str_M}:{match_str_S} {match_str_Y}')
+    match_str_a = r"(Sun|Mon|Tue|Wed|Thu|Fri|Sat)"
+    match_str_A = r"(Sunday|Monday|Tuesday|Wednesday|Thursday|Friday|Saturday)"
+    match_str_d = r"([0-2][0-9]|3[0-1])"
+    match_str_b = r"(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)"
+    match_str_B = (
+        r"(January|February|March|April|May|June|July|August"
+        r"|September|October|November|December)"
+    )
+    match_str_m = r"(0[1-9]|1[0-2])"
+    match_str_w = r"[0-6]"
+    match_str_y = r"[0-9]{2,2}"
+    match_str_Y = r"[1-9][0-9]{3,3}"
+
+    match_str_H = r"([0-1][0-9]|2[0-3])"
+    match_str_I = r"(0[1-9]|1[0-2])"
+    match_str_p = r"(AM|PM)"
+    match_str_M = r"[0-5][0-9]"
+    match_str_S = r"[0-5][0-9]"
+    match_str_f = r"[0-9]{6,6}"
+    match_str_z = r"[+-]" + f"{match_str_H}{match_str_M}"
+    match_str_Z = r"(UTC|GMT)([+-]" + f"({match_str_H}:{match_str_M}))*"
+    match_str_j = r"[0-3][0-9]{2,2}"
+    match_str_U = r"[0-5][0-9]"
+    match_str_W = r"[0-5][0-9]"
+    match_str_c = (
+        f"{match_str_a} {match_str_b} ( [1-9]|[0-2][0-9]|3[0-1]) "
+        f"{match_str_H}:{match_str_M}:{match_str_S} {match_str_Y}"
+    )
     # match_str_x = f'{match_str_m}/{match_str_d}/{match_str_Y}'
-    match_str_x = f'{match_str_m}/{match_str_d}/{match_str_y}'
-    match_str_X = f'{match_str_H}:{match_str_M}:{match_str_S}'
+    match_str_x = f"{match_str_m}/{match_str_d}/{match_str_y}"
+    match_str_X = f"{match_str_H}:{match_str_M}:{match_str_S}"
     match_str_G = match_str_Y
-    match_str_u = r'[1-7]'
-    match_str_V = r'(0[1-9]|[1-5][0-9])'
+    match_str_u = r"[1-7]"
+    match_str_V = r"(0[1-9]|[1-5][0-9])"
 
-    match_str = re.escape(format)
-    match_str = re.sub('%a', match_str_a, match_str)
-    match_str = re.sub('%A', match_str_A, match_str)
-    match_str = re.sub('%d', match_str_d, match_str)
-    match_str = re.sub('%b', match_str_b, match_str)
-    match_str = re.sub('%B', match_str_B, match_str)
-    match_str = re.sub('%m', match_str_m, match_str)
-    match_str = re.sub('%w', match_str_w, match_str)
-    match_str = re.sub('%y', match_str_y, match_str)
-    match_str = re.sub('%Y', match_str_Y, match_str)
-    match_str = re.sub('%H', match_str_H, match_str)
-    match_str = re.sub('%I', match_str_I, match_str)
-    match_str = re.sub('%p', match_str_p, match_str)
-    match_str = re.sub('%M', match_str_M, match_str)
-    match_str = re.sub('%S', match_str_S, match_str)
-    match_str = re.sub('%f', match_str_f, match_str)
-    match_str = re.sub('%z', match_str_z, match_str)
-    match_str = re.sub('%Z', match_str_Z, match_str)
-    match_str = re.sub('%j', match_str_j, match_str)
-    match_str = re.sub('%U', match_str_U, match_str)
-    match_str = re.sub('%W', match_str_W, match_str)
-    match_str = re.sub('%c', match_str_c, match_str)
-    match_str = re.sub('%x', match_str_x, match_str)
-    match_str = re.sub('%X', match_str_X, match_str)
-    match_str = re.sub('%G', match_str_G, match_str)
-    match_str = re.sub('%u', match_str_u, match_str)
-    match_str = re.sub('%V', match_str_V, match_str)
+    match_str = re.escape(format_str)
+    match_str = re.sub("%a", match_str_a, match_str)
+    match_str = re.sub("%A", match_str_A, match_str)
+    match_str = re.sub("%d", match_str_d, match_str)
+    match_str = re.sub("%b", match_str_b, match_str)
+    match_str = re.sub("%B", match_str_B, match_str)
+    match_str = re.sub("%m", match_str_m, match_str)
+    match_str = re.sub("%w", match_str_w, match_str)
+    match_str = re.sub("%y", match_str_y, match_str)
+    match_str = re.sub("%Y", match_str_Y, match_str)
+    match_str = re.sub("%H", match_str_H, match_str)
+    match_str = re.sub("%I", match_str_I, match_str)
+    match_str = re.sub("%p", match_str_p, match_str)
+    match_str = re.sub("%M", match_str_M, match_str)
+    match_str = re.sub("%S", match_str_S, match_str)
+    match_str = re.sub("%f", match_str_f, match_str)
+    match_str = re.sub("%z", match_str_z, match_str)
+    match_str = re.sub("%Z", match_str_Z, match_str)
+    match_str = re.sub("%j", match_str_j, match_str)
+    match_str = re.sub("%U", match_str_U, match_str)
+    match_str = re.sub("%W", match_str_W, match_str)
+    match_str = re.sub("%c", match_str_c, match_str)
+    match_str = re.sub("%x", match_str_x, match_str)
+    match_str = re.sub("%X", match_str_X, match_str)
+    match_str = re.sub("%G", match_str_G, match_str)
+    match_str = re.sub("%u", match_str_u, match_str)
+    match_str = re.sub("%V", match_str_V, match_str)
     return match_str
```

### Comparing `scottbrian_utils-3.0.0/src/scottbrian_utils/timer.py` & `scottbrian_utils-4.0.0/src/scottbrian_utils/timer.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/src/scottbrian_utils/unique_ts.py` & `scottbrian_utils-4.0.0/src/scottbrian_utils/unique_ts.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/src/scottbrian_utils.egg-info/PKG-INFO` & `scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scottbrian-utils
-Version: 3.0.0
+Name: scottbrian_utils
+Version: 4.0.0
 Summary: Miscellaneous utilities
 Author-email: Scott Tuttle <sbtuttle@outlook.com>
 License: MIT License
         
         Copyright (c) [2020] [Scott Tuttle]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,40 +32,44 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Recovery Tools
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Requires-Python: >=3.12
+Requires-Python: ~=3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: typing_extensions
-Requires-Dist: wrapt
+Requires-Dist: more-itertools~=10.2
+Requires-Dist: pandas~=2.2
+Requires-Dist: typing_extensions~=4.11
+Requires-Dist: wrapt~=1.16
 
 ================
 scottbrian-utils
 ================
 
 Intro
 =====
 
 This is a collection of generally useful functions for use with any application.
 
 1. The diag_msg function allows you to print a message with the time and caller sequence added for you.
-2. The FileCatalog item allows you to map file names to their paths.
-3. The @time_box decorator allows you to print start, stop, and execution times.
-4. The print_flower_box_msg function allows you to print text in a flower box (i.e., surrounded by asterisks).
-5. The log_verifier allows you to verify that expected log messages have been issued.
-6. The msgs item is a simple facility you can use to send messages between threads.
-7. The stop_watch item is a simple timing function that you can use in test cases.
-8. The timer item provides a way to keep track of time to determine when a function has timed out.
-9. The Pauser class provides a pause function similar to the python sleep function, but with improved accuracy.
-10. The UniqueTS class provides a way to obtain a unique timestamp.
-11. The doc_checker module provides an easy way to do doctest.
+2. The doc_checker module provides an easy way to do a doctest.
+3. The etrace decorator provide entry and exit tracing including passed args and returned values.
+4. The FileCatalog item allows you to map file names to their paths.
+5. The print_flower_box_msg function allows you to print text in a flower box (i.e., surrounded by asterisks).
+6. The log_verifier allows you to verify that expected log messages have been issued.
+7. The msgs item is a simple facility you can use in test cases to send messages between threads.
+8. The Pauser class provides a pause function similar to the python sleep function, but with improved accuracy.
+9. The stop_watch item is a simple timing function that you can use in test cases.
+10. The @time_box decorator allows you to print start, stop, and execution times.
+11. The timer item provides a way to keep track of time to determine when a function has timed out.
+12. The UniqueTS class provides a way to obtain a unique timestamp.
+
 
 Examples:
 =========
 
 With **diag_msg** you can print messages with the time and caller info added automatically.
 
 :Example: print a diagnostic message (<input> appears as the module name when run from the console)
@@ -183,14 +187,24 @@
 
 * 3.0.0
     * added unique_ts
     * added doc_checker
     * support python 3.12
     * drop support python < 3.12
 
+* 4.0.0
+    * added timedelta_match_string to time_hdr.py
+    * added entry_trace.py
+    * restructured log_verifier:
+        * performance improvements
+        * changes to clarify that regex patterns are used
+        * changed report format
+        * method add_pattern replaces deprecated method add_msg
+        * method verify_match_results replaces deprecated verify_log_results
+
 
 Meta
 ====
 
 Scott Tuttle
 
 Distributed under the MIT license. See ``LICENSE`` for more information.
```

### Comparing `scottbrian_utils-3.0.0/src/scottbrian_utils.egg-info/SOURCES.txt` & `scottbrian_utils-4.0.0/src/scottbrian_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 .idea/inspectionProfiles/profiles_settings.xml
 docs/requirements.txt
 docs/source/UniqueTS_UseCase1.svg
 docs/source/_static
 docs/source/conf.py
 docs/source/diag_msg_link.rst
 docs/source/doc_checker_link.rst
+docs/source/entry_trace_link.rst
 docs/source/file_catalog_link.rst
 docs/source/flower_box_link.rst
 docs/source/index.rst
 docs/source/log_verifier_link.rst
 docs/source/msgs_link.rst
 docs/source/pauser_link.rst
 docs/source/setup.py
@@ -38,14 +39,15 @@
 docs/source/adjust_sphinx/__init__.py
 docs/source/adjust_sphinx/adjust_sphinx.py
 src/conftest.py
 src/scottbrian_utils/__init__.py
 src/scottbrian_utils/__init__.pyi
 src/scottbrian_utils/diag_msg.py
 src/scottbrian_utils/doc_checker.py
+src/scottbrian_utils/entry_trace.py
 src/scottbrian_utils/file_catalog.py
 src/scottbrian_utils/flower_box.py
 src/scottbrian_utils/log_verifier.py
 src/scottbrian_utils/msgs.py
 src/scottbrian_utils/pauser.py
 src/scottbrian_utils/py.typed
 src/scottbrian_utils/stop_watch.py
@@ -57,14 +59,15 @@
 src/scottbrian_utils.egg-info/dependency_links.txt
 src/scottbrian_utils.egg-info/requires.txt
 src/scottbrian_utils.egg-info/top_level.txt
 tests/test_scottbrian_utils/__init__.py
 tests/test_scottbrian_utils/adjust_diag_msg_tcode.py
 tests/test_scottbrian_utils/conftest.py
 tests/test_scottbrian_utils/test_diag_msg.py
+tests/test_scottbrian_utils/test_entry_trace.py
 tests/test_scottbrian_utils/test_file_catalog.py
 tests/test_scottbrian_utils/test_flower_box.py
 tests/test_scottbrian_utils/test_log_verifier.py
 tests/test_scottbrian_utils/test_msgs.py
 tests/test_scottbrian_utils/test_pauser.py
 tests/test_scottbrian_utils/test_stop_watch.py
 tests/test_scottbrian_utils/test_time_hdr.py
```

### Comparing `scottbrian_utils-3.0.0/tests/test_scottbrian_utils/adjust_diag_msg_tcode.py` & `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/adjust_diag_msg_tcode.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/tests/test_scottbrian_utils/conftest.py` & `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 from typing import Any, cast, Generator
 
 import logging
 
 ########################################################################
 # logging
 ########################################################################
-logging.basicConfig(filename='MyLogFile.log',
-                    filemode='w',
-                    level=logging.DEBUG,
-                    format='%(asctime)s '
-                           '%(msecs)03d '
-                           '[%(levelname)8s] '
-                           '%(filename)s:'
-                           '%(funcName)s:'
-                           '%(lineno)d '
-                           '%(message)s')
+# logging.basicConfig(filename='MyLogFile.log',
+#                     filemode='w',
+#                     level=logging.DEBUG,
+#                     format='%(asctime)s '
+#                            '%(msecs)03d '
+#                            '[%(levelname)8s] '
+#                            '%(filename)s:'
+#                            '%(funcName)s:'
+#                            '%(lineno)d '
+#                            '%(message)s')
 
 logger = logging.getLogger(__name__)
 
 
 ########################################################################
 # Thread exceptions
 # The following fixture depends on the following pytest specification:
 # -p no:threadexception
 
+
 # For PyCharm, the above specification goes into field Additional
 # Arguments found at Run -> edit configurations
 #
 # For tox, the above specification goes into tox.ini in the string for
 # the commands=
 # For example, in tox.ini for the pytest section:
 # [testenv:py{36, 37, 38, 39}-pytest]
@@ -60,41 +61,41 @@
 #
 ########################################################################
 class ExcHook:
     """ExcHook class."""
 
     def __init__(self) -> None:
         """Initialize the ExcHook class instance."""
-        self.exc_err_msg1 = ''
+        self.exc_err_msg1 = ""
 
     def raise_exc_if_one(self) -> None:
         """Raise an error is we have one.
 
         Raises:
             Exception: exc_msg
 
         """
         if self.exc_err_msg1:
             exc_msg = self.exc_err_msg1
-            self.exc_err_msg1 = ''
-            raise Exception(f'{exc_msg}')
+            self.exc_err_msg1 = ""
+            raise Exception(f"{exc_msg}")
 
 
 @pytest.fixture(autouse=True)
 def thread_exc(monkeypatch: Any) -> Generator[ExcHook, None, None]:
     """Instantiate and return a ThreadExc for testing.
 
     Args:
         monkeypatch: pytest fixture used to modify code for testing
 
     Yields:
         a thread exception handler
 
     """
-    logger.debug(f'hook before: {threading.excepthook}')
+    # logger.debug(f"hook before: {threading.excepthook}")
     exc_hook = ExcHook()
 
     def mock_threading_excepthook(args: Any) -> None:
         """Build error message from exception.
 
         Args:
             args: contains:
@@ -102,52 +103,65 @@
                       args.exc_value: Optional[BaseException]
                       args.exc_traceback: Optional[TracebackType]
 
         Raises:
             Exception: Test case thread test error
 
         """
-        exc_err_msg = (f'Test case excepthook: {args.exc_type}, '
-                       f'{args.exc_value}, {args.exc_traceback},'
-                       f' {args.thread}')
+        exc_err_msg = (
+            f"Test case excepthook: {args.exc_type}, "
+            f"{args.exc_value}, {args.exc_traceback},"
+            f" {args.thread}"
+        )
         traceback.print_tb(args.exc_traceback)
         logger.debug(exc_err_msg)
         current_thread = threading.current_thread()
-        logger.debug(f'excepthook current thread is {current_thread}')
+        logging.exception(f"exception caught for {current_thread}")
+        logger.debug(f"excepthook current thread is {current_thread}")
         # ExcHook.exc_err_msg1 = exc_err_msg
         exc_hook.exc_err_msg1 = exc_err_msg
-        raise Exception(f'Test case thread test error: {exc_err_msg}')
+        raise Exception(f"Test case thread test error: {exc_err_msg}")
 
     monkeypatch.setattr(threading, "excepthook", mock_threading_excepthook)
-    logger.debug(f'hook after: {threading.excepthook}')
+    # logger.debug(f"hook after: {threading.excepthook}")
     new_hook = threading.excepthook
 
     yield exc_hook
+
+    # surface any remote thread uncaught exceptions
     exc_hook.raise_exc_if_one()
 
+    # the following check ensures that the test case waited via join for
+    # any started threads to come home
+    if threading.active_count() > 1:
+        for thread in threading.enumerate():
+            print(f"conftest thread: {thread}")
+    assert threading.active_count() == 1
+
     # the following assert ensures -p no:threadexception was specified
     assert threading.excepthook == new_hook
 
 
 ########################################################################
 # dt_format_arg_list
 ########################################################################
-dt_format_arg_list = [None,
-                      '%H:%M',
-                      '%H:%M:%S',
-                      '%m/%d %H:%M:%S',
-                      '%b %d %H:%M:%S',
-                      '%m/%d/%y %H:%M:%S',
-                      '%m/%d/%Y %H:%M:%S',
-                      '%b %d %Y %H:%M:%S',
-                      '%a %b %d %Y %H:%M:%S',
-                      '%a %b %d %H:%M:%S.%f',
-                      '%A %b %d %H:%M:%S.%f',
-                      '%A %B %d %H:%M:%S.%f'
-                      ]
+dt_format_arg_list = [
+    None,
+    "%H:%M",
+    "%H:%M:%S",
+    "%m/%d %H:%M:%S",
+    "%b %d %H:%M:%S",
+    "%m/%d/%y %H:%M:%S",
+    "%m/%d/%Y %H:%M:%S",
+    "%b %d %Y %H:%M:%S",
+    "%a %b %d %Y %H:%M:%S",
+    "%a %b %d %H:%M:%S.%f",
+    "%A %b %d %H:%M:%S.%f",
+    "%A %B %d %H:%M:%S.%f",
+]
 
 
 @pytest.fixture(params=dt_format_arg_list)
 def dt_format_arg(request: Any) -> str:
     """Using different time formats.
 
     Args:
```

### Comparing `scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_diag_msg.py` & `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_diag_msg.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_file_catalog.py` & `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_file_catalog.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_flower_box.py` & `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_flower_box.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_msgs.py` & `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_msgs.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,49 +25,31 @@
 ########################################################################
 IntFloat = Union[int, float]
 OptIntFloat = Optional[IntFloat]
 
 ########################################################################
 # Set up logging
 ########################################################################
-logger = logging.getLogger('test_msgs')
-logger.debug('about to start the tests')
+logger = logging.getLogger("test_msgs")
+logger.debug("about to start the tests")
 
 
 ########################################################################
 # Msgs test exceptions
 ########################################################################
 class ErrorTstMsgs(Exception):
     """Base class for exception in this module."""
-    pass
-
-
-########################################################################
-# timeout_arg fixture
-########################################################################
-timeout_arg_list = [0.0, 0.3, 0.5, 1, 2, 4]
-
-
-@pytest.fixture(params=timeout_arg_list)
-def timeout_arg(request: Any) -> float:
-    """Using different seconds for timeout.
-
-    Args:
-        request: special fixture that returns the fixture params
 
-    Returns:
-        The params values are returned one at a time
-    """
-    return cast(float, request.param)
+    pass
 
 
 ########################################################################
 # who_arg fixture
 ########################################################################
-who_arg_list = ['beta', 'charlie', 'both']
+who_arg_list = ["beta", "charlie", "both"]
 
 
 @pytest.fixture(params=who_arg_list)
 def who_arg(request: Any) -> str:
     """Using different msg targets.
 
     Args:
@@ -78,15 +60,15 @@
     """
     return cast(str, request.param)
 
 
 #######################################################################
 # msg_arg fixture
 ########################################################################
-msg_arg_list = [0, '0', 0.0, 'hello', 1, [1, 2, 3], ('a', 'b', 'c')]
+msg_arg_list = [0, "0", 0.0, "hello", 1, [1, 2, 3], ("a", "b", "c")]
 
 
 @pytest.fixture(params=msg_arg_list)
 def msg_arg(request: Any) -> Any:
     """Using different msgs.
 
     Args:
@@ -97,15 +79,15 @@
     """
     return request.param
 
 
 #######################################################################
 # start_arg fixture
 ########################################################################
-start_arg_list = ['before', 'mid1', 'mid2', 'after']
+start_arg_list = ["before", "mid1", "mid2", "after"]
 
 
 @pytest.fixture(params=start_arg_list)
 def start_arg(request: Any) -> str:
     """Using different remote thread start points.
 
     Args:
@@ -118,338 +100,335 @@
 
 
 ########################################################################
 # TestMsgsErrors class
 ########################################################################
 class TestMsgsErrors:
     """TestMsgsErrors class."""
-    def test_msgs_timeout(self,
-                          timeout_arg: float,
-                          caplog: pytest.LogCaptureFixture) -> None:
+
+    @pytest.mark.parametrize("timeout_arg", [0.0, 0.3, 0.5, 1, 2, 4])
+    @pytest.mark.cover
+    def test_msgs_timeout(
+        self, timeout_arg: float, caplog: pytest.LogCaptureFixture
+    ) -> None:
         """test_msgs_timeout.
 
         Args:
             timeout_arg: number of seconds to use for timeout value
                            on get_msg request
             caplog: pytest fixture to capture log output
 
         """
+
         ################################################################
         # log_test_msg
         ################################################################
-        def log_test_msg(log_ver: LogVer,
-                         log_msg: str) -> None:
+        def log_test_msg(log_ver: LogVer, log_msg: str) -> None:
             """Issue log msgs for test rtn.
 
             Args:
                 log_ver: instance of LogVer
                 log_msg: the message to log
 
             """
-            log_ver.add_msg(log_msg=re.escape(log_msg))
+            log_ver.add_pattern(pattern=re.escape(log_msg))
             logger.debug(log_msg, stacklevel=2)
 
         ################################################################
         # f1
         ################################################################
         def f1() -> None:
             """Beta f1 function."""
-            log_test_msg(log_ver, 'f1 beta entered')
+            log_test_msg(log_ver, "f1 beta entered")
 
             f1_to_low = f1_timeout
             f1_to_high = f1_timeout * 1.1
 
             f1_stop_watch = StopWatch()
 
-            log_test_msg(log_ver, 'f1 beta starting timeout -1')
+            log_test_msg(log_ver, "f1 beta starting timeout -1")
 
             f1_stop_watch.start_clock(clock_iter=1)
-            msgs.get_msg('beta', timeout=-1)
+            msgs.get_msg("beta", timeout=-1)
             assert f1_to_low <= f1_stop_watch.duration() <= f1_to_high
 
-            log_test_msg(log_ver, 'f1 beta starting timeout 0')
+            log_test_msg(log_ver, "f1 beta starting timeout 0")
 
             f1_stop_watch.start_clock(clock_iter=2)
-            msgs.get_msg('beta', timeout=0)
+            msgs.get_msg("beta", timeout=0)
             assert f1_to_low <= f1_stop_watch.duration() <= f1_to_high
 
-            log_test_msg(log_ver, 'f1 beta starting timeout None')
+            log_test_msg(log_ver, "f1 beta starting timeout None")
 
             f1_stop_watch.start_clock(clock_iter=3)
-            msgs.get_msg('beta', timeout=None)
+            msgs.get_msg("beta", timeout=None)
             assert f1_to_low <= f1_stop_watch.duration() <= f1_to_high
 
-            log_test_msg(log_ver, 'f1 beta exiting')
+            log_test_msg(log_ver, "f1 beta exiting")
 
         ################################################################
         # mainline
         ################################################################
         msgs = Msgs()
         ml_stop_watch = StopWatch()
-        log_ver = LogVer(log_name='test_msgs')
-        alpha_call_seq = 'test_msgs.py::TestMsgsErrors.test_msgs_timeout'
-        log_ver.add_call_seq(name='alpha',
-                             seq=alpha_call_seq)
+        log_ver = LogVer(log_name="test_msgs")
+        alpha_call_seq = "test_msgs.py::TestMsgsErrors.test_msgs_timeout"
+        log_ver.add_call_seq(name="alpha", seq=alpha_call_seq)
 
-        log_test_msg(log_ver, 'mainline entered')
+        log_test_msg(log_ver, "mainline entered")
 
         f1_timeout = 5
         f1_thread = threading.Thread(target=f1)
 
         # we expect to get this log message in the following code
-        thread_info = re.escape(f'{threading.current_thread()}')
-        log_msg = (f'Thread {thread_info} '
-                   f'timed out on get_msg for recipient: beta '
-                   f'{log_ver.get_call_seq("alpha")}')
-        log_ver.add_msg(
-            log_name='scottbrian_utils.msgs',
-            log_level=logging.DEBUG,
-            log_msg=log_msg)
+        thread_info = re.escape(f"{threading.current_thread()}")
+        log_msg = (
+            f"Thread {thread_info} "
+            f"timed out on get_msg for recipient: beta "
+            f'{log_ver.get_call_seq("alpha")}'
+        )
+        log_ver.add_pattern(
+            log_name="scottbrian_utils.msgs", level=logging.DEBUG, pattern=log_msg
+        )
 
         # we will try -1 as a timeout value in the section below, and
         # we also use the -1 value to do the default value
         if timeout_arg == 0.0:  # if do default timeout
             ############################################################
             # get_msg timeout with default
             ############################################################
             to_low = Msgs.GET_CMD_TIMEOUT
             to_high = Msgs.GET_CMD_TIMEOUT * 1.1
             ml_stop_watch.start_clock(clock_iter=1)
 
             with pytest.raises(GetMsgTimedOut):
-                _ = msgs.get_msg('beta')
+                _ = msgs.get_msg("beta")
             assert to_low <= ml_stop_watch.duration() <= to_high
 
             f1_thread.start()
-            log_test_msg(log_ver, 'mainline starting timeout loop')
+            log_test_msg(log_ver, "mainline starting timeout loop")
 
             for idx in range(2, 5):  # 2, 3, 4
-                log_test_msg(log_ver, f'mainline starting timeout loop {idx}')
+                log_test_msg(log_ver, f"mainline starting timeout loop {idx}")
 
                 ml_stop_watch.start_clock(clock_iter=idx)
                 ml_stop_watch.pause(seconds=f1_timeout, clock_iter=idx)
-                log_test_msg(log_ver,
-                             f'mainline duration {ml_stop_watch.duration()}')
-
-                msgs.queue_msg('beta')
+                log_test_msg(log_ver, f"mainline duration {ml_stop_watch.duration()}")
 
+                msgs.queue_msg("beta")
+            f1_thread.join()
         else:
             ############################################################
             # get_msg timeout with timeout_arg
             ############################################################
             to_low = timeout_arg
             to_high = timeout_arg * 1.2
-            log_test_msg(log_ver, f'mainline starting timeout {timeout_arg}')
+            log_test_msg(log_ver, f"mainline starting timeout {timeout_arg}")
 
             ml_stop_watch.start_clock(clock_iter=1)
             with pytest.raises(GetMsgTimedOut):
-                _ = msgs.get_msg('beta', timeout_arg)
+                _ = msgs.get_msg("beta", timeout_arg)
             assert to_low <= ml_stop_watch.duration() <= to_high
 
         match_results = log_ver.get_match_results(caplog=caplog)
-        log_ver.print_match_results(match_results)
-        log_ver.verify_log_results(match_results)
+        log_ver.print_match_results(match_results, print_matched=True)
+        log_ver.verify_match_results(match_results)
 
-        logger.debug('mainline exiting')
+        logger.debug("mainline exiting")
 
 
 ########################################################################
 # TestMsgsExamples class
 ########################################################################
 class TestMsgsExamples:
     """Test examples of Msgs."""
 
     ####################################################################
     # test_msgs_example1
     ####################################################################
-    def test_msgs_example1(self,
-                           capsys: Any) -> None:
+    def test_msgs_example1(self, capsys: Any) -> None:
         """Test msgs example1.
 
         Args:
             capsys: pytest fixture to capture print output
 
         """
+
         def f1() -> None:
             """Beta f1 function."""
-            print('f1 beta entered')
-            my_msg = msgs.get_msg('beta')
+            print("f1 beta entered")
+            my_msg = msgs.get_msg("beta")
             print(my_msg)
-            print('f1 beta exiting')
+            print("f1 beta exiting")
 
-        print('mainline entered')
+        print("mainline entered")
         msgs = Msgs()
         f1_thread = threading.Thread(target=f1)
         f1_thread.start()
-        msgs.queue_msg('beta', 'hello beta')
+        msgs.queue_msg("beta", "hello beta")
         f1_thread.join()
-        print('mainline exiting')
+        print("mainline exiting")
 
-        expected_result = 'mainline entered\n'
-        expected_result += 'f1 beta entered\n'
-        expected_result += 'hello beta\n'
-        expected_result += 'f1 beta exiting\n'
-        expected_result += 'mainline exiting\n'
+        expected_result = "mainline entered\n"
+        expected_result += "f1 beta entered\n"
+        expected_result += "hello beta\n"
+        expected_result += "f1 beta exiting\n"
+        expected_result += "mainline exiting\n"
 
         captured = capsys.readouterr().out
 
         assert captured == expected_result
 
     ####################################################################
     # test_msgs_example2
     ####################################################################
-    def test_msgs_example2(self,
-                           capsys: Any) -> None:
+    def test_msgs_example2(self, capsys: Any) -> None:
         """Test msgs example2.
 
         Args:
             capsys: pytest fixture to capture print output
 
         """
+
         def f1() -> None:
             """Beta f1 function."""
-            print('f1 beta entered')
+            print("f1 beta entered")
             while True:
-                my_msg = msgs.get_msg('beta')
-                if my_msg == 'exit':
+                my_msg = msgs.get_msg("beta")
+                if my_msg == "exit":
                     break
                 else:
                     # handle command
-                    print(f'beta received cmd: {my_msg}')
-                    msgs.queue_msg('alpha', f'cmd "{my_msg}" completed')
-            print('f1 beta exiting')
+                    print(f"beta received cmd: {my_msg}")
+                    msgs.queue_msg("alpha", f'cmd "{my_msg}" completed')
+            print("f1 beta exiting")
 
-        print('mainline alpha entered')
+        print("mainline alpha entered")
         msgs = Msgs()
         f1_thread = threading.Thread(target=f1)
         f1_thread.start()
-        msgs.queue_msg('beta', 'do command a')
-        print(msgs.get_msg('alpha'))
-        msgs.queue_msg('beta', 'do command b')
+        msgs.queue_msg("beta", "do command a")
+        print(msgs.get_msg("alpha"))
+        msgs.queue_msg("beta", "do command b")
         print(f"alpha received response: {msgs.get_msg('alpha')}")
-        msgs.queue_msg('beta', 'exit')
+        msgs.queue_msg("beta", "exit")
         f1_thread.join()
-        print('mainline alpha exiting')
+        print("mainline alpha exiting")
 
-        expected_result = 'mainline alpha entered'
-        expected_result += 'f1 beta entered'
-        expected_result += 'beta received cmd: do command a'
-        expected_result += ('alpha received response: '
-                            'cmd "do command a" completed')
-        expected_result += 'beta received cmd: do command b'
-        expected_result += ('alpha received response: '
-                            'cmd "do command b" completed')
-        expected_result += 'f1 beta exiting'
-        expected_result += 'mainline alpha exiting'
+        expected_result = "mainline alpha entered"
+        expected_result += "f1 beta entered"
+        expected_result += "beta received cmd: do command a"
+        expected_result += "alpha received response: " 'cmd "do command a" completed'
+        expected_result += "beta received cmd: do command b"
+        expected_result += "alpha received response: " 'cmd "do command b" completed'
+        expected_result += "f1 beta exiting"
+        expected_result += "mainline alpha exiting"
 
 
 ########################################################################
 # TestMsgsMsgs class
 ########################################################################
 class TestMsgsMsgs:
     """Test queue_msg and get_msg methods of Msgs."""
 
     ####################################################################
     # test_msgs_example1
     ####################################################################
-    def test_msgs_msgs1(self,
-                        who_arg: str,
-                        msg_arg: Any,
-                        start_arg: str) -> None:
+    def test_msgs_msgs1(self, who_arg: str, msg_arg: Any, start_arg: str) -> None:
         """Test msgs queue_msg and get_msg methods.
 
         Args:
             who_arg: who to send msg to
             msg_arg: what to send
             start_arg: when to start the remote thread
 
         """
 
         def f1() -> None:
             """Beta f1 function."""
-            logger.debug('f1 beta entered')
+            logger.debug("f1 beta entered")
             f1_event.set()
-            assert msgs.get_msg('beta') == 'go'
+            assert msgs.get_msg("beta") == "go"
             while True:
-                my_msg = msgs.get_msg('beta')
-                if my_msg == 'exit now':
+                my_msg = msgs.get_msg("beta")
+                if my_msg == "exit now":
                     break
                 else:
                     assert my_msg == msg_arg
-            logger.debug('f1 beta exiting')
+            logger.debug("f1 beta exiting")
 
         def f2() -> None:
             """Charlie f2 function."""
-            logger.debug('f2 charlie entered')
+            logger.debug("f2 charlie entered")
             f2_event.set()
-            msgs.queue_msg('alpha', 'charlie ready')
-            assert msgs.get_msg('charlie') == 'go'
+            msgs.queue_msg("alpha", "charlie ready")
+            assert msgs.get_msg("charlie") == "go"
             while True:
-                my_msg = msgs.get_msg('charlie')
-                if my_msg == 'exit now':
+                my_msg = msgs.get_msg("charlie")
+                if my_msg == "exit now":
                     break
                 else:
                     assert my_msg == msg_arg
 
-            logger.debug('f2 charlie exiting')
+            logger.debug("f2 charlie exiting")
 
-        logger.debug('mainline entered')
+        logger.debug("mainline entered")
         msgs = Msgs()
         f1_event = threading.Event()
         f2_event = threading.Event()
 
-        if who_arg == 'beta' or who_arg == 'both':
+        if who_arg == "beta" or who_arg == "both":
             f1_thread = threading.Thread(target=f1)
-            if start_arg == 'before':
-                logger.debug('mainline starting beta before')
+            if start_arg == "before":
+                logger.debug("mainline starting beta before")
                 f1_thread.start()
                 f1_event.wait()
-            msgs.queue_msg('beta')  # no arg, default is 'go'
-            if start_arg == 'mid1':
-                logger.debug('mainline starting beta mid1')
+            msgs.queue_msg("beta")  # no arg, default is 'go'
+            if start_arg == "mid1":
+                logger.debug("mainline starting beta mid1")
                 f1_thread.start()
                 f1_event.wait()
-            msgs.queue_msg('beta', msg_arg)
-            if start_arg == 'mid2':
-                logger.debug('mainline starting beta mid2')
+            msgs.queue_msg("beta", msg_arg)
+            if start_arg == "mid2":
+                logger.debug("mainline starting beta mid2")
                 f1_thread.start()
                 f1_event.wait()
-            if who_arg == 'beta':
-                msgs.queue_msg(who_arg, 'exit now')
+            if who_arg == "beta":
+                msgs.queue_msg(who_arg, "exit now")
             else:
-                msgs.queue_msg('beta', 'exit now')
-            if start_arg == 'after':
-                logger.debug('mainline starting beta after')
+                msgs.queue_msg("beta", "exit now")
+            if start_arg == "after":
+                logger.debug("mainline starting beta after")
                 f1_thread.start()
                 f1_event.wait()
-            logger.debug('mainline about to join f1 beta')
+            logger.debug("mainline about to join f1 beta")
             f1_thread.join()
 
-        if who_arg == 'charlie' or who_arg == 'both':
-            logger.debug('mainline starting charlie')
+        if who_arg == "charlie" or who_arg == "both":
+            logger.debug("mainline starting charlie")
             f2_thread = threading.Thread(target=f2)
-            if start_arg == 'before':
-                logger.debug('mainline starting charlie before')
+            if start_arg == "before":
+                logger.debug("mainline starting charlie before")
                 f2_thread.start()
                 f2_event.wait()
-            msgs.queue_msg('charlie')  # no arg, default is 'go'
-            if start_arg == 'mid1':
-                logger.debug('mainline starting charlie mid1')
+            msgs.queue_msg("charlie")  # no arg, default is 'go'
+            if start_arg == "mid1":
+                logger.debug("mainline starting charlie mid1")
                 f2_thread.start()
                 f2_event.wait()
-            msgs.queue_msg('charlie', msg_arg)
-            if start_arg == 'mid2':
-                logger.debug('mainline starting charlie mid2')
+            msgs.queue_msg("charlie", msg_arg)
+            if start_arg == "mid2":
+                logger.debug("mainline starting charlie mid2")
                 f2_thread.start()
                 f2_event.wait()
-            if who_arg == 'charlie':
-                msgs.queue_msg(who_arg, 'exit now')
+            if who_arg == "charlie":
+                msgs.queue_msg(who_arg, "exit now")
             else:
-                msgs.queue_msg('charlie', 'exit now')
-            logger.debug('mainline about to join f2 charlie')
-            if start_arg == 'after':
-                logger.debug('mainline starting charlie after')
+                msgs.queue_msg("charlie", "exit now")
+            logger.debug("mainline about to join f2 charlie")
+            if start_arg == "after":
+                logger.debug("mainline starting charlie after")
                 f2_thread.start()
                 f2_event.wait()
             f2_thread.join()
 
-        logger.debug('mainline exiting')
+        logger.debug("mainline exiting")
```

### Comparing `scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_pauser.py` & `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_pauser.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_stop_watch.py` & `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_stop_watch.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_time_hdr.py` & `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_time_hdr.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 
 ########################################################################
 # Local
 ########################################################################
 from scottbrian_utils.time_hdr import StartStopHeader as StartStopHeader
 from scottbrian_utils.time_hdr import time_box as time_box
 from scottbrian_utils.time_hdr import DT_Format as DT_Format
-from scottbrian_utils.time_hdr import get_datetime_match_string
+from scottbrian_utils.time_hdr import (
+    get_datetime_match_string,
+    timedelta_match_string,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class ErrorTstTimeHdr(Exception):
     """Base class for exception in this module."""
 
@@ -492,14 +495,146 @@
 
         adjusted_old_dt = re.sub(match_str, new_datetime, formatted_old_dt)
         print(f"{adjusted_old_dt=}")
 
         assert formatted_new_dt == adjusted_old_dt
 
 
+class TestTimedeltaMatchStr:
+    """Test formatted re string for timedelta."""
+
+    ####################################################################
+    # test_timedelta_match_str
+    ####################################################################
+    @pytest.mark.parametrize("num_days_arg", (-999999999, -1, 0, 1, 999999999))
+    @pytest.mark.parametrize(
+        "num_hours_arg",
+        (
+            0,
+            1,
+            2,
+            11,
+            20,
+            21,
+            23,
+        ),
+    )
+    @pytest.mark.parametrize("num_mins_arg", (0, 1, 2, 9, 10, 58, 59))
+    @pytest.mark.parametrize("num_secs_arg", (0, 1, 2, 9, 11, 58, 59))
+    @pytest.mark.parametrize("num_usecs_arg", (0, 1, 2, 9, 10, 11, 100000, 999999))
+    def test_timedelta_match_str(
+        self,
+        num_days_arg: int,
+        num_hours_arg: int,
+        num_mins_arg: int,
+        num_secs_arg: int,
+        num_usecs_arg: int,
+        capsys: pytest.CaptureFixture[str],
+    ) -> None:
+        """Test the timedelta match string.
+
+        Args:
+            num_days_arg: number days
+            num_hours_arg: number hours
+            num_mins_arg: number minutes
+            num_secs_arg: number seconds
+            num_usecs_arg: number micro seconds
+
+        """
+        time_delta = timedelta(
+            days=num_days_arg,
+            hours=num_hours_arg,
+            minutes=num_mins_arg,
+            seconds=num_secs_arg,
+            microseconds=num_usecs_arg,
+        )
+        logger.debug(f"time_delta: {time_delta}")
+        elapsed_time_pattern_regex = re.compile(f"time_delta: {timedelta_match_string}")
+        print(f"time_delta: {time_delta}")
+
+        captured = capsys.readouterr().out
+        captured_lines = captured.split("\n")
+
+        assert elapsed_time_pattern_regex.match(captured_lines[0])
+        assert elapsed_time_pattern_regex.fullmatch(captured_lines[0])
+
+    ####################################################################
+    # test_timedelta_fail_match_str
+    ####################################################################
+    @pytest.mark.parametrize(
+        "num_days_arg",
+        (
+            "skip",
+            "1 day, ",
+            "1 days, ",
+            "-9999999999 days, ",
+            "=2 days, ",
+            "9999999999 days, ",
+        ),
+    )
+    @pytest.mark.parametrize("num_hours_arg", ("22:", "01", "111:", "24:", "hh:"))
+    @pytest.mark.parametrize("num_mins_arg", ("59:", "33", "55:55:", "63", "mm:"))
+    @pytest.mark.parametrize("num_secs_arg", ("42", "333", "11:11", "99", "ss"))
+    @pytest.mark.parametrize(
+        "num_usecs_arg",
+        ("skip", ".424242", ".3", "11:11", ".9999999", ",123456", "usecs"),
+    )
+    def test_timedelta_fail_match_str(
+        self,
+        num_days_arg: str,
+        num_hours_arg: str,
+        num_mins_arg: str,
+        num_secs_arg: str,
+        num_usecs_arg: str,
+        capsys: pytest.CaptureFixture[str],
+    ) -> None:
+        """Test the timedelta match string.
+
+        Args:
+            num_days_arg: number days
+            num_hours_arg: number hours
+            num_mins_arg: number minutes
+            num_secs_arg: number seconds
+            num_usecs_arg: number micro seconds
+
+        """
+        good_time = False
+        if (
+            num_days_arg in ("skip", "1 day, ")
+            and num_hours_arg == "22:"
+            and num_mins_arg == "59:"
+            and num_secs_arg == "42"
+            and num_usecs_arg in ("skip", ".424242")
+        ):
+            good_time = True
+
+        elapsed_time_pattern_regex = re.compile(f"time_delta: {timedelta_match_string}")
+        time_delta = "time_delta: "
+        if num_days_arg != "skip":
+            time_delta = f"{time_delta}{num_days_arg}"
+
+        time_delta = f"{time_delta}{num_hours_arg}{num_mins_arg}{num_secs_arg}"
+
+        if num_usecs_arg != "skip":
+            time_delta = f"{time_delta}{num_usecs_arg}"
+
+        logger.debug(f"{good_time=}, {time_delta}")
+
+        print(f"{time_delta}")
+
+        captured = capsys.readouterr().out
+        captured_lines = captured.split("\n")
+
+        if good_time:
+            assert elapsed_time_pattern_regex.match(captured_lines[0])
+            assert elapsed_time_pattern_regex.fullmatch(captured_lines[0])
+        else:
+            assert not elapsed_time_pattern_regex.fullmatch(captured_lines[0])
+
+
 class TestStartStopHeader:
     """TestStartStopHeader class."""
 
     @pytest.fixture(scope="class")
     def hdr(self) -> "StartStopHeader":
         """Method hdr.
```

### Comparing `scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_timer.py` & `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_timer.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/tests/test_scottbrian_utils/test_unique_ts.py` & `scottbrian_utils-4.0.0/tests/test_scottbrian_utils/test_unique_ts.py`

 * *Files identical despite different names*

### Comparing `scottbrian_utils-3.0.0/tox.ini` & `scottbrian_utils-4.0.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 commands =
     bandit -r src
 
 [testenv:py{312}-safety]
 description = invoke safety to verify security
 deps =
     safety
-    pip>=21.1.1
+    pip~=24.0
 
 commands =
     safety check
 
 [check-manifest]
 ignore =
     .idea/codeStyles/codeStyleConfig.xml
@@ -86,16 +86,16 @@
 
 deps =
     mypy
     pytest
     sybil
 
 commands =
-    python -m pip show mypy
-    python -m pip show pytest
+;    python -m pip show mypy
+;    python -m pip show pytest
     mypy src/scottbrian_utils/
     mypy tests/test_scottbrian_utils/ --cache-dir=/dev/null --show-absolute-path
 ;    mypy src/scottbrian_utils/diag_msg.py
 ;    mypy src/scottbrian_utils/file_catalog.py
 ;    mypy src/scottbrian_utils/flower_box.py
 ;    mypy src/scottbrian_utils/log_verifier.py
 ;    mypy src/scottbrian_utils/msgs.py
@@ -156,14 +156,16 @@
 deps =
     pytest
     pytest-cov
     sybil
 
 commands =
     pytest --cov=scottbrian_utils --cov-report=term --cov-report=html -p no:threadexception {posargs}
+;    pytest --cov=scottbrian_utils --cov-report=term --cov-report=html -m cover -p no:threadexception tests/test_scottbrian_utils/test_log_verifier.py
+;    pytest --cov=scottbrian_utils --cov-report=term --cov-report=html -p no:threadexception tests/test_scottbrian_utils/test_msgs.py
 ;    pytest --cov=scottbrian_utils --cov-report=term --cov-report=html -p no:threadexception -m cover2 {posargs}
 
 [testenv:py{312}-pytest]
 description = invoke pytest on the package
 deps =
     pytest
     sybil
```

### Comparing `scottbrian_utils-3.0.0/type_stubs/mypywrapt/adjust_src/adjust_src.py` & `scottbrian_utils-4.0.0/type_stubs/mypywrapt/adjust_src/adjust_src.py`

 * *Files identical despite different names*

