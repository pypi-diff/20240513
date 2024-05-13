# Comparing `tmp/plico-0.26.0.tar.gz` & `tmp/plico-0.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plico-0.26.0.tar", last modified: Wed Jan 11 11:24:12 2023, max compression
+gzip compressed data, was "plico-0.27.0.tar", last modified: Mon May 13 14:00:01 2024, max compression
```

## Comparing `plico-0.26.0.tar` & `plico-0.27.0.tar`

### file list

```diff
@@ -1,89 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:24:12.401634 plico-0.26.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-11 11:24:02.000000 plico-0.26.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-11 11:24:02.000000 plico-0.26.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-01-11 11:24:12.401634 plico-0.26.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-01-11 11:24:02.000000 plico-0.26.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:24:12.389634 plico-0.26.0/plico/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 11:24:02.000000 plico-0.26.0/plico/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-11 11:24:02.000000 plico-0.26.0/plico/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:24:12.389634 plico-0.26.0/plico/client/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 11:24:02.000000 plico-0.26.0/plico/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-11 11:24:02.000000 plico-0.26.0/plico/client/hackerable_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-01-11 11:24:02.000000 plico-0.26.0/plico/client/serverinfo_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:24:12.389634 plico-0.26.0/plico/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 11:24:02.000000 plico-0.26.0/plico/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-01-11 11:24:02.000000 plico-0.26.0/plico/rpc/abstract_remote_procedure_call.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-01-11 11:24:02.000000 plico-0.26.0/plico/rpc/dummy_remote_procedure_call.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-01-11 11:24:02.000000 plico-0.26.0/plico/rpc/dummy_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-01-11 11:24:02.000000 plico-0.26.0/plico/rpc/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-11 11:24:02.000000 plico-0.26.0/plico/rpc/zmq_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-01-11 11:24:02.000000 plico-0.26.0/plico/rpc/zmq_remote_procedure_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:24:12.389634 plico-0.26.0/plico/types/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 11:24:02.000000 plico-0.26.0/plico/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-01-11 11:24:02.000000 plico-0.26.0/plico/types/server_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-01-11 11:24:02.000000 plico-0.26.0/plico/types/zernike_coefficients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:24:12.397634 plico-0.26.0/plico/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/addtree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/calibration_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/concurrent_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/config_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/control_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/convergeable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/fake_convergeable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/fake_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/fits_file_based_calibration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/hackerable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/image_moments.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/kill_process_by_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/plico_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/serverinfoable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/snapshotable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/starter_script_creator_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/stepable.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/timekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/usb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-01-11 11:24:02.000000 plico-0.26.0/plico/utils/zernike_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:24:12.389634 plico-0.26.0/plico.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-01-11 11:24:12.000000 plico-0.26.0/plico.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-01-11 11:24:12.000000 plico-0.26.0/plico.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 11:24:12.000000 plico-0.26.0/plico.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-11 11:24:12.000000 plico-0.26.0/plico.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-11 11:24:12.000000 plico-0.26.0/plico.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 11:24:12.401634 plico-0.26.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-01-11 11:24:02.000000 plico-0.26.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:24:12.397634 plico-0.26.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 11:24:02.000000 plico-0.26.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-01-11 11:24:02.000000 plico-0.26.0/test/fake_time_mod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:24:12.397634 plico-0.26.0/test/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 11:24:02.000000 plico-0.26.0/test/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-11 11:24:02.000000 plico-0.26.0/test/rpc/zmq_ports_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-01-11 11:24:02.000000 plico-0.26.0/test/rpc/zmq_remote_procedure_call_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16705 2023-01-11 11:24:02.000000 plico-0.26.0/test/test_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:24:12.401634 plico-0.26.0/test/types/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 11:24:02.000000 plico-0.26.0/test/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-01-11 11:24:02.000000 plico-0.26.0/test/types/zernike_coefficients_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 11:24:12.401634 plico-0.26.0/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 11:24:02.000000 plico-0.26.0/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-01-11 11:24:02.000000 plico-0.26.0/test/utils/addtree_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-01-11 11:24:02.000000 plico-0.26.0/test/utils/barrier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-01-11 11:24:02.000000 plico-0.26.0/test/utils/calibration_installer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-01-11 11:24:02.000000 plico-0.26.0/test/utils/concurrent_loop_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-01-11 11:24:02.000000 plico-0.26.0/test/utils/configExample.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-01-11 11:24:02.000000 plico-0.26.0/test/utils/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16912 2023-01-11 11:24:02.000000 plico-0.26.0/test/utils/executor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-01-11 11:24:02.000000 plico-0.26.0/test/utils/hackerable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-01-11 11:24:02.000000 plico-0.26.0/test/utils/snapshotable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-01-11 11:24:02.000000 plico-0.26.0/test/utils/starter_script_creator_base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-01-11 11:24:02.000000 plico-0.26.0/test/utils/zernike_generator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:01.395769 plico-0.27.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-13 13:59:57.000000 plico-0.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 13:59:57.000000 plico-0.27.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-05-13 14:00:01.395769 plico-0.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-13 13:59:57.000000 plico-0.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:01.379769 plico-0.27.0/plico/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:59:57.000000 plico-0.27.0/plico/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 13:59:57.000000 plico-0.27.0/plico/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:01.383769 plico-0.27.0/plico/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:59:57.000000 plico-0.27.0/plico/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-13 13:59:57.000000 plico-0.27.0/plico/client/hackerable_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-13 13:59:57.000000 plico-0.27.0/plico/client/serverinfo_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:01.383769 plico-0.27.0/plico/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:59:57.000000 plico-0.27.0/plico/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-13 13:59:57.000000 plico-0.27.0/plico/rpc/abstract_remote_procedure_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-13 13:59:57.000000 plico-0.27.0/plico/rpc/dummy_remote_procedure_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-13 13:59:57.000000 plico-0.27.0/plico/rpc/dummy_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-13 13:59:57.000000 plico-0.27.0/plico/rpc/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-13 13:59:57.000000 plico-0.27.0/plico/rpc/zmq_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-13 13:59:57.000000 plico-0.27.0/plico/rpc/zmq_remote_procedure_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:01.383769 plico-0.27.0/plico/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:59:57.000000 plico-0.27.0/plico/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-13 13:59:57.000000 plico-0.27.0/plico/types/server_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-13 13:59:57.000000 plico-0.27.0/plico/types/zernike_coefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:01.391769 plico-0.27.0/plico/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/addtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/calibration_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/concurrent_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/config_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/control_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/convergeable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/fake_convergeable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/fake_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/fits_file_based_calibration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/hackerable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/image_moments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/kill_process_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/plico_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/reconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/serial_or_usb_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/serverinfoable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/snapshotable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/starter_script_creator_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/stepable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/timekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-05-13 13:59:57.000000 plico-0.27.0/plico/utils/zernike_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:01.395769 plico-0.27.0/plico.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-05-13 14:00:01.000000 plico-0.27.0/plico.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-13 14:00:01.000000 plico-0.27.0/plico.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:00:01.000000 plico-0.27.0/plico.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 14:00:01.000000 plico-0.27.0/plico.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 14:00:01.000000 plico-0.27.0/plico.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:00:01.395769 plico-0.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-13 13:59:57.000000 plico-0.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:01.391769 plico-0.27.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:59:57.000000 plico-0.27.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-13 13:59:57.000000 plico-0.27.0/test/fake_time_mod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:01.391769 plico-0.27.0/test/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:59:57.000000 plico-0.27.0/test/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-13 13:59:57.000000 plico-0.27.0/test/rpc/zmq_ports_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-05-13 13:59:57.000000 plico-0.27.0/test/rpc/zmq_remote_procedure_call_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16705 2024-05-13 13:59:57.000000 plico-0.27.0/test/test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:01.391769 plico-0.27.0/test/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:59:57.000000 plico-0.27.0/test/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-13 13:59:57.000000 plico-0.27.0/test/types/zernike_coefficients_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:01.395769 plico-0.27.0/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:59:57.000000 plico-0.27.0/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-13 13:59:57.000000 plico-0.27.0/test/utils/addtree_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-13 13:59:57.000000 plico-0.27.0/test/utils/barrier_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-13 13:59:57.000000 plico-0.27.0/test/utils/calibration_installer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-13 13:59:57.000000 plico-0.27.0/test/utils/concurrent_loop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-13 13:59:57.000000 plico-0.27.0/test/utils/configExample.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-13 13:59:57.000000 plico-0.27.0/test/utils/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-13 13:59:57.000000 plico-0.27.0/test/utils/control_loop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16912 2024-05-13 13:59:57.000000 plico-0.27.0/test/utils/executor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-13 13:59:57.000000 plico-0.27.0/test/utils/hackerable_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-13 13:59:57.000000 plico-0.27.0/test/utils/snapshotable_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-13 13:59:57.000000 plico-0.27.0/test/utils/starter_script_creator_base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-13 13:59:57.000000 plico-0.27.0/test/utils/zernike_generator_test.py
```

### Comparing `plico-0.26.0/LICENSE` & `plico-0.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/PKG-INFO` & `plico-0.27.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 Metadata-Version: 2.1
 Name: plico
-Version: 0.26.0
+Version: 0.27.0
 Summary: Python Laboratory Instrumentation COntrol
 Home-page: https://github.com/lbusoni/plico
 Author: Lorenzo Busoni
 Author-email: lorenzo.busoni@inaf.it
 License: MIT
 Keywords: laboratory,instrumentation controllaboratory,instrumentation control
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: psutil
+Requires-Dist: configparser
+Requires-Dist: six
+Requires-Dist: appdirs
+Requires-Dist: pyzmq
+Requires-Dist: futures; python_version == "2.7"
+Requires-Dist: astropy
+Requires-Dist: pyserial
 
 # PLICO: Python Laboratory Instrumentation COntrol
 
  ![Python package](https://github.com/ArcetriAdaptiveOptics/plico/workflows/Python%20package/badge.svg)
  [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico/branch/master/graph/badge.svg?token=04PRSBMW11)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico)
  [![Documentation Status](https://readthedocs.org/projects/plico/badge/?version=latest)](https://plico.readthedocs.io/en/latest/?badge=latest)
  [![PyPI version][pypiversion]][pypiversionlink]
@@ -35,18 +44,23 @@
  --- | --- | --- | --- | --- 
 [plico_motor](https://github.com/ArcetriAdaptiveOptics/plico_motor) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_motor/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_motor/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_motor) | [![Documentation Status](https://readthedocs.org/projects/plico_motor/badge/?version=latest)](https://plico_motor.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-motor.svg)](https://badge.fury.io/py/plico-motor) 
 [plico_motor_server](https://github.com/ArcetriAdaptiveOptics/plico_motor_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_motor_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_motor_server/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_motor_server) |  [![Documentation Status](https://readthedocs.org/projects/plico_motor_server/badge/?version=latest)](https://plico_motor_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-motor-server.svg)](https://badge.fury.io/py/plico-motor-server) |
 [pysilico](https://github.com/ArcetriAdaptiveOptics/pysilico) | ![Python package](https://github.com/ArcetriAdaptiveOptics/pysilico/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico/branch/master/graph/badge.svg?token=GTDOW6IWDE)](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico) | [![Documentation Status](https://readthedocs.org/projects/pysilico/badge/?version=latest)](https://pysilico.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/pysilico.svg)](https://badge.fury.io/py/pysilico)
 [pysilico_server](https://github.com/ArcetriAdaptiveOptics/pysilico_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/pysilico_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico_server/branch/master/graph/badge.svg?token=04PRSBMW11)](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico_server) | [![Documentation Status](https://readthedocs.org/projects/pysilico_server/badge/?version=latest)](https://pysilico_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/pysilico-server.svg)](https://badge.fury.io/py/pysilico-server)
 [plico_dm](https://github.com/ArcetriAdaptiveOptics/plico_dm) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_dm/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm/branch/master/graph/badge.svg?token=OTSP5O5WCW)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm) | [![Documentation Status](https://readthedocs.org/projects/plico_dm/badge/?version=latest)](https://plico_dm.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-dm.svg)](https://badge.fury.io/py/plico-dm)
 [plico_dm_server](https://github.com/ArcetriAdaptiveOptics/plico_dm_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_dm_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm_server/branch/master/graph/badge.svg?token=L6E5WVO4O5)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm_server) | [![Documentation Status](https://readthedocs.org/projects/plico_dm_server/badge/?version=latest)](https://plico_dm_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-dm-server.svg)](https://badge.fury.io/py/plico-dm-server)
+[plico_dm_characterization](https://github.com/ArcetriAdaptiveOptics/plico_dm_characterization) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_dm_characterization/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm_characterization/branch/master/graph/badge.svg?token=TO8MHXVC5W)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm_characterization) | [![Documentation Status](https://readthedocs.org/projects/plico_dm_characterization/badge/?version=latest)](https://plico_dm_characterization.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-dm-characterization.svg)](https://badge.fury.io/py/plico-dm-characterization)
 [plico_interferometer](https://github.com/ArcetriAdaptiveOptics/plico_interferometer) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_interferometer/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer) | [![Documentation Status](https://readthedocs.org/projects/plico_interferometer/badge/?version=latest)](https://plico_interferometer.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-interferometer.svg)](https://badge.fury.io/py/plico-interferometer)
 [plico_interferometer_server](https://github.com/ArcetriAdaptiveOptics/plico_interferometer_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_interferometer_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer_server/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer_server) | [![Documentation Status](https://readthedocs.org/projects/plico_interferometer_server/badge/?version=latest)](https://plico_interferometer_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-interferometer-server.svg)](https://badge.fury.io/py/plico-interferometer-server)
+
+
+<!---
 [tipico](https://github.com/ArcetriAdaptiveOptics/tipico) | ![Python package](https://github.com/ArcetriAdaptiveOptics/tipico/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/tipico/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/tipico) | [![Documentation Status](https://readthedocs.org/projects/tipico/badge/?version=latest)](https://tipico.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/tipico.svg)](https://badge.fury.io/py/tipico)
 [tipico_server](https://github.com/ArcetriAdaptiveOptics/tipico_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/tipico_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/tipico_server/branch/master/graph/badge.svg?token=SLRM2OEX3B)](https://codecov.io/gh/ArcetriAdaptiveOptics/tipico_server) | [![Documentation Status](https://readthedocs.org/projects/tipico_server/badge/?version=latest)](https://tipico_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/tipico-server.svg)](https://badge.fury.io/py/tipico_server)
+--->
 
 
 
 [zmq]: http://zeromq.org
 [plico]: https://github.com/ArcetriAdaptiveOptics/plico
 [tipico]: https://github.com/ArcetriAdaptiveOptics/tipico
 [tipico-server]: https://github.com/ArcetriAdaptiveOptics/tipico_server
```

### Comparing `plico-0.26.0/README.md` & `plico-0.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -20,18 +20,23 @@
  --- | --- | --- | --- | --- 
 [plico_motor](https://github.com/ArcetriAdaptiveOptics/plico_motor) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_motor/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_motor/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_motor) | [![Documentation Status](https://readthedocs.org/projects/plico_motor/badge/?version=latest)](https://plico_motor.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-motor.svg)](https://badge.fury.io/py/plico-motor) 
 [plico_motor_server](https://github.com/ArcetriAdaptiveOptics/plico_motor_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_motor_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_motor_server/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_motor_server) |  [![Documentation Status](https://readthedocs.org/projects/plico_motor_server/badge/?version=latest)](https://plico_motor_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-motor-server.svg)](https://badge.fury.io/py/plico-motor-server) |
 [pysilico](https://github.com/ArcetriAdaptiveOptics/pysilico) | ![Python package](https://github.com/ArcetriAdaptiveOptics/pysilico/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico/branch/master/graph/badge.svg?token=GTDOW6IWDE)](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico) | [![Documentation Status](https://readthedocs.org/projects/pysilico/badge/?version=latest)](https://pysilico.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/pysilico.svg)](https://badge.fury.io/py/pysilico)
 [pysilico_server](https://github.com/ArcetriAdaptiveOptics/pysilico_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/pysilico_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico_server/branch/master/graph/badge.svg?token=04PRSBMW11)](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico_server) | [![Documentation Status](https://readthedocs.org/projects/pysilico_server/badge/?version=latest)](https://pysilico_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/pysilico-server.svg)](https://badge.fury.io/py/pysilico-server)
 [plico_dm](https://github.com/ArcetriAdaptiveOptics/plico_dm) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_dm/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm/branch/master/graph/badge.svg?token=OTSP5O5WCW)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm) | [![Documentation Status](https://readthedocs.org/projects/plico_dm/badge/?version=latest)](https://plico_dm.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-dm.svg)](https://badge.fury.io/py/plico-dm)
 [plico_dm_server](https://github.com/ArcetriAdaptiveOptics/plico_dm_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_dm_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm_server/branch/master/graph/badge.svg?token=L6E5WVO4O5)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm_server) | [![Documentation Status](https://readthedocs.org/projects/plico_dm_server/badge/?version=latest)](https://plico_dm_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-dm-server.svg)](https://badge.fury.io/py/plico-dm-server)
+[plico_dm_characterization](https://github.com/ArcetriAdaptiveOptics/plico_dm_characterization) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_dm_characterization/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm_characterization/branch/master/graph/badge.svg?token=TO8MHXVC5W)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm_characterization) | [![Documentation Status](https://readthedocs.org/projects/plico_dm_characterization/badge/?version=latest)](https://plico_dm_characterization.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-dm-characterization.svg)](https://badge.fury.io/py/plico-dm-characterization)
 [plico_interferometer](https://github.com/ArcetriAdaptiveOptics/plico_interferometer) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_interferometer/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer) | [![Documentation Status](https://readthedocs.org/projects/plico_interferometer/badge/?version=latest)](https://plico_interferometer.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-interferometer.svg)](https://badge.fury.io/py/plico-interferometer)
 [plico_interferometer_server](https://github.com/ArcetriAdaptiveOptics/plico_interferometer_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_interferometer_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer_server/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer_server) | [![Documentation Status](https://readthedocs.org/projects/plico_interferometer_server/badge/?version=latest)](https://plico_interferometer_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-interferometer-server.svg)](https://badge.fury.io/py/plico-interferometer-server)
+
+
+<!---
 [tipico](https://github.com/ArcetriAdaptiveOptics/tipico) | ![Python package](https://github.com/ArcetriAdaptiveOptics/tipico/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/tipico/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/tipico) | [![Documentation Status](https://readthedocs.org/projects/tipico/badge/?version=latest)](https://tipico.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/tipico.svg)](https://badge.fury.io/py/tipico)
 [tipico_server](https://github.com/ArcetriAdaptiveOptics/tipico_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/tipico_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/tipico_server/branch/master/graph/badge.svg?token=SLRM2OEX3B)](https://codecov.io/gh/ArcetriAdaptiveOptics/tipico_server) | [![Documentation Status](https://readthedocs.org/projects/tipico_server/badge/?version=latest)](https://tipico_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/tipico-server.svg)](https://badge.fury.io/py/tipico_server)
+--->
 
 
 
 [zmq]: http://zeromq.org
 [plico]: https://github.com/ArcetriAdaptiveOptics/plico
 [tipico]: https://github.com/ArcetriAdaptiveOptics/tipico
 [tipico-server]: https://github.com/ArcetriAdaptiveOptics/tipico_server
```

### Comparing `plico-0.26.0/plico/client/hackerable_client.py` & `plico-0.27.0/plico/client/hackerable_client.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/client/serverinfo_client.py` & `plico-0.27.0/plico/client/serverinfo_client.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/rpc/abstract_remote_procedure_call.py` & `plico-0.27.0/plico/rpc/abstract_remote_procedure_call.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/rpc/dummy_remote_procedure_call.py` & `plico-0.27.0/plico/rpc/dummy_remote_procedure_call.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/rpc/dummy_sockets.py` & `plico-0.27.0/plico/rpc/dummy_sockets.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/rpc/sockets.py` & `plico-0.27.0/plico/rpc/sockets.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/rpc/zmq_ports.py` & `plico-0.27.0/plico/rpc/zmq_ports.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/rpc/zmq_remote_procedure_call.py` & `plico-0.27.0/plico/rpc/zmq_remote_procedure_call.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/types/zernike_coefficients.py` & `plico-0.27.0/plico/types/zernike_coefficients.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/addtree.py` & `plico-0.27.0/plico/utils/addtree.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/barrier.py` & `plico-0.27.0/plico/utils/barrier.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/base_runner.py` & `plico-0.27.0/plico/utils/base_runner.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/calibration_installer.py` & `plico-0.27.0/plico/utils/calibration_installer.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/concurrent_loop.py` & `plico-0.27.0/plico/utils/concurrent_loop.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,44 +38,36 @@
         self._flagAsDone()
 
     @synchronized("_runEnabledCondition")
     def _waitForNextStep(self):
         if self._runEnabled:
             self._runEnabledCondition.wait(self._interStepTimeSec)
 
-    def _markAsClosed(self):
-        self._openEvent.clear()
-        self._closeEvent.set()
-
-    def _markAsOpen(self):
-        self._openEvent.set()
-        self._closeEvent.clear()
-
     def _step(self):
         if self._closedFunc():
             self._stepCounter.inc()
             self._convergable.performOneConvergenceStep()
         else:
             self._convergable.measureConvergence()
 
     def _flagAsDone(self):
         self._doneEvent.set()
-        assert self._doneEvent.isSet()
+        assert self._doneEvent.is_set()
 
     def _isDone(self):
-        return self._doneEvent.isSet()
+        return self._doneEvent.is_set()
 
     @synchronized("_runEnabledCondition")
     def _isRunEnabled(self):
         return self._runEnabled
 
     @synchronized("_runEnabledCondition")
     def _disableRun(self):
         self._runEnabled = False
-        self._runEnabledCondition.notifyAll()
+        self._runEnabledCondition.notify_all()
 
     def setStopDurationLimitSec(self, limitSec):
         self._stopDurationLimitSec = limitSec
 
     def _waitForDone(self):
         self._doneEvent.wait(self._stopDurationLimitSec)
         if not self._isDone():
@@ -156,15 +148,16 @@
     @override
     def performOnePass(self):
         if self.isInitialized():
             if not self.isClosed():
                 self._stepCounter.inc()
                 self._convergable.performOneConvergenceStep()
             else:
-                raise Exception("Loop is closed")
+                raise Exception(
+                    "Loop is closed, cannot execute performOnePass")
         else:
             self._logger.error("%s is not yet initialized" % self._name)
 #             raise Exception("%s is not yet initialized" % self._name)
 
     @synchronized("_mtx")
     @override
     def close(self):
```

### Comparing `plico-0.26.0/plico/utils/config_file_manager.py` & `plico-0.27.0/plico/utils/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/configuration.py` & `plico-0.27.0/plico/utils/configuration.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,82 +5,65 @@
 import configparser
 import appdirs
 from pkg_resources import resource_filename
 from plico.utils.calibration_installer import CalibrationInstaller
 from plico.utils.addtree import mkdirp
 
 
-__version__= "$Id: configuration.py 50 2018-04-26 21:42:20Z lbusoni $"
-
-
 class LogFolderManager():
 
     def __init__(self, appDirs):
-        self._appdirs= appDirs
-
+        self._appdirs = appDirs
 
     def getLogFolderPath(self):
         return self._appdirs.user_log_dir
 
-
     def doesLogFolderExists(self):
         return os.path.isdir(self.getLogFolderPath())
 
-
     def createLogFolder(self):
         mkdirp(os.path.dirname(self.getLogFolderPath()))
 
 
 class Configuration(object):
 
-
     def __init__(self):
-        NOT_INITIALIZED= None
+        NOT_INITIALIZED = None
         self._cfg = configparser.ConfigParser()
 
-
     def networkHostName(self, section):
         return self.getValue(section, 'host')
 
-
     def calibrationRootDir(self):
         return self._getCalibDir()
 
-
     def loggingDir(self):
         return self._getLogDir()
 
-
     def deviceModel(self, section):
         return self.getValue(section, 'model')
 
-
     def deviceName(self, section):
         return self.getValue(section, 'name')
 
-
     def basePort(self, section):
         return self.getValue(section, 'port', getint=True)
 
-
     def logLevel(self, section):
         return self.getValue(section, 'log_level')
 
-
     def numberedSectionList(self, prefix=''):
-        pattern = prefix+'\\d+'
+        pattern = prefix + '\\d+'
         return list(filter(lambda x: re.search(pattern, x), self._cfg.sections()))
 
-
     def _assertSectionExists(self, section):
         if section not in self._cfg.sections():
             raise Exception('Section "%s" not found in configuration file' %
                             section)
 
-
     def getValue(self, section, entry, getint=False,
                  getfloat=False, getboolean=False):
         if entry not in list(dict(self._cfg.items(section)).keys()):
             raise KeyError(
                 'Section "%s" must contain a "%s" entry. File is %s. Keys %s' %
                 (section, entry, self._filename,
                  list(dict(self._cfg.items(section)).keys())))
@@ -105,49 +88,42 @@
                 raise ValueError(
                     'Value for entry "%s" in section "%s"'
                     ' must be a boolean' % (entry, section))
         else:
             value = self._cfg.get(section, entry)
         return value
 
-
     def load(self, filename):
         if not os.path.exists(filename):
             raise Exception('Configuration file not found: %s' % filename)
         self._cfg.read(filename)
-        self._filename= filename
-
+        self._filename = filename
 
     def _getLogDir(self):
         try:
             return self.getValue('global', 'force_log_dir')
         except Exception:
-            lfm= LogFolderManager(self._getAppDirs())
+            lfm = LogFolderManager(self._getAppDirs())
             lfm.createLogFolder()
             return lfm.getLogFolderPath()
 
-
     def _getCalibDir(self):
         try:
             return self.getValue('global', 'force_calib_folder_dest')
         except Exception:
-            calibInst= CalibrationInstaller(
+            calibInst = CalibrationInstaller(
                 self._getAppDirs(), self._getPythonPackageName())
             calibInst.installCalibrationFilesFromPackage()
             return calibInst.getCalibrationFolderPath()
 
-
     def _getPythonPackageName(self):
-            return self.getValue('global', 'python_package_name')
-
+        return self.getValue('global', 'python_package_name')
 
     def _getAppName(self):
-            return self.getValue('global', 'app_name')
-
+        return self.getValue('global', 'app_name')
 
     def _getAppAuthor(self):
-            return self.getValue('global', 'app_author')
-
+        return self.getValue('global', 'app_author')
 
     def _getAppDirs(self):
         return appdirs.AppDirs(self._getAppName(),
                                self._getAppAuthor())
```

### Comparing `plico-0.26.0/plico/utils/control_loop.py` & `plico-0.27.0/plico/utils/control_loop.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/decorator.py` & `plico-0.27.0/plico/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/executor.py` & `plico-0.27.0/plico/utils/executor.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/fake_convergeable.py` & `plico-0.27.0/plico/utils/fake_convergeable.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         return self._measureConvergenceInvocationCnt
 
     def requestPanic(self):
         self._exceptionRequested = True
 
     @synchronized("_condition")
     def unblockStep(self):
-        self._condition.notifyAll()
+        self._condition.notify_all()
         self._stepBlockingEnabled = False
 
     @synchronized("_condition")
     def blockStep(self):
         self._stepBlockingEnabled = True
 
     @synchronized("_condition")
```

### Comparing `plico-0.26.0/plico/utils/fake_loop.py` & `plico-0.27.0/plico/utils/fake_loop.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/hackerable.py` & `plico-0.27.0/plico/utils/hackerable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from plico.utils.logger import Logger
 
 
-__version__= "$Id: hackerable.py 25 2018-01-26 19:00:40Z lbusoni $"
-
-
 class Hackerable(object):
 
     def __init__(self, logger=None):
         self._hackerableExecuteCnt= 0
         self._hackerableEvalCnt= 0
         if logger is None:
             self._logger= Logger.of('Hackerable')
```

### Comparing `plico-0.26.0/plico/utils/image_moments.py` & `plico-0.27.0/plico/utils/image_moments.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/kill_process_by_name.py` & `plico-0.27.0/plico/utils/kill_process_by_name.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/logger.py` & `plico-0.27.0/plico/utils/logger.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/loop.py` & `plico-0.27.0/plico/utils/loop.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/plico_scipy.py` & `plico-0.27.0/plico/utils/plico_scipy.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/sandbox.py` & `plico-0.27.0/plico/utils/sandbox.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/serverinfoable.py` & `plico-0.27.0/plico/utils/serverinfoable.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/snapshotable.py` & `plico-0.27.0/plico/utils/snapshotable.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/starter_script_creator_base.py` & `plico-0.27.0/plico/utils/starter_script_creator_base.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/timekeeper.py` & `plico-0.27.0/plico/utils/timekeeper.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/timestamp.py` & `plico-0.27.0/plico/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico/utils/zernike_generator.py` & `plico-0.27.0/plico/utils/zernike_generator.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/plico.egg-info/PKG-INFO` & `plico-0.27.0/plico.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 Metadata-Version: 2.1
 Name: plico
-Version: 0.26.0
+Version: 0.27.0
 Summary: Python Laboratory Instrumentation COntrol
 Home-page: https://github.com/lbusoni/plico
 Author: Lorenzo Busoni
 Author-email: lorenzo.busoni@inaf.it
 License: MIT
 Keywords: laboratory,instrumentation controllaboratory,instrumentation control
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: psutil
+Requires-Dist: configparser
+Requires-Dist: six
+Requires-Dist: appdirs
+Requires-Dist: pyzmq
+Requires-Dist: futures; python_version == "2.7"
+Requires-Dist: astropy
+Requires-Dist: pyserial
 
 # PLICO: Python Laboratory Instrumentation COntrol
 
  ![Python package](https://github.com/ArcetriAdaptiveOptics/plico/workflows/Python%20package/badge.svg)
  [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico/branch/master/graph/badge.svg?token=04PRSBMW11)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico)
  [![Documentation Status](https://readthedocs.org/projects/plico/badge/?version=latest)](https://plico.readthedocs.io/en/latest/?badge=latest)
  [![PyPI version][pypiversion]][pypiversionlink]
@@ -35,18 +44,23 @@
  --- | --- | --- | --- | --- 
 [plico_motor](https://github.com/ArcetriAdaptiveOptics/plico_motor) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_motor/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_motor/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_motor) | [![Documentation Status](https://readthedocs.org/projects/plico_motor/badge/?version=latest)](https://plico_motor.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-motor.svg)](https://badge.fury.io/py/plico-motor) 
 [plico_motor_server](https://github.com/ArcetriAdaptiveOptics/plico_motor_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_motor_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_motor_server/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_motor_server) |  [![Documentation Status](https://readthedocs.org/projects/plico_motor_server/badge/?version=latest)](https://plico_motor_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-motor-server.svg)](https://badge.fury.io/py/plico-motor-server) |
 [pysilico](https://github.com/ArcetriAdaptiveOptics/pysilico) | ![Python package](https://github.com/ArcetriAdaptiveOptics/pysilico/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico/branch/master/graph/badge.svg?token=GTDOW6IWDE)](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico) | [![Documentation Status](https://readthedocs.org/projects/pysilico/badge/?version=latest)](https://pysilico.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/pysilico.svg)](https://badge.fury.io/py/pysilico)
 [pysilico_server](https://github.com/ArcetriAdaptiveOptics/pysilico_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/pysilico_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico_server/branch/master/graph/badge.svg?token=04PRSBMW11)](https://codecov.io/gh/ArcetriAdaptiveOptics/pysilico_server) | [![Documentation Status](https://readthedocs.org/projects/pysilico_server/badge/?version=latest)](https://pysilico_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/pysilico-server.svg)](https://badge.fury.io/py/pysilico-server)
 [plico_dm](https://github.com/ArcetriAdaptiveOptics/plico_dm) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_dm/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm/branch/master/graph/badge.svg?token=OTSP5O5WCW)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm) | [![Documentation Status](https://readthedocs.org/projects/plico_dm/badge/?version=latest)](https://plico_dm.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-dm.svg)](https://badge.fury.io/py/plico-dm)
 [plico_dm_server](https://github.com/ArcetriAdaptiveOptics/plico_dm_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_dm_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm_server/branch/master/graph/badge.svg?token=L6E5WVO4O5)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm_server) | [![Documentation Status](https://readthedocs.org/projects/plico_dm_server/badge/?version=latest)](https://plico_dm_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-dm-server.svg)](https://badge.fury.io/py/plico-dm-server)
+[plico_dm_characterization](https://github.com/ArcetriAdaptiveOptics/plico_dm_characterization) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_dm_characterization/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm_characterization/branch/master/graph/badge.svg?token=TO8MHXVC5W)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_dm_characterization) | [![Documentation Status](https://readthedocs.org/projects/plico_dm_characterization/badge/?version=latest)](https://plico_dm_characterization.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-dm-characterization.svg)](https://badge.fury.io/py/plico-dm-characterization)
 [plico_interferometer](https://github.com/ArcetriAdaptiveOptics/plico_interferometer) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_interferometer/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer) | [![Documentation Status](https://readthedocs.org/projects/plico_interferometer/badge/?version=latest)](https://plico_interferometer.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-interferometer.svg)](https://badge.fury.io/py/plico-interferometer)
 [plico_interferometer_server](https://github.com/ArcetriAdaptiveOptics/plico_interferometer_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_interferometer_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer_server/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer_server) | [![Documentation Status](https://readthedocs.org/projects/plico_interferometer_server/badge/?version=latest)](https://plico_interferometer_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/plico-interferometer-server.svg)](https://badge.fury.io/py/plico-interferometer-server)
+
+
+<!---
 [tipico](https://github.com/ArcetriAdaptiveOptics/tipico) | ![Python package](https://github.com/ArcetriAdaptiveOptics/tipico/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/tipico/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/tipico) | [![Documentation Status](https://readthedocs.org/projects/tipico/badge/?version=latest)](https://tipico.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/tipico.svg)](https://badge.fury.io/py/tipico)
 [tipico_server](https://github.com/ArcetriAdaptiveOptics/tipico_server) | ![Python package](https://github.com/ArcetriAdaptiveOptics/tipico_server/workflows/Python%20package/badge.svg) | [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/tipico_server/branch/master/graph/badge.svg?token=SLRM2OEX3B)](https://codecov.io/gh/ArcetriAdaptiveOptics/tipico_server) | [![Documentation Status](https://readthedocs.org/projects/tipico_server/badge/?version=latest)](https://tipico_server.readthedocs.io/en/latest/?badge=latest) | [![PyPI version](https://badge.fury.io/py/tipico-server.svg)](https://badge.fury.io/py/tipico_server)
+--->
 
 
 
 [zmq]: http://zeromq.org
 [plico]: https://github.com/ArcetriAdaptiveOptics/plico
 [tipico]: https://github.com/ArcetriAdaptiveOptics/tipico
 [tipico-server]: https://github.com/ArcetriAdaptiveOptics/tipico_server
```

### Comparing `plico-0.26.0/plico.egg-info/SOURCES.txt` & `plico-0.27.0/plico.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,23 +40,24 @@
 plico/utils/fits_file_based_calibration_manager.py
 plico/utils/hackerable.py
 plico/utils/image_moments.py
 plico/utils/kill_process_by_name.py
 plico/utils/logger.py
 plico/utils/loop.py
 plico/utils/plico_scipy.py
+plico/utils/reconnect.py
 plico/utils/sandbox.py
+plico/utils/serial_or_usb_connection.py
 plico/utils/serverinfoable.py
 plico/utils/snapshotable.py
 plico/utils/starter_script_creator_base.py
 plico/utils/stepable.py
 plico/utils/timekeeper.py
 plico/utils/timeout.py
 plico/utils/timestamp.py
-plico/utils/usb.py
 plico/utils/zernike_generator.py
 test/__init__.py
 test/fake_time_mod.py
 test/test_helper.py
 test/rpc/__init__.py
 test/rpc/zmq_ports_test.py
 test/rpc/zmq_remote_procedure_call_integration_test.py
@@ -65,12 +66,13 @@
 test/utils/__init__.py
 test/utils/addtree_test.py
 test/utils/barrier_test.py
 test/utils/calibration_installer_test.py
 test/utils/concurrent_loop_test.py
 test/utils/configExample.conf
 test/utils/configuration_test.py
+test/utils/control_loop_test.py
 test/utils/executor_test.py
 test/utils/hackerable_test.py
 test/utils/snapshotable_test.py
 test/utils/starter_script_creator_base_test.py
 test/utils/zernike_generator_test.py
```

### Comparing `plico-0.26.0/setup.py` & `plico-0.27.0/setup.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/test/fake_time_mod.py` & `plico-0.27.0/test/fake_time_mod.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/test/rpc/zmq_remote_procedure_call_integration_test.py` & `plico-0.27.0/test/rpc/zmq_remote_procedure_call_integration_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
 
 class ZmqRemoteProcedureCallTest(unittest.TestCase):
 
     THIS_DIR= os.path.abspath(os.path.dirname(__file__))
     TEST_DIR= os.path.join(THIS_DIR, "./tmp/")
     LOG_DIR= os.path.join(TEST_DIR, "log")
-    SERVER_LOG_PATH= os.path.join(LOG_DIR, "server.log")
+    PROCESS_MONITOR_LOG_PATH= os.path.join(LOG_DIR, "server.log")
     PUBLISHER_LOG_PATH= os.path.join(LOG_DIR, "publisher.log")
 
 
 
     def setUp(self, timeModule=time):
         logging.basicConfig(level=logging.DEBUG,
                             format='%(asctime)s %(message)s')
@@ -241,28 +241,28 @@
         Poller(5).check(MessageInFileProbe(runningMessage,
                                            logFilePath))
         return process
 
 
     def _spawnServer(self):
         self._server= self._spawnProcess(MyServer.commandToSpawn,
-                                         self.SERVER_LOG_PATH,
+                                         self.PROCESS_MONITOR_LOG_PATH,
                                          MyServer.RUNNING_MESSAGE)
 
 
     def _spawnPublisher(self):
         self._publisher= self._spawnProcess(MyPublisher.commandToSpawn,
                                             self.PUBLISHER_LOG_PATH,
                                             MyPublisher.RUNNING_MESSAGE)
 
 
 
     def tearDown(self):
         print('tearingDown')
-        TestHelper.dumpFileToStdout(self.SERVER_LOG_PATH)
+        TestHelper.dumpFileToStdout(self.PROCESS_MONITOR_LOG_PATH)
         TestHelper.dumpFileToStdout(self.PUBLISHER_LOG_PATH)
 
         if self._server is not None:
             TestHelper.terminateSubprocess(self._server)
         if self._publisher is not None:
             TestHelper.terminateSubprocess(self._publisher)
```

### Comparing `plico-0.26.0/test/test_helper.py` & `plico-0.27.0/test/test_helper.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/test/types/zernike_coefficients_test.py` & `plico-0.27.0/test/types/zernike_coefficients_test.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/test/utils/addtree_test.py` & `plico-0.27.0/test/utils/addtree_test.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/test/utils/barrier_test.py` & `plico-0.27.0/test/utils/barrier_test.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/test/utils/calibration_installer_test.py` & `plico-0.27.0/test/utils/calibration_installer_test.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/test/utils/concurrent_loop_test.py` & `plico-0.27.0/test/utils/concurrent_loop_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,17 +211,17 @@
                 N_ACTIONS = 5
                 r = random.randint(0, N_ACTIONS - 1)
                 if r == 0:
                     self._loop.close()
                 elif r == 1:
                     self._loop.open()
                 elif r == 2:
-                    self._loop.setGain(7.0)
+                    self._loop.initialize()
                 elif r == 3:
-                    self._loop.getGain()
+                    self._loop.hasConverged()
                 elif r == 4:
                     self._loop.isClosed()
                 else:
                     raise ValueError("Programming mistake")
 
         stressers = []
         for _ in range(0, N_THREADS):
```

### Comparing `plico-0.26.0/test/utils/configuration_test.py` & `plico-0.27.0/test/utils/configuration_test.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/test/utils/executor_test.py` & `plico-0.27.0/test/utils/executor_test.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/test/utils/hackerable_test.py` & `plico-0.27.0/test/utils/hackerable_test.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/test/utils/snapshotable_test.py` & `plico-0.27.0/test/utils/snapshotable_test.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/test/utils/starter_script_creator_base_test.py` & `plico-0.27.0/test/utils/starter_script_creator_base_test.py`

 * *Files identical despite different names*

### Comparing `plico-0.26.0/test/utils/zernike_generator_test.py` & `plico-0.27.0/test/utils/zernike_generator_test.py`

 * *Files identical despite different names*

