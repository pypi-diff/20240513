# Comparing `tmp/alibabacloud_adcp20220101-3.0.0.tar.gz` & `tmp/alibabacloud_adcp20220101-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_adcp20220101-3.0.0.tar", last modified: Mon Apr 22 02:57:54 2024, max compression
+gzip compressed data, was "dist/alibabacloud_adcp20220101-3.1.0.tar", last modified: Mon May 13 17:14:53 2024, max compression
```

## Comparing `alibabacloud_adcp20220101-3.0.0.tar` & `alibabacloud_adcp20220101-3.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/
--rw-r--r--   0 root         (0) root         (0)     1141 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2408 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1099 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1184 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81543 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101/client.py
--rw-r--r--   0 root         (0) root         (0)   208339 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2408 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2616 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1643 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/alibabacloud_adcp20220101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/alibabacloud_adcp20220101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   111113 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/alibabacloud_adcp20220101/client.py
+-rw-r--r--   0 root         (0) root         (0)   225818 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/alibabacloud_adcp20220101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/alibabacloud_adcp20220101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/alibabacloud_adcp20220101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/alibabacloud_adcp20220101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/alibabacloud_adcp20220101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/alibabacloud_adcp20220101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/alibabacloud_adcp20220101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2616 2024-05-13 17:14:53.000000 alibabacloud_adcp20220101-3.1.0/setup.py
```

### Comparing `alibabacloud_adcp20220101-3.0.0/LICENSE` & `alibabacloud_adcp20220101-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_adcp20220101-3.0.0/PKG-INFO` & `alibabacloud_adcp20220101-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_adcp20220101
-Version: 3.0.0
+Version: 3.1.0
 Summary: Alibaba Cloud adcp (20220101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adcp20220101-3.0.0/README-CN.md` & `alibabacloud_adcp20220101-3.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adcp20220101-3.0.0/README.md` & `alibabacloud_adcp20220101-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101/models.py` & `alibabacloud_adcp20220101-3.1.0/alibabacloud_adcp20220101/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,62 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import List, Dict
 
 
+class Tag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class AttachClusterToHubRequest(TeaModel):
     def __init__(
         self,
         attach_to_mesh: bool = None,
         cluster_id: str = None,
         cluster_ids: str = None,
     ):
         # The operation that you want to perform. Set the value to **AttachClusterToHub**.
         self.attach_to_mesh = attach_to_mesh
         # The ID of the task.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # The ID of the request.
+        # 
+        # This parameter is required.
         self.cluster_ids = cluster_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -131,26 +168,142 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AttachClusterToHubResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ChangeResourceGroupRequest(TeaModel):
+    def __init__(
+        self,
+        new_resource_group_id: str = None,
+        resource_id: str = None,
+        resource_type: str = None,
+    ):
+        # The ID of the new resource group.
+        # 
+        # This parameter is required.
+        self.new_resource_group_id = new_resource_group_id
+        # The resource ID. If ResourceType=cluster, the resource ID is ClusterId.
+        # 
+        # This parameter is required.
+        self.resource_id = resource_id
+        # The type of the resource. Only cluster are supported. Set the value to cluster.
+        self.resource_type = resource_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.new_resource_group_id is not None:
+            result['NewResourceGroupId'] = self.new_resource_group_id
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('NewResourceGroupId') is not None:
+            self.new_resource_group_id = m.get('NewResourceGroupId')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        return self
+
+
+class ChangeResourceGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        # Id of the request
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ChangeResourceGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ChangeResourceGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ChangeResourceGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateHubClusterRequest(TeaModel):
     def __init__(
         self,
         api_server_public_eip: bool = None,
         argo_server_enabled: bool = None,
         audit_log_enabled: bool = None,
         is_enterprise_security_group: bool = None,
         name: str = None,
         price_limit: str = None,
         profile: str = None,
         region_id: str = None,
         resource_group_id: str = None,
+        tag: List[Tag] = None,
         v_switches: str = None,
         vpc_id: str = None,
         workflow_schedule_mode: str = None,
     ):
         # Specifies whether to expose the API server to the Internet. Valid values:
         # 
         # *   true: exposes the API server to the Internet.
@@ -176,20 +329,169 @@
         # 
         # *   `Default`: The master instance is suitable for standard scenarios.
         # *   `XFlow`: The master instance is suitable for workflow scenarios.
         # 
         # Default value: `Default`.
         self.profile = profile
         # The ID of the region. You can call the DescribeRegions operation to query available regions.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The Resource Group ID.
         self.resource_group_id = resource_group_id
+        self.tag = tag
         # The ID of the vSwitch.
+        # 
+        # This parameter is required.
         self.v_switches = v_switches
         # The ID of the virtual private cloud (VPC) to which the master instance belongs. You can call the DescribeVpcs operation to query available VPCs.
+        # 
+        # This parameter is required.
+        self.vpc_id = vpc_id
+        # The scheduling mode of the workflow. This parameter takes effect only if Profile is set to XFlow. Valid values:
+        # 
+        # *   cost-optimized: cost-prioritized scheduling mode.
+        # *   stock-optimized: inventory-prioritized scheduling mode.
+        self.workflow_schedule_mode = workflow_schedule_mode
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_server_public_eip is not None:
+            result['ApiServerPublicEip'] = self.api_server_public_eip
+        if self.argo_server_enabled is not None:
+            result['ArgoServerEnabled'] = self.argo_server_enabled
+        if self.audit_log_enabled is not None:
+            result['AuditLogEnabled'] = self.audit_log_enabled
+        if self.is_enterprise_security_group is not None:
+            result['IsEnterpriseSecurityGroup'] = self.is_enterprise_security_group
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.price_limit is not None:
+            result['PriceLimit'] = self.price_limit
+        if self.profile is not None:
+            result['Profile'] = self.profile
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupID'] = self.resource_group_id
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        if self.v_switches is not None:
+            result['VSwitches'] = self.v_switches
+        if self.vpc_id is not None:
+            result['VpcId'] = self.vpc_id
+        if self.workflow_schedule_mode is not None:
+            result['WorkflowScheduleMode'] = self.workflow_schedule_mode
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiServerPublicEip') is not None:
+            self.api_server_public_eip = m.get('ApiServerPublicEip')
+        if m.get('ArgoServerEnabled') is not None:
+            self.argo_server_enabled = m.get('ArgoServerEnabled')
+        if m.get('AuditLogEnabled') is not None:
+            self.audit_log_enabled = m.get('AuditLogEnabled')
+        if m.get('IsEnterpriseSecurityGroup') is not None:
+            self.is_enterprise_security_group = m.get('IsEnterpriseSecurityGroup')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('PriceLimit') is not None:
+            self.price_limit = m.get('PriceLimit')
+        if m.get('Profile') is not None:
+            self.profile = m.get('Profile')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupID') is not None:
+            self.resource_group_id = m.get('ResourceGroupID')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = Tag()
+                self.tag.append(temp_model.from_map(k))
+        if m.get('VSwitches') is not None:
+            self.v_switches = m.get('VSwitches')
+        if m.get('VpcId') is not None:
+            self.vpc_id = m.get('VpcId')
+        if m.get('WorkflowScheduleMode') is not None:
+            self.workflow_schedule_mode = m.get('WorkflowScheduleMode')
+        return self
+
+
+class CreateHubClusterShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        api_server_public_eip: bool = None,
+        argo_server_enabled: bool = None,
+        audit_log_enabled: bool = None,
+        is_enterprise_security_group: bool = None,
+        name: str = None,
+        price_limit: str = None,
+        profile: str = None,
+        region_id: str = None,
+        resource_group_id: str = None,
+        tag_shrink: str = None,
+        v_switches: str = None,
+        vpc_id: str = None,
+        workflow_schedule_mode: str = None,
+    ):
+        # Specifies whether to expose the API server to the Internet. Valid values:
+        # 
+        # *   true: exposes the API server to the Internet.
+        # *   false: exposes the API server to the internal network.
+        self.api_server_public_eip = api_server_public_eip
+        # Specifies whether to enable the workflow instance UI. This parameter takes effect only if Profile is set to XFlow. Valid values:
+        # 
+        # *   true
+        # *   false
+        self.argo_server_enabled = argo_server_enabled
+        # Specifies whether to enable the audit log feature. Valid values:
+        # 
+        # *   true: enables the audit log feature.
+        # *   false: disables the audit log feature.
+        self.audit_log_enabled = audit_log_enabled
+        # Specifies whether to use an advanced security group.
+        self.is_enterprise_security_group = is_enterprise_security_group
+        # The name of the master instance.
+        self.name = name
+        # The limit on the prices of containers in the workflow. This parameter takes effect only if the WorkflowScheduleMode parameter is set to cost-optimized.
+        self.price_limit = price_limit
+        # The type of scenario for which the master instance is suitable. Valid values:
+        # 
+        # *   `Default`: The master instance is suitable for standard scenarios.
+        # *   `XFlow`: The master instance is suitable for workflow scenarios.
+        # 
+        # Default value: `Default`.
+        self.profile = profile
+        # The ID of the region. You can call the DescribeRegions operation to query available regions.
+        # 
+        # This parameter is required.
+        self.region_id = region_id
+        # The Resource Group ID.
+        self.resource_group_id = resource_group_id
+        self.tag_shrink = tag_shrink
+        # The ID of the vSwitch.
+        # 
+        # This parameter is required.
+        self.v_switches = v_switches
+        # The ID of the virtual private cloud (VPC) to which the master instance belongs. You can call the DescribeVpcs operation to query available VPCs.
+        # 
+        # This parameter is required.
         self.vpc_id = vpc_id
         # The scheduling mode of the workflow. This parameter takes effect only if Profile is set to XFlow. Valid values:
         # 
         # *   cost-optimized: cost-prioritized scheduling mode.
         # *   stock-optimized: inventory-prioritized scheduling mode.
         self.workflow_schedule_mode = workflow_schedule_mode
 
@@ -216,14 +518,16 @@
             result['PriceLimit'] = self.price_limit
         if self.profile is not None:
             result['Profile'] = self.profile
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['ResourceGroupID'] = self.resource_group_id
+        if self.tag_shrink is not None:
+            result['Tag'] = self.tag_shrink
         if self.v_switches is not None:
             result['VSwitches'] = self.v_switches
         if self.vpc_id is not None:
             result['VpcId'] = self.vpc_id
         if self.workflow_schedule_mode is not None:
             result['WorkflowScheduleMode'] = self.workflow_schedule_mode
         return result
@@ -244,14 +548,16 @@
             self.price_limit = m.get('PriceLimit')
         if m.get('Profile') is not None:
             self.profile = m.get('Profile')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupID') is not None:
             self.resource_group_id = m.get('ResourceGroupID')
+        if m.get('Tag') is not None:
+            self.tag_shrink = m.get('Tag')
         if m.get('VSwitches') is not None:
             self.v_switches = m.get('VSwitches')
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         if m.get('WorkflowScheduleMode') is not None:
             self.workflow_schedule_mode = m.get('WorkflowScheduleMode')
         return self
@@ -344,14 +650,16 @@
     def __init__(
         self,
         cluster_id: str = None,
         force: bool = None,
         retain_resources: List[str] = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # Specifies whether to forcefully delete the master instance in ACK One. Valid values:
         # 
         # *   true: forcefully deletes the master instance in ACK One.
         # *   false: does not forcibly delete the master instance in ACK One.
         # 
         # Default value: false.
@@ -391,14 +699,16 @@
     def __init__(
         self,
         cluster_id: str = None,
         force: bool = None,
         retain_resources_shrink: str = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # Specifies whether to forcefully delete the master instance in ACK One. Valid values:
         # 
         # *   true: forcefully deletes the master instance in ACK One.
         # *   false: does not forcibly delete the master instance in ACK One.
         # 
         # Default value: false.
@@ -521,18 +831,22 @@
     def __init__(
         self,
         cluster_id: str = None,
         cluster_ids: List[str] = None,
         policy_name: str = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # A array of JSON strings. The JSON strings in the array indicate the IDs of the associated clusters for which the policy is deleted.
         self.cluster_ids = cluster_ids
         # The name of the policy.
+        # 
+        # This parameter is required.
         self.policy_name = policy_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -563,18 +877,22 @@
     def __init__(
         self,
         cluster_id: str = None,
         cluster_ids_shrink: str = None,
         policy_name: str = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # A array of JSON strings. The JSON strings in the array indicate the IDs of the associated clusters for which the policy is deleted.
         self.cluster_ids_shrink = cluster_ids_shrink
         # The name of the policy.
+        # 
+        # This parameter is required.
         self.policy_name = policy_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -673,16 +991,20 @@
 class DeleteUserPermissionRequest(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
         user_id: str = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # The ID of the RAM user.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -780,25 +1102,33 @@
         cluster_id: str = None,
         cluster_ids: List[str] = None,
         namespaces: List[str] = None,
         policy_action: str = None,
         policy_name: str = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # An array of JSON strings. The JSON strings in the array indicate the IDs of the associated clusters in which the policy instance is deployed.
+        # 
+        # This parameter is required.
         self.cluster_ids = cluster_ids
         # A list of namespaces.
         self.namespaces = namespaces
         # The action of the policy. Valid values:
         # 
         # *   deny: blocks deployments that match the policy.
         # *   warn: generates alerts for deployments that match the policy.
+        # 
+        # This parameter is required.
         self.policy_action = policy_action
         # The name of the policy.
+        # 
+        # This parameter is required.
         self.policy_name = policy_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -839,25 +1169,33 @@
         cluster_id: str = None,
         cluster_ids_shrink: str = None,
         namespaces_shrink: str = None,
         policy_action: str = None,
         policy_name: str = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # An array of JSON strings. The JSON strings in the array indicate the IDs of the associated clusters in which the policy instance is deployed.
+        # 
+        # This parameter is required.
         self.cluster_ids_shrink = cluster_ids_shrink
         # A list of namespaces.
         self.namespaces_shrink = namespaces_shrink
         # The action of the policy. Valid values:
         # 
         # *   deny: blocks deployments that match the policy.
         # *   warn: generates alerts for deployments that match the policy.
+        # 
+        # This parameter is required.
         self.policy_action = policy_action
         # The name of the policy.
+        # 
+        # This parameter is required.
         self.policy_name = policy_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -963,14 +1301,16 @@
 
 class DescribeHubClusterDetailsRequest(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1246,27 +1586,61 @@
         m = m or dict()
         if m.get('ACKOne') is not None:
             temp_model = DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOne()
             self.ackone = temp_model.from_map(m['ACKOne'])
         return self
 
 
+class DescribeHubClusterDetailsResponseBodyClusterClusterInfoTags(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class DescribeHubClusterDetailsResponseBodyClusterClusterInfo(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
         cluster_spec: str = None,
         creation_time: str = None,
         error_message: str = None,
         meta_data: DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaData = None,
         name: str = None,
         profile: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         state: str = None,
+        tags: List[DescribeHubClusterDetailsResponseBodyClusterClusterInfoTags] = None,
         update_time: str = None,
         version: str = None,
     ):
         # The ID of the master instance.
         self.cluster_id = cluster_id
         # The specification of the master instance. Valid value:
         # 
@@ -1292,22 +1666,27 @@
         # *   failed: The master instance failed to be created.
         # *   running: The master instance is running
         # *   inactive: The master instance is pending.
         # *   deleting: The master instance is being deleted.
         # *   delete_failed: The master instance failed to be deleted.
         # *   deleted: The master instance is deleted.
         self.state = state
+        self.tags = tags
         # The time when the master instance was updated.
         self.update_time = update_time
         # The version of the master instance.
         self.version = version
 
     def validate(self):
         if self.meta_data:
             self.meta_data.validate()
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1327,14 +1706,18 @@
             result['Profile'] = self.profile
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['ResourceGroupID'] = self.resource_group_id
         if self.state is not None:
             result['State'] = self.state
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
         if self.update_time is not None:
             result['UpdateTime'] = self.update_time
         if self.version is not None:
             result['Version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
@@ -1356,14 +1739,19 @@
             self.profile = m.get('Profile')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupID') is not None:
             self.resource_group_id = m.get('ResourceGroupID')
         if m.get('State') is not None:
             self.state = m.get('State')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = DescribeHubClusterDetailsResponseBodyClusterClusterInfoTags()
+                self.tags.append(temp_model.from_map(k))
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         if m.get('Version') is not None:
             self.version = m.get('Version')
         return self
 
 
@@ -1604,15 +1992,15 @@
         vswitch_id: str = None,
         zone_id: str = None,
     ):
         # The ID of the vSwitch.
         self.vswitch_id = vswitch_id
         # The zone ID of the cluster.
         # 
-        # > You can call the [DescribeRegions](~~143074~~) operation to query the most recent zone list.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/143074.html) operation to query the most recent zone list.
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1640,15 +2028,15 @@
         self,
         region_id: str = None,
         v_switches: List[DescribeHubClusterDetailsResponseBodyClusterWorkflowConfigWorkflowUnitsVSwitches] = None,
         vpc_id: str = None,
     ):
         # The region ID of the cluster.
         # 
-        # >  You can call the [DescribeRegions](~~143074~~) operation to query the most recent region list.
+        # >  You can call the [DescribeRegions](https://help.aliyun.com/document_detail/143074.html) operation to query the most recent region list.
         self.region_id = region_id
         # The vSwitches.
         self.v_switches = v_switches
         # The ID of the VPC.
         self.vpc_id = vpc_id
 
     def validate(self):
@@ -1937,14 +2325,16 @@
 class DescribeHubClusterKubeconfigRequest(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
         private_ip_address: bool = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # Specifies whether to obtain the kubeconfig file that is used to connect to the cluster over the internal network. Valid values:
         # 
         # *   `true`: obtains the kubeconfig file that is used to connect to the master instance over the internal network.
         # *   `false`: obtains the kubeconfig file that is used to connect to the master instance over the Internet.
         # 
         # Default value: `false`
@@ -2052,14 +2442,16 @@
 
 class DescribeHubClusterLogsRequest(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2212,41 +2604,96 @@
 
 
 class DescribeHubClustersRequest(TeaModel):
     def __init__(
         self,
         profile: str = None,
         resource_group_id: str = None,
+        tag: List[Tag] = None,
+    ):
+        # The configurations of the cluster.
+        self.profile = profile
+        # The resource group ID.
+        self.resource_group_id = resource_group_id
+        self.tag = tag
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.profile is not None:
+            result['Profile'] = self.profile
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Profile') is not None:
+            self.profile = m.get('Profile')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = Tag()
+                self.tag.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeHubClustersShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        profile: str = None,
+        resource_group_id: str = None,
+        tag_shrink: str = None,
     ):
         # The configurations of the cluster.
         self.profile = profile
         # The resource group ID.
         self.resource_group_id = resource_group_id
+        self.tag_shrink = tag_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.profile is not None:
             result['Profile'] = self.profile
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
+        if self.tag_shrink is not None:
+            result['Tag'] = self.tag_shrink
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Profile') is not None:
             self.profile = m.get('Profile')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('Tag') is not None:
+            self.tag_shrink = m.get('Tag')
         return self
 
 
 class DescribeHubClustersResponseBodyClustersApiServer(TeaModel):
     def __init__(
         self,
         api_server_eip_id: str = None,
@@ -2287,26 +2734,60 @@
         if m.get('EnabledPublic') is not None:
             self.enabled_public = m.get('EnabledPublic')
         if m.get('LoadBalancerId') is not None:
             self.load_balancer_id = m.get('LoadBalancerId')
         return self
 
 
+class DescribeHubClustersResponseBodyClustersClusterInfoTags(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class DescribeHubClustersResponseBodyClustersClusterInfo(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
         cluster_spec: str = None,
         creation_time: str = None,
         error_message: str = None,
         name: str = None,
         profile: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         state: str = None,
+        tags: List[DescribeHubClustersResponseBodyClustersClusterInfoTags] = None,
         update_time: str = None,
         version: str = None,
     ):
         # The cluster ID.
         self.cluster_id = cluster_id
         # The specification of the cluster.
         # 
@@ -2330,21 +2811,25 @@
         # *   failed: The cluster failed to be created.
         # *   running: The cluster is running
         # *   inactive: The cluster is pending.
         # *   deleting: The cluster is being deleted.
         # *   delete_failed: The cluster failed to be deleted.
         # *   deleted: The cluster is deleted.
         self.state = state
+        self.tags = tags
         # The time when the cluster was last updated.
         self.update_time = update_time
         # The Kubernetes version of the cluster.
         self.version = version
 
     def validate(self):
-        pass
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -2362,14 +2847,18 @@
             result['Profile'] = self.profile
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['ResourceGroupID'] = self.resource_group_id
         if self.state is not None:
             result['State'] = self.state
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
         if self.update_time is not None:
             result['UpdateTime'] = self.update_time
         if self.version is not None:
             result['Version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
@@ -2388,14 +2877,19 @@
             self.profile = m.get('Profile')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupID') is not None:
             self.resource_group_id = m.get('ResourceGroupID')
         if m.get('State') is not None:
             self.state = m.get('State')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = DescribeHubClustersResponseBodyClustersClusterInfoTags()
+                self.tags.append(temp_model.from_map(k))
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         if m.get('Version') is not None:
             self.version = m.get('Version')
         return self
 
 
@@ -2801,14 +3295,16 @@
 
 class DescribeManagedClustersRequest(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
     ):
         # The status of the association between the clusters and Service Mesh (ASM).
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3459,14 +3955,16 @@
 
 class DescribePolicyGovernanceInClusterRequest(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4151,16 +4649,20 @@
 class DescribePolicyInstancesRequest(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
         policy_name: str = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # The name of the policy.
+        # 
+        # This parameter is required.
         self.policy_name = policy_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4212,15 +4714,15 @@
         self.policy_description = policy_description
         # The name of the policy.
         self.policy_name = policy_name
         # The parameters of the policy instance.
         self.policy_parameters = policy_parameters
         # The applicable scope of the policy instance.
         # 
-        # A value of \* indicates all namespaces. This is the default value.
+        # A value of \\* indicates all namespaces. This is the default value.
         # 
         # Multiple namespaces are separated by commas (,).
         self.policy_scope = policy_scope
         # The severity level of the policy.
         self.policy_severity = policy_severity
         # The total number of deployments that match the policy in the associated cluster, including the deployments that are blocked and the deployments that have triggered alerting.
         self.total_violations = total_violations
@@ -4367,14 +4869,16 @@
 
 class DescribePolicyInstancesStatusRequest(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4813,14 +5317,16 @@
 
 class DescribeUserPermissionsRequest(TeaModel):
     def __init__(
         self,
         user_id: str = None,
     ):
         # The ID of the RAM user that you want to query.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4986,16 +5492,20 @@
     def __init__(
         self,
         cluster_id: str = None,
         cluster_ids: str = None,
         detach_from_mesh: bool = None,
     ):
         # The ID of the request.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # The operation that you want to perform. Set the value to **DetachClusterFromHub**.
+        # 
+        # This parameter is required.
         self.cluster_ids = cluster_ids
         # Example 1
         self.detach_from_mesh = detach_from_mesh
 
     def validate(self):
         pass
 
@@ -5119,30 +5629,38 @@
         is_ram_role: bool = None,
         namespace: str = None,
         role_name: str = None,
         role_type: str = None,
         user_id: str = None,
     ):
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # The entity to which the permissions are granted. A value of `true` indicates that the permissions are granted to a RAM user. A value of `false` indicates that the permissions are granted to a RAM role.
         self.is_ram_role = is_ram_role
         # The namespace to which the permissions are scoped. By default, this parameter is empty when you set RoleType to cluster.
         self.namespace = namespace
         # The predefined role that you want to assign. Valid values:
         # 
         # *   admin: the administrator role.
         # *   dev: the developer role.
+        # 
+        # This parameter is required.
         self.role_name = role_name
         # The authorization type. Valid values:
         # 
         # *   cluster: specifies that the permissions are scoped to a master instance.
         # *   namespace: specifies that the permissions are scoped to a namespace of a cluster.
+        # 
+        # This parameter is required.
         self.role_type = role_type
         # The ID of the RAM user or RAM role.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5267,20 +5785,24 @@
         self.is_ram_role = is_ram_role
         # The namespace to which the permissions are scoped. By default, this parameter is empty when you set RoleType to cluster.
         self.namespace = namespace
         # The predefined role that you want to assign. Valid values:
         # 
         # *   admin: the administrator role.
         # *   dev: the developer role.
+        # 
+        # This parameter is required.
         self.role_name = role_name
         # The authorization type. Valid values:
         # 
         # *   cluster: specifies that the permissions are scoped to a master instance.
         # *   namespace: specifies that the permissions are scoped to a namespace of a cluster.
         # *   all-clusters: specifies that the permissions are scoped to all master instances.
+        # 
+        # This parameter is required.
         self.role_type = role_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5320,14 +5842,16 @@
         self,
         permissions: List[GrantUserPermissionsRequestPermissions] = None,
         user_id: str = None,
     ):
         # The list of permissions that you want to grant to the RAM user.
         self.permissions = permissions
         # The ID of the RAM user.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         if self.permissions:
             for k in self.permissions:
                 if k:
                     k.validate()
@@ -5363,14 +5887,16 @@
         self,
         permissions_shrink: str = None,
         user_id: str = None,
     ):
         # The list of permissions that you want to grant to the RAM user.
         self.permissions_shrink = permissions_shrink
         # The ID of the RAM user.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5510,14 +6036,16 @@
         self.argo_server_enabled = argo_server_enabled
         # Specifies whether to enable the audit logging feature. Valid values:
         # 
         # *   true: enables the audit logging feature.
         # *   false: disables the audit logging feature.
         self.audit_log_enabled = audit_log_enabled
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # Specifies whether to enable the deletion protection feature for the cluster. After you enable the deletion protection feature for the cluster, you cannot delete the cluster in the console or by calling the DeleteHubCluster operation. Valid values:
         # 
         # *   true
         # *   false
         # 
         # Default value: false.
@@ -5532,15 +6060,15 @@
         # - false
         self.gateway_enabled = gateway_enabled
         # Specifies whether to enable the monitoring dashboard feature for the workflow instance. This parameter takes effect only if Profile is set to XFlow. Valid values:
         # 
         # *   true
         # *   false
         self.monitor_enabled = monitor_enabled
-        # The name of the master instance. The name must be 1 to 63 characters in length. It must start with a letter, and can contain letters, digits, underscores (\_), and hyphens (-).
+        # The name of the master instance. The name must be 1 to 63 characters in length. It must start with a letter, and can contain letters, digits, underscores (_), and hyphens (-).
         self.name = name
         # The limit on the prices of containers in the workflow. This parameter takes effect only if the WorkflowScheduleMode parameter is set to cost-optimized.
         self.price_limit = price_limit
         # Specifies whether to enable public domain name resolution in the Argo CD or Argo Workflow console. Valid values:
         # 
         # *   true
         # *   false
@@ -5694,14 +6222,16 @@
         self.argo_server_enabled = argo_server_enabled
         # Specifies whether to enable the audit logging feature. Valid values:
         # 
         # *   true: enables the audit logging feature.
         # *   false: disables the audit logging feature.
         self.audit_log_enabled = audit_log_enabled
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # Specifies whether to enable the deletion protection feature for the cluster. After you enable the deletion protection feature for the cluster, you cannot delete the cluster in the console or by calling the DeleteHubCluster operation. Valid values:
         # 
         # *   true
         # *   false
         # 
         # Default value: false.
@@ -5716,15 +6246,15 @@
         # - false
         self.gateway_enabled = gateway_enabled
         # Specifies whether to enable the monitoring dashboard feature for the workflow instance. This parameter takes effect only if Profile is set to XFlow. Valid values:
         # 
         # *   true
         # *   false
         self.monitor_enabled = monitor_enabled
-        # The name of the master instance. The name must be 1 to 63 characters in length. It must start with a letter, and can contain letters, digits, underscores (\_), and hyphens (-).
+        # The name of the master instance. The name must be 1 to 63 characters in length. It must start with a letter, and can contain letters, digits, underscores (_), and hyphens (-).
         self.name = name
         # The limit on the prices of containers in the workflow. This parameter takes effect only if the WorkflowScheduleMode parameter is set to cost-optimized.
         self.price_limit = price_limit
         # Specifies whether to enable public domain name resolution in the Argo CD or Argo Workflow console. Valid values:
         # 
         # *   true
         # *   false
@@ -5905,28 +6435,36 @@
         cluster_id: str = None,
         namespace: str = None,
         role_name: str = None,
         role_type: str = None,
         user_id: str = None,
     ):
         # The ID of the master instance.
+        # 
+        # This parameter is required.
         self.cluster_id = cluster_id
         # The namespace to which the permissions are scoped. By default, this parameter is empty when you set RoleType to cluster.
         self.namespace = namespace
         # Specifies the predefined role that you want to assign. Valid values:
         # 
         # *   admin: the administrator role.
         # *   dev: the developer role.
+        # 
+        # This parameter is required.
         self.role_name = role_name
         # The authorization type. Valid values:
         # 
         # *   cluster: specifies that the permissions are scoped to a master instance.
         # *   namespace: specifies that the permissions are scoped to a namespace of a cluster.
+        # 
+        # This parameter is required.
         self.role_type = role_type
         # The ID of the RAM user.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/PKG-INFO` & `alibabacloud_adcp20220101-3.1.0/alibabacloud_adcp20220101.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-adcp20220101
-Version: 3.0.0
+Version: 3.1.0
 Summary: Alibaba Cloud adcp (20220101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adcp20220101-3.0.0/setup.py` & `alibabacloud_adcp20220101-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_adcp20220101.
 
-Created on 22/04/2024
+Created on 13/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_adcp20220101"
 NAME = "alibabacloud_adcp20220101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud adcp (20220101) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

