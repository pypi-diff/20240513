# Comparing `tmp/tkan-0.1.0.tar.gz` & `tmp/tkan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkan-0.1.0.tar", max compression
+gzip compressed data, was "tkan-0.1.1.tar", max compression
```

## Comparing `tkan-0.1.0.tar` & `tkan-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      489 2024-05-09 15:22:47.296178 tkan-0.1.0/README.md
--rw-r--r--   0        0        0      390 2024-05-09 16:03:50.680826 tkan-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      115 2024-05-09 15:54:41.624393 tkan-0.1.0/tkan/__init__.py
--rw-r--r--   0        0        0    11439 2024-05-09 15:49:06.996207 tkan-0.1.0/tkan/spline.py
--rw-r--r--   0        0        0    10619 2024-05-09 16:00:16.308645 tkan-0.1.0/tkan/tkan.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tkan-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2303 2024-05-13 19:32:19.328997 tkan-0.1.1/README.md
+-rw-r--r--   0        0        0      370 2024-05-13 19:32:19.328997 tkan-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      115 2024-05-09 15:54:41.624393 tkan-0.1.1/tkan/__init__.py
+-rw-r--r--   0        0        0    11439 2024-05-09 15:49:06.996207 tkan-0.1.1/tkan/spline.py
+-rw-r--r--   0        0        0    11030 2024-05-13 19:28:56.416159 tkan-0.1.1/tkan/tkan.py
+-rw-r--r--   0        0        0     2740 1970-01-01 00:00:00.000000 tkan-0.1.1/PKG-INFO
```

### Comparing `tkan-0.1.0/tkan/spline.py` & `tkan-0.1.1/tkan/spline.py`

 * *Files identical despite different names*

### Comparing `tkan-0.1.0/tkan/tkan.py` & `tkan-0.1.1/tkan/tkan.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     """
 
     def __init__(self, 
                  activation_funcs: List[Union[str, int, None, Callable]], 
                  num_outputs: int, 
                  return_sequences: bool = False, 
                  trainable_power_spline: bool = False, 
+                 return_state=False,
                  **kwargs) -> None:
         """
         Initializes a TKAN layer with specified activations, number of output units, and other configurations.
 
         Args:
             activation_funcs (List[Union[str, int, None, Callable]]): A list containing elements that specify the
                 type of activation function for each sub-layer. This can be a string for TensorFlow activations,
@@ -44,14 +45,15 @@
                 Defaults to False.
             **kwargs: Standard parameters for Keras layers (e.g., `name`).
         """
         super(TKAN, self).__init__(**kwargs)
         self.activation_funcs = activation_funcs
         self.num_outputs = num_outputs
         self.return_sequences = return_sequences
+        self.return_state = return_state
         self.aggregation_transform = tf.keras.layers.Dense(num_outputs, activation="sigmoid")
         # Sub-layer LSTM components
         self.global_biases = {}
         self.global_lstm_gates = {}
         self.global_recurrent_weights = {}
         self.sub_layers_lstm_weights = {}
         self.sub_layers = []
@@ -151,16 +153,18 @@
             c_tilde = tf.nn.sigmoid(tf.linalg.matmul(current_input, self.global_lstm_gates['Wc']) + tf.linalg.matmul(global_hidden_state , self.global_recurrent_weights['Uc']) + self.global_biases['bc'])
 
             global_cell_state = global_xf * global_cell_state + global_xi * c_tilde
             global_hidden_state = global_xo * tf.nn.tanh(global_cell_state)
             
             if self.return_sequences:
                 outputs.append(global_hidden_state)
-
-        return tf.stack(outputs, axis=1) if self.return_sequences else global_hidden_state
+        out = tf.stack(outputs, axis=1) if self.return_sequences else global_hidden_state
+        if self.return_state:
+            return out, global_hidden_state, global_cell_state
+        return out
 
 
     def compute_output_shape(self, input_shape: Tuple[int, int, int]) -> Union[Tuple[int, int, int], Tuple[int, int]]:
         """
         Computes the output shape of the layer based on the given input shape.
 
         Args:
@@ -171,13 +175,19 @@
         Returns:
             Union[Tuple[int, int, int], Tuple[int, int]]: Depending on the value of `return_sequences`,
             returns a tuple indicating the shape of the output tensor. If `return_sequences` is True,
             the output shape will be (batch_size, sequence_length, num_outputs), reflecting the full sequence
             of outputs. If False, the output shape will be (batch_size, num_outputs), reflecting the final
             output state only.
         """
+        batch_size = input_shape[0]
+        length = input_shape[1]
+
         if self.return_sequences:
-            return (input_shape[0], input_shape[1], self.num_outputs)
+            output_shape = (batch_size, length, self.num_outputs)
         else:
-            return (input_shape[0], self.num_outputs)
+            output_shape = (batch_size, self.num_outputs)
+        if self.return_state:
+            return output_shape, (batch_size, self.num_outputs), (batch_size, self.num_outputs)
+        return output_shape
```

