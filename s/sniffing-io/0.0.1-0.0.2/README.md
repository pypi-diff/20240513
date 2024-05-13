# Comparing `tmp/sniffing-io-0.0.1.tar.gz` & `tmp/sniffing-io-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniffing-io-0.0.1.tar", last modified: Mon May 13 14:05:40 2024, max compression
+gzip compressed data, was "sniffing-io-0.0.2.tar", last modified: Mon May 13 14:12:51 2024, max compression
```

## Comparing `sniffing-io-0.0.1.tar` & `sniffing-io-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:05:39.998859 sniffing-io-0.0.1/
--rw-rw-rw-   0        0        0       44 2024-05-13 14:05:39.000000 sniffing-io-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6191 2024-05-13 14:05:39.998859 sniffing-io-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5339 2024-03-07 09:00:19.000000 sniffing-io-0.0.1/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 sniffing-io-0.0.1/build.py
--rw-rw-rw-   0        0        0        5 2024-03-07 08:05:04.000000 sniffing-io-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 14:05:40.000100 sniffing-io-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1546 2024-05-13 14:05:36.000000 sniffing-io-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:05:39.997580 sniffing-io-0.0.1/sniffing_io.egg-info/
--rw-rw-rw-   0        0        0     6191 2024-05-13 14:05:39.000000 sniffing-io-0.0.1/sniffing_io.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-05-13 14:05:39.000000 sniffing-io-0.0.1/sniffing_io.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:05:39.000000 sniffing-io-0.0.1/sniffing_io.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-13 14:05:39.000000 sniffing-io-0.0.1/sniffing_io.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 14:05:39.000000 sniffing-io-0.0.1/sniffing_io.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 14:05:39.995551 sniffing-io-0.0.1/sniffingio/
--rw-rw-rw-   0        0        0      150 2024-03-02 10:06:09.000000 sniffing-io-0.0.1/sniffingio/__init__.py
--rw-rw-rw-   0        0        0     1119 2024-03-04 08:50:47.000000 sniffing-io-0.0.1/sniffingio/callbacks.py
--rw-rw-rw-   0        0        0      859 2024-03-07 07:55:55.000000 sniffing-io-0.0.1/sniffingio/data.py
--rw-rw-rw-   0        0        0    10566 2024-05-13 14:05:36.000000 sniffing-io-0.0.1/sniffingio/filters.py
--rw-rw-rw-   0        0        0     2490 2024-03-07 07:55:55.000000 sniffing-io-0.0.1/sniffingio/sniff.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:12:51.072831 sniffing-io-0.0.2/
+-rw-rw-rw-   0        0        0       44 2024-05-13 14:12:50.000000 sniffing-io-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6191 2024-05-13 14:12:51.071831 sniffing-io-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5339 2024-03-07 09:00:19.000000 sniffing-io-0.0.2/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 sniffing-io-0.0.2/build.py
+-rw-rw-rw-   0        0        0        5 2024-03-07 08:05:04.000000 sniffing-io-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:12:51.072831 sniffing-io-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1546 2024-05-13 14:12:47.000000 sniffing-io-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:12:51.070831 sniffing-io-0.0.2/sniffing_io.egg-info/
+-rw-rw-rw-   0        0        0     6191 2024-05-13 14:12:51.000000 sniffing-io-0.0.2/sniffing_io.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-05-13 14:12:51.000000 sniffing-io-0.0.2/sniffing_io.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:12:51.000000 sniffing-io-0.0.2/sniffing_io.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-13 14:12:51.000000 sniffing-io-0.0.2/sniffing_io.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 14:12:51.000000 sniffing-io-0.0.2/sniffing_io.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 14:12:51.069831 sniffing-io-0.0.2/sniffingio/
+-rw-rw-rw-   0        0        0      150 2024-03-02 10:06:09.000000 sniffing-io-0.0.2/sniffingio/__init__.py
+-rw-rw-rw-   0        0        0     1119 2024-03-04 08:50:47.000000 sniffing-io-0.0.2/sniffingio/callbacks.py
+-rw-rw-rw-   0        0        0      859 2024-03-07 07:55:55.000000 sniffing-io-0.0.2/sniffingio/data.py
+-rw-rw-rw-   0        0        0    10794 2024-05-13 14:11:35.000000 sniffing-io-0.0.2/sniffingio/filters.py
+-rw-rw-rw-   0        0        0     2490 2024-03-07 07:55:55.000000 sniffing-io-0.0.2/sniffingio/sniff.py
```

### Comparing `sniffing-io-0.0.1/PKG-INFO` & `sniffing-io-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffing-io
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple package for packet sniffing, with static/dynamic filtering options, real-time reaction, I/O operations and more.
 Home-page: https://github.com/Shahaf-F-S/sniffing-io
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sniffing-io-0.0.1/README.md` & `sniffing-io-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.1/build.py` & `sniffing-io-0.0.2/build.py`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.1/setup.py` & `sniffing-io-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='sniffing-io',
-        version='0.0.1',
+        version='0.0.2',
         description=(
             "A simple package for packet sniffing, "
             "with static/dynamic filtering options, "
             "real-time reaction, I/O operations and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sniffing-io-0.0.1/sniffing_io.egg-info/PKG-INFO` & `sniffing-io-0.0.2/sniffing_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffing-io
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple package for packet sniffing, with static/dynamic filtering options, real-time reaction, I/O operations and more.
 Home-page: https://github.com/Shahaf-F-S/sniffing-io
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sniffing-io-0.0.1/sniffingio/callbacks.py` & `sniffing-io-0.0.2/sniffingio/callbacks.py`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.1/sniffingio/data.py` & `sniffing-io-0.0.2/sniffingio/data.py`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.1/sniffingio/filters.py` & `sniffing-io-0.0.2/sniffingio/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,24 @@
 
     @staticmethod
     def format_join(values: Iterable[str], joiner: str) -> str:
 
         if not values:
             return ""
 
+        values = tuple(values)
+
+        if len(values) == 1:
+            data = values[0]
+
+            if not (data.startswith("(") and data.endswith(")")):
+                data = f"({data})"
+
+            return data
+
         return f'({f" {joiner} ".join((value for value in values if value))})'
 
 class BasePacketFilterUnion(BasePacketFilterOperator, metaclass=ABCMeta):
 
     @classmethod
     def format_union(cls, values: Iterable[str]) -> str:
```

### Comparing `sniffing-io-0.0.1/sniffingio/sniff.py` & `sniffing-io-0.0.2/sniffingio/sniff.py`

 * *Files identical despite different names*

