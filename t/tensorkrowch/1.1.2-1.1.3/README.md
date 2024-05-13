# Comparing `tmp/tensorkrowch-1.1.2.tar.gz` & `tmp/tensorkrowch-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorkrowch-1.1.2.tar", last modified: Fri May 10 08:17:47 2024, max compression
+gzip compressed data, was "tensorkrowch-1.1.3.tar", last modified: Mon May 13 13:39:42 2024, max compression
```

## Comparing `tensorkrowch-1.1.2.tar` & `tensorkrowch-1.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-10 08:17:47.743049 tensorkrowch-1.1.2/
--rw-rw-r--   0 jose      (1000) jose      (1000)     1086 2023-05-25 11:43:07.000000 tensorkrowch-1.1.2/LICENSE.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       11 2024-03-06 17:59:45.000000 tensorkrowch-1.1.2/MANIFEST.in
--rw-r--r--   0 jose      (1000) jose      (1000)    10354 2024-05-10 08:17:47.743049 tensorkrowch-1.1.2/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)     7808 2024-05-10 08:16:58.000000 tensorkrowch-1.1.2/README.md
--rw-rw-r--   0 jose      (1000) jose      (1000)     1482 2024-05-10 08:16:58.000000 tensorkrowch-1.1.2/pyproject.toml
--rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-05-10 08:17:47.743049 tensorkrowch-1.1.2/setup.cfg
--rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-03-06 17:59:45.000000 tensorkrowch-1.1.2/setup.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-10 08:17:47.739049 tensorkrowch-1.1.2/tensorkrowch/
--rw-rw-r--   0 jose      (1000) jose      (1000)     1382 2024-05-10 08:16:58.000000 tensorkrowch-1.1.2/tensorkrowch/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   198461 2024-05-09 19:05:34.000000 tensorkrowch-1.1.2/tensorkrowch/components.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-10 08:17:47.739049 tensorkrowch-1.1.2/tensorkrowch/decompositions/
--rw-rw-r--   0 jose      (1000) jose      (1000)       81 2024-05-10 08:17:27.000000 tensorkrowch-1.1.2/tensorkrowch/decompositions/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    10787 2024-05-09 20:25:43.000000 tensorkrowch-1.1.2/tensorkrowch/decompositions/svd_decompositions.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    13298 2024-04-18 22:46:59.000000 tensorkrowch-1.1.2/tensorkrowch/embeddings.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     6401 2024-04-18 22:46:59.000000 tensorkrowch-1.1.2/tensorkrowch/initializers.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-10 08:17:47.743049 tensorkrowch-1.1.2/tensorkrowch/models/
--rw-rw-r--   0 jose      (1000) jose      (1000)      384 2024-04-14 00:06:08.000000 tensorkrowch-1.1.2/tensorkrowch/models/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    51467 2024-05-10 08:16:58.000000 tensorkrowch-1.1.2/tensorkrowch/models/mpo.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   179253 2024-05-10 08:16:58.000000 tensorkrowch-1.1.2/tensorkrowch/models/mps.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    21760 2024-04-18 22:46:59.000000 tensorkrowch-1.1.2/tensorkrowch/models/mps_data.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    58352 2024-04-18 22:46:59.000000 tensorkrowch-1.1.2/tensorkrowch/models/peps.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    37360 2024-03-06 17:59:45.000000 tensorkrowch-1.1.2/tensorkrowch/models/tree.py
--rw-rw-r--   0 jose      (1000) jose      (1000)   182494 2024-05-10 08:16:58.000000 tensorkrowch-1.1.2/tensorkrowch/operations.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     9156 2024-04-14 00:06:08.000000 tensorkrowch-1.1.2/tensorkrowch/utils.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-10 08:17:47.743049 tensorkrowch-1.1.2/tensorkrowch.egg-info/
--rw-r--r--   0 jose      (1000) jose      (1000)    10354 2024-05-10 08:17:47.000000 tensorkrowch-1.1.2/tensorkrowch.egg-info/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)      657 2024-05-10 08:17:47.000000 tensorkrowch-1.1.2/tensorkrowch.egg-info/SOURCES.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        1 2024-05-10 08:17:47.000000 tensorkrowch-1.1.2/tensorkrowch.egg-info/dependency_links.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)      307 2024-05-10 08:17:47.000000 tensorkrowch-1.1.2/tensorkrowch.egg-info/requires.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       13 2024-05-10 08:17:47.000000 tensorkrowch-1.1.2/tensorkrowch.egg-info/top_level.txt
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-13 13:39:42.157220 tensorkrowch-1.1.3/
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1086 2023-05-25 11:43:07.000000 tensorkrowch-1.1.3/LICENSE.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)       11 2024-03-06 17:59:45.000000 tensorkrowch-1.1.3/MANIFEST.in
+-rw-r--r--   0 jose      (1000) jose      (1000)    10354 2024-05-13 13:39:42.157220 tensorkrowch-1.1.3/PKG-INFO
+-rw-rw-r--   0 jose      (1000) jose      (1000)     7808 2024-05-10 08:16:58.000000 tensorkrowch-1.1.3/README.md
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1482 2024-05-10 08:16:58.000000 tensorkrowch-1.1.3/pyproject.toml
+-rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-05-13 13:39:42.157220 tensorkrowch-1.1.3/setup.cfg
+-rw-rw-r--   0 jose      (1000) jose      (1000)       38 2024-03-06 17:59:45.000000 tensorkrowch-1.1.3/setup.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-13 13:39:42.153220 tensorkrowch-1.1.3/tensorkrowch/
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1382 2024-05-13 13:38:52.000000 tensorkrowch-1.1.3/tensorkrowch/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   198462 2024-05-13 12:13:53.000000 tensorkrowch-1.1.3/tensorkrowch/components.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-13 13:39:42.153220 tensorkrowch-1.1.3/tensorkrowch/decompositions/
+-rw-rw-r--   0 jose      (1000) jose      (1000)       81 2024-05-10 08:17:27.000000 tensorkrowch-1.1.3/tensorkrowch/decompositions/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    10787 2024-05-09 20:25:43.000000 tensorkrowch-1.1.3/tensorkrowch/decompositions/svd_decompositions.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    13298 2024-04-18 22:46:59.000000 tensorkrowch-1.1.3/tensorkrowch/embeddings.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)     6401 2024-04-18 22:46:59.000000 tensorkrowch-1.1.3/tensorkrowch/initializers.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-13 13:39:42.153220 tensorkrowch-1.1.3/tensorkrowch/models/
+-rw-rw-r--   0 jose      (1000) jose      (1000)      384 2024-04-14 00:06:08.000000 tensorkrowch-1.1.3/tensorkrowch/models/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    52552 2024-05-13 13:37:43.000000 tensorkrowch-1.1.3/tensorkrowch/models/mpo.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   180174 2024-05-13 13:36:20.000000 tensorkrowch-1.1.3/tensorkrowch/models/mps.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    21760 2024-04-18 22:46:59.000000 tensorkrowch-1.1.3/tensorkrowch/models/mps_data.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    58352 2024-04-18 22:46:59.000000 tensorkrowch-1.1.3/tensorkrowch/models/peps.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    37360 2024-03-06 17:59:45.000000 tensorkrowch-1.1.3/tensorkrowch/models/tree.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)   182494 2024-05-10 08:16:58.000000 tensorkrowch-1.1.3/tensorkrowch/operations.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)     9156 2024-04-14 00:06:08.000000 tensorkrowch-1.1.3/tensorkrowch/utils.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2024-05-13 13:39:42.153220 tensorkrowch-1.1.3/tensorkrowch.egg-info/
+-rw-r--r--   0 jose      (1000) jose      (1000)    10354 2024-05-13 13:39:42.000000 tensorkrowch-1.1.3/tensorkrowch.egg-info/PKG-INFO
+-rw-rw-r--   0 jose      (1000) jose      (1000)      657 2024-05-13 13:39:42.000000 tensorkrowch-1.1.3/tensorkrowch.egg-info/SOURCES.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)        1 2024-05-13 13:39:42.000000 tensorkrowch-1.1.3/tensorkrowch.egg-info/dependency_links.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)      307 2024-05-13 13:39:42.000000 tensorkrowch-1.1.3/tensorkrowch.egg-info/requires.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)       13 2024-05-13 13:39:42.000000 tensorkrowch-1.1.3/tensorkrowch.egg-info/top_level.txt
```

### Comparing `tensorkrowch-1.1.2/LICENSE.txt` & `tensorkrowch-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.2/PKG-INFO` & `tensorkrowch-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorkrowch
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tensor Networks with PyTorch
 Author-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 Maintainer-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 José Ramón Pareja Monturiol
```

### Comparing `tensorkrowch-1.1.2/README.md` & `tensorkrowch-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.2/pyproject.toml` & `tensorkrowch-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.2/tensorkrowch/__init__.py` & `tensorkrowch-1.1.3/tensorkrowch/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 TensorKrowch
 ============
 
 Tensor Networks with PyTorch
 """
 
 # Version
-__version__ = '1.1.2'
+__version__ = '1.1.3'
 
 # Network components
 from tensorkrowch.components import Axis
 from tensorkrowch.components import AbstractNode, Node, ParamNode
 from tensorkrowch.components import StackNode, ParamStackNode
 from tensorkrowch.components import Edge, StackEdge
 from tensorkrowch.components import Successor, TensorNetwork
```

### Comparing `tensorkrowch-1.1.2/tensorkrowch/components.py` & `tensorkrowch-1.1.3/tensorkrowch/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -930,34 +930,34 @@
             aux_shape = list(self._shape)
             aux_shape[axis_num] = size
             self._shape = Size(aux_shape)
 
         else:
             if size < self._shape[axis_num]:
                 # If new size is smaller than current, tensor is cropped
-                # starting from the "left", "top", "front", etc. in each dimension
+                # starting from the "right", "bottom", "back", etc. in each dimension
                 index = []
                 for i, dim in enumerate(self._shape):
                     if i == axis_num:
-                        index.append(slice(dim - size, dim))
+                        index.append(slice(0, size))
                     else:
                         index.append(slice(0, dim))
                 aux_shape = list(self._shape)
                 aux_shape[axis_num] = size
                 self._shape = Size(aux_shape)
                 correct_format_tensor = self._set_tensor_format(tensor[index])
                 self._direct_set_tensor(correct_format_tensor)
 
             elif size > self._shape[axis_num]:
                 # If new size is greater than current, tensor is expanded with
-                # zeros in the "left", "top", "front", etc. dimension
+                # zeros in the "right", "bottom", "back", etc. dimension
                 pad = []
                 for i, dim in enumerate(self._shape):
                     if i == axis_num:
-                        pad += [0, size - dim]
+                        pad += [size - dim, 0]
                     else:
                         pad += [0, 0]
                 pad.reverse()
                 aux_shape = list(self._shape)
                 aux_shape[axis_num] = size
                 self._shape = Size(aux_shape)
                 correct_format_tensor = self._set_tensor_format(
@@ -3266,16 +3266,16 @@
         return self._nodes[0]._shape[self._axes[0]._num]
 
     def change_size(self, size: int) -> None:
         """
         Changes size of the edge, thus changing the size of tensors of ``node1``
         and ``node2`` at the corresponding axes. If new size is smaller, the
         tensor will be cropped; if larger, the tensor will be expanded with zeros.
-        In both cases, the process (cropping/expanding) occurs at the "left",
-        "top", "front", etc. of each dimension.
+        In both cases, the process (cropping/expanding) occurs at the "right",
+        "bottom", "back", etc. of each dimension.
         
         Parameters
         ----------
         size : int
             New size of the edge.
             
         Examples
@@ -3284,22 +3284,22 @@
         >>> nodeB = tk.ones((3, 4))
         >>> _ = edge = nodeA[1] ^ nodeB[0]
         >>> edge.size()
         3
         
         >>> edge.change_size(4)
         >>> nodeA.tensor
-        tensor([[0., 1., 1., 1.],
-                [0., 1., 1., 1.]])
+        tensor([[1., 1., 1., 0.],
+                [1., 1., 1., 0.]])
         
         >>> nodeB.tensor
-        tensor([[0., 0., 0., 0.],
+        tensor([[1., 1., 1., 1.],
                 [1., 1., 1., 1.],
                 [1., 1., 1., 1.],
-                [1., 1., 1., 1.]])
+                [0., 0., 0., 0.]])
                 
         >>> edge.size()
         4
         
         >>> edge.change_size(2)
         >>> nodeA.tensor
         tensor([[1., 1.],
```

### Comparing `tensorkrowch-1.1.2/tensorkrowch/decompositions/svd_decompositions.py` & `tensorkrowch-1.1.3/tensorkrowch/decompositions/svd_decompositions.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.2/tensorkrowch/embeddings.py` & `tensorkrowch-1.1.3/tensorkrowch/embeddings.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.2/tensorkrowch/initializers.py` & `tensorkrowch-1.1.3/tensorkrowch/initializers.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.2/tensorkrowch/models/mpo.py` & `tensorkrowch-1.1.3/tensorkrowch/models/mpo.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,16 +333,20 @@
         return self._mats_env
     
     @property
     def tensors(self) -> List[torch.Tensor]:
         """Returns the list of MPO tensors."""
         mpo_tensors = [node.tensor for node in self._mats_env]
         if self._boundary == 'obc':
-            mpo_tensors[0] = mpo_tensors[0][0, :, :]
-            mpo_tensors[-1] = mpo_tensors[-1][:, :, 0]
+            mpo_tensors[0] = torch.einsum('l,liro->iro',
+                                          self.left_node.tensor,
+                                          mpo_tensors[0])
+            mpo_tensors[-1] = torch.einsum('liro,r->lio',
+                                           mpo_tensors[-1],
+                                           self.right_node.tensor)
         return mpo_tensors
     
     # -------
     # Methods
     # -------
     def _make_nodes(self) -> None:
         """Creates all the nodes of the MPO."""
@@ -557,19 +561,37 @@
             
         return net
     
     def update_bond_dim(self) -> None:
         """
         Updates the :attr:`bond_dim` attribute of the ``MPO``, in case it is
         outdated.
+        
+        If bond dimensions are changed, usually due to decompositions like
+        :func:`~tensorkrowch.svd`, ``update_bond_dim`` should be
+        called. This might modify some elements of the model, so it is
+        recommended to do this before saving the ``state_dict`` of the model.
+        Besides, if one wants to continue training, the ``parameters`` of the
+        model that are passed to the optimizer should be updated also.
+        Otherwise, the optimizer could be tracking outdated parameters that are
+        not members of the model any more.
         """
         if self._boundary == 'obc':
-            self._bond_dim = [node.shape[2] for node in self._mats_env[:-1]]
+            self._bond_dim = [node._shape[2] for node in self._mats_env[:-1]]
+            
+            if self._bond_dim:
+                left_size = self._bond_dim[0]
+                if left_size != self._mats_env[0]._shape[0]:
+                    self._mats_env[0]['left'].change_size(left_size)
+                
+                right_size = self._bond_dim[-1]
+                if right_size != self._mats_env[-1]._shape[2]:
+                    self._mats_env[-1]['right'].change_size(right_size)
         else:
-            self._bond_dim = [node.shape[2] for node in self._mats_env]
+            self._bond_dim = [node._shape[2] for node in self._mats_env]
     
     def _input_contraction(self,
                            nodes_env: List[AbstractNode],
                            input_nodes: List[AbstractNode],
                            inline_input: bool = False) -> Tuple[
                                                        Optional[List[Node]],
                                                        Optional[List[Node]]]:
@@ -956,19 +978,16 @@
             rescale = (log_norm / len(nodes)).exp()
         
         if renormalize and (log_norm != 0):
             for node in nodes:
                 node.tensor = node.tensor * rescale
         
         # Update variables
-        if self._boundary == 'obc':
-            self._bond_dim = [node['right'].size() for node in nodes[:-1]]
-        else:
-            self._bond_dim = [node['right'].size() for node in nodes]
         self._mats_env = nodes
+        self.update_bond_dim()
 
         self.auto_stack = prev_auto_stack
 
 
 class UMPO(MPO):  # MARK: UMPO
     """
     Class for Uniform (translationally invariant) Matrix Product Operators. It is
```

### Comparing `tensorkrowch-1.1.2/tensorkrowch/models/mps.py` & `tensorkrowch-1.1.3/tensorkrowch/models/mps.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,16 +518,20 @@
         return [self._mats_env[i] for i in self._out_features]
 
     @property
     def tensors(self) -> List[torch.Tensor]:
         """Returns the list of MPS tensors."""
         mps_tensors = [node.tensor for node in self._mats_env]
         if self._boundary == 'obc':
-            mps_tensors[0] = mps_tensors[0][0, :, :]
-            mps_tensors[-1] = mps_tensors[-1][:, :, 0]
+            mps_tensors[0] = torch.einsum('l,lir->ir',
+                                          self.left_node.tensor,
+                                          mps_tensors[0])
+            mps_tensors[-1] = torch.einsum('lir,r->li',
+                                           mps_tensors[-1],
+                                           self.right_node.tensor)
         return mps_tensors
     
     # -------
     # Methods
     # -------
     def _make_nodes(self) -> None:
         """Creates all the nodes of the MPS."""
@@ -853,19 +857,37 @@
             
         return net
     
     def update_bond_dim(self) -> None:
         """
         Updates the :attr:`bond_dim` attribute of the ``MPS``, in case it is
         outdated.
+        
+        If bond dimensions are changed, usually due to decompositions like
+        :func:`~tensorkrowch.svd`, ``update_bond_dim`` should be
+        called. This might modify some elements of the model, so it is
+        recommended to do this before saving the ``state_dict`` of the model.
+        Besides, if one wants to continue training, the ``parameters`` of the
+        model that are passed to the optimizer should be updated also.
+        Otherwise, the optimizer could be tracking outdated parameters that are
+        not members of the model any more.
         """
         if self._boundary == 'obc':
-            self._bond_dim = [node.shape[-1] for node in self._mats_env[:-1]]
+            self._bond_dim = [node._shape[-1] for node in self._mats_env[:-1]]
+            
+            if self._bond_dim:
+                left_size = self._bond_dim[0]
+                if left_size != self._mats_env[0]._shape[0]:
+                    self._mats_env[0]['left'].change_size(left_size)
+                
+                right_size = self._bond_dim[-1]
+                if right_size != self._mats_env[-1]._shape[-1]:
+                    self._mats_env[-1]['right'].change_size(right_size)
         else:
-            self._bond_dim = [node.shape[-1] for node in self._mats_env]
+            self._bond_dim = [node._shape[-1] for node in self._mats_env]
 
     def _input_contraction(self,
                            nodes_env: List[AbstractNode],
                            input_nodes: List[AbstractNode],
                            inline_input: bool = False) -> Tuple[
                                                        Optional[List[Node]],
                                                        Optional[List[Node]]]:
@@ -1661,19 +1683,16 @@
             rescale = (log_norm / len(nodes)).exp()
         
         if renormalize and (log_norm != 0):
             for node in nodes:
                 node.tensor = node.tensor * rescale
         
         # Update variables
-        if self._boundary == 'obc':
-            self._bond_dim = [node['right'].size() for node in nodes[:-1]]
-        else:
-            self._bond_dim = [node['right'].size() for node in nodes]
         self._mats_env = nodes
+        self.update_bond_dim()
 
         self.auto_stack = prev_auto_stack
         
         if renormalize:
             return entropy, log_norm
         else:
             return entropy
@@ -1834,19 +1853,16 @@
             rescale = (log_norm / len(nodes)).exp()
         
         if renormalize and (log_norm != 0):
             for node in nodes:
                 node.tensor = node.tensor * rescale
         
         # Update variables
-        if self._boundary == 'obc':
-            self._bond_dim = [node['right'].size() for node in nodes[:-1]]
-        else:
-            self._bond_dim = [node['right'].size() for node in nodes]
         self._mats_env = nodes
+        self.update_bond_dim()
 
         self.auto_stack = prev_auto_stack
 
     def _project_to_bond_dim(self,
                              nodes: List[AbstractNode],
                              bond_dim: int,
                              side: Text = 'right'):
@@ -1994,20 +2010,20 @@
         self.auto_stack = False
 
         nodes = self._mats_env[:]
         for node in nodes:
             if not node['input'].is_dangling():
                 node['input'].disconnect()
         
-        if self._boundary == 'obc':
-            nodes[0] = self._left_node @ nodes[0]
-            nodes[0].reattach_edges(axes=['input'])
-            
-            nodes[-1] = nodes[-1] @ self._right_node
-            nodes[-1].reattach_edges(axes=['input'])
+        # Boundary is 'obc'
+        nodes[0] = self._left_node @ nodes[0]
+        nodes[0].reattach_edges(axes=['input'])
+        
+        nodes[-1] = nodes[-1] @ self._right_node
+        nodes[-1].reattach_edges(axes=['input'])
 
         new_tensors = []
         left_nodeC = None
         for i in range(self._n_features):
             tensor, left_nodeC = self._aux_canonicalize_univocal(
                 nodes=nodes,
                 idx=i,
@@ -2020,14 +2036,15 @@
                     node['right'].change_size(self._bond_dim[i])
 
             if not node['input'].is_dangling():
                 self.delete_node(node.neighbours('input'))
         
         self.reset()
         self.initialize(tensors=new_tensors)
+        self.update_bond_dim()
 
         for node, data_node in zip(self._mats_env, self._data_nodes.values()):
             node['input'] ^ data_node['feature']
 
         self.auto_stack = prev_auto_stack
```

### Comparing `tensorkrowch-1.1.2/tensorkrowch/models/mps_data.py` & `tensorkrowch-1.1.3/tensorkrowch/models/mps_data.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.2/tensorkrowch/models/peps.py` & `tensorkrowch-1.1.3/tensorkrowch/models/peps.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.2/tensorkrowch/models/tree.py` & `tensorkrowch-1.1.3/tensorkrowch/models/tree.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.2/tensorkrowch/operations.py` & `tensorkrowch-1.1.3/tensorkrowch/operations.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.2/tensorkrowch/utils.py` & `tensorkrowch-1.1.3/tensorkrowch/utils.py`

 * *Files identical despite different names*

### Comparing `tensorkrowch-1.1.2/tensorkrowch.egg-info/PKG-INFO` & `tensorkrowch-1.1.3/tensorkrowch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorkrowch
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tensor Networks with PyTorch
 Author-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 Maintainer-email: José Ramón Pareja Monturiol <joserapa98@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 José Ramón Pareja Monturiol
```

### Comparing `tensorkrowch-1.1.2/tensorkrowch.egg-info/SOURCES.txt` & `tensorkrowch-1.1.3/tensorkrowch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

