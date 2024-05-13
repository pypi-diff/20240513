# Comparing `tmp/parameterframe-0.1.1.tar.gz` & `tmp/parameterframe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parameterframe-0.1.1.tar", last modified: Tue May  7 18:09:30 2024, max compression
+gzip compressed data, was "parameterframe-0.1.2.tar", last modified: Mon May 13 21:35:15 2024, max compression
```

## Comparing `parameterframe-0.1.1.tar` & `parameterframe-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:09:30.053840 parameterframe-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-07 18:06:28.000000 parameterframe-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40400 2024-05-07 18:09:30.053840 parameterframe-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-07 18:06:28.000000 parameterframe-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:09:30.049840 parameterframe-0.1.1/parameterframe/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    93187 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe/parameterframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:09:30.053840 parameterframe-0.1.1/parameterframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40400 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-07 18:09:30.000000 parameterframe-0.1.1/parameterframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 18:09:30.053840 parameterframe-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:35:15.268926 parameterframe-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-13 21:31:50.000000 parameterframe-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40400 2024-05-13 21:35:15.268926 parameterframe-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-13 21:31:50.000000 parameterframe-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:35:15.268926 parameterframe-0.1.2/parameterframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 21:34:48.000000 parameterframe-0.1.2/parameterframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96932 2024-05-13 21:34:48.000000 parameterframe-0.1.2/parameterframe/parameterframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-13 21:35:14.000000 parameterframe-0.1.2/parameterframe/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:35:15.268926 parameterframe-0.1.2/parameterframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40400 2024-05-13 21:35:15.000000 parameterframe-0.1.2/parameterframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-13 21:35:15.000000 parameterframe-0.1.2/parameterframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:35:15.000000 parameterframe-0.1.2/parameterframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 21:35:15.000000 parameterframe-0.1.2/parameterframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 21:35:15.000000 parameterframe-0.1.2/parameterframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:35:15.268926 parameterframe-0.1.2/setup.cfg
```

### Comparing `parameterframe-0.1.1/LICENSE` & `parameterframe-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parameterframe-0.1.1/PKG-INFO` & `parameterframe-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameterframe
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','parameter storage']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `parameterframe-0.1.1/README.md` & `parameterframe-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `parameterframe-0.1.1/parameterframe/parameterframe.py` & `parameterframe-0.1.2/parameterframe/parameterframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,26 @@
 import hashlib
 from datetime import datetime
 from mocker_db import MockerDB, MockerConnector #==0.1.1
 import yaml
 from collections import defaultdict
 import logging
 import ast
-
+import pandas as pd
 from sqlalchemy import create_engine, Column, String, Text, ForeignKey, DateTime
 from sqlalchemy.orm import relationship, sessionmaker, declarative_base
 from sqlalchemy.exc import SQLAlchemyError, IntegrityError, DBAPIError
 from sqlalchemy import inspect
+# encodeing and compression
+import base64
+import zlib
+# encrypting
+from cryptography.hazmat.primitives.kdf.scrypt import Scrypt
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 
 
 __design_choices__ = {
     "FileTypeHandler" : ['prepares one parameter file and reconstructs one parameter file at a time',
                          'txt and yaml files can be processed',
                          'yaml files are not reconstructed 1to1 but are first make into python dictionary, with python type mapping'],
     "ParameterFrame" : ['parameter_names and paramer_description are optional'],
@@ -415,21 +422,27 @@
         __tablename__ = 'parameter_description'
         parameter_id = Column(String, primary_key=True)
         parameter_name = Column(String)
         parameter_description = Column(Text)
         file_name = Column(String)
         file_type = Column(String)
 
+    # class ParameterAttribute(Base):
+    #     __tablename__ = 'parameter_attribute'
+    #     parameter_id = Column(String, ForeignKey('parameter_description.parameter_id'), primary_key=True)
+    #     attribute_id = Column(String, ForeignKey('attribute_values.attribute_id'), primary_key=True)
+    #     previous_attribute_id = Column(String, nullable=True)
+    #     attribute_values = relationship("AttributeValues")
+    #     parameter_description = relationship("ParameterDescription")
+
     class ParameterAttribute(Base):
         __tablename__ = 'parameter_attribute'
-        parameter_id = Column(String, ForeignKey('parameter_description.parameter_id'), primary_key=True)
-        attribute_id = Column(String, ForeignKey('attribute_values.attribute_id'), primary_key=True)
+        parameter_id = Column(String, primary_key=True)
+        attribute_id = Column(String, primary_key=True)
         previous_attribute_id = Column(String, nullable=True)
-        attribute_values = relationship("AttributeValues")
-        parameter_description = relationship("ParameterDescription")
 
     class ParameterSet(Base):
         __tablename__ = 'parameter_set'
         parameter_set_id = Column(String, primary_key=True)
         parameter_id = Column(String,primary_key=True)
         #parameter_description = relationship("ParameterDescription")
         # If ParameterAttribute should be related here, it needs adjustment.
@@ -697,14 +710,15 @@
     """
     Handles raw files, processes them for storage
     and reconstructs when pulling from storage.
     """
 
     # inputs
     file_path = attr.ib(default=None, type = str)
+    password = attr.ib(default=None, type = str)
 
     # inputs for reconstruction
     parameter_name = attr.ib(default='', type = str)
     parameter_description = attr.ib(default='', type = str)
     parameter_attributes_list = attr.ib(default=None, type = list)
     attribute_values_list = attr.ib(default=None, type = list)
 
@@ -724,15 +738,14 @@
     loggerLvl = attr.ib(default=logging.INFO)
     logger_format = attr.ib(default=None)
 
 
     def __attrs_post_init__(self):
         self._initialize_logger()
 
-
     def _initialize_logger(self):
 
         """
         Initialize a logger for the class instance based on the specified logging level and logger name.
         """
 
         if self.logger is None:
@@ -903,21 +916,89 @@
         return encoded_bytes#.decode('utf-8')
 
     def _decode_obj(self, encoded_data : object) -> object:
         """Decode data from serialized object."""
         decoded_bytes = dill.loads(encoded_data)
         return decoded_bytes
 
-    def _encode_binary(self, data : str) -> str:
-        """Encode data using Base64."""
-        return str(data)
-
-    def _decode_binary(self, encoded_data : str) -> str:
-        """Decode data from Base64."""
-        return ast.literal_eval(encoded_data)
+    def _compress_string_zlib(self, input_string : str):
+        # Compressing directly from string bytes
+        compressed_data = str(zlib.compress(input_string.encode('utf-8')))
+        return compressed_data
+
+    def _decompress_zlib(self, compressed_data : bin):
+        # Decompressing and decoding the bytes back to a string
+        return zlib.decompress(compressed_data).decode('utf-8')
+
+    def _derive_key(self,password: str, salt: bytes, key_length=32):
+        """ Derive a key from a password and salt. """
+        kdf = Scrypt(
+            salt=salt,
+            length=key_length,
+            n=2**14,
+            r=8,
+            p=1,
+            backend=default_backend()
+        )
+        return kdf.derive(password.encode())
+
+    def _encrypt_data(self, data, password):
+        """Encrypts data using AES-CBC."""
+
+        salt = os.urandom(16)
+        key = self._derive_key(password, salt=salt)
+
+        iv = os.urandom(16)  # Generate a random IV
+        cipher = Cipher(algorithms.AES(key), modes.CBC(iv), backend=default_backend())
+        encryptor = cipher.encryptor()
+        # Ensure the data is a multiple of 16 in length
+        padded_data = data + (16 - len(data) % 16) * bytes([16 - len(data) % 16])
+        encrypted_data = encryptor.update(padded_data) + encryptor.finalize()
+        return salt + iv + encrypted_data  # Include salt and IV for decryption
+
+    def _decrypt_data(self, encrypted_data, password):
+        """Decrypts data that was encrypted with AES-CBC."""
+        salt = encrypted_data[:16]
+        iv = encrypted_data[16:32]
+        encrypted_data = encrypted_data[32:]
+
+        key = self._derive_key(password,salt)  # Derive the key again with the new salt
+        cipher = Cipher(algorithms.AES(key), modes.CBC(iv), backend=default_backend())
+        decryptor = cipher.decryptor()
+        decrypted_padded_data = decryptor.update(encrypted_data) + decryptor.finalize()
+        pad_length = decrypted_padded_data[-1]  # Remove padding
+        return decrypted_padded_data[:-pad_length]
+
+    def _encode_binary(self, data, password = None):
+        """Encodes binary data to a compressed base64 string, with optional encryption."""
+
+        if password is None:
+            password = self.password
+
+        compressed_data = zlib.compress(data)
+        if password:
+            encrypted_data = self._encrypt_data(compressed_data, password=password)
+            base64_encoded = base64.b64encode(encrypted_data).decode('utf-8')
+        else:
+            base64_encoded = base64.b64encode(compressed_data).decode('utf-8')
+        return base64_encoded
+
+    def _decode_binary(self, encoded_data, password = None):
+        """Decodes a base64 string back to original binary, with optional decryption."""
+
+        if password is None:
+            password = self.password
+
+        data = base64.b64decode(encoded_data.encode('utf-8'))
+        if password:
+            decrypted_data = self._decrypt_data(data, password=password)
+            decompressed_data = zlib.decompress(decrypted_data)
+        else:
+            decompressed_data = zlib.decompress(data)
+        return decompressed_data
 
 
     def _process_dill(self,
                      content : dict,
                      parameter_id : str = None) -> tuple:
 
         """
@@ -952,15 +1033,15 @@
 
         if chunk_size is None:
             chunk_size = self.chunk_size
 
         parameter_attributes = []
         attribute_values = []
 
-        str_content = str(content)
+        str_content = self._encode_binary(data = content)
 
         # Split the text into chunks of chunk_size
         for i in range(0, len(str_content), chunk_size):
             chunk = str_content[i:i+chunk_size]
             attribute_id = self._generate_unique_id(chunk)
 
             parameter_attributes.append({
@@ -969,15 +1050,15 @@
                 # Assuming each chunk is sequential and does not have a 'parent' as in a tree structure
                 'previous_attribute_id': None if i == 0 else parameter_attributes[-1]['attribute_id']
             })
 
             attribute_values.append({
                 'attribute_id': attribute_id,
                 'attribute_name': f'{int(i//chunk_size)}',
-                'attribute_value': self._encode_binary(data = chunk),
+                'attribute_value':  chunk,
             'attribute_value_type': type(content).__name__
             })
 
         return parameter_attributes, attribute_values
 
 
     def _process_yaml(self,
@@ -1387,14 +1468,16 @@
     params_path = attr.ib(default=None)
 
     # optional
     solution_id = attr.ib(default=None, type=str)
     param_names = attr.ib(default=None, type=dict)
     param_descriptions = attr.ib(default=None, type=dict)
     seed = attr.ib(default=None, type=int)
+    chunk_size = attr.ib(default=255, type=int)
+    password = attr.ib(default=None, type=str)
 
     connection_details = attr.ib(default = {
         'base_url' : "http://localhost:8000"})
 
     # dependancies
     database_connector = attr.ib(default=None, type=MockerDatabaseConnector)
     file_type_handler = attr.ib(default=FileTypeHandler)
@@ -1419,16 +1502,14 @@
         self._initialize_logger()
 
         if self.database_connector is None:
             self.database_connector = MockerDatabaseConnector(connection_details = self.connection_details)
 
         self._initialize_name_generator()
 
-        import pandas as pd
-
         self.pd = pd
         self.pd.set_option('display.max_colwidth', 70)
 
         self.solutions = {}
         self.param_sets = {}
         self.commited_tables = {}
         self.param_attributes = {}
@@ -1490,15 +1571,17 @@
             param_descriptions = {pn : '' for pn in param_names}
 
         for param_name in param_names:
 
             self.param_attributes[param_name] = self.file_type_handler(
                 file_path = param_names[param_name],
                 parameter_name = param_name,
-                parameter_description = param_descriptions[param_name]
+                parameter_description = param_descriptions[param_name],
+                chunk_size = self.chunk_size,
+                password = self.password
             )
 
             self.param_attributes[param_name].process_file()
 
         return True
 
     def make_parameter_set(self,
@@ -1878,15 +1961,17 @@
             file_name = param_id_paths[param_id]
             file_path = os.path.join(params_path, file_name)
 
             fth = self.file_type_handler(
                         file_path = file_path,
                         parameter_id = param_id,
                         parameter_attributes_list = parameter_attribute_list,
-                        attribute_values_list = attribute_values_list
+                        attribute_values_list = attribute_values_list,
+                        chunk_size = self.chunk_size,
+                        password = self.password
                     )
             fth.reconstruct_file()
 
 
         return True
 
     def reconstruct_parameter_set(self,
```

### Comparing `parameterframe-0.1.1/parameterframe/setup.py` & `parameterframe-0.1.2/parameterframe/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="parameterframe",
     packages=["parameterframe"],
-    install_requires=['### parameterframe.py', 'attrs', 'sqlalchemy', 'mocker_db==0.1.1', 'dill', 'pyyaml'],
+    install_requires=['### parameterframe.py', 'dill', 'attrs', 'pyyaml', 'sqlalchemy', 'pandas', 'mocker_db==0.1.1', 'cryptography'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.1.1"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.1.2"
 )
```

### Comparing `parameterframe-0.1.1/parameterframe.egg-info/PKG-INFO` & `parameterframe-0.1.2/parameterframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameterframe
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','parameter storage']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

