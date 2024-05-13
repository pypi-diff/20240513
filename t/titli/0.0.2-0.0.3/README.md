# Comparing `tmp/titli-0.0.2.tar.gz` & `tmp/titli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titli-0.0.2.tar", last modified: Thu May  2 08:59:10 2024, max compression
+gzip compressed data, was "titli-0.0.3.tar", last modified: Mon May 13 04:05:32 2024, max compression
```

## Comparing `titli-0.0.2.tar` & `titli-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:10.660381 titli-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-02 08:59:05.000000 titli-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-02 08:59:10.660381 titli-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 08:59:05.000000 titli-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 08:59:10.660381 titli-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-02 08:59:05.000000 titli-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:10.656381 titli-0.0.2/titli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:05.000000 titli-0.0.2/titli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:10.656381 titli-0.0.2/titli/fe/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 08:59:05.000000 titli-0.0.2/titli/fe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23767 2024-05-02 08:59:05.000000 titli-0.0.2/titli/fe/after_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-02 08:59:05.000000 titli-0.0.2/titli/fe/base_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-02 08:59:05.000000 titli-0.0.2/titli/fe/corClust.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:10.656381 titli-0.0.2/titli/ids/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 08:59:05.000000 titli-0.0.2/titli/ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-02 08:59:05.000000 titli-0.0.2/titli/ids/base_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    17521 2024-05-02 08:59:05.000000 titli-0.0.2/titli/ids/kitsune.py
--rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-02 08:59:05.000000 titli-0.0.2/titli/ids/pytorch_kitsune.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-02 08:59:05.000000 titli-0.0.2/titli/ids/torch_kitnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:10.656381 titli-0.0.2/titli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-02 08:59:05.000000 titli-0.0.2/titli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 08:59:05.000000 titli-0.0.2/titli/utils/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:10.660381 titli-0.0.2/titli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-02 08:59:10.000000 titli-0.0.2/titli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-02 08:59:10.000000 titli-0.0.2/titli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:59:10.000000 titli-0.0.2/titli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:59:10.000000 titli-0.0.2/titli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 08:59:10.000000 titli-0.0.2/titli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 08:59:10.000000 titli-0.0.2/titli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:32.617271 titli-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-13 04:05:26.000000 titli-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-13 04:05:32.617271 titli-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-13 04:05:26.000000 titli-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 04:05:32.617271 titli-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-13 04:05:26.000000 titli-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:32.613271 titli-0.0.3/titli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:26.000000 titli-0.0.3/titli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:32.617271 titli-0.0.3/titli/fe/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 04:05:26.000000 titli-0.0.3/titli/fe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23767 2024-05-13 04:05:26.000000 titli-0.0.3/titli/fe/after_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-13 04:05:26.000000 titli-0.0.3/titli/fe/base_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-13 04:05:26.000000 titli-0.0.3/titli/fe/corClust.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:32.617271 titli-0.0.3/titli/ids/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 04:05:26.000000 titli-0.0.3/titli/ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-13 04:05:26.000000 titli-0.0.3/titli/ids/base_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17521 2024-05-13 04:05:26.000000 titli-0.0.3/titli/ids/kitsune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-13 04:05:26.000000 titli-0.0.3/titli/ids/pytorch_kitsune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-13 04:05:26.000000 titli-0.0.3/titli/ids/torch_kitnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:32.617271 titli-0.0.3/titli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 04:05:26.000000 titli-0.0.3/titli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-13 04:05:26.000000 titli-0.0.3/titli/utils/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:05:32.617271 titli-0.0.3/titli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-13 04:05:32.000000 titli-0.0.3/titli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-13 04:05:32.000000 titli-0.0.3/titli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 04:05:32.000000 titli-0.0.3/titli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 04:05:32.000000 titli-0.0.3/titli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 04:05:32.000000 titli-0.0.3/titli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 04:05:32.000000 titli-0.0.3/titli.egg-info/top_level.txt
```

### Comparing `titli-0.0.2/LICENSE` & `titli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `titli-0.0.2/setup.py` & `titli-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='titli',
-    version='0.0.2',
+    version='0.0.3',
     description='A library for collection of IDS and tools for evaluating them',
     long_description=open("README.md").read(),
     long_description_content_type = "text/markdown",
     url='https://github.com/spg-iitd/raids',
     packages=find_packages(),
     license='MIT',
     author="Subrat Kumar Swain",
```

### Comparing `titli-0.0.2/titli/fe/after_image.py` & `titli-0.0.3/titli/fe/after_image.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.2/titli/fe/base_feature_extractor.py` & `titli-0.0.3/titli/fe/base_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.2/titli/fe/corClust.py` & `titli-0.0.3/titli/fe/corClust.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.2/titli/ids/base_ids.py` & `titli-0.0.3/titli/ids/base_ids.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.2/titli/ids/kitsune.py` & `titli-0.0.3/titli/ids/kitsune.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.2/titli/ids/pytorch_kitsune.py` & `titli-0.0.3/titli/ids/pytorch_kitsune.py`

 * *Files 7% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     def train(self, pcap_path: str) -> None:
         self.train_rmse = []
         self.print_interval = 100
         self.train_mode = True
         self.device = torch.device("mps" if torch.cuda.is_available() else "cpu")
         self.rmse = RMSELoss()
         self.FMgrace = np.floor(self.FMgrace_rate * len(rdpcap(pcap_path)))
+        self.dataset = pcap_path.split("/")[-1].split(".")[0]
         
         print("Training Feature Mapping (FM) phase")
         for i, packet in enumerate(PcapReader(pcap_path)):
 
             # get feature vector
             traffic_vector = self.fe.get_traffic_vector(packet)
 
@@ -175,18 +176,23 @@
 
             self.train_rmse.append(loss.data)
 
             optimiser.zero_grad()
             loss.backward()
             optimiser.step()
 
-            # Making the decoder weight the transpose of the encoder weight
+            # # Making the decoder weight the transpose of the encoder weight
+            # for tail in self.tails:
+            #     tail.decoder.weight.data = tail.encoder.weight.data.t()
+            # self.head.decoder.weight.data = self.head.encoder.weight.data.t()
+
+            # Making the encoder weight the transpose of the decoder weight
             for tail in self.tails:
-                tail.decoder.weight.data = tail.encoder.weight.data.t()
-            self.head.decoder.weight.data = self.head.encoder.weight.data.t()
+                tail.encoder.weight.data = tail.decoder.weight.data.t()
+            self.head.encoder.weight.data = self.head.decoder.weight.data.t()
 
             if (i + 1) % self.print_interval == 0:
                 print(f"Packet: {i} | Loss: {loss.data}")
         
         self.threshold = self.get_threshold(pcap_path)
 
         return self.threshold
@@ -208,14 +214,16 @@
             x = self.fe.update(traffic_vector)
 
             # forward pass
             x_hat, tails = self(x)
 
             # loss
             loss = self.rmse(x_hat, tails)
+            if loss.data == 0:
+                loss.data = torch.tensor(1e-2)
             self.threshold_rmse.append(loss.data)
 
         log_re = np.log(self.threshold_rmse)
         mean = np.mean(log_re)
         std = np.std(log_re)
         threshold_std = np.exp(mean + 3 * std)
         threshold_max = max(self.threshold_rmse)
@@ -240,38 +248,34 @@
             x = self.fe.update(traffic_vector)
 
             # forward pass
             x_hat, tails = self(x)
 
             # loss
             loss = self.rmse(x_hat, tails)
+            if loss.data == 0:
+                loss.data = torch.tensor(1e-2)
             self.rmse_array.append(loss.data)
 
             if (i + 1) % self.print_interval == 0:
                 print(f"Inferencing: {i} | Loss: {loss.data}")
 
-    def plot_kitsune(self,threshold,plot_with_time = True, meta_file = False, out_image = "kitsune_plot.png"):
-        cmap = plt.get_cmap('Set3')
-
-        f, ax1 = plt.subplots(constrained_layout=True, figsize=(10, 5), dpi=200)
+    def plot_kitsune(self, threshold, out_image = "kitsune_plot.png"):
+        _ = plt.get_cmap('Set3')
 
-        if plot_with_time:
-            x_val = range(len(self.rmse_array))
-            ax1.xaxis.set_major_locator(ticker.MultipleLocator(0.85))
-            ax1.tick_params(labelrotation=90)
-        else:
-            x_val = range(len(self.rmse_array))
+        f, ax1 = plt.subplots(constrained_layout=True, figsize=(10, 5), dpi=600)
+        x_val = np.arange(len(self.rmse_array))
 
-        if meta_file:
+        try:
             ax1.scatter(x_val, self.rmse_array, s=1, c='#00008B')
-        else:
+        except:
             ax1.scatter(x_val, self.rmse_array, s=1, alpha=1.0, c='#FF8C00')
 
-        ax1.axhline(y=threshold, color='r', linestyle='-')
+        ax1.axhline(y=threshold, color='b', linestyle='-')
         ax1.set_yscale("log")
-        ax1.set_title("Anomaly Scores from Kitsune Execution Phase")
-        ax1.set_ylabel("RMSE (log scaled)")
-        ax1.set_xlabel("packet index")
+        ax1.set_title(f"Anomaly Scores of Kitsune Execution Phase: {self.dataset}")
+        ax1.set_ylabel("RMSE")
+        ax1.set_xlabel("Packet Index")
 
         f.savefig(out_image)
         print("plot path:", out_image)
         plt.close()
```

### Comparing `titli-0.0.2/titli/ids/torch_kitnet.py` & `titli-0.0.3/titli/ids/torch_kitnet.py`

 * *Files identical despite different names*

