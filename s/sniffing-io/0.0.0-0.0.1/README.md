# Comparing `tmp/sniffing-io-0.0.0.tar.gz` & `tmp/sniffing-io-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniffing-io-0.0.0.tar", last modified: Thu Mar  7 08:14:10 2024, max compression
+gzip compressed data, was "sniffing-io-0.0.1.tar", last modified: Mon May 13 14:05:40 2024, max compression
```

## Comparing `sniffing-io-0.0.0.tar` & `sniffing-io-0.0.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 08:14:10.703056 sniffing-io-0.0.0/
--rw-rw-rw-   0        0        0       74 2024-03-07 08:14:10.000000 sniffing-io-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      982 2024-03-07 08:14:10.701054 sniffing-io-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       13 2024-03-07 08:03:14.000000 sniffing-io-0.0.0/README.md
--rw-rw-rw-   0        0        0    12832 2023-11-23 19:36:32.000000 sniffing-io-0.0.0/build.py
--rw-rw-rw-   0        0        0       29 2024-03-07 08:13:57.000000 sniffing-io-0.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0        5 2024-03-07 08:05:04.000000 sniffing-io-0.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-07 08:14:10.703056 sniffing-io-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1546 2024-03-07 08:14:08.000000 sniffing-io-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-07 08:14:10.699057 sniffing-io-0.0.0/sniffing_io.egg-info/
--rw-rw-rw-   0        0        0      982 2024-03-07 08:14:10.000000 sniffing-io-0.0.0/sniffing_io.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2024-03-07 08:14:10.000000 sniffing-io-0.0.0/sniffing_io.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 08:14:10.000000 sniffing-io-0.0.0/sniffing_io.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-03-07 08:14:10.000000 sniffing-io-0.0.0/sniffing_io.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-07 08:14:10.000000 sniffing-io-0.0.0/sniffing_io.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-07 08:14:10.696554 sniffing-io-0.0.0/sniffingio/
--rw-rw-rw-   0        0        0      150 2024-03-02 10:06:09.000000 sniffing-io-0.0.0/sniffingio/__init__.py
--rw-rw-rw-   0        0        0     1119 2024-03-04 08:50:47.000000 sniffing-io-0.0.0/sniffingio/callbacks.py
--rw-rw-rw-   0        0        0      859 2024-03-07 07:55:55.000000 sniffing-io-0.0.0/sniffingio/data.py
--rw-rw-rw-   0        0        0    10240 2024-03-07 07:39:31.000000 sniffing-io-0.0.0/sniffingio/filters.py
--rw-rw-rw-   0        0        0     2490 2024-03-07 07:55:55.000000 sniffing-io-0.0.0/sniffingio/sniff.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:05:39.998859 sniffing-io-0.0.1/
+-rw-rw-rw-   0        0        0       44 2024-05-13 14:05:39.000000 sniffing-io-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6191 2024-05-13 14:05:39.998859 sniffing-io-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5339 2024-03-07 09:00:19.000000 sniffing-io-0.0.1/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 sniffing-io-0.0.1/build.py
+-rw-rw-rw-   0        0        0        5 2024-03-07 08:05:04.000000 sniffing-io-0.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:05:40.000100 sniffing-io-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1546 2024-05-13 14:05:36.000000 sniffing-io-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:05:39.997580 sniffing-io-0.0.1/sniffing_io.egg-info/
+-rw-rw-rw-   0        0        0     6191 2024-05-13 14:05:39.000000 sniffing-io-0.0.1/sniffing_io.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-05-13 14:05:39.000000 sniffing-io-0.0.1/sniffing_io.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:05:39.000000 sniffing-io-0.0.1/sniffing_io.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-13 14:05:39.000000 sniffing-io-0.0.1/sniffing_io.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 14:05:39.000000 sniffing-io-0.0.1/sniffing_io.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 14:05:39.995551 sniffing-io-0.0.1/sniffingio/
+-rw-rw-rw-   0        0        0      150 2024-03-02 10:06:09.000000 sniffing-io-0.0.1/sniffingio/__init__.py
+-rw-rw-rw-   0        0        0     1119 2024-03-04 08:50:47.000000 sniffing-io-0.0.1/sniffingio/callbacks.py
+-rw-rw-rw-   0        0        0      859 2024-03-07 07:55:55.000000 sniffing-io-0.0.1/sniffingio/data.py
+-rw-rw-rw-   0        0        0    10566 2024-05-13 14:05:36.000000 sniffing-io-0.0.1/sniffingio/filters.py
+-rw-rw-rw-   0        0        0     2490 2024-03-07 07:55:55.000000 sniffing-io-0.0.1/sniffingio/sniff.py
```

### Comparing `sniffing-io-0.0.0/setup.py` & `sniffing-io-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='sniffing-io',
-        version='0.0.0',
+        version='0.0.1',
         description=(
             "A simple package for packet sniffing, "
             "with static/dynamic filtering options, "
             "real-time reaction, I/O operations and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sniffing-io-0.0.0/sniffingio/callbacks.py` & `sniffing-io-0.0.1/sniffingio/callbacks.py`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.0/sniffingio/data.py` & `sniffing-io-0.0.1/sniffingio/data.py`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.0.0/sniffingio/filters.py` & `sniffing-io-0.0.1/sniffingio/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,18 +110,14 @@
         return NotImplemented
 
     @classmethod
     def load(cls, data: dict[str, ...]) -> "PacketFilterOperand":
 
         data = data.copy()
 
-        for key, value in data.items():
-            if isinstance(value, dict) and '__type__' in value:
-                data[key] = cls.TYPES[data['__type__']][0].load(value)
-
         return cls.TYPES[data.pop('__type__')][0].load(data)
 
     def dump(self) -> dict[str, ...]:
 
         data = {'__type__': type(self).__name__}
 
         for key in self.ATTRIBUTES:
@@ -215,34 +211,38 @@
             return ""
 
         return f"(not {data})"
 
     @classmethod
     def load(cls, data: dict[str, ...]) -> "PacketFilterNegation":
 
-        return cls(PacketFilterOperand.load(data['filter']))
+        return cls(cls.TYPES[data['filter']['__type__']][0].load(data['filter']))
 
     def dump(self) -> dict[str, ...]:
 
         return {
             '__type__': type(self).__name__,
             'filter': self.filter.dump()
         }
 
 @dataclass(slots=True, frozen=True, eq=False)
 class PacketFilter(PacketFilterOperand):
 
     protocols: list[str] = None
+    hosts: list[str] = None
+    ports: list[int] = None
     source_hosts: list[str] = None
     source_ports: list[int] = None
     destination_hosts: list[str] = None
     destination_ports: list[int] = None
 
     ATTRIBUTES: ClassVar[set[str]] = {
         'protocols',
+        'hosts'
+        'ports'
         'source_hosts',
         'source_ports',
         'destination_hosts',
         'destination_ports'
     }
 
     @classmethod
@@ -283,21 +283,35 @@
     def format_source_hosts(self) -> str:
 
         if not self.source_hosts:
             return ""
 
         return self.format_values(self.source_hosts, key="src host")
 
+    def format_hosts(self) -> str:
+
+        if not self.hosts:
+            return ""
+
+        return self.format_values(self.hosts, key="host")
+
     def format_destination_hosts(self) -> str:
 
         if not self.destination_hosts:
             return ""
 
         return self.format_values(self.destination_hosts, key="dst host")
 
+    def format_ports(self) -> str:
+
+        if not self.ports:
+            return ""
+
+        return self.format_values((str(port) for port in self.ports), key="port")
+
     def format_source_ports(self) -> str:
 
         if not self.source_ports:
             return ""
 
         return self.format_values(
             (str(port) for port in self.source_ports), key="src port"
@@ -314,14 +328,16 @@
 
     def format_data(self) -> str:
 
         data = self.format_intersection(
             (
                 data for data in (
                     self.format_protocols(),
+                    self.format_hosts(),
+                    self.format_ports(),
                     self.format_source_hosts(),
                     self.format_source_ports(),
                     self.format_destination_hosts(),
                     self.format_destination_ports()
                 )
                 if data
             )
@@ -383,15 +399,15 @@
     PacketFilterIntersection |
     PacketFilterNegation |
     StaticPacketFilter
 )
 
 def dump_packet_filter(data: PF) -> dict[str, ...]:
 
-    return PacketFilterOperand.dump(data)
+    return data.dump()
 
 def load_packet_filter(data: PF | str | dict[str, ...]) -> PF:
 
     if isinstance(data, PacketFilterOperand):
         return data
 
     if isinstance(data, str):
```

### Comparing `sniffing-io-0.0.0/sniffingio/sniff.py` & `sniffing-io-0.0.1/sniffingio/sniff.py`

 * *Files identical despite different names*

