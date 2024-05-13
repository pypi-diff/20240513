# Comparing `tmp/heflwr-0.1.0.tar.gz` & `tmp/heflwr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heflwr-0.1.0.tar", last modified: Sun May 12 17:53:53 2024, max compression
+gzip compressed data, was "heflwr-0.1.1.tar", last modified: Mon May 13 08:30:22 2024, max compression
```

## Comparing `heflwr-0.1.0.tar` & `heflwr-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 17:53:53.804567 heflwr-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-03-07 16:35:19.000000 heflwr-0.1.0/LICENSE
--rw-rw-rw-   0        0        0        0 2024-05-12 17:05:41.000000 heflwr-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      552 2024-05-12 17:53:53.802507 heflwr-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-05-12 17:35:02.000000 heflwr-0.1.0/README.rst
--rw-rw-rw-   0        0        0       42 2024-05-12 17:53:53.804567 heflwr-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      608 2024-05-12 17:03:33.000000 heflwr-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:53:53.720293 heflwr-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-12 17:53:53.729607 heflwr-0.1.0/src/heflwr/
--rw-rw-rw-   0        0        0       79 2024-05-12 16:35:15.000000 heflwr-0.1.0/src/heflwr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:53:53.773891 heflwr-0.1.0/src/heflwr/fed/
--rw-rw-rw-   0        0        0       87 2024-05-12 16:19:55.000000 heflwr-0.1.0/src/heflwr/fed/__init__.py
--rw-rw-rw-   0        0        0     3067 2024-05-12 16:37:39.000000 heflwr-0.1.0/src/heflwr/fed/aggregate.py
--rw-rw-rw-   0        0        0        0 2024-05-12 14:56:04.000000 heflwr-0.1.0/src/heflwr/fed/client_manager.py
--rw-rw-rw-   0        0        0     3228 2024-05-12 16:11:10.000000 heflwr-0.1.0/src/heflwr/fed/hetero_aggregate.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:53:53.777178 heflwr-0.1.0/src/heflwr/log/
--rw-rw-rw-   0        0        0       22 2024-05-12 16:35:15.000000 heflwr-0.1.0/src/heflwr/log/__init__.py
--rw-rw-rw-   0        0        0     3463 2024-04-27 12:54:05.000000 heflwr-0.1.0/src/heflwr/log/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:53:53.778199 heflwr-0.1.0/src/heflwr/monitor/
--rw-rw-rw-   0        0        0       61 2024-05-12 16:24:06.000000 heflwr-0.1.0/src/heflwr/monitor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:53:53.784288 heflwr-0.1.0/src/heflwr/monitor/process_monitor/
--rw-rw-rw-   0        0        0       92 2024-05-12 16:31:05.000000 heflwr-0.1.0/src/heflwr/monitor/process_monitor/__init__.py
--rw-rw-rw-   0        0        0     5515 2024-05-09 05:57:30.000000 heflwr-0.1.0/src/heflwr/monitor/process_monitor/file_monitor.py
--rw-rw-rw-   0        0        0     5537 2024-05-06 09:59:01.000000 heflwr-0.1.0/src/heflwr/monitor/process_monitor/prometheus_monitor.py
--rw-rw-rw-   0        0        0     5356 2024-05-12 16:17:37.000000 heflwr-0.1.0/src/heflwr/monitor/process_monitor/remote_monitor.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:53:53.790607 heflwr-0.1.0/src/heflwr/monitor/thread_monitor/
--rw-rw-rw-   0        0        0       92 2024-05-12 16:31:05.000000 heflwr-0.1.0/src/heflwr/monitor/thread_monitor/__init__.py
--rw-rw-rw-   0        0        0     4934 2024-05-09 05:58:40.000000 heflwr-0.1.0/src/heflwr/monitor/thread_monitor/file_monitor.py
--rw-rw-rw-   0        0        0     5295 2024-05-06 10:11:38.000000 heflwr-0.1.0/src/heflwr/monitor/thread_monitor/prometheus_monitor.py
--rw-rw-rw-   0        0        0     5025 2024-05-12 16:17:37.000000 heflwr-0.1.0/src/heflwr/monitor/thread_monitor/remote_monitor.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:53:53.795107 heflwr-0.1.0/src/heflwr/monitor/utils/
--rw-rw-rw-   0        0        0        0 2024-04-27 15:24:20.000000 heflwr-0.1.0/src/heflwr/monitor/utils/__init__.py
--rw-rw-rw-   0        0        0     1028 2024-04-27 16:14:14.000000 heflwr-0.1.0/src/heflwr/monitor/utils/network.py
--rw-rw-rw-   0        0        0     4446 2024-05-05 09:02:05.000000 heflwr-0.1.0/src/heflwr/monitor/utils/power.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:53:53.801468 heflwr-0.1.0/src/heflwr/nn/
--rw-rw-rw-   0        0        0      144 2024-05-12 16:17:37.000000 heflwr-0.1.0/src/heflwr/nn/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-12 09:40:17.000000 heflwr-0.1.0/src/heflwr/nn/scaler.py
--rw-rw-rw-   0        0        0     7103 2024-05-07 05:00:50.000000 heflwr-0.1.0/src/heflwr/nn/ssconv2d.py
--rw-rw-rw-   0        0        0    10915 2024-05-05 14:44:54.000000 heflwr-0.1.0/src/heflwr/nn/sslinear.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:53:53.765968 heflwr-0.1.0/src/heflwr.egg-info/
--rw-rw-rw-   0        0        0      552 2024-05-12 17:53:53.000000 heflwr-0.1.0/src/heflwr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2024-05-12 17:53:53.000000 heflwr-0.1.0/src/heflwr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 17:53:53.000000 heflwr-0.1.0/src/heflwr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-12 17:53:53.000000 heflwr-0.1.0/src/heflwr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 08:30:22.782930 heflwr-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2023-03-07 16:35:19.000000 heflwr-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-05-12 17:05:41.000000 heflwr-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      552 2024-05-13 08:30:22.782930 heflwr-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-12 17:35:02.000000 heflwr-0.1.1/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-13 08:30:22.782930 heflwr-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      608 2024-05-13 08:30:07.000000 heflwr-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:30:22.753121 heflwr-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 08:30:22.759100 heflwr-0.1.1/src/heflwr/
+-rw-rw-rw-   0        0        0       79 2024-05-12 16:35:15.000000 heflwr-0.1.1/src/heflwr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:30:22.768071 heflwr-0.1.1/src/heflwr/fed/
+-rw-rw-rw-   0        0        0       87 2024-05-12 16:19:55.000000 heflwr-0.1.1/src/heflwr/fed/__init__.py
+-rw-rw-rw-   0        0        0     6687 2024-05-13 08:14:45.000000 heflwr-0.1.1/src/heflwr/fed/aggregate.py
+-rw-rw-rw-   0        0        0        0 2024-05-12 14:56:04.000000 heflwr-0.1.1/src/heflwr/fed/he_client_manager.py
+-rw-rw-rw-   0        0        0     4734 2024-05-13 08:13:27.000000 heflwr-0.1.1/src/heflwr/fed/hetero_aggregate.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:30:22.769067 heflwr-0.1.1/src/heflwr/log/
+-rw-rw-rw-   0        0        0       22 2024-05-12 16:35:15.000000 heflwr-0.1.1/src/heflwr/log/__init__.py
+-rw-rw-rw-   0        0        0     3463 2024-04-27 12:54:05.000000 heflwr-0.1.1/src/heflwr/log/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:30:22.770063 heflwr-0.1.1/src/heflwr/monitor/
+-rw-rw-rw-   0        0        0       61 2024-05-12 16:24:06.000000 heflwr-0.1.1/src/heflwr/monitor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:30:22.773053 heflwr-0.1.1/src/heflwr/monitor/process_monitor/
+-rw-rw-rw-   0        0        0       92 2024-05-12 16:31:05.000000 heflwr-0.1.1/src/heflwr/monitor/process_monitor/__init__.py
+-rw-rw-rw-   0        0        0     5523 2024-05-13 08:30:07.000000 heflwr-0.1.1/src/heflwr/monitor/process_monitor/file_monitor.py
+-rw-rw-rw-   0        0        0     5541 2024-05-13 07:35:10.000000 heflwr-0.1.1/src/heflwr/monitor/process_monitor/prometheus_monitor.py
+-rw-rw-rw-   0        0        0     5356 2024-05-13 07:35:10.000000 heflwr-0.1.1/src/heflwr/monitor/process_monitor/remote_monitor.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:30:22.777040 heflwr-0.1.1/src/heflwr/monitor/thread_monitor/
+-rw-rw-rw-   0        0        0       92 2024-05-12 16:31:05.000000 heflwr-0.1.1/src/heflwr/monitor/thread_monitor/__init__.py
+-rw-rw-rw-   0        0        0     4938 2024-05-13 07:35:10.000000 heflwr-0.1.1/src/heflwr/monitor/thread_monitor/file_monitor.py
+-rw-rw-rw-   0        0        0     5299 2024-05-13 07:35:10.000000 heflwr-0.1.1/src/heflwr/monitor/thread_monitor/prometheus_monitor.py
+-rw-rw-rw-   0        0        0     5025 2024-05-13 07:35:10.000000 heflwr-0.1.1/src/heflwr/monitor/thread_monitor/remote_monitor.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:30:22.778037 heflwr-0.1.1/src/heflwr/monitor/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-27 15:24:20.000000 heflwr-0.1.1/src/heflwr/monitor/utils/__init__.py
+-rw-rw-rw-   0        0        0     1028 2024-05-13 07:35:10.000000 heflwr-0.1.1/src/heflwr/monitor/utils/network.py
+-rw-rw-rw-   0        0        0     4500 2024-05-13 08:10:14.000000 heflwr-0.1.1/src/heflwr/monitor/utils/power.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:30:22.781027 heflwr-0.1.1/src/heflwr/nn/
+-rw-rw-rw-   0        0        0      153 2024-05-13 07:44:10.000000 heflwr-0.1.1/src/heflwr/nn/__init__.py
+-rw-rw-rw-   0        0        0      351 2024-05-13 07:27:27.000000 heflwr-0.1.1/src/heflwr/nn/scaler.py
+-rw-rw-rw-   0        0        0     9696 2024-05-13 07:35:10.000000 heflwr-0.1.1/src/heflwr/nn/ssconv2d.py
+-rw-rw-rw-   0        0        0     9284 2024-05-13 07:35:10.000000 heflwr-0.1.1/src/heflwr/nn/sslinear.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:30:22.766082 heflwr-0.1.1/src/heflwr.egg-info/
+-rw-rw-rw-   0        0        0      552 2024-05-13 08:30:22.000000 heflwr-0.1.1/src/heflwr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2024-05-13 08:30:22.000000 heflwr-0.1.1/src/heflwr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 08:30:22.000000 heflwr-0.1.1/src/heflwr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 08:30:22.000000 heflwr-0.1.1/src/heflwr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 08:30:22.782024 heflwr-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-12 18:35:12.000000 heflwr-0.1.1/tests/test.py
```

### Comparing `heflwr-0.1.0/LICENSE` & `heflwr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.0/PKG-INFO` & `heflwr-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: heflwr
-Version: 0.1.0
-Summary: 「HeFlwr」is a federated learning package for Heterogeneous devices.
+Version: 0.1.1
+Summary: 「HeFlwr」is a federated learning package for heterogeneous devices.
 Home-page: https://github.com/QVQZZZ/HeFlwr
 Author: Zhu Yaolin
 Author-email: zhuyaolinluck@qq.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `heflwr-0.1.0/setup.py` & `heflwr-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 def readme():
     with open("README.rst", encoding="UTF-8") as f:
         return f.read()
 
 
 setup(
     name="heflwr",
-    version="0.1.0",
-    description="「HeFlwr」is a federated learning package for Heterogeneous devices.",
+    version="0.1.1",
+    description="「HeFlwr」is a federated learning package for heterogeneous devices.",
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     author="Zhu Yaolin",
     author_email="zhuyaolinluck@qq.com",
     long_description=readme(),
     long_description_content_type='text/x-rst',
     include_package_data=True,
```

### Comparing `heflwr-0.1.0/src/heflwr/fed/hetero_aggregate.py` & `heflwr-0.1.1/src/heflwr/fed/hetero_aggregate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,87 @@
+from typing import List, Union, Tuple
+
+import numpy as np
 import torch
 import torch.nn as nn
-from typing import List, Union, Tuple
 from flwr.common.parameter import parameters_to_ndarrays, ndarrays_to_parameters
-import numpy as np
 from flwr.common.typing import Parameters, FitRes
 from flwr.server.client_proxy import ClientProxy
+
+from .aggregate import aggregate_layer
 from ..nn import SSLinear, SSConv2d
+from ..log.logger import log
 
 
 def extract(parameters: Parameters, client_net: nn.Module, server_net: nn.Module) -> Parameters:
+    """
+    Extracts the parameters of a client model (`client_net`) from the global server model (`server_net`)
+    based on a given `Parameters` object.
+
+    This function takes the serialized parameters from the global model, represented by the `Parameters` object,
+    and transfers them to the client model's architecture.
+    The parameters are deserialized and be extracted so that it can suit the client model's architecture.
+    This ensures that the client model aligns with the global model's parameters before local training commences,
+    which is a common step in system-heterogeneous federated learning setups.
+
+    :param parameters: A `Parameters` object containing serialized parameters of the global model.
+    :param client_net: The neural network model on the client-side that needs to be updated with global parameters.
+    :param server_net: The global server-side neural network model from which the parameters are sourced.
+
+    :return: An updated `Parameters` object containing the newly extracted parameters for the client model.
+    """
     with torch.no_grad():
         tensor_list: List[torch.Tensor] = [torch.Tensor(_) for _ in parameters_to_ndarrays(parameters)]
         global_dict = {name: tensor for name, tensor in zip(server_net.state_dict().keys(), tensor_list)}
         server_net.load_state_dict(global_dict)
+
         for layer, father_layer in zip(client_net.modules(), server_net.modules()):
             if hasattr(layer, 'reset_parameters_from_father_layer'):
                 layer.reset_parameters_from_father_layer(father_layer)
-        # for layer, father_layer in zip(client_net.modules(), server_net.modules()):
-        #     try:
-        #         layer.reset_parameters_from_father_layer(father_layer)
-        #     except AttributeError:
-        #         pass
-        #     except Exception as e:
-        #         raise RuntimeError(e)
+
         array_list: List[np.ndarray] = [_.numpy() for _ in list(client_net.parameters())]
         parameters = ndarrays_to_parameters(array_list)
     return parameters
 
 
-def merge(results:List[Tuple[ClientProxy, FitRes]], client_nets: List[nn.Module], server_net: nn.Module) -> Parameters:
+def merge(results: List[Tuple[ClientProxy, FitRes]], client_nets: List[nn.Module], server_net: nn.Module) -> Parameters:
+    """
+    Merges parameters from multiple client models into a global server model.
+
+    This function collects the trained parameters from a list of client models
+    and aggregates them into the server model's architecture.
+    It is a crucial step in system-heterogeneous federated learning setups where each client
+    performs local updates to the model, and the server then integrates these updates.
+    Each client model's parameters are weighted by the number of examples it used for training,
+    ensuring that the aggregation accounts for the different amounts of data each client has.
+
+    :param results: A list of tuples, each containing a `ClientProxy`
+    and its corresponding `FitRes` containing training results.
+    :param client_nets: A list of neural network models from each client that participated in the training.
+    :param server_net: The global server-side neural network model that will be updated with the aggregated parameters.
+
+    :return: A `Parameters` object containing the aggregated parameters after merging updates from client models.
+    """
     with torch.no_grad():
-        from aggregate import aggregate_layer
         num_examples_list = []
         parameters_list = []
+
         for _, fit_res in results:
             num_examples_list.append(fit_res.num_examples)
             array_parameters: List[np.ndarray] = parameters_to_ndarrays(fit_res.parameters)
             tensor_parameters: List[torch.Tensor] = [torch.Tensor(_) for _ in array_parameters]
             parameters_list.append(tensor_parameters)
-        # 还需要用results.para为client_nets赋值
+
         for client_net, parameters in zip(client_nets, parameters_list):
             client_dict = {name: tensor for name, tensor in zip(client_net.state_dict().keys(), parameters)}
             client_net.load_state_dict(client_dict)
+
         for layer_name, layer in dict(server_net.named_modules()).items():
             if isinstance(layer, Union[SSConv2d, SSLinear]):
                 client_layers = [dict(client_net.named_modules())[layer_name] for client_net in client_nets]
                 aggregate_layer(layer, client_layers, num_examples_list)
             else:
-                print(layer)
-        # for layer_name, layer in server_net._modules.items():
-        #     try:
-        #         print(layer_name)
-        #         client_layers = [client_net._modules[layer_name] for client_net in client_nets]
-        #         aggregate_layer(layer, client_layers, num_examples_list)
-        #     except Exception as e:
-        #         print(e)
+                log(f"Can't merge {layer}, ignore it.")
 
         array_list: List[np.ndarray] = [_.numpy() for _ in list(server_net.parameters())]
         parameters = ndarrays_to_parameters(array_list)
     return parameters
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `heflwr-0.1.0/src/heflwr/log/logger.py` & `heflwr-0.1.1/src/heflwr/log/logger.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.0/src/heflwr/monitor/process_monitor/file_monitor.py` & `heflwr-0.1.1/src/heflwr/monitor/process_monitor/file_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import os
 import time
 import multiprocessing
-import psutil
 import datetime
+
+import psutil
+
 from ..utils.network import NetTrafficMonitor
 from ..utils.power import PowerMonitor
 
 
 class FileMonitor:
     def __init__(self, file, interval=5):
         self.pid = os.getpid()
         # self.process = psutil.Process(self.pid)
         self.file = file
         self.interval = interval
         self.monitoring = multiprocessing.Event()
-        self.monitor_process = None  # 监控进程
+        self.monitor_process = None  # the monitor process
         self.metrics = {
             'cpu': True,
             'memory': True,
             'network': True,
             'power': True,
         }
         manager = multiprocessing.Manager()
@@ -39,15 +41,15 @@
             if not isinstance(value, bool):
                 raise TypeError(f"Value for metric '{metric}' must be a boolean, got {type(value)} instead.")
             self.metrics[metric] = value
 
     def update_metrics(self):
         # 在子进程内部创建Process对象，避免Windows使用multiprocessing情况下可能出现的错误
         # 具体的错误为TypeError: cannot pickle '_thread.RLock' object
-        # 这是因为在Windows下使用multiprocessing时，尝试在多个进程之间共享了不可序列化的_thread.RLock对象。
+        # 这是因为在Windows下使用multiprocessing时，尝试在多个进程之间共享了不可序列化的_thread.RLock对象
         process = psutil.Process(self.pid)
         with open(self.file, 'a') as f:
             current_time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             f.write(f"{current_time}\n")
             while self.monitoring.is_set():
                 if self.metrics['cpu']:
                     cpu_usage = process.cpu_percent()
```

### Comparing `heflwr-0.1.0/src/heflwr/monitor/process_monitor/prometheus_monitor.py` & `heflwr-0.1.1/src/heflwr/monitor/process_monitor/prometheus_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import time
 import multiprocessing
+
 import psutil
 from prometheus_client import start_http_server, Gauge
+
 from ..utils.network import NetTrafficMonitor
 from ..utils.power import PowerMonitor
 
 
 class PrometheusMonitor:
     def __init__(self, port=8003, interval=5):
         self.pid = os.getpid()
```

### Comparing `heflwr-0.1.0/src/heflwr/monitor/process_monitor/remote_monitor.py` & `heflwr-0.1.1/src/heflwr/monitor/process_monitor/remote_monitor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 import multiprocessing
-import psutil
 
+import psutil
 import uuid
-from ...log.logger import logger, configure
 
+from ...log.logger import logger, configure
 from ..utils.network import NetTrafficMonitor
 from ..utils.power import PowerMonitor
 
 
 class RemoteMonitor:
     def __init__(self, host, interval=5, identifier=None, simple=True):
         self.pid = os.getpid()
```

### Comparing `heflwr-0.1.0/src/heflwr/monitor/thread_monitor/file_monitor.py` & `heflwr-0.1.1/src/heflwr/monitor/thread_monitor/file_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import time
 import threading
-import psutil
 import datetime
+
+import psutil
+
 from ..utils.network import NetTrafficMonitor
 from ..utils.power import PowerMonitor
 
 
 class FileMonitor:
     def __init__(self, file, interval=5):
         self.pid = os.getpid()
```

### Comparing `heflwr-0.1.0/src/heflwr/monitor/thread_monitor/prometheus_monitor.py` & `heflwr-0.1.1/src/heflwr/monitor/thread_monitor/prometheus_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import time
 import threading
+
 import psutil
 from prometheus_client import start_http_server, Gauge
+
 from ..utils.network import NetTrafficMonitor
 from ..utils.power import PowerMonitor
 
 
 class PrometheusMonitor:
     def __init__(self, port=8003, interval=5):
         self.pid = os.getpid()
```

### Comparing `heflwr-0.1.0/src/heflwr/monitor/thread_monitor/remote_monitor.py` & `heflwr-0.1.1/src/heflwr/monitor/thread_monitor/remote_monitor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 import threading
-import psutil
 
+import psutil
 import uuid
-from ...log.logger import logger, configure
 
+from ...log.logger import logger, configure
 from ..utils.network import NetTrafficMonitor
 from ..utils.power import PowerMonitor
 
 
 class RemoteMonitor:
     def __init__(self, host, interval=5, identifier=None, simple=True):
         self.pid = os.getpid()
```

### Comparing `heflwr-0.1.0/src/heflwr/monitor/utils/network.py` & `heflwr-0.1.1/src/heflwr/monitor/utils/network.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import psutil
 import time
 
+import psutil
+
 
 class NetTrafficMonitor:
     _instance = None
 
     def __new__(cls, *args, **kwargs):
         if not cls._instance:
             cls._instance = super(NetTrafficMonitor, cls).__new__(cls, *args, **kwargs)
@@ -25,8 +26,7 @@
         if self.first_call:
             time.sleep(5)  # Wait for a second to get initial reading
             self.first_call = False
         curr_sent, curr_recv = self.get_net_io()
         diff_sent, diff_recv = curr_sent - self.last_sent, curr_recv - self.last_recv
         self.last_sent, self.last_recv = curr_sent, curr_recv
         return diff_sent, diff_recv
-
```

### Comparing `heflwr-0.1.0/src/heflwr/monitor/utils/power.py` & `heflwr-0.1.1/src/heflwr/monitor/utils/power.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import subprocess
 import re
+import subprocess
 
 
 def get_jetson_model():
     try:
         model = subprocess.check_output('cat /sys/firmware/devicetree/base/model', shell=True)
         model = str(model, encoding='utf-8')  # model.decode('utf-8')
         return model.strip()
@@ -52,17 +52,20 @@
             else:
                 raise RuntimeError(f"No output was captured. Current e={self.e}, try a large number of 'e'.")
             if isinstance(first_line, bytes):  # text=True may have no effect, so we need to confirm `first_line` is a str
                 first_line = str(first_line, encoding='utf-8')
                 power_data = self._extract_power_dict(first_line)
                 """
                 `Jetson stats` for jetson devices.
-                See https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/SD/PlatformPowerAndPerformance.html
-                Orin Series: https://docs.nvidia.com/jetson/archives/r35.5.0/DeveloperGuide/SD/PlatformPowerAndPerformance/JetsonOrinNanoSeriesJetsonOrinNxSeriesAndJetsonAgxOrinSeries.html#jetson-orin-nx-series-and-jetson-orin-nano-series
-                Xavier Series: https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/SD/PlatformPowerAndPerformance/JetsonXavierNxSeriesAndJetsonAgxXavierSeries.html#sd-platformpowerandperformance-jetsonxaviernxandjetsonagxxavier
+                See:
+                https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/SD/PlatformPowerAndPerformance.html
+                Orin Series: 
+                https://docs.nvidia.com/jetson/archives/r35.5.0/DeveloperGuide/SD/PlatformPowerAndPerformance/JetsonOrinNanoSeriesJetsonOrinNxSeriesAndJetsonAgxOrinSeries.html#jetson-orin-nx-series-and-jetson-orin-nano-series
+                Xavier Series: 
+                https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/SD/PlatformPowerAndPerformance/JetsonXavierNxSeriesAndJetsonAgxXavierSeries.html#sd-platformpowerandperformance-jetsonxaviernxandjetsonagxxavier
                 """
                 if self.jetson_model in ('Jetson-AGX\x00', ):
                     # power_data = {
                     #     'GPU': 0,
                     #     'CPU': 0,
                     #     'SOC': 0,
                     #     'CV': 0,
```

### Comparing `heflwr-0.1.0/src/heflwr.egg-info/PKG-INFO` & `heflwr-0.1.1/src/heflwr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: heflwr
-Version: 0.1.0
-Summary: 「HeFlwr」is a federated learning package for Heterogeneous devices.
+Version: 0.1.1
+Summary: 「HeFlwr」is a federated learning package for heterogeneous devices.
 Home-page: https://github.com/QVQZZZ/HeFlwr
 Author: Zhu Yaolin
 Author-email: zhuyaolinluck@qq.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `heflwr-0.1.0/src/heflwr.egg-info/SOURCES.txt` & `heflwr-0.1.1/src/heflwr.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 src/heflwr/__init__.py
 src/heflwr.egg-info/PKG-INFO
 src/heflwr.egg-info/SOURCES.txt
 src/heflwr.egg-info/dependency_links.txt
 src/heflwr.egg-info/top_level.txt
 src/heflwr/fed/__init__.py
 src/heflwr/fed/aggregate.py
-src/heflwr/fed/client_manager.py
+src/heflwr/fed/he_client_manager.py
 src/heflwr/fed/hetero_aggregate.py
 src/heflwr/log/__init__.py
 src/heflwr/log/logger.py
 src/heflwr/monitor/__init__.py
 src/heflwr/monitor/process_monitor/__init__.py
 src/heflwr/monitor/process_monitor/file_monitor.py
 src/heflwr/monitor/process_monitor/prometheus_monitor.py
@@ -24,8 +24,9 @@
 src/heflwr/monitor/thread_monitor/remote_monitor.py
 src/heflwr/monitor/utils/__init__.py
 src/heflwr/monitor/utils/network.py
 src/heflwr/monitor/utils/power.py
 src/heflwr/nn/__init__.py
 src/heflwr/nn/scaler.py
 src/heflwr/nn/ssconv2d.py
-src/heflwr/nn/sslinear.py
+src/heflwr/nn/sslinear.py
+tests/test.py
```

