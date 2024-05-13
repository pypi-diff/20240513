# Comparing `tmp/bbpb-1.1.2.tar.gz` & `tmp/bbpb-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbpb-1.1.2.tar", max compression
+gzip compressed data, was "bbpb-1.2.0.tar", max compression
```

## Comparing `bbpb-1.1.2.tar` & `bbpb-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
--rw-r--r--   0        0        0    10944 2024-03-11 14:46:25.909121 bbpb-1.1.2/README.md
--rw-r--r--   0        0        0     1577 2024-03-11 14:46:25.909121 bbpb-1.1.2/blackboxprotobuf/__init__.py
--rw-r--r--   0        0        0     1382 2024-03-11 14:46:25.909121 bbpb-1.1.2/blackboxprotobuf/lib/__init__.py
--rw-r--r--   0        0        0    27266 2024-03-11 14:46:25.909121 bbpb-1.1.2/blackboxprotobuf/lib/api.py
--rw-r--r--   0        0        0     2265 2024-03-11 14:46:25.909121 bbpb-1.1.2/blackboxprotobuf/lib/config.py
--rw-r--r--   0        0        0     3760 2024-03-11 14:46:25.909121 bbpb-1.1.2/blackboxprotobuf/lib/exceptions.py
--rw-r--r--   0        0        0    16054 2024-03-11 14:46:25.909121 bbpb-1.1.2/blackboxprotobuf/lib/protofile.py
--rw-r--r--   0        0        0     1296 2024-03-11 14:46:25.909121 bbpb-1.1.2/blackboxprotobuf/lib/types/__init__.py
--rw-r--r--   0        0        0     3911 2024-03-11 14:46:25.909121 bbpb-1.1.2/blackboxprotobuf/lib/types/fixed.py
--rw-r--r--   0        0        0    26259 2024-03-11 14:46:25.909121 bbpb-1.1.2/blackboxprotobuf/lib/types/length_delim.py
--rw-r--r--   0        0        0     5089 2024-03-11 14:46:25.909121 bbpb-1.1.2/blackboxprotobuf/lib/types/type_maps.py
--rw-r--r--   0        0        0     5889 2024-03-11 14:46:25.909121 bbpb-1.1.2/blackboxprotobuf/lib/types/varint.py
--rw-r--r--   0        0        0     1217 2024-03-11 14:46:25.909121 bbpb-1.1.2/blackboxprotobuf/lib/types/wiretypes.py
--rw-r--r--   0        0        0      660 2024-03-11 14:46:25.909121 bbpb-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    11762 1970-01-01 00:00:00.000000 bbpb-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11001 2024-05-13 04:43:10.974932 bbpb-1.2.0/README.md
+-rw-r--r--   0        0        0     1577 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/__init__.py
+-rw-r--r--   0        0        0     8896 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/__main__.py
+-rw-r--r--   0        0        0     1382 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/__init__.py
+-rw-r--r--   0        0        0    27799 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/api.py
+-rw-r--r--   0        0        0     2265 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/config.py
+-rw-r--r--   0        0        0     3760 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/exceptions.py
+-rw-r--r--   0        0        0     2798 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/payloads/__init__.py
+-rw-r--r--   0        0        0     3469 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/payloads/grpc.py
+-rw-r--r--   0        0        0     1695 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/payloads/gzip.py
+-rw-r--r--   0        0        0    16052 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/protofile.py
+-rw-r--r--   0        0        0     1296 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/types/__init__.py
+-rw-r--r--   0        0        0     3911 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/types/fixed.py
+-rw-r--r--   0        0        0    26259 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/types/length_delim.py
+-rw-r--r--   0        0        0     5089 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/types/type_maps.py
+-rw-r--r--   0        0        0     5889 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/types/varint.py
+-rw-r--r--   0        0        0     1217 2024-05-13 04:43:10.974932 bbpb-1.2.0/blackboxprotobuf/lib/types/wiretypes.py
+-rw-r--r--   0        0        0      660 2024-05-13 04:43:10.974932 bbpb-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11819 1970-01-01 00:00:00.000000 bbpb-1.2.0/PKG-INFO
```

### Comparing `bbpb-1.1.2/README.md` & `bbpb-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 BlackBox Protobuf is also available on PyPi at <https://pypi.org/project/bbpb>.
 It can be installed with:
 
 ```
 pip install bbpb
 ```
 
+## CLI
+For command line usage see [CLI.md](./CLI.md).
+
 ## Interface
 The main `blackboxprotobuf` module defines an API with the core encode/decode
 message functions, along with several convenience functions to make it easier
 to use blackboxprotobuf with a user interface, such as encoding/decoding
 directly to JSON and validating modified type definitions.
 
 ### Decode 
@@ -173,15 +176,15 @@
 `blackboxprotobuf.lib.config.Config` class. The config object allows modifying
 some of the encoding/decoding functionality and storing some state. This
 replaces some variables that were global before.
 
 At the moment this includes:
 
 * `known_types` - Mapping of message type names to typedef (previously
-  `blackboxprotobuf.known_messages)
+  `blackboxprotobuf.known_messages`)
 
 * `default_binary_type` - Change the default type choice for binary fields when
   decoding previously unknown fields. Defaults to `bytes` but can be set to
   `bytes_hex` to return a hex encoded string instead. `bytes_base64` might be
   another option in the future. The type can always be changed for an
   individual field by changing the `type` in the typedef.
 
@@ -223,15 +226,15 @@
 
 ### Length Delimited
 Length delimited wire types are prefixed with a `varint` indicating the length.
 This is used for strings, bytestrings, inner messages and packed repeated
 fields. Messages can generally be identified by validating if it is a valid
 protobuf binary. If it is not a message, the default type is a string/byte
 which are relatively interchangeable in Python. A different default type (such
-as `bytes_hex` can be specified by changing
+as `bytes_hex`) can be specified by changing
 `blackboxprotobuf.lib.types.default_binary_type`.
 
 Packed repeated fields are arrays of either `varints` or a fixed length wire
 type. Non-packed repeated fields use a separate tag (wire type + field number)
 for each element, allowing them to be easily identified and parsed. However,
 packed repeated fields only have the initial length delimited wire type tag.
 The parser is assumed to know the full type already for parsing out the
```

### Comparing `bbpb-1.1.2/blackboxprotobuf/__init__.py` & `bbpb-1.2.0/blackboxprotobuf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 This module is split into two submodules:
 
     - The `lib` submodule contains the decoding/encoding logic and provides a python interface.
     - The `burp` submodule defines the Burp Suite plugin and UI.
 """
 
-# Copyright (c) 2018-2023 NCC Group Plc
+# Copyright (c) 2018-2024 NCC Group Plc
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `bbpb-1.1.2/blackboxprotobuf/lib/__init__.py` & `bbpb-1.2.0/blackboxprotobuf/lib/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The `blackboxprotobuf.lib` module provides APIs for decoding and encoding
 binary protobuf messages.
 
 This module re-exports the functions defined in `blackboxprotobuf.lib.api`,
 which provides a high level interface for the module and convenience functions.
 """
 
-# Copyright (c) 2018-2023 NCC Group Plc
+# Copyright (c) 2018-2024 NCC Group Plc
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `bbpb-1.1.2/blackboxprotobuf/lib/api.py` & `bbpb-1.2.0/blackboxprotobuf/lib/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 The config argument is the Config object from `blackboxprotobuf.lib.config` and
 allows reconfiguring default types and stores "known" message typedefs that can
 be referenced within other typedefs. This argument can be left out to use a
 default shared config object.
 """
 
-# Copyright (c) 2018-2023 NCC Group Plc
+# Copyright (c) 2018-2024 NCC Group Plc
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -73,15 +73,17 @@
 
     if config is None:
         config = blackboxprotobuf.lib.config.default
 
     if isinstance(buf, bytearray):
         buf = bytes(buf)
     buf = six.ensure_binary(buf)
-    if message_type is None or isinstance(message_type, str):
+    if message_type is None:
+        message_type = {}
+    elif isinstance(message_type, str):
         if message_type not in config.known_types:
             message_type = {}
         else:
             message_type = config.known_types[message_type]
 
     value, typedef, _, _ = blackboxprotobuf.lib.types.length_delim.decode_message(
         buf, config, message_type
@@ -104,14 +106,28 @@
             `blackboxprotobuf.lib.config.default` if not provided.
     Returns:
         A bytearray containing the encoded protobuf message.
     """
 
     if config is None:
         config = blackboxprotobuf.lib.config.default
+
+    if message_type is None:
+        raise EncoderException(
+            "Encode message must have valid type definition. message_type cannot be None"
+        )
+
+    if isinstance(message_type, str):
+        if message_type not in config.known_types:
+            raise EncoderException(
+                "The provided message type name (%s) is not known. Encoding requires a valid type definition"
+                % message_type
+            )
+        message_type = config.known_types[message_type]
+
     return bytes(
         blackboxprotobuf.lib.types.length_delim.encode_message(
             value, config, message_type
         )
     )
```

### Comparing `bbpb-1.1.2/blackboxprotobuf/lib/config.py` & `bbpb-1.2.0/blackboxprotobuf/lib/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 NCC Group Plc
+# Copyright (c) 2018-2024 NCC Group Plc
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `bbpb-1.1.2/blackboxprotobuf/lib/exceptions.py` & `bbpb-1.2.0/blackboxprotobuf/lib/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Exception classes for BlackboxProtobuf"""
 
-# Copyright (c) 2018-2023 NCC Group Plc
+# Copyright (c) 2018-2024 NCC Group Plc
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `bbpb-1.1.2/blackboxprotobuf/lib/protofile.py` & `bbpb-1.2.0/blackboxprotobuf/lib/protofile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Python methods for importing and exporting '.proto' files from the BBP type
 definition format.
 """
 
-# Copyright (c) 2018-2023 NCC Group Plc
+# Copyright (c) 2018-2024 NCC Group Plc
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -441,15 +441,15 @@
         raise ProtofileException(
             "Could not get a type for field %s: %s" % (field_name, field_type)
         )
 
     # figure out packed
     # default based on repeated + proto3, fallback to options
     field_options = match.group(5)
-    is_packed = is_repeated and is_proto3 and (field_type in PACKABLE_TYPES)
+    is_packed = is_repeated and is_proto3 and (bbp_type in PACKABLE_TYPES)
     if is_packed and field_options and "packed=false" in field_options:
         is_packed = False
     elif is_repeated and field_options and "packed=true" in field_options:
         is_packed = True
 
     # make sure the type lines up with packable
     if is_packed and bbp_type not in PACKABLE_TYPES:
```

### Comparing `bbpb-1.1.2/blackboxprotobuf/lib/types/__init__.py` & `bbpb-1.2.0/blackboxprotobuf/lib/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module contains classes/methods for decoding individual field types.
 
 Grouped into submodules based on wire type.
 Re-exports type_maps items for easier access.
 """
 
-# Copyright (c) 2018-2023 NCC Group Plc
+# Copyright (c) 2018-2024 NCC Group Plc
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `bbpb-1.1.2/blackboxprotobuf/lib/types/fixed.py` & `bbpb-1.2.0/blackboxprotobuf/lib/types/fixed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Functions for encoding and decoding fixed size integers and floats"""
 
-# Copyright (c) 2018-2023 NCC Group Plc
+# Copyright (c) 2018-2024 NCC Group Plc
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `bbpb-1.1.2/blackboxprotobuf/lib/types/length_delim.py` & `bbpb-1.2.0/blackboxprotobuf/lib/types/length_delim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for encoding and decoding length delimited fields"""
 
-# Copyright (c) 2018-2023 NCC Group Plc
+# Copyright (c) 2018-2024 NCC Group Plc
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `bbpb-1.1.2/blackboxprotobuf/lib/types/type_maps.py` & `bbpb-1.2.0/blackboxprotobuf/lib/types/type_maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Contains various maps for protobuf types, including encoding/decoding
 functions, wiretypes and default types
 """
 
-# Copyright (c) 2018-2023 NCC Group Plc
+# Copyright (c) 2018-2024 NCC Group Plc
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `bbpb-1.1.2/blackboxprotobuf/lib/types/varint.py` & `bbpb-1.2.0/blackboxprotobuf/lib/types/varint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Classes for encoding and decoding varint types"""
 
-# Copyright (c) 2018-2023 NCC Group Plc
+# Copyright (c) 2018-2024 NCC Group Plc
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `bbpb-1.1.2/blackboxprotobuf/lib/types/wiretypes.py` & `bbpb-1.2.0/blackboxprotobuf/lib/types/wiretypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 NCC Group Plc
+# Copyright (c) 2018-2024 NCC Group Plc
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `bbpb-1.1.2/pyproject.toml` & `bbpb-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbpb"
-version = "1.1.2"
+version = "1.2.0"
 description = "Library for working with protobuf messages without a protobuf type definition."
 authors = ["Ryan Winkelmaier <ryan.winkelmaier@nccgroup.com>"]
 license = "MIT"
 repository = "https://github.com/nccgroup/blackboxprotobuf"
 readme = "README.md"
 keywords = ["protobuf"]
 exclude = ["./tests"]
```

### Comparing `bbpb-1.1.2/PKG-INFO` & `bbpb-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbpb
-Version: 1.1.2
+Version: 1.2.0
 Summary: Library for working with protobuf messages without a protobuf type definition.
 Home-page: https://github.com/nccgroup/blackboxprotobuf
 License: MIT
 Keywords: protobuf
 Author: Ryan Winkelmaier
 Author-email: ryan.winkelmaier@nccgroup.com
 Requires-Python: >=3.8,<4.0
@@ -76,14 +76,17 @@
 BlackBox Protobuf is also available on PyPi at <https://pypi.org/project/bbpb>.
 It can be installed with:
 
 ```
 pip install bbpb
 ```
 
+## CLI
+For command line usage see [CLI.md](./CLI.md).
+
 ## Interface
 The main `blackboxprotobuf` module defines an API with the core encode/decode
 message functions, along with several convenience functions to make it easier
 to use blackboxprotobuf with a user interface, such as encoding/decoding
 directly to JSON and validating modified type definitions.
 
 ### Decode 
@@ -194,15 +197,15 @@
 `blackboxprotobuf.lib.config.Config` class. The config object allows modifying
 some of the encoding/decoding functionality and storing some state. This
 replaces some variables that were global before.
 
 At the moment this includes:
 
 * `known_types` - Mapping of message type names to typedef (previously
-  `blackboxprotobuf.known_messages)
+  `blackboxprotobuf.known_messages`)
 
 * `default_binary_type` - Change the default type choice for binary fields when
   decoding previously unknown fields. Defaults to `bytes` but can be set to
   `bytes_hex` to return a hex encoded string instead. `bytes_base64` might be
   another option in the future. The type can always be changed for an
   individual field by changing the `type` in the typedef.
 
@@ -244,15 +247,15 @@
 
 ### Length Delimited
 Length delimited wire types are prefixed with a `varint` indicating the length.
 This is used for strings, bytestrings, inner messages and packed repeated
 fields. Messages can generally be identified by validating if it is a valid
 protobuf binary. If it is not a message, the default type is a string/byte
 which are relatively interchangeable in Python. A different default type (such
-as `bytes_hex` can be specified by changing
+as `bytes_hex`) can be specified by changing
 `blackboxprotobuf.lib.types.default_binary_type`.
 
 Packed repeated fields are arrays of either `varints` or a fixed length wire
 type. Non-packed repeated fields use a separate tag (wire type + field number)
 for each element, allowing them to be easily identified and parsed. However,
 packed repeated fields only have the initial length delimited wire type tag.
 The parser is assumed to know the full type already for parsing out the
```

