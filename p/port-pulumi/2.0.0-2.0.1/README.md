# Comparing `tmp/port_pulumi-2.0.0.tar.gz` & `tmp/port_pulumi-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_pulumi-2.0.0.tar", last modified: Sat May 11 09:52:22 2024, max compression
+gzip compressed data, was "port_pulumi-2.0.1.tar", last modified: Mon May 13 06:36:54 2024, max compression
```

## Comparing `port_pulumi-2.0.0.tar` & `port_pulumi-2.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:52:22.334064 port_pulumi-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-11 09:52:22.334064 port_pulumi-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:52:22.334064 port_pulumi-2.0.0/port_pulumi/
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   196235 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    43486 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30278 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/aggregation_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/aggregation_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    36508 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/blueprint_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:52:22.334064 port_pulumi-2.0.0/port_pulumi/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    22571 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)   167091 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24949 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/page_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/scorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    22539 2024-05-11 09:52:21.000000 port_pulumi-2.0.0/port_pulumi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:52:22.334064 port_pulumi-2.0.0/port_pulumi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/port_pulumi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/port_pulumi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/port_pulumi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/port_pulumi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/port_pulumi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/port_pulumi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 09:52:22.338064 port_pulumi-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-11 09:52:22.000000 port_pulumi-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:36:54.550242 port_pulumi-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-13 06:36:54.550242 port_pulumi-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:36:54.550242 port_pulumi-2.0.1/port_pulumi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196235 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43486 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30278 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/aggregation_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/aggregation_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36508 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/blueprint_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:36:54.550242 port_pulumi-2.0.1/port_pulumi/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22571 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167091 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26699 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/page_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/scorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22539 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:36:54.550242 port_pulumi-2.0.1/port_pulumi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 06:36:54.550242 port_pulumi-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/setup.py
```

### Comparing `port_pulumi-2.0.0/PKG-INFO` & `port_pulumi-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port_pulumi
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `port_pulumi-2.0.0/README.md` & `port_pulumi-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/__init__.py` & `port_pulumi-2.0.1/port_pulumi/__init__.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/_inputs.py` & `port_pulumi-2.0.1/port_pulumi/_inputs.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/_utilities.py` & `port_pulumi-2.0.1/port_pulumi/_utilities.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/action.py` & `port_pulumi-2.0.1/port_pulumi/action.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/action_permissions.py` & `port_pulumi-2.0.1/port_pulumi/action_permissions.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/aggregation_properties.py` & `port_pulumi-2.0.1/port_pulumi/aggregation_properties.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/aggregation_property.py` & `port_pulumi-2.0.1/port_pulumi/aggregation_property.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/blueprint.py` & `port_pulumi-2.0.1/port_pulumi/blueprint.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/blueprint_permissions.py` & `port_pulumi-2.0.1/port_pulumi/blueprint_permissions.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/config/vars.py` & `port_pulumi-2.0.1/port_pulumi/config/vars.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/entity.py` & `port_pulumi-2.0.1/port_pulumi/entity.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/outputs.py` & `port_pulumi-2.0.1/port_pulumi/outputs.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/page.py` & `port_pulumi-2.0.1/port_pulumi/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,37 +14,41 @@
 @pulumi.input_type
 class PageArgs:
     def __init__(__self__, *,
                  identifier: pulumi.Input[str],
                  type: pulumi.Input[str],
                  after: Optional[pulumi.Input[str]] = None,
                  blueprint: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  locked: Optional[pulumi.Input[bool]] = None,
                  parent: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  widgets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a Page resource.
         :param pulumi.Input[str] identifier: The Identifier of the page
         :param pulumi.Input[str] type: The type of the page, can be one of "blueprint-entities", "dashboard" or "home"
         :param pulumi.Input[str] after: The identifier of the page/folder after which the page should be placed
         :param pulumi.Input[str] blueprint: The blueprint for which the page is created, relevant only for pages of type "blueprint-entities"
+        :param pulumi.Input[str] description: The page description
         :param pulumi.Input[str] icon: The icon of the page
         :param pulumi.Input[bool] locked: Whether the page is locked, if true, viewers will not be able to edit the page widgets and filters
         :param pulumi.Input[str] parent: The identifier of the folder in which the page is in, default is the root of the sidebar
         :param pulumi.Input[str] title: The title of the page
         :param pulumi.Input[Sequence[pulumi.Input[str]]] widgets: The widgets of the page
         """
         pulumi.set(__self__, "identifier", identifier)
         pulumi.set(__self__, "type", type)
         if after is not None:
             pulumi.set(__self__, "after", after)
         if blueprint is not None:
             pulumi.set(__self__, "blueprint", blueprint)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if locked is not None:
             pulumi.set(__self__, "locked", locked)
         if parent is not None:
             pulumi.set(__self__, "parent", parent)
         if title is not None:
@@ -98,14 +102,26 @@
 
     @blueprint.setter
     def blueprint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "blueprint", value)
 
     @property
     @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
+        """
+        The page description
+        """
+        return pulumi.get(self, "description")
+
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
+
+    @property
+    @pulumi.getter
     def icon(self) -> Optional[pulumi.Input[str]]:
         """
         The icon of the page
         """
         return pulumi.get(self, "icon")
 
     @icon.setter
@@ -164,14 +180,15 @@
 @pulumi.input_type
 class _PageState:
     def __init__(__self__, *,
                  after: Optional[pulumi.Input[str]] = None,
                  blueprint: Optional[pulumi.Input[str]] = None,
                  created_at: Optional[pulumi.Input[str]] = None,
                  created_by: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  locked: Optional[pulumi.Input[bool]] = None,
                  parent: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  updated_at: Optional[pulumi.Input[str]] = None,
@@ -179,14 +196,15 @@
                  widgets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering Page resources.
         :param pulumi.Input[str] after: The identifier of the page/folder after which the page should be placed
         :param pulumi.Input[str] blueprint: The blueprint for which the page is created, relevant only for pages of type "blueprint-entities"
         :param pulumi.Input[str] created_at: The creation date of the page
         :param pulumi.Input[str] created_by: The creator of the page
+        :param pulumi.Input[str] description: The page description
         :param pulumi.Input[str] icon: The icon of the page
         :param pulumi.Input[str] identifier: The Identifier of the page
         :param pulumi.Input[bool] locked: Whether the page is locked, if true, viewers will not be able to edit the page widgets and filters
         :param pulumi.Input[str] parent: The identifier of the folder in which the page is in, default is the root of the sidebar
         :param pulumi.Input[str] title: The title of the page
         :param pulumi.Input[str] type: The type of the page, can be one of "blueprint-entities", "dashboard" or "home"
         :param pulumi.Input[str] updated_at: The last update date of the page
@@ -197,14 +215,16 @@
             pulumi.set(__self__, "after", after)
         if blueprint is not None:
             pulumi.set(__self__, "blueprint", blueprint)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if created_by is not None:
             pulumi.set(__self__, "created_by", created_by)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if identifier is not None:
             pulumi.set(__self__, "identifier", identifier)
         if locked is not None:
             pulumi.set(__self__, "locked", locked)
         if parent is not None:
@@ -266,14 +286,26 @@
 
     @created_by.setter
     def created_by(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_by", value)
 
     @property
     @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
+        """
+        The page description
+        """
+        return pulumi.get(self, "description")
+
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
+
+    @property
+    @pulumi.getter
     def icon(self) -> Optional[pulumi.Input[str]]:
         """
         The icon of the page
         """
         return pulumi.get(self, "icon")
 
     @icon.setter
@@ -380,28 +412,30 @@
 class Page(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  after: Optional[pulumi.Input[str]] = None,
                  blueprint: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  locked: Optional[pulumi.Input[bool]] = None,
                  parent: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  widgets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Create a Page resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] after: The identifier of the page/folder after which the page should be placed
         :param pulumi.Input[str] blueprint: The blueprint for which the page is created, relevant only for pages of type "blueprint-entities"
+        :param pulumi.Input[str] description: The page description
         :param pulumi.Input[str] icon: The icon of the page
         :param pulumi.Input[str] identifier: The Identifier of the page
         :param pulumi.Input[bool] locked: Whether the page is locked, if true, viewers will not be able to edit the page widgets and filters
         :param pulumi.Input[str] parent: The identifier of the folder in which the page is in, default is the root of the sidebar
         :param pulumi.Input[str] title: The title of the page
         :param pulumi.Input[str] type: The type of the page, can be one of "blueprint-entities", "dashboard" or "home"
         :param pulumi.Input[Sequence[pulumi.Input[str]]] widgets: The widgets of the page
@@ -427,14 +461,15 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  after: Optional[pulumi.Input[str]] = None,
                  blueprint: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  locked: Optional[pulumi.Input[bool]] = None,
                  parent: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  widgets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
@@ -445,14 +480,15 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PageArgs.__new__(PageArgs)
 
             __props__.__dict__["after"] = after
             __props__.__dict__["blueprint"] = blueprint
+            __props__.__dict__["description"] = description
             __props__.__dict__["icon"] = icon
             if identifier is None and not opts.urn:
                 raise TypeError("Missing required property 'identifier'")
             __props__.__dict__["identifier"] = identifier
             __props__.__dict__["locked"] = locked
             __props__.__dict__["parent"] = parent
             __props__.__dict__["title"] = title
@@ -474,14 +510,15 @@
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             after: Optional[pulumi.Input[str]] = None,
             blueprint: Optional[pulumi.Input[str]] = None,
             created_at: Optional[pulumi.Input[str]] = None,
             created_by: Optional[pulumi.Input[str]] = None,
+            description: Optional[pulumi.Input[str]] = None,
             icon: Optional[pulumi.Input[str]] = None,
             identifier: Optional[pulumi.Input[str]] = None,
             locked: Optional[pulumi.Input[bool]] = None,
             parent: Optional[pulumi.Input[str]] = None,
             title: Optional[pulumi.Input[str]] = None,
             type: Optional[pulumi.Input[str]] = None,
             updated_at: Optional[pulumi.Input[str]] = None,
@@ -494,14 +531,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] after: The identifier of the page/folder after which the page should be placed
         :param pulumi.Input[str] blueprint: The blueprint for which the page is created, relevant only for pages of type "blueprint-entities"
         :param pulumi.Input[str] created_at: The creation date of the page
         :param pulumi.Input[str] created_by: The creator of the page
+        :param pulumi.Input[str] description: The page description
         :param pulumi.Input[str] icon: The icon of the page
         :param pulumi.Input[str] identifier: The Identifier of the page
         :param pulumi.Input[bool] locked: Whether the page is locked, if true, viewers will not be able to edit the page widgets and filters
         :param pulumi.Input[str] parent: The identifier of the folder in which the page is in, default is the root of the sidebar
         :param pulumi.Input[str] title: The title of the page
         :param pulumi.Input[str] type: The type of the page, can be one of "blueprint-entities", "dashboard" or "home"
         :param pulumi.Input[str] updated_at: The last update date of the page
@@ -512,14 +550,15 @@
 
         __props__ = _PageState.__new__(_PageState)
 
         __props__.__dict__["after"] = after
         __props__.__dict__["blueprint"] = blueprint
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["created_by"] = created_by
+        __props__.__dict__["description"] = description
         __props__.__dict__["icon"] = icon
         __props__.__dict__["identifier"] = identifier
         __props__.__dict__["locked"] = locked
         __props__.__dict__["parent"] = parent
         __props__.__dict__["title"] = title
         __props__.__dict__["type"] = type
         __props__.__dict__["updated_at"] = updated_at
@@ -557,14 +596,22 @@
         """
         The creator of the page
         """
         return pulumi.get(self, "created_by")
 
     @property
     @pulumi.getter
+    def description(self) -> pulumi.Output[Optional[str]]:
+        """
+        The page description
+        """
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter
     def icon(self) -> pulumi.Output[Optional[str]]:
         """
         The icon of the page
         """
         return pulumi.get(self, "icon")
 
     @property
```

### Comparing `port_pulumi-2.0.0/port_pulumi/page_permissions.py` & `port_pulumi-2.0.1/port_pulumi/page_permissions.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/provider.py` & `port_pulumi-2.0.1/port_pulumi/provider.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/scorecard.py` & `port_pulumi-2.0.1/port_pulumi/scorecard.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/team.py` & `port_pulumi-2.0.1/port_pulumi/team.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi/webhook.py` & `port_pulumi-2.0.1/port_pulumi/webhook.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/port_pulumi.egg-info/PKG-INFO` & `port_pulumi-2.0.1/port_pulumi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-pulumi
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `port_pulumi-2.0.0/port_pulumi.egg-info/SOURCES.txt` & `port_pulumi-2.0.1/port_pulumi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.0/setup.py` & `port_pulumi-2.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.0.0"
+VERSION = "2.0.1"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "port Pulumi Package - Development Version"
```

