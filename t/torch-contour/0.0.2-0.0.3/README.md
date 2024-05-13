# Comparing `tmp/torch_contour-0.0.2.tar.gz` & `tmp/torch_contour-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_contour-0.0.2.tar", last modified: Wed Dec  6 16:38:21 2023, max compression
+gzip compressed data, was "torch_contour-0.0.3.tar", last modified: Mon May 13 12:17:16 2024, max compression
```

## Comparing `torch_contour-0.0.2.tar` & `torch_contour-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2023-12-06 16:38:21.245895 torch_contour-0.0.2/
--rw-rw-r--   0 antoine   (1001) antoine   (1001)     1068 2023-12-06 15:01:07.000000 torch_contour-0.0.2/LICENSE
--rw-r--r--   0 antoine   (1001) antoine   (1001)      913 2023-12-06 16:38:21.245895 torch_contour-0.0.2/PKG-INFO
--rw-rw-r--   0 antoine   (1001) antoine   (1001)       15 2023-12-06 15:01:07.000000 torch_contour-0.0.2/README.md
--rw-rw-r--   0 antoine   (1001) antoine   (1001)      138 2023-12-06 15:01:07.000000 torch_contour-0.0.2/pyproject.toml
--rw-rw-r--   0 antoine   (1001) antoine   (1001)     1054 2023-12-06 16:38:21.249895 torch_contour-0.0.2/setup.cfg
--rw-rw-r--   0 antoine   (1001) antoine   (1001)       53 2023-12-06 15:01:07.000000 torch_contour-0.0.2/setup.py
-drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2023-12-06 16:38:21.245895 torch_contour-0.0.2/torch_contour/
--rw-rw-r--   0 antoine   (1001) antoine   (1001)      122 2023-12-06 16:37:34.000000 torch_contour-0.0.2/torch_contour/__init__.py
--rw-rw-r--   0 antoine   (1001) antoine   (1001)        0 2023-12-06 15:01:07.000000 torch_contour-0.0.2/torch_contour/py.typed
--rw-rw-r--   0 antoine   (1001) antoine   (1001)     2605 2023-12-06 16:36:35.000000 torch_contour-0.0.2/torch_contour/torch_contour.py
-drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2023-12-06 16:38:21.245895 torch_contour-0.0.2/torch_contour.egg-info/
--rw-r--r--   0 antoine   (1001) antoine   (1001)      913 2023-12-06 16:38:21.000000 torch_contour-0.0.2/torch_contour.egg-info/PKG-INFO
--rw-rw-r--   0 antoine   (1001) antoine   (1001)      315 2023-12-06 16:38:21.000000 torch_contour-0.0.2/torch_contour.egg-info/SOURCES.txt
--rw-rw-r--   0 antoine   (1001) antoine   (1001)        1 2023-12-06 16:38:21.000000 torch_contour-0.0.2/torch_contour.egg-info/dependency_links.txt
--rw-rw-r--   0 antoine   (1001) antoine   (1001)        6 2023-12-06 16:38:21.000000 torch_contour-0.0.2/torch_contour.egg-info/requires.txt
--rw-rw-r--   0 antoine   (1001) antoine   (1001)       14 2023-12-06 16:38:21.000000 torch_contour-0.0.2/torch_contour.egg-info/top_level.txt
+drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-13 12:17:16.750321 torch_contour-0.0.3/
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)     1068 2023-12-06 15:01:07.000000 torch_contour-0.0.3/LICENSE
+-rw-r--r--   0 antoine   (1001) antoine   (1001)     2104 2024-05-13 12:17:16.750321 torch_contour-0.0.3/PKG-INFO
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)     1207 2024-05-13 12:03:31.000000 torch_contour-0.0.3/README.md
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)      138 2023-12-06 15:01:07.000000 torch_contour-0.0.3/pyproject.toml
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)     1054 2024-05-13 12:17:16.750321 torch_contour-0.0.3/setup.cfg
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)       53 2023-12-06 15:01:07.000000 torch_contour-0.0.3/setup.py
+drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-13 12:17:16.750321 torch_contour-0.0.3/torch_contour/
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)      146 2024-05-13 12:17:04.000000 torch_contour-0.0.3/torch_contour/__init__.py
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)        0 2023-12-06 15:01:07.000000 torch_contour-0.0.3/torch_contour/py.typed
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)     2983 2024-05-13 12:07:20.000000 torch_contour-0.0.3/torch_contour/torch_contour.py
+drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-13 12:17:16.750321 torch_contour-0.0.3/torch_contour.egg-info/
+-rw-r--r--   0 antoine   (1001) antoine   (1001)     2104 2024-05-13 12:17:16.000000 torch_contour-0.0.3/torch_contour.egg-info/PKG-INFO
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)      315 2024-05-13 12:17:16.000000 torch_contour-0.0.3/torch_contour.egg-info/SOURCES.txt
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)        1 2024-05-13 12:17:16.000000 torch_contour-0.0.3/torch_contour.egg-info/dependency_links.txt
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)        6 2024-05-13 12:17:16.000000 torch_contour-0.0.3/torch_contour.egg-info/requires.txt
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)       14 2024-05-13 12:17:16.000000 torch_contour-0.0.3/torch_contour.egg-info/top_level.txt
```

### Comparing `torch_contour-0.0.2/LICENSE` & `torch_contour-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_contour-0.0.2/setup.cfg` & `torch_contour-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `torch_contour-0.0.2/torch_contour/torch_contour.py` & `torch_contour-0.0.3/torch_contour/torch_contour.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,73 +4,80 @@
 
 class Contour_to_mask(nn.Module):
     def __init__(self, size, k=1e5, eps=1e-5):
         super().__init__()
         self.k = k
         self.eps = eps
         self.size = size
-        self.mesh = torch.unsqueeze(
-            torch.stack(
-                torch.meshgrid(torch.arange(self.size), torch.arange(self.size)),
-                dim=-1,
-            ).reshape(-1, 2),
-            dim=1,
+        self.mesh = (
+            torch.unsqueeze(
+                torch.stack(
+                    torch.meshgrid(torch.arange(self.size), torch.arange(self.size)),
+                    dim=-1,
+                ).reshape(-1, 2),
+                dim=1,
+            )
+            / self.size
         )
 
     def forward(self, contour):
 
-        
-        contour = torch.unsqueeze(contour, dim=0)
-        diff = -self.mesh + contour
+        contours = torch.unsqueeze(contour, dim=0)
+        diff = -self.mesh + contours
         roll_diff = torch.roll(diff, -1, dims=1)
         sign = diff * torch.roll(roll_diff, 1, dims=2)
         sign = sign[:, :, 1] - sign[:, :, 0]
         sign = torch.tanh(self.k * sign)
-        norm_diff = torch.norm(diff, dim=2)
-        norm_roll = torch.norm(roll_diff, dim=2)
+        norm_diff = torch.linalg.vector_norm(diff, dim=2)
+        norm_roll = torch.linalg.vector_norm(roll_diff, dim=2)
         scalar_product = torch.sum(diff * roll_diff, dim=2)
-        clip = scalar_product / (norm_diff * norm_roll + self.eps)
-        angles = torch.arccos(torch.clip(clip, eps, 1 - self.eps))
+        clip = torch.clamp(scalar_product / (norm_diff * norm_roll), -1 + self.eps, 1 - self.eps)
+        angles = torch.acos(clip)
         torch.pi = torch.acos(torch.zeros(1)).item() * 2
-        sum_angles = torch.clip(-torch.sum(sign * angles, dim=1) / (2 * torch.pi), 0, 1)
+        sum_angles = torch.clamp(torch.sum(sign * angles, dim=1) / (2 * torch.pi), 0, 1)
         out0 = sum_angles.reshape(1, self.size, self.size)
         mask = torch.unsqueeze(out0, dim=0)
 
         return mask
+    
 
+    
 
 
 class Contour_to_distance_map(nn.Module):
     def __init__(self, size, k=1e5, eps=1e-5):
         super().__init__()
         self.k = k
         self.eps = eps
         self.size = size
-        self.mesh = torch.unsqueeze(
-            torch.stack(
-                torch.meshgrid(torch.arange(self.size), torch.arange(self.size)),
-                dim=-1,
-            ).reshape(-1, 2),
-            dim=1,
+        self.mesh = (
+            torch.unsqueeze(
+                torch.stack(
+                    torch.meshgrid(torch.arange(self.size), torch.arange(self.size)),
+                    dim=-1,
+                ).reshape(-1, 2),
+                dim=1,
+            )
+            / self.size
         )
 
     def forward(self, contour):
 
-        
+        k = 1e5
         contour = torch.unsqueeze(contour, dim=0)
         diff = -self.mesh + contour
+        min_diff = torch.min(torch.norm(diff, dim=-1), dim=1)[0]
+        min_diff = min_diff.reshape((self.size, self.size))
         roll_diff = torch.roll(diff, -1, dims=1)
         sign = diff * torch.roll(roll_diff, 1, dims=2)
         sign = sign[:, :, 1] - sign[:, :, 0]
-        sign = torch.tanh(self.k * sign)
-        norm_diff = torch.norm(diff, dim=2)
-        norm_roll = torch.norm(roll_diff, dim=2)
+        sign = torch.tanh(k * sign)
+        norm_diff = torch.clip(torch.norm(diff, dim=2), self.eps, None)
+        norm_roll = torch.clip(torch.norm(roll_diff, dim=2), self.eps, None)
         scalar_product = torch.sum(diff * roll_diff, dim=2)
-        clip = scalar_product / (norm_diff * norm_roll + self.eps)
-        angles = torch.arccos(torch.clip(clip, eps, 1 - self.eps))
+        clip = torch.clip(scalar_product / (norm_diff * norm_roll), -1 + self.eps, 1 - self.eps)
+        angles = torch.arccos(clip)
         torch.pi = torch.acos(torch.zeros(1)).item() * 2
-        sum_angles = torch.clip(-torch.sum(sign * angles, dim=1) / (2 * torch.pi), 0, 1)
-        out0 = sum_angles.reshape(1, self.size, self.size)
-        mask = torch.unsqueeze(out0, dim=0)
-
-        return mask
-
+        sum_angles = torch.sum(sign * angles, dim=1) / (2 * torch.pi)
+        resize = sum_angles.reshape(1, self.size, self.size)
+        dmap = torch.unsqueeze((resize * min_diff) / torch.max(resize * min_diff), 0)
+        return dmap
```

