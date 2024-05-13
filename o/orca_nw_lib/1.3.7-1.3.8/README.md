# Comparing `tmp/orca_nw_lib-1.3.7.tar.gz` & `tmp/orca_nw_lib-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orca_nw_lib-1.3.7.tar", max compression
+gzip compressed data, was "orca_nw_lib-1.3.8.tar", max compression
```

## Comparing `orca_nw_lib-1.3.7.tar` & `orca_nw_lib-1.3.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      626 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/LICENSE
--rw-r--r--   0        0        0      373 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/__init__.py
--rw-r--r--   0        0        0    13119 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/bgp.py
--rw-r--r--   0        0        0     8802 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/bgp_db.py
--rw-r--r--   0        0        0    11382 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/bgp_gnmi.py
--rw-r--r--   0        0        0     2466 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/common.py
--rw-r--r--   0        0        0      226 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/constants.py
--rw-r--r--   0        0        0     1938 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/device.py
--rw-r--r--   0        0        0      743 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/device_db.py
--rw-r--r--   0        0        0     4613 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/device_gnmi.py
--rw-r--r--   0        0        0     6464 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/discovery.py
--rw-r--r--   0        0        0     4276 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/generate_code.py
--rw-r--r--   0        0        0     2677 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.py
--rw-r--r--   0        0        0     2711 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/github.com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2_grpc.py
--rw-r--r--   0        0        0    12062 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/gnmi_pb2.py
--rw-r--r--   0        0        0    16347 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/gnmi_pb2.pyi
--rw-r--r--   0        0        0     7757 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/gnmi_pb2_grpc.py
--rw-r--r--   0        0        0    13499 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/gnmi_sub.py
--rw-r--r--   0        0        0     5522 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/gnmi_util.py
--rw-r--r--   0        0        0     7666 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/graph_db_models.py
--rw-r--r--   0        0        0    12476 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/interface.py
--rw-r--r--   0        0        0     8327 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/interface_db.py
--rw-r--r--   0        0        0    18809 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/interface_gnmi.py
--rw-r--r--   0        0        0     7190 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/lldp.py
--rw-r--r--   0        0        0    12716 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/mclag.py
--rw-r--r--   0        0        0    11774 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/mclag_db.py
--rw-r--r--   0        0        0     7836 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/mclag_gnmi.py
--rw-r--r--   0        0        0       75 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/orca_exceptions.py
--rw-r--r--   0        0        0      777 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/orca_nw_lib.yml
--rw-r--r--   0        0        0      577 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/orca_nw_lib_logging.yml
--rw-r--r--   0        0        0     8967 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/port_chnl.py
--rw-r--r--   0        0        0     5712 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/port_chnl_db.py
--rw-r--r--   0        0        0     9590 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/port_chnl_gnmi.py
--rw-r--r--   0        0        0     5578 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/portgroup.py
--rw-r--r--   0        0        0     4539 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/portgroup_db.py
--rw-r--r--   0        0        0     3959 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/portgroup_gnmi.py
--rw-r--r--   0        0        0     4030 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/utils.py
--rw-r--r--   0        0        0     9628 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/vlan.py
--rw-r--r--   0        0        0     4455 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/vlan_db.py
--rw-r--r--   0        0        0    13314 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/vlan_gnmi.py
--rw-r--r--   0        0        0      508 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     7034 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/readme.md
--rw-r--r--   0        0        0     7908 1970-01-01 00:00:00.000000 orca_nw_lib-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0      626 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/LICENSE
+-rw-r--r--   0        0        0      373 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/__init__.py
+-rw-r--r--   0        0        0    13119 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/bgp.py
+-rw-r--r--   0        0        0     8802 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/bgp_db.py
+-rw-r--r--   0        0        0    11382 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/bgp_gnmi.py
+-rw-r--r--   0        0        0     2466 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/common.py
+-rw-r--r--   0        0        0      226 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/constants.py
+-rw-r--r--   0        0        0     1938 2024-05-13 10:38:00.674425 orca_nw_lib-1.3.8/orca_nw_lib/device.py
+-rw-r--r--   0        0        0      743 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/device_db.py
+-rw-r--r--   0        0        0     4613 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/device_gnmi.py
+-rw-r--r--   0        0        0     6464 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/discovery.py
+-rw-r--r--   0        0        0     4276 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/generate_code.py
+-rw-r--r--   0        0        0     2677 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.py
+-rw-r--r--   0        0        0     2711 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/github.com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2_grpc.py
+-rw-r--r--   0        0        0    12062 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/gnmi_pb2.py
+-rw-r--r--   0        0        0    16347 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/gnmi_pb2.pyi
+-rw-r--r--   0        0        0     7757 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/gnmi_pb2_grpc.py
+-rw-r--r--   0        0        0    13499 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/gnmi_sub.py
+-rw-r--r--   0        0        0     5522 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/gnmi_util.py
+-rw-r--r--   0        0        0     7697 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/graph_db_models.py
+-rw-r--r--   0        0        0    12476 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/interface.py
+-rw-r--r--   0        0        0     8327 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/interface_db.py
+-rw-r--r--   0        0        0    18809 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/interface_gnmi.py
+-rw-r--r--   0        0        0     7190 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/lldp.py
+-rw-r--r--   0        0        0    12716 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/mclag.py
+-rw-r--r--   0        0        0    11774 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/mclag_db.py
+-rw-r--r--   0        0        0     7836 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/mclag_gnmi.py
+-rw-r--r--   0        0        0       75 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/orca_exceptions.py
+-rw-r--r--   0        0        0      777 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/orca_nw_lib.yml
+-rw-r--r--   0        0        0      577 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/orca_nw_lib_logging.yml
+-rw-r--r--   0        0        0     8967 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/port_chnl.py
+-rw-r--r--   0        0        0     5712 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/port_chnl_db.py
+-rw-r--r--   0        0        0     9590 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/port_chnl_gnmi.py
+-rw-r--r--   0        0        0     5578 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/portgroup.py
+-rw-r--r--   0        0        0     4539 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/portgroup_db.py
+-rw-r--r--   0        0        0     3959 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/portgroup_gnmi.py
+-rw-r--r--   0        0        0     4708 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/utils.py
+-rw-r--r--   0        0        0     9703 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/vlan.py
+-rw-r--r--   0        0        0     4507 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/vlan_db.py
+-rw-r--r--   0        0        0    14539 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/orca_nw_lib/vlan_gnmi.py
+-rw-r--r--   0        0        0      508 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     7034 2024-05-13 10:38:00.678426 orca_nw_lib-1.3.8/readme.md
+-rw-r--r--   0        0        0     7908 1970-01-01 00:00:00.000000 orca_nw_lib-1.3.8/PKG-INFO
```

### Comparing `orca_nw_lib-1.3.7/LICENSE` & `orca_nw_lib-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/bgp.py` & `orca_nw_lib-1.3.8/orca_nw_lib/bgp.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/bgp_db.py` & `orca_nw_lib-1.3.8/orca_nw_lib/bgp_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/bgp_gnmi.py` & `orca_nw_lib-1.3.8/orca_nw_lib/bgp_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/common.py` & `orca_nw_lib-1.3.8/orca_nw_lib/common.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/device.py` & `orca_nw_lib-1.3.8/orca_nw_lib/device.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/device_db.py` & `orca_nw_lib-1.3.8/orca_nw_lib/device_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/device_gnmi.py` & `orca_nw_lib-1.3.8/orca_nw_lib/device_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/discovery.py` & `orca_nw_lib-1.3.8/orca_nw_lib/discovery.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/generate_code.py` & `orca_nw_lib-1.3.8/orca_nw_lib/generate_code.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.py` & `orca_nw_lib-1.3.8/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.pyi` & `orca_nw_lib-1.3.8/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.pyi`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/gnmi_pb2.py` & `orca_nw_lib-1.3.8/orca_nw_lib/gnmi_pb2.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/gnmi_pb2.pyi` & `orca_nw_lib-1.3.8/orca_nw_lib/gnmi_pb2.pyi`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/gnmi_pb2_grpc.py` & `orca_nw_lib-1.3.8/orca_nw_lib/gnmi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/gnmi_sub.py` & `orca_nw_lib-1.3.8/orca_nw_lib/gnmi_sub.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/gnmi_util.py` & `orca_nw_lib-1.3.8/orca_nw_lib/gnmi_util.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/graph_db_models.py` & `orca_nw_lib-1.3.8/orca_nw_lib/graph_db_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,19 +271,20 @@
     """
     Represents a VLAN in the database.
     """
 
     vlanid = IntegerProperty()
     name = StringProperty()
     mtu = IntegerProperty()
-    admin_status = StringProperty()
     oper_status = StringProperty()
     autostate = StringProperty()
     ip_address = StringProperty()
     sag_ip_address = StringProperty()
+    enabled = BooleanProperty()
+    description = StringProperty()
 
     memberInterfaces = RelationshipTo("Interface", "MEMBER_IF", model=VlanMemRel)
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return self.vlanid == other.vlanid
         return NotImplemented
```

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/interface.py` & `orca_nw_lib-1.3.8/orca_nw_lib/interface.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/interface_db.py` & `orca_nw_lib-1.3.8/orca_nw_lib/interface_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/interface_gnmi.py` & `orca_nw_lib-1.3.8/orca_nw_lib/interface_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/lldp.py` & `orca_nw_lib-1.3.8/orca_nw_lib/lldp.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/mclag.py` & `orca_nw_lib-1.3.8/orca_nw_lib/mclag.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/mclag_db.py` & `orca_nw_lib-1.3.8/orca_nw_lib/mclag_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/mclag_gnmi.py` & `orca_nw_lib-1.3.8/orca_nw_lib/mclag_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/orca_nw_lib.yml` & `orca_nw_lib-1.3.8/orca_nw_lib/orca_nw_lib.yml`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/orca_nw_lib_logging.yml` & `orca_nw_lib-1.3.8/orca_nw_lib/orca_nw_lib_logging.yml`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/port_chnl.py` & `orca_nw_lib-1.3.8/orca_nw_lib/port_chnl.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/port_chnl_db.py` & `orca_nw_lib-1.3.8/orca_nw_lib/port_chnl_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/port_chnl_gnmi.py` & `orca_nw_lib-1.3.8/orca_nw_lib/port_chnl_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/portgroup.py` & `orca_nw_lib-1.3.8/orca_nw_lib/portgroup.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/portgroup_db.py` & `orca_nw_lib-1.3.8/orca_nw_lib/portgroup_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/portgroup_gnmi.py` & `orca_nw_lib-1.3.8/orca_nw_lib/portgroup_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/utils.py` & `orca_nw_lib-1.3.8/orca_nw_lib/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Utils for ORCA Network Library """
 
 import os
+import re
 import ipaddress
 import logging.config
 import logging
 from neomodel import config, db, clear_neo4j_database
 import yaml
 from . import constants as const
 
@@ -131,14 +132,32 @@
             time.sleep(1)  # Wait before retrying
         finally:
             sock.close()
             return status
 
 
 
-def validate_and_get_ip_prefix(ip_address):
+def validate_and_get_ip_prefix(network_address:str):
+    """
+    Validates and extracts the IP prefix from a given network address.
+
+    Args:
+        network_address (str): The network address to validate and extract the IP prefix from.
+
+    Returns:
+        Tuple[str, str, int] or Tuple[None, None, None]: A tuple containing the network address, the IP address, and the prefix length.
+        If the network address is invalid, returns (None, None, None).
+    """
     try:
-        ip_network = ipaddress.ip_network(ip_address,strict=False)
-        return str(ip_network.network_address), ip_network.prefixlen
+        ip_network = ipaddress.ip_network(network_address, strict=False)
+        return (
+            (
+                network_address.split(match.group(), 1)[0]
+                if (match := re.search("/", network_address))
+                else network_address
+            ),
+            str(ip_network.network_address),
+            ip_network.prefixlen
+        )
     except ValueError:
-        _logger.error(f"Invalid IP address: {ip_address}")
-        return None, None
+        _logger.error(f"Invalid network address: {network_address}")
+        return None, None, None
```

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/vlan.py` & `orca_nw_lib-1.3.8/orca_nw_lib/vlan.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,18 @@
             )
         )
 
     for vlan in vlan_details.get("sonic-vlan:VLAN_TABLE_LIST") or []:
         for v in vlans:
             if v.name == vlan.get("name"):
                 v.mtu = vlan.get("mtu")
-                v.admin_status = vlan.get("admin_status")
+                v.enabled = True if vlan.get("admin_status")== "up" else False
                 v.oper_status = vlan.get("oper_status")
                 v.autostate = vlan.get("autostate")
+                v.description=vlan.get("description")
 
     vlans_obj_vs_mem = {}
     for v in vlans:
         members = []
         for item in vlan_details.get("sonic-vlan:VLAN_MEMBER_LIST") or []:
             if v.name == item.get("name"):
                 members.append(item)
```

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/vlan_db.py` & `orca_nw_lib-1.3.8/orca_nw_lib/vlan_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,19 +71,20 @@
 
     Returns:
         None
     """
     target_vlan_obj.vlanid = source_vlan_obj.vlanid
     target_vlan_obj.name = source_vlan_obj.name
     target_vlan_obj.mtu = source_vlan_obj.mtu
-    target_vlan_obj.admin_status = source_vlan_obj.admin_status
+    target_vlan_obj.enabled = source_vlan_obj.enabled
     target_vlan_obj.oper_status = source_vlan_obj.oper_status
     target_vlan_obj.autostate = source_vlan_obj.autostate
     target_vlan_obj.ip_address = source_vlan_obj.ip_address
     target_vlan_obj.sag_ip_address = source_vlan_obj.sag_ip_address
+    target_vlan_obj.description = source_vlan_obj.description
 
 
 def insert_vlan_in_db(device: Device, vlans_obj_vs_mem):
     """
     Inserts VLAN information into the database.
 
     Args:
```

### Comparing `orca_nw_lib-1.3.7/orca_nw_lib/vlan_gnmi.py` & `orca_nw_lib-1.3.8/orca_nw_lib/vlan_gnmi.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,18 +150,16 @@
 
 
 def del_vlan_from_device(device_ip: str, vlan_name: str):
 
     return send_gnmi_set(
         get_gnmi_del_req(
             get_gnmi_path(
-                f"/openconfig-interfaces:interfaces/interface={{'name': {vlan_name}}}"
+                f"/openconfig-interfaces:interfaces/interface[name={vlan_name}]"
             )
-            if not vlan_name
-            else get_vlan_list_path(vlan_name)
         ),
         device_ip,
     )
 
 
 def config_vlan_on_device(
     device_ip: str,
@@ -201,15 +199,15 @@
                 "openconfig-interfaces:interfaces": {
                     "interface": [{"name": vlan_name, "config": {"name": vlan_name}}]
                 }
             },
         )
     )
 
-    if enabled:
+    if enabled is not None:
         update_req.append(
             create_gnmi_update(
                 get_gnmi_path(
                     f"openconfig-interfaces:interfaces/interface[name={vlan_name}]/config/enabled",
                 ),
                 {"openconfig-interfaces:enabled": enabled},
             )
@@ -230,15 +228,15 @@
                     f"openconfig-interfaces:interfaces/interface[name={vlan_name}]/config/mtu",
                 ),
                 {"openconfig-interfaces:mtu": mtu},
             )
         )
 
     if ip_addr_with_prefix:
-        ip, prefix_len = validate_and_get_ip_prefix(ip_addr_with_prefix)
+        ip, nw_addr, prefix_len = validate_and_get_ip_prefix(ip_addr_with_prefix)
         if ip and prefix_len:
             update_req.append(
                 create_gnmi_update(
                     get_gnmi_path(
                         f"/openconfig-interfaces:interfaces/interface[name={vlan_name}]/openconfig-vlan:routed-vlan/openconfig-if-ip:ipv4/addresses",
                     ),
                     {
@@ -267,29 +265,65 @@
             )
         )
     if mem_ifs:
         ## add an array to update_req returned by get_add_vlan_mem_req()
         update_req.extend(get_add_vlan_mem_req(vlan_id, mem_ifs))
 
     if anycast_addr:
+        ip, nw_addr, prefix_len = validate_and_get_ip_prefix(anycast_addr)
         update_req.append(
             create_gnmi_update(
                 get_gnmi_path(
                     f"openconfig-interfaces:interfaces/interface[name={vlan_name}]/openconfig-vlan:routed-vlan/openconfig-if-ip:ipv4/openconfig-interfaces-ext:sag-ipv4/config/static-anycast-gateway"
                 ),
-                {"openconfig-interfaces-ext:static-anycast-gateway": [anycast_addr]},
+                {
+                    "openconfig-interfaces-ext:static-anycast-gateway": [
+                        f"{ip}/{prefix_len}"
+                    ]
+                },
             )
         )
 
     return send_gnmi_set(
         create_req_for_update(update_req),
         device_ip,
     )
 
 
+def set_ip_addr_on_vlan_on_device(
+    device_ip: str, vlan_name: str, ip_addr_with_prefix: str
+):
+    ip, nw_addr, prefix_len = validate_and_get_ip_prefix(ip_addr_with_prefix)
+    return send_gnmi_set(
+        create_req_for_update(
+            [
+                create_gnmi_update(
+                    get_gnmi_path(
+                        f"/openconfig-interfaces:interfaces/interface[name={vlan_name}]/openconfig-vlan:routed-vlan/openconfig-if-ip:ipv4/addresses",
+                    ),
+                    {
+                        "openconfig-if-ip:addresses": {
+                            "address": [
+                                {
+                                    "ip": ip,
+                                    "openconfig-if-ip:config": {
+                                        "ip": ip,
+                                        "prefix-length": prefix_len,
+                                    },
+                                }
+                            ]
+                        }
+                    },
+                )
+            ]
+        ),
+        device_ip,
+    )
+
+
 def get_add_vlan_mem_req(vlan_id: int, mem_ifs: dict[str:IFMode]):
     """
     Generates a list of GNMI updates for adding VLAN member interfaces.
 
     Args:
         vlan_id (int): The ID of the VLAN.
         mem_ifs (dict[str:IFMode]): A dictionary mapping interface names to their mode.
@@ -319,15 +353,17 @@
     """
     return send_gnmi_set(
         create_req_for_update(get_add_vlan_mem_req(vlan_id, mem_ifs)),
         device_ip,
     )
 
 
-def del_vlan_mem_interface_on_device(device_ip: str, vlan_id: int, if_name: str, if_mode: IFMode):
+def del_vlan_mem_interface_on_device(
+    device_ip: str, vlan_id: int, if_name: str, if_mode: IFMode
+):
     """
     Deletes a VLAN member interface on a device using the specified device IP, VLAN ID, and interface name.
 
     Args:
         device_ip (str): The IP address of the device.
         vlan_id (int): The ID of the VLAN.
         if_name (str): The name of the interface to be removed from the VLAN.
@@ -335,15 +371,16 @@
 
     Returns:
         Result of sending a GNMI set request to delete the VLAN member interface.
     """
     return send_gnmi_set(
         get_gnmi_del_req(
             get_gnmi_path(
-                f"openconfig-interfaces:interfaces/interface[name={if_name}]/openconfig-if-ethernet:ethernet/openconfig-vlan:switched-vlan/config/trunk-vlans[trunk-vlans={vlan_id}]" if if_mode == IFMode.TRUNK
+                f"openconfig-interfaces:interfaces/interface[name={if_name}]/openconfig-if-ethernet:ethernet/openconfig-vlan:switched-vlan/config/trunk-vlans[trunk-vlans={vlan_id}]"
+                if if_mode == IFMode.TRUNK
                 else f"openconfig-interfaces:interfaces/interface[name={if_name}]/openconfig-if-ethernet:ethernet/openconfig-vlan:switched-vlan/config/access-vlan"
             )
         ),
         device_ip,
     )
```

### Comparing `orca_nw_lib-1.3.7/readme.md` & `orca_nw_lib-1.3.8/readme.md`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.7/PKG-INFO` & `orca_nw_lib-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orca_nw_lib
-Version: 1.3.7
+Version: 1.3.8
 Summary: APIs to interact with SONiC NW
 Author: Kamal Krishna Bhatt
 Author-email: kamal.bhatt@stordis.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

