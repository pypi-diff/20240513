# Comparing `tmp/sophosfirewall_python-0.1.36.tar.gz` & `tmp/sophosfirewall_python-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sophosfirewall_python-0.1.36.tar", max compression
+gzip compressed data, was "sophosfirewall_python-0.1.37.tar", max compression
```

## Comparing `sophosfirewall_python-0.1.36.tar` & `sophosfirewall_python-0.1.37.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-05-08 19:41:34.017393 sophosfirewall_python-0.1.36/LICENSE
--rw-r--r--   0        0        0     9124 2024-05-08 19:41:34.017393 sophosfirewall_python-0.1.36/README.md
--rw-r--r--   0        0        0      675 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/pyproject.toml
--rw-r--r--   0        0        0    46031 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/firewallapi.py
--rw-r--r--   0        0        0     1681 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createfwrule.j2
--rw-r--r--   0        0        0      356 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createiphost.j2
--rw-r--r--   0        0        0      463 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createiphostgroup.j2
--rw-r--r--   0        0        0      397 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createipnetwork.j2
--rw-r--r--   0        0        0      402 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createiprange.j2
--rw-r--r--   0        0        0      713 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createservice.j2
--rw-r--r--   0        0        0      406 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createurlgroup.j2
--rw-r--r--   0        0        0     2210 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createuser.j2
--rw-r--r--   0        0        0      326 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateadminpassword.j2
--rw-r--r--   0        0        0     1432 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updatebackup.j2
--rw-r--r--   0        0        0      482 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateiphostgroup.j2
--rw-r--r--   0        0        0      716 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateservice.j2
--rw-r--r--   0        0        0      615 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateserviceacl.j2
--rw-r--r--   0        0        0      409 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateurlgroup.j2
--rw-r--r--   0        0        0     2231 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateuserpassword.j2
--rw-r--r--   0        0        0        0 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/tests/__init__.py
--rw-r--r--   0        0        0    16512 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/tests/functional.py
--rw-r--r--   0        0        0      103 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/tests/pytest.ini
--rw-r--r--   0        0        0    30393 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/tests/unittests.py
--rw-r--r--   0        0        0      522 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/urlgroup_example.j2
--rw-r--r--   0        0        0     9733 1970-01-01 00:00:00.000000 sophosfirewall_python-0.1.36/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 21:55:02.926198 sophosfirewall_python-0.1.37/LICENSE
+-rw-r--r--   0        0        0     9124 2024-05-13 21:55:02.926198 sophosfirewall_python-0.1.37/README.md
+-rw-r--r--   0        0        0      675 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/pyproject.toml
+-rw-r--r--   0        0        0    48371 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/firewallapi.py
+-rw-r--r--   0        0        0     1681 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createfwrule.j2
+-rw-r--r--   0        0        0      356 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createiphost.j2
+-rw-r--r--   0        0        0      463 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createiphostgroup.j2
+-rw-r--r--   0        0        0      397 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createipnetwork.j2
+-rw-r--r--   0        0        0      402 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createiprange.j2
+-rw-r--r--   0        0        0     1491 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createservice.j2
+-rw-r--r--   0        0        0      406 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createurlgroup.j2
+-rw-r--r--   0        0        0     2210 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createuser.j2
+-rw-r--r--   0        0        0      326 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateadminpassword.j2
+-rw-r--r--   0        0        0     1432 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updatebackup.j2
+-rw-r--r--   0        0        0      482 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateiphostgroup.j2
+-rw-r--r--   0        0        0     1493 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateservice.j2
+-rw-r--r--   0        0        0      615 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateserviceacl.j2
+-rw-r--r--   0        0        0      409 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateurlgroup.j2
+-rw-r--r--   0        0        0     2231 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateuserpassword.j2
+-rw-r--r--   0        0        0        0 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/tests/__init__.py
+-rw-r--r--   0        0        0    16562 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/tests/functional.py
+-rw-r--r--   0        0        0      103 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/tests/pytest.ini
+-rw-r--r--   0        0        0    30393 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/tests/unittests.py
+-rw-r--r--   0        0        0      522 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/urlgroup_example.j2
+-rw-r--r--   0        0        0     9733 1970-01-01 00:00:00.000000 sophosfirewall_python-0.1.37/PKG-INFO
```

### Comparing `sophosfirewall_python-0.1.36/LICENSE` & `sophosfirewall_python-0.1.37/LICENSE`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.36/README.md` & `sophosfirewall_python-0.1.37/README.md`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.36/pyproject.toml` & `sophosfirewall_python-0.1.37/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "sophosfirewall-python"
 packages = [
     { include = "sophosfirewall_python" },
 ]
-version = "0.1.36"
+version = "0.1.37"
 description = "Python SDK for Sophos Firewall"
 authors = ["Matt Mullen <matt.mullen@sophos.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 requests = "^2.31.0"
@@ -20,14 +20,14 @@
 pylint = "^3.0.1"
 pytest = "^7.4.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^7.2.6"
-sphinx-rtd-theme = "^1.3.0"
+sphinx = "^7.3.7"
+sphinx-rtd-theme = "^2.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sophosfirewall_python-0.1.36/sophosfirewall_python/firewallapi.py` & `sophosfirewall_python-0.1.37/sophosfirewall_python/firewallapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -292,24 +292,24 @@
 
     def update(
         self,
         xml_tag: str,
         update_params: dict,
         name: str = None,
         output_format: str = "dict",
-        debug: bool = False
+        debug: bool = False,
     ):
         """Update an existing object on the firewall.
 
         Args:
             xml_tag (str): The XML tag indicating the type of object to be updated.
             update_params (dict): Keys/values to be updated. Keys must match an existing XML key.
             name (str, optional): The name of the object to be updated, if applicable.
             output_format(str): Output format. Valid options are "dict" or "xml". Defaults to dict.
-            debug (bool): Displays the XML payload that was submitted 
+            debug (bool): Displays the XML payload that was submitted
         """
         if name:
             resp = self.get_tag_with_filter(
                 xml_tag=xml_tag, key="Name", value=name, operator="="
             )
         else:
             resp = self.get_tag(xml_tag=xml_tag)
@@ -824,30 +824,31 @@
             "createiprange.j2", template_vars=params, debug=debug
         )
         return resp
 
     def create_service(
         self,
         name: str,
+        service_type: str,
         service_list: list[dict],
         debug: bool = False,
     ):
         """Create a TCP or UDP service
 
         Args:
-        name (str): Service name
-        service_list(list): List of dictionaries containing the below keys for each port/proto pair
-            src_port (str, optional): Source TCP/UDP port. Default=1:65535.
-            dst_port (str): Destination TCP/UDP port
-            protocol (str): TCP or UDP
-        debug (bool, optional): Enable debug mode. Defaults to False.
+            name (str): Service name.
+            service_type (str): Service type. Valid values are TCPorUDP, IP, ICMP, or ICMPv6.
+            service_list(list): List of dictionaries. 
+                For type TCPorUDP, src_port(str, optional) default=1:65535, dst_port(str), and protocol(str).
+                For type IP, protocol(str). For type ICMP and ICMPv6, icmp_type (str) and icmp_code (str).
+            debug (bool, optional): Enable debug mode. Defaults to False.
         Returns:
             dict: XML response converted to Python dictionary
         """
-        params = {"name": name, "service_list": service_list}
+        params = {"name": name, "service_list": service_list, "type": service_type}
         resp = self.submit_template(
             "createservice.j2", template_vars=params, debug=debug
         )
         return resp
 
     def create_ip_hostgroup(
         self,
@@ -1025,24 +1026,29 @@
         params = {"name": name, "domain_list": new_domain_list}
         resp = self.submit_template(
             "updateurlgroup.j2", template_vars=params, debug=debug
         )
         return resp
 
     def update_service(
-        self, name: str, service_list: list[dict], action: str = "add", debug: bool = False
+        self,
+        name: str,
+        service_type: str,
+        service_list: list[dict],
+        action: str = "add",
+        debug: bool = False,
     ):
         """Add or remove a service entry to/from a service
 
         Args:
             name (str): Service name.
-            service_list (list[dict]): List of dicts containing port/protocol pairs to be added or removed.
-              src_port(str, optional): Source TCP/UDP port range. Default=1:65535.
-              dst_port(str): Destination TCP/UDP port range.
-              protocol(str): TCP or UDP
+            service_type (str): Service type. Valid values are TCPorUDP, IP, ICMP, or ICMPv6.
+            service_list(list): List of dictionaries. 
+                For type TCPorUDP, src_port(str, optional) default=1:65535, dst_port(str), and protocol(str).
+                For type IP, protocol(str). For type ICMP and ICMPv6, icmp_type (str) and icmp_code (str).
             action (str): Options are 'add', 'remove' or 'replace'. Defaults to 'add'.
             debug (bool, optional): Enable debug mode. Defaults to False.
 
         Returns:
             dict: XML response converted to Python dictionary
         """
         if not isinstance(service_list, list):
@@ -1057,45 +1063,98 @@
                 valid_choices=["add", "remove", "replace"],
             )
 
         # Get the existing Service list first
         resp = self.get_service(name=name)
         if "ServiceDetail" in resp["Response"]["Services"]["ServiceDetails"]:
             exist_list = (
-                resp.get("Response").get("Services").get("ServiceDetails").get("ServiceDetail")
+                resp.get("Response")
+                .get("Services")
+                .get("ServiceDetails")
+                .get("ServiceDetail")
             )
         else:
             exist_list = None
 
         # Add src_port to input if not present
         for service in service_list:
             if not "src_port" in service:
                 service["src_port"] = "1:65535"
         if action == "replace":
             exist_list = None
         new_service_list = []
         if exist_list:
             if isinstance(exist_list, dict):
-                new_service_list.append({"src_port": exist_list["SourcePort"],
-                                         "dst_port": exist_list["DestinationPort"],
-                                         "protocol": exist_list["Protocol"]})
+                if service_type == "TCPorUDP":
+                    new_service_list.append(
+                        {
+                            "src_port": exist_list["SourcePort"],
+                            "dst_port": exist_list["DestinationPort"],
+                            "protocol": exist_list["Protocol"],
+                        }
+                    )
+                if service_type == "IP":
+                    new_service_list.append(
+                        {
+                            "protocol": exist_list["ProtocolName"]
+                        }
+                    )
+                if service_type == "ICMP":
+                    new_service_list.append(
+                        {
+                            "icmp_type": exist_list["ICMPType"],
+                            "icmp_code": exist_list["ICMPCode"]
+                        }
+                    )
+                if service_type == "ICMPv6":
+                    new_service_list.append(
+                        {
+                            "icmp_type": exist_list["ICMPv6Type"],
+                            "icmp_code": exist_list["ICMPv6Code"]
+                        }
+                    )
             elif isinstance(exist_list, list):
                 for service in exist_list:
-                    new_service_list.append({"src_port": service["SourcePort"],
-                                             "dst_port": service["DestinationPort"],
-                                             "protocol": service["Protocol"]})
+                    if service_type == "TCPorUDP":
+                        new_service_list.append(
+                            {
+                                "src_port": service["SourcePort"],
+                                "dst_port": service["DestinationPort"],
+                                "protocol": service["Protocol"],
+                            }
+                        )
+                    if service_type == "IP":
+                        new_service_list.append(
+                            {
+                                "protocol": service["ProtocolName"]
+                            }
+                        )
+                    if service_type == "ICMP":
+                        new_service_list.append(
+                            {
+                                "icmp_type": service["ICMPType"],
+                                "icmp_code": service["ICMPCode"]
+                            }
+                        )
+                    if service_type == "ICMPv6":
+                        new_service_list.append(
+                            {
+                                "icmp_type": service["ICMPv6Type"],
+                                "icmp_code": service["ICMPv6Code"]
+                            }
+                        )
         for service in service_list:
             if action.lower() == "add" and service not in new_service_list:
                 new_service_list.append(service)
             elif action.lower() == "remove" and service in new_service_list:
                 new_service_list.remove(service)
             elif action.lower() == "replace":
                 new_service_list.append(service)
 
-        params = {"name": name, "service_list": new_service_list}
+        params = {"name": name, "service_list": new_service_list, "type": service_type}
         resp = self.submit_template(
             "updateservice.j2", template_vars=params, debug=debug
         )
         return resp
 
     def update_ip_hostgroup(
         self,
@@ -1182,21 +1241,23 @@
             Date (str): Numeric representation of month
             EncryptionPassword (str, optional): Encryption password
 
         Returns:
             dict: XML response converted to Python dictionary
         """
         updated_params = {}
-        current_params = self.get_backup()['Response']['BackupRestore']['ScheduleBackup']
+        current_params = self.get_backup()["Response"]["BackupRestore"][
+            "ScheduleBackup"
+        ]
         for param in current_params:
             if param in backup_params:
                 updated_params[param] = backup_params[param]
             else:
                 updated_params[param] = current_params[param]
-            
+
         resp = self.submit_template(
             "updatebackup.j2", template_vars=updated_params, debug=debug
         )
         return resp
 
     def update_service_acl(
         self,
```

### Comparing `sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createfwrule.j2` & `sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createfwrule.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createuser.j2` & `sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createuser.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updatebackup.j2` & `sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updatebackup.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateserviceacl.j2` & `sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateserviceacl.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateuserpassword.j2` & `sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateuserpassword.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.36/sophosfirewall_python/tests/functional.py` & `sophosfirewall_python-0.1.37/sophosfirewall_python/tests/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
             },
         }
     }
     if float(API_VERSION) >= 2000.2:
         expected_result["Response"]["@IS_WIFI6"] = "0"
 
     assert (
-        setup.create_service(name="FUNC_TESTSVC1", service_list=[{"dst_port": 1234, "protocol": "tcp"}])
+        setup.create_service(name="FUNC_TESTSVC1", service_type="TCPorUDP", service_list=[{"dst_port": 1234, "protocol": "tcp"}])
         == expected_result
     )
 
 
 def test_create_rule(setup):
     """Test create_rule method."""
 
@@ -468,15 +468,15 @@
             },
         }
     }
     if float(API_VERSION) >= 2000.2:
         get_result["Response"]["@IS_WIFI6"] = "0"
 
     assert (
-        setup.update_service(name="FUNC_TESTSVC1", service_list=[{"dst_port": "2222","protocol": "TCP"}])
+        setup.update_service(name="FUNC_TESTSVC1", service_type="TCPorUDP", service_list=[{"dst_port": "2222","protocol": "TCP"}])
         == update_result
     )
 
     assert setup.get_service(name="FUNC_TESTSVC1") == get_result
 
 def test_update_service_acl(setup):
     """Test update_service_acl method."""
```

### Comparing `sophosfirewall_python-0.1.36/sophosfirewall_python/tests/unittests.py` & `sophosfirewall_python-0.1.37/sophosfirewall_python/tests/unittests.py`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.36/sophosfirewall_python/urlgroup_example.j2` & `sophosfirewall_python-0.1.37/sophosfirewall_python/urlgroup_example.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.36/PKG-INFO` & `sophosfirewall_python-0.1.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sophosfirewall-python
-Version: 0.1.36
+Version: 0.1.37
 Summary: Python SDK for Sophos Firewall
 Author: Matt Mullen
 Author-email: matt.mullen@sophos.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

