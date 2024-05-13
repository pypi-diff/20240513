# Comparing `tmp/brukeropus-1.0.3.tar.gz` & `tmp/brukeropus-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brukeropus-1.0.3.tar", last modified: Sat May 11 02:18:02 2024, max compression
+gzip compressed data, was "brukeropus-1.0.4.tar", last modified: Mon May 13 12:33:52 2024, max compression
```

## Comparing `brukeropus-1.0.3.tar` & `brukeropus-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 02:18:02.519623 brukeropus-1.0.3/
--rw-rw-rw-   0        0        0     1087 2024-02-29 18:02:08.000000 brukeropus-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     5274 2024-05-11 02:18:02.519623 brukeropus-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4523 2024-05-03 14:26:32.000000 brukeropus-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 02:18:02.488390 brukeropus-1.0.3/brukeropus/
--rw-rw-rw-   0        0        0     2581 2024-05-03 13:47:15.000000 brukeropus-1.0.3/brukeropus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 02:18:02.504010 brukeropus-1.0.3/brukeropus/control/
--rw-rw-rw-   0        0        0     1746 2024-04-24 01:13:04.000000 brukeropus-1.0.3/brukeropus/control/__init__.py
--rw-rw-rw-   0        0        0     9678 2024-04-23 16:48:27.000000 brukeropus-1.0.3/brukeropus/control/dde.py
--rw-rw-rw-   0        0        0    11639 2024-04-24 00:59:48.000000 brukeropus-1.0.3/brukeropus/control/opus.py
-drwxrwxrwx   0        0        0        0 2024-05-11 02:18:02.519623 brukeropus-1.0.3/brukeropus/file/
--rw-rw-rw-   0        0        0    17333 2024-04-23 18:20:14.000000 brukeropus-1.0.3/brukeropus/file/__init__.py
--rw-rw-rw-   0        0        0     9467 2024-03-05 15:18:18.000000 brukeropus-1.0.3/brukeropus/file/constants.py
--rw-rw-rw-   0        0        0    26208 2024-05-11 02:14:16.000000 brukeropus-1.0.3/brukeropus/file/file.py
--rw-rw-rw-   0        0        0    13123 2024-05-11 02:12:49.000000 brukeropus-1.0.3/brukeropus/file/parser.py
--rw-rw-rw-   0        0        0     9949 2024-02-29 18:02:08.000000 brukeropus-1.0.3/brukeropus/file/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-11 02:18:02.519623 brukeropus-1.0.3/brukeropus.egg-info/
--rw-rw-rw-   0        0        0     5274 2024-05-11 02:18:02.000000 brukeropus-1.0.3/brukeropus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2024-05-11 02:18:02.000000 brukeropus-1.0.3/brukeropus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 02:18:02.000000 brukeropus-1.0.3/brukeropus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-11 02:18:02.000000 brukeropus-1.0.3/brukeropus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-11 02:18:02.000000 brukeropus-1.0.3/brukeropus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      816 2024-05-11 02:16:06.000000 brukeropus-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 02:18:02.519623 brukeropus-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 12:33:52.294297 brukeropus-1.0.4/
+-rw-rw-rw-   0        0        0     1087 2024-02-29 18:02:08.000000 brukeropus-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5274 2024-05-13 12:33:52.294297 brukeropus-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4523 2024-05-03 14:26:32.000000 brukeropus-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 12:33:52.263112 brukeropus-1.0.4/brukeropus/
+-rw-rw-rw-   0        0        0     2581 2024-05-03 13:47:15.000000 brukeropus-1.0.4/brukeropus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 12:33:52.278703 brukeropus-1.0.4/brukeropus/control/
+-rw-rw-rw-   0        0        0     1746 2024-04-24 01:13:04.000000 brukeropus-1.0.4/brukeropus/control/__init__.py
+-rw-rw-rw-   0        0        0     9678 2024-04-23 16:48:27.000000 brukeropus-1.0.4/brukeropus/control/dde.py
+-rw-rw-rw-   0        0        0    11639 2024-04-24 00:59:48.000000 brukeropus-1.0.4/brukeropus/control/opus.py
+drwxrwxrwx   0        0        0        0 2024-05-13 12:33:52.278703 brukeropus-1.0.4/brukeropus/file/
+-rw-rw-rw-   0        0        0    17333 2024-04-23 18:20:14.000000 brukeropus-1.0.4/brukeropus/file/__init__.py
+-rw-rw-rw-   0        0        0     9467 2024-05-11 03:08:24.000000 brukeropus-1.0.4/brukeropus/file/constants.py
+-rw-rw-rw-   0        0        0    26497 2024-05-11 03:37:06.000000 brukeropus-1.0.4/brukeropus/file/file.py
+-rw-rw-rw-   0        0        0    13123 2024-05-11 02:12:49.000000 brukeropus-1.0.4/brukeropus/file/parser.py
+-rw-rw-rw-   0        0        0    10049 2024-05-11 03:55:21.000000 brukeropus-1.0.4/brukeropus/file/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 12:33:52.294297 brukeropus-1.0.4/brukeropus.egg-info/
+-rw-rw-rw-   0        0        0     5274 2024-05-13 12:33:52.000000 brukeropus-1.0.4/brukeropus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2024-05-13 12:33:52.000000 brukeropus-1.0.4/brukeropus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 12:33:52.000000 brukeropus-1.0.4/brukeropus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-13 12:33:52.000000 brukeropus-1.0.4/brukeropus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 12:33:52.000000 brukeropus-1.0.4/brukeropus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      816 2024-05-13 12:32:20.000000 brukeropus-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 12:33:52.294297 brukeropus-1.0.4/setup.cfg
```

### Comparing `brukeropus-1.0.3/LICENSE` & `brukeropus-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.3/PKG-INFO` & `brukeropus-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brukeropus
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python package for communicating with Bruker OPUS spectroscopy software and reading its binary file format.
 Author-email: Josh Duran <josh.m.duran@gmail.com>
 Project-URL: Homepage, https://github.com/joshduran/brukeropus
 Project-URL: Issues, https://github.com/joshduran/brukeropus/issues
 Project-URL: Documentation, https://joshduran.github.io/brukeropus/brukeropus.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `brukeropus-1.0.3/README.md` & `brukeropus-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.3/brukeropus/__init__.py` & `brukeropus-1.0.4/brukeropus/__init__.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.3/brukeropus/control/__init__.py` & `brukeropus-1.0.4/brukeropus/control/__init__.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.3/brukeropus/control/dde.py` & `brukeropus-1.0.4/brukeropus/control/dde.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.3/brukeropus/control/opus.py` & `brukeropus-1.0.4/brukeropus/control/opus.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.3/brukeropus/file/__init__.py` & `brukeropus-1.0.4/brukeropus/file/__init__.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.3/brukeropus/file/constants.py` & `brukeropus-1.0.4/brukeropus/file/constants.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.3/brukeropus/file/file.py` & `brukeropus-1.0.4/brukeropus/file/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,56 +157,53 @@
 
     Attributes:
         type: six integer tuple that describes the type of data in the file block
         size: size of block in number of bytes
         start: pointer to start location of the block within the file
         keys: tuple of three char keys contained in parameter blocks. This attribute is set by the OPUSFile class only
             when the block is parameter block. This enables grouping parameters by block if desired.
+        bytes: raw bytes of file block (currently only set for unknown blocks)
     '''
 
-    __slots__ = ('type', 'size', 'start', 'keys')
+    __slots__ = ('type', 'size', 'start', 'keys', 'bytes')
 
     keys: tuple
 
     def __init__(self, block_type: tuple, size: int, start: int):
         self.type = block_type
         self.size = size
         self.start = start
 
     def __str__(self):
         label = self.get_label()
         return 'Block Info: ' + label + ' (size: ' + str(self.size) + ' bytes; start: ' + str(self.start) + ')'
 
-    def is_valid(self):
-        '''Returns False if FileBlockInfo is undefined (i.e. FileBlockInfo.type == (0, 0, 0, 0, 0, 0))'''
-        return self.type != (0, 0, 0, 0, 0, 0)
-
     def is_data_status(self):
         '''Returns True if FileBlockInfo is a data status parameter block'''
         return self.type[2] == 1
 
     def is_rf_param(self):
         '''Returns True if FileBlockInfo is a parameter block associated with the reference measurement'''
         return self.type[2] > 1 and self.type[1] == 2
 
     def is_param(self):
         '''Returns True if FileBlockInfo is a parameter block'''
-        return self.type[2] > 1
+        return self.type[2] > 1 or self.type == (0, 0, 0, 0, 0, 1)
 
     def is_directory(self):
         '''Returns True if FileBlockInfo is the directory block'''
         return self.type == (0, 0, 0, 13, 0, 0)
 
     def is_file_log(self):
         '''Returns True if FileBlockInfo is the file log block'''
         return self.type == (0, 0, 0, 0, 0, 5)
 
     def is_data(self):
         '''Returns True if FileBlockInfo is a data block or 3D data block'''
-        return self.type[2] == 0 and self.type[3] > 0 and self.type[3] != 13
+        return self.type[0] > 0 and self.type[1] > 0 and self.type[2] == 0 and self.type[3] > 0
 
     def is_3d_data(self):
         '''Returns True if FileBlockInfo is a 3D data block (i.e. data series)'''
         return self.is_data() and self.type[5] == 2
 
     def is_data_status_match(self, data_block_info):
         '''Returns True if FileBlockInfo is a data status block and a match to the data_block_info argument.
@@ -462,41 +459,47 @@
         data_status_blocks: list of `FileBlockInfo` that contain metadata specific to a data block (units, etc.)
         param_blocks: list of `FileBlockInfo` that contain metadata about the measurement sample
         rf_param_blocks: list of `FileBlockInfo` that contain metatdata about the reference measurement
         directory_block: `FileBlockInfo` for directory block that contains all the block info in the file
         file_log_block: `FileBlockInfo` of the file log (changes, etc.)
         data_and_status_block_pairs: (data: `FileBlockInfo`, data_status: `FileBlockInfo`) which pairs the data status
             parameter block (time, x units, y units, etc.) with the data block it informs
+        unknown_blocks: list of `FileBlockInfo` with an unrecognized type (i.e. not sure how to parse)
     '''
 
     __slots__ = ('version', 'start', 'max_blocks', 'num_blocks', 'data_blocks', 'data_status_blocks', 'param_blocks',
-                 'rf_param_blocks', 'directory_block', 'file_log_block', 'data_and_status_block_pairs')
+                 'rf_param_blocks', 'directory_block', 'file_log_block', 'data_and_status_block_pairs',
+                 'unknown_blocks')
 
     def __init__(self, filebytes: bytes):
         self.version, self.start, self.max_blocks, self.num_blocks = parse_header(filebytes)
         self.data_blocks: list = []
         self.data_status_blocks: list = []
         self.param_blocks: list = []
         self.rf_param_blocks: list = []
         self.directory_block: FileBlockInfo
         self.file_log_block: FileBlockInfo
+        self.unknown_blocks: list = []
         for block_type, size, start in parse_directory(filebytes, self.start, self.num_blocks):
             block = FileBlockInfo(block_type=block_type, size=size, start=start)
             if block.is_data_status():
                 self.data_status_blocks.append(block)
             elif block.is_rf_param():
                 self.rf_param_blocks.append(block)
             elif block.is_param():
                 self.param_blocks.append(block)
             elif block.is_directory():
                 self.directory_block = block
             elif block.is_file_log():
                 self.file_log_block = block
-            elif block.is_valid():
+            elif block.is_data():
                 self.data_blocks.append(block)
+            else:
+                block.bytes = filebytes[block.start:block.start + block.size]
+                self.unknown_blocks.append(block)
         self.data_and_status_block_pairs = []
         self._pair_data_and_status_blocks()
 
     def __str__(self):
         data_keys = [b.get_data_key() for b in self.data_blocks]
         data_str = ', '.join(data_keys)
         return 'File Directory: ' + str(self.num_blocks) + ' total blocks; data blocks: (' + data_str + ')'
```

### Comparing `brukeropus-1.0.3/brukeropus/file/parser.py` & `brukeropus-1.0.4/brukeropus/file/parser.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.3/brukeropus/file/utils.py` & `brukeropus-1.0.4/brukeropus/file/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,34 +195,34 @@
     param_col_widths = (10, 45, 45)
     key_width = 10
     key_label_width = 45
     param_col_widths = (key_width, key_label_width, width - key_width - key_label_width)
     param_col_labels = ('Key', 'Friendly Name', 'Value')
     if block_info[0] != (0, 0, 0, 13, 0, 0):
         _print_block_header(get_block_type_label(block_info[0]), width)
-        if block_info[0][2] > 0:
+        if block_info[0][2] > 0 or block_info[0] == (0, 0, 0, 0, 0, 1):
             _print_cols(param_col_labels, param_col_widths)
             for key, val in parse_param_block(filebytes, block_info[1], block_info[2]):
                 _print_cols((key, get_param_label(key), val), param_col_widths)
         elif block_info[0] == (0, 0, 0, 0, 0, 5):
             log = parse_file_log(filebytes, block_info[1], block_info[2])
             for entry in log:
                 for line in textwrap.wrap(entry, width=width):
                     print(line)
         elif block_info[0][5] == 2:
             data = parse_3d_data_block(filebytes, block_info[2])
             _print_centered('Num Blocks: ' + str(data['num_blocks']), width)
             _print_centered('Store Table: ' + str(data['store_table']), width)
             print(data['y'])
-        elif block_info[0] == (0, 0, 0, 0, 0, 0):
-            _print_centered('Undefined Block Type: Raw Bytes', width)
-            print(filebytes[block_info[1]: block_info[1] + block_info[2]])
-        else:
+        elif block_info[0][0] > 0 and block_info[0][1] > 0 and block_info[0][2] == 0 and block_info[0][3] > 0:
             array = parse_data_block(filebytes, block_info[1], block_info[2])
             print(array)
+        else:
+            _print_centered('Undefined Block Type: Raw Bytes', width)
+            print(filebytes[block_info[2]: block_info[2] + block_info[1]])
 
 
 def _print_cols(vals, col_widths,):
     'Helper function for: parse_file_and_print'
     string = ''
     for i, val in enumerate(vals):
         col_width = col_widths[i]
```

### Comparing `brukeropus-1.0.3/brukeropus.egg-info/PKG-INFO` & `brukeropus-1.0.4/brukeropus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brukeropus
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python package for communicating with Bruker OPUS spectroscopy software and reading its binary file format.
 Author-email: Josh Duran <josh.m.duran@gmail.com>
 Project-URL: Homepage, https://github.com/joshduran/brukeropus
 Project-URL: Issues, https://github.com/joshduran/brukeropus/issues
 Project-URL: Documentation, https://joshduran.github.io/brukeropus/brukeropus.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `brukeropus-1.0.3/pyproject.toml` & `brukeropus-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "brukeropus"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Josh Duran", email="josh.m.duran@gmail.com" },
 ]
 description = "A python package for communicating with Bruker OPUS spectroscopy software and reading its binary file format."
 readme = "README.md"
 dependencies = ["numpy"]
 requires-python = ">=3.6"
```

