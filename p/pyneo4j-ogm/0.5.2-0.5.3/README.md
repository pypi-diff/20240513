# Comparing `tmp/pyneo4j_ogm-0.5.2.tar.gz` & `tmp/pyneo4j_ogm-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneo4j_ogm-0.5.2.tar", max compression
+gzip compressed data, was "pyneo4j_ogm-0.5.3.tar", max compression
```

## Comparing `pyneo4j_ogm-0.5.2.tar` & `pyneo4j_ogm-0.5.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1070 2024-02-22 18:15:50.684199 pyneo4j_ogm-0.5.2/LICENSE
--rw-r--r--   0        0        0   101982 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/README.md
--rw-r--r--   0        0        0      415 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/__init__.py
--rw-r--r--   0        0        0    34639 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/core/base.py
--rw-r--r--   0        0        0    31571 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/core/client.py
--rw-r--r--   0        0        0    46979 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/core/node.py
--rw-r--r--   0        0        0    32693 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/core/relationship.py
--rw-r--r--   0        0        0     6528 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/exceptions.py
--rw-r--r--   0        0        0     1864 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/fields/property_options.py
--rw-r--r--   0        0        0    45334 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/fields/relationship_property.py
--rw-r--r--   0        0        0     2065 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/fields/settings.py
--rw-r--r--   0        0        0      771 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/logger.py
--rw-r--r--   0        0        0      203 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/__init__.py
--rw-r--r--   0        0        0     1680 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/actions/create.py
--rw-r--r--   0        0        0     2509 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/actions/down.py
--rw-r--r--   0        0        0     2087 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/actions/init.py
--rw-r--r--   0        0        0     3945 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/actions/status.py
--rw-r--r--   0        0        0     2149 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/actions/up.py
--rw-r--r--   0        0        0     3888 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/cli.py
--rw-r--r--   0        0        0     3718 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/utils/client.py
--rw-r--r--   0        0        0      640 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/utils/defaults.py
--rw-r--r--   0        0        0     3334 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/utils/migration.py
--rw-r--r--   0        0        0     4429 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/utils/models.py
--rw-r--r--   0        0        0     2017 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/pydantic_utils.py
--rw-r--r--   0        0        0    17636 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/queries/operators.py
--rw-r--r--   0        0        0    16707 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/queries/query_builder.py
--rw-r--r--   0        0        0     5945 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/queries/types.py
--rw-r--r--   0        0        0    15032 2024-02-22 18:15:50.688199 pyneo4j_ogm-0.5.2/pyneo4j_ogm/queries/validators.py
--rw-r--r--   0        0        0     1846 2024-02-22 18:15:51.572194 pyneo4j_ogm-0.5.2/pyproject.toml
--rw-r--r--   0        0        0   103285 1970-01-01 00:00:00.000000 pyneo4j_ogm-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/LICENSE
+-rw-r--r--   0        0        0    22292 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/README.md
+-rw-r--r--   0        0        0      415 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/__init__.py
+-rw-r--r--   0        0        0    39179 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/base.py
+-rw-r--r--   0        0        0    33617 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/client.py
+-rw-r--r--   0        0        0    47837 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/node.py
+-rw-r--r--   0        0        0    32758 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/relationship.py
+-rw-r--r--   0        0        0     7053 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/exceptions.py
+-rw-r--r--   0        0        0     1864 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/fields/property_options.py
+-rw-r--r--   0        0        0    45294 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/fields/relationship_property.py
+-rw-r--r--   0        0        0     2025 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/fields/settings.py
+-rw-r--r--   0        0        0      749 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/logger.py
+-rw-r--r--   0        0        0      203 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/__init__.py
+-rw-r--r--   0        0        0     1680 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/create.py
+-rw-r--r--   0        0        0     2746 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/down.py
+-rw-r--r--   0        0        0     2087 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/init.py
+-rw-r--r--   0        0        0     3945 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/status.py
+-rw-r--r--   0        0        0     2368 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/up.py
+-rw-r--r--   0        0        0     3888 2024-05-13 10:57:00.245032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/cli.py
+-rw-r--r--   0        0        0     3718 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/client.py
+-rw-r--r--   0        0        0      640 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/defaults.py
+-rw-r--r--   0        0        0     3334 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/migration.py
+-rw-r--r--   0        0        0     4429 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/models.py
+-rw-r--r--   0        0        0     1951 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/pydantic_utils.py
+-rw-r--r--   0        0        0    17636 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/operators.py
+-rw-r--r--   0        0        0    16707 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/query_builder.py
+-rw-r--r--   0        0        0     5945 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/types.py
+-rw-r--r--   0        0        0    14993 2024-05-13 10:57:00.249032 pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/validators.py
+-rw-r--r--   0        0        0     2744 2024-05-13 10:57:01.945021 pyneo4j_ogm-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    23595 1970-01-01 00:00:00.000000 pyneo4j_ogm-0.5.3/PKG-INFO
```

### Comparing `pyneo4j_ogm-0.5.2/LICENSE` & `pyneo4j_ogm-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/core/base.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """
-Base class for both `NodeModel` and `RelationshipModel`. This class handles shared logic for both
-model types like registering hooks and exporting/importing models to/from dictionaries.
+Base Node/Relationship class module.
 """
 
-# pyright: reportUnboundVariable=false
-
 import asyncio
 import json
 from asyncio import iscoroutinefunction
 from copy import deepcopy
 from functools import wraps
 from typing import (
     TYPE_CHECKING,
@@ -34,15 +31,19 @@
 
 from pyneo4j_ogm.exceptions import ListItemNotEncodable, UnregisteredModel
 from pyneo4j_ogm.fields.relationship_property import (
     RelationshipProperty,
     RelationshipPropertyCardinality,
     RelationshipPropertyDirection,
 )
-from pyneo4j_ogm.fields.settings import BaseModelSettings
+from pyneo4j_ogm.fields.settings import (
+    BaseModelSettings,
+    NodeModelSettings,
+    RelationshipModelSettings,
+)
 from pyneo4j_ogm.logger import logger
 from pyneo4j_ogm.pydantic_utils import (
     IS_PYDANTIC_V2,
     get_field_type,
     get_model_dump,
     get_model_fields,
     parse_model,
@@ -74,16 +75,17 @@
 DictStrAny = Dict[str, Any]
 AbstractSetIntStr = AbstractSet[int | str]
 IncEx = Optional[Union[Set[int], Set[str], Dict[int, Any], Dict[str, Any]]]
 
 
 def hooks(func):
     """
-    Decorator which runs defined pre- and post hooks for the decorated method. The decorator expects the
-    hooks to have the name of the decorated method. Both synchronous and asynchronous hooks are supported.
+    Calls all defined hooks for the decorated method. Pre-hooks are called before the method is executed and they
+    receive the same arguments as the decorated method. Post-hooks are called after the method is executed and they
+    receive the same arguments as a pre-hook, but with the result as the second argument.
 
     Args:
         func (Callable): The method to decorate.
 
     Returns:
         Callable: The decorated method.
     """
@@ -91,32 +93,41 @@
     if iscoroutinefunction(func):
 
         @wraps(func)
         async def async_wrapper(self, *args, **kwargs):
             settings: BaseModelSettings = getattr(self, "_settings")
 
             if func.__name__ in settings.pre_hooks:
-                logger.debug(
+                logger.info(
                     "Found %s pre-hook functions for method %s", len(settings.pre_hooks[func.__name__]), func.__name__
                 )
+
+                # Run each pre-hook function with the same arguments as the decorated method
                 for hook_function in settings.pre_hooks[func.__name__]:
                     logger.debug("Running pre-hook function %s", hook_function.__name__)
+
+                    # Check if the hook function is asynchronous, if so await it to prevent unawaited coroutine warnings
                     if iscoroutinefunction(hook_function):
                         await hook_function(self, *args, **kwargs)
                     else:
                         hook_function(self, *args, **kwargs)
 
             result = await func(self, *args, **kwargs)
 
             if func.__name__ in settings.post_hooks:
-                logger.debug(
+                logger.info(
                     "Found %s post-hook functions for method %s", len(settings.post_hooks[func.__name__]), func.__name__
                 )
+
+                # Run any post-hook functions with the same arguments as the decorated method and the result
+                # as the second argument
                 for hook_function in settings.post_hooks[func.__name__]:
                     logger.debug("Running post-hook function %s", hook_function.__name__)
+
+                    # Check again if the hook function is asynchronous and await it if necessary
                     if iscoroutinefunction(hook_function):
                         await hook_function(self, result, *args, **kwargs)
                     else:
                         hook_function(self, result, *args, **kwargs)
 
             return result
 
@@ -125,30 +136,36 @@
     else:
 
         @wraps(func)
         def sync_wrapper(self, *args, **kwargs):
             settings: BaseModelSettings = getattr(self, "_settings")
 
             if func.__name__ in settings.pre_hooks:
+                # Run each pre-hook function with the same arguments as the decorated method
                 logger.debug(
                     "Found %s pre-hook functions for method %s", len(settings.pre_hooks[func.__name__]), func.__name__
                 )
+
+                # Check if the hook function is asynchronous, if so create a new task to run it
                 for hook_function in settings.pre_hooks[func.__name__]:
                     logger.debug("Running pre-hook function %s", hook_function.__name__)
                     if iscoroutinefunction(hook_function):
                         asyncio.create_task(hook_function(self, *args, **kwargs))
                     else:
                         hook_function(self, *args, **kwargs)
 
             result = func(self, *args, **kwargs)
 
             if func.__name__ in settings.post_hooks:
+                # Run any post-hook functions with the same arguments as the decorated method and the result
                 logger.debug(
                     "Found %s post-hook functions for method %s", len(settings.post_hooks[func.__name__]), func.__name__
                 )
+
+                # Check again if the hook function is asynchronous and create a new task to run it if necessary
                 for hook_function in settings.post_hooks[func.__name__]:
                     logger.debug("Running post-hook function %s", hook_function.__name__)
                     if iscoroutinefunction(hook_function):
                         asyncio.create_task(hook_function(self, result, *args, **kwargs))
                     else:
                         hook_function(self, result, *args, **kwargs)
 
@@ -165,29 +182,34 @@
         and adds index and uniqueness constraint information to the generated schema.
         """
 
         def generate(self, *args, **kwargs):
             model_cls: Optional[Type[BaseModel]] = None
 
             if "definitions" in args[0]:
+                # If a `definitions` key is present, the JSON schema contains multiple schemas for multiple models
+                # We need to get the schema ref for the model we want to add the additional information to
                 schema_ref = args[0]["schema"]["schema_ref"]
 
                 for definition in args[0]["definitions"]:
                     if definition["ref"] == schema_ref and "cls" in definition:
                         model_cls = cast(Type[BaseModel], definition["cls"])
                         break
             elif "cls" in args[0]:
+                # If a `cls` key is present, the JSON schema only contains our current model
                 model_cls = cast(Type[BaseModel], args[0]["cls"])
 
             if model_cls is None:
                 raise PydanticSchemaGenerationError("Could not find model class in definitions")
 
             generated_schema = super().generate(*args, **kwargs)
 
             for field_name, field in get_model_fields(model_cls).items():
+                # Check all fields defined on the model, if we find a index or constraint field, add the information
+                # to the generated schema
                 point_index = getattr(get_field_type(field), "_point_index", False)
                 range_index = getattr(get_field_type(field), "_range_index", False)
                 text_index = getattr(get_field_type(field), "_text_index", False)
                 unique = getattr(get_field_type(field), "_unique", False)
 
                 if field_name not in generated_schema["properties"]:
                     continue
@@ -207,38 +229,44 @@
             if isinstance(dft, RelationshipProperty):
                 dft = str(dft)
             return super().encode_default(dft)
 
 
 class ModelBase(BaseModel, Generic[V]):
     """
-    Base class for both `NodeModel` and `RelationshipModel`. This class handles shared logic for both
-    model types like registering hooks and exporting/importing models to/from dictionaries.
+    Base class for both `NodeModel` and `RelationshipModel`. This class handles shared logic between the two model types
+    and defines common serializers/validators used for Pydantic models.
 
-    Should not be used directly.
+    If you come across this class and want to use it in your own models then DON'T. This class is not meant to be used
+    directly and is only used as a base class for `NodeModel` and `RelationshipModel`.
     """
 
-    _settings: BaseModelSettings = PrivateAttr()
+    _settings: Union[NodeModelSettings, RelationshipModelSettings] = PrivateAttr()
     _client: Pyneo4jClient = PrivateAttr()
     _query_builder: QueryBuilder = PrivateAttr()
     _db_properties: Dict[str, Any] = PrivateAttr(default={})
     _destroyed: bool = PrivateAttr(default=False)
     _element_id: Optional[str] = PrivateAttr(default=None)
     _id: Optional[int] = PrivateAttr(default=None)
     Settings: ClassVar[Type[BaseModelSettings]]
 
     if IS_PYDANTIC_V2:
 
         @model_serializer(mode="wrap")
         def _model_serializer(self, serializer: Any, info: SerializationInfo) -> Any:
+            """
+            Custom model serializer which adds support for serializing `RelationshipProperty` fields, `element_id` and
+            `id` fields and any additional fields defined on the model.
+            """
             if isinstance(self, RelationshipProperty):
                 return self.nodes
 
             serialized = serializer(self)
 
+            # If the field is not excluded and not `None`, add it to the serialized dictionary
             if not (self.id is None and info.exclude_none) and not (info.exclude is not None and "id" in info.exclude):
                 serialized["id"] = self.id
 
             if not (self.element_id is None and info.exclude_none) and not (
                 info.exclude is not None and "element_id" in info.exclude
             ):
                 serialized["element_id"] = self.element_id
@@ -269,24 +297,31 @@
                 and not (cast(RelationshipModel, self).end_node_id is None and info.exclude_none)
                 and not (info.exclude is not None and "end_node_id" in info.exclude)
             ):
                 serialized["end_node_id"] = cast(RelationshipModel, self)._end_node_id
 
             if hasattr(self, "_relationship_properties"):
                 for field_name in getattr(self, "_relationship_properties"):
+                    # If a relationship property has been found and it has fetched nodes, we add the nodes to
+                    # the serialized dictionary as well
                     if field_name in serialized:
                         serialized[field_name] = cast(RelationshipProperty, getattr(self, field_name)).nodes
 
             return serialized
 
         @model_validator(mode="before")  # type: ignore
         def _model_validator(cls, values: Any) -> Any:
+            """
+            Custom validation for validating the fetched nodes from a relationship property.
+            """
             relationship_properties = getattr(cls, "_relationship_properties", set())
 
             for field_name, field in get_model_fields(cls).items():
+                # Go over each relationship property field and try to build the relationship property for that
+                # field.
                 if (
                     field_name in relationship_properties
                     and field_name in values
                     and isinstance(values[field_name], list)
                 ):
                     field_default = cast(RelationshipProperty, field.default)
                     instance_copy = RelationshipProperty(
@@ -299,14 +334,16 @@
 
                     instance_copy._build_property(cls, field_name)
                     target_model = getattr(instance_copy, "_target_model", None)
 
                     if target_model is not None:
                         nodes: List[NodeModel] = []
 
+                        # Check if the nodes are of the correct model type and if they are alive
+                        # If so add them to the parsed instance
                         for node in values[field_name]:
                             if isinstance(node, target_model):
                                 nodes.append(node)
                                 continue
 
                             instance = target_model(**node)
                             if "element_id" in node:
@@ -330,14 +367,16 @@
     else:
 
         @root_validator(pre=True)
         def _parse_dict_fields(cls, values: Dict[str, Any]) -> Dict[str, Any]:
             relationship_properties = getattr(cls, "_relationship_properties", set())
 
             for field_name, field in get_model_fields(cls).items():
+                # Go over each relationship property field and try to build the relationship property for that
+                # field.
                 if (
                     field_name in relationship_properties
                     and field_name in values
                     and isinstance(values[field_name], list)
                 ):
                     field_default = cast(RelationshipProperty, field.default)
                     instance_copy = RelationshipProperty(
@@ -350,14 +389,16 @@
 
                     instance_copy._build_property(cls, field_name)
                     target_model = getattr(instance_copy, "_target_model", None)
 
                     if target_model is not None:
                         nodes: List[NodeModel] = []
 
+                        # Check if the nodes are of the correct model type and if they are alive
+                        # If so add them to the parsed instance
                         for node in values[field_name]:
                             if isinstance(node, target_model):
                                 nodes.append(node)
                                 continue
 
                             instance = target_model(**node)
                             if "element_id" in node:
@@ -383,28 +424,31 @@
             exclude_unset: bool = False,
             exclude_defaults: bool = False,
             exclude_none: bool = False,
         ) -> DictStrAny:
             excluded_fields = set()
             excluded_fields.update(exclude or set())
 
+            # Add all relationship properties to the list of excluded fields since we will handle them
+            # later on ourself
             if hasattr(self, "_relationship_properties"):
                 excluded_fields.update(cast(Set[str], getattr(self, "_relationship_properties")))
 
             # pylint: disable=unexpected-keyword-arg
             base_dict = super().dict(
                 include=include,
                 exclude=excluded_fields,
                 by_alias=by_alias,
                 skip_defaults=skip_defaults,  # type: ignore
                 exclude_unset=exclude_unset,
                 exclude_defaults=exclude_defaults,
                 exclude_none=exclude_none,
             )
 
+            # Add all `element_id` and `id` fields it they have not specifically been excluded
             if not (self._id is None and exclude_none) and not (exclude is not None and "id" in exclude):
                 base_dict["id"] = self._id
 
             if not (self._element_id is None and exclude_none) and not (
                 exclude is not None and "element_id" in exclude
             ):
                 base_dict["element_id"] = self._element_id
@@ -434,14 +478,16 @@
                 and not (cast(RelationshipModel, self).end_node_id is None and exclude_none)
                 and not (exclude is not None and "end_node_id" in exclude)
             ):
                 base_dict["end_node_id"] = cast(RelationshipModel, self)._end_node_id
 
             if hasattr(self, "_relationship_properties"):
                 for field_name in getattr(self, "_relationship_properties"):
+                    # Each relationship property gets the fetched nodes when serializing it rather than it's indexes
+                    # or constraints
                     field = cast(Union[RelationshipProperty, List], getattr(self, field_name))
 
                     if not isinstance(field, list) and not (exclude is not None and field_name in exclude):
                         base_dict[field_name] = [
                             cast(Union[RelationshipModel, NodeModel], node).dict() for node in field.nodes
                         ]
 
@@ -478,14 +524,16 @@
                 encoder=encoder,
                 models_as_dict=models_as_dict,
                 **dumps_kwargs,
             )
 
             modified_json = json.loads(base_json)
 
+            # Add all relationship properties to the list of excluded fields since we will handle them
+            # later on ourself
             if not (self._id is None and exclude_none) and not (exclude is not None and "id" in exclude):
                 modified_json["id"] = self._id
 
             if not (self._element_id is None and exclude_none) and not (
                 exclude is not None and "element_id" in exclude
             ):
                 modified_json["element_id"] = self._element_id
@@ -515,24 +563,29 @@
                 and not (cast(RelationshipModel, self).end_node_id is None and exclude_none)
                 and not (exclude is not None and "end_node_id" in exclude)
             ):
                 modified_json["end_node_id"] = cast(RelationshipModel, self)._end_node_id
 
             if hasattr(self, "_relationship_properties"):
                 for field_name in getattr(self, "_relationship_properties"):
+                    # Each relationship property gets the fetched nodes when serializing it rather than it's indexes
+                    # or constraints
                     field = cast(Union[RelationshipProperty, List], getattr(self, field_name))
 
                     if not isinstance(field, list) and not (exclude is not None and field_name in exclude):
+                        # Serialize and then deserialize each model to prevent double serialization when doing the whole
+                        # model at the end
                         modified_json[field_name] = [
                             json.loads(cast(Union[RelationshipModel, NodeModel], node).json()) for node in field.nodes
                         ]
 
             return json.dumps(modified_json)
 
     def __init__(self, *args, **kwargs) -> None:
+        # Check if the models has been registered with a client
         if not hasattr(self, "_client"):
             raise UnregisteredModel(model=self.__class__.__name__)
 
         super().__init__(*args, **kwargs)
 
     def __init_subclass__(cls, *args, **kwargs) -> None:
         setattr(cls, "_query_builder", QueryBuilder())
@@ -552,14 +605,16 @@
         if not IS_PYDANTIC_V2:
             for _, field in get_model_fields(cls).items():
                 point_index = getattr(get_field_type(field), "_point_index", False)
                 range_index = getattr(get_field_type(field), "_range_index", False)
                 text_index = getattr(get_field_type(field), "_text_index", False)
                 unique = getattr(get_field_type(field), "_unique", False)
 
+                # In Pydantic 2.x.x we need to add the index and constraint information to the field's
+                # `field_info.extra` attribute to make it available in the JSON schema
                 if point_index:
                     field.field_info.extra["point_index"] = True  # type: ignore
                 if range_index:
                     field.field_info.extra["range_index"] = True  # type: ignore
                 if text_index:
                     field.field_info.extra["text_index"] = True  # type: ignore
                 if unique:
@@ -603,29 +658,30 @@
         Args:
             hook_name (str): Name of the hook to register the function for.
             hook_functions (Union[List[Callable], Callable]): References of the functions to call if the hook is
                 triggered.
             overwrite (bool, optional): Whether to overwrite all defined hook functions if a new hooks function for
                 the same hook is registered. Defaults to `False`.
         """
+        logger.info("Registering pre-hook for %s", hook_name)
         valid_hook_functions: List[Callable] = []
 
-        logger.info("Registering pre-hook for %s", hook_name)
         # Normalize hooks to a list of functions
         if isinstance(hook_functions, list):
             for hook_function in hook_functions:
                 if callable(hook_function):
                     valid_hook_functions.append(hook_function)
         elif callable(hook_functions):
             valid_hook_functions.append(hook_functions)
 
         if hook_name not in cls._settings.pre_hooks:
             cls._settings.pre_hooks[hook_name] = []
 
         if overwrite:
+            # If `overwrite` is set to `True`, we overwrite all existing hook functions for the given hook
             logger.debug("Overwriting %s existing pre-hook functions", len(cls._settings.pre_hooks[hook_name]))
             cls._settings.pre_hooks[hook_name] = valid_hook_functions
         else:
             logger.debug("Adding %s pre-hook functions", len(valid_hook_functions))
             for hook_function in valid_hook_functions:
                 cls._settings.pre_hooks[hook_name].append(hook_function)
 
@@ -642,29 +698,30 @@
         Args:
             hook_name (str): Name of the hook to register the function for.
             hook_functions (Union[List[Callable], Callable]): References of the functions to call if the hook is
                 triggered.
             overwrite (bool, optional): Whether to overwrite all defined hook functions if a new hooks function for
                 the same hook is registered. Defaults to `False`.
         """
+        logger.info("Registering post-hook for %s", hook_name)
         valid_hook_functions: List[Callable] = []
 
-        logger.info("Registering post-hook for %s", hook_name)
         # Normalize hooks to a list of functions
         if isinstance(hook_functions, list):
             for hook_function in hook_functions:
                 if callable(hook_function):
                     valid_hook_functions.append(hook_function)
         elif callable(hook_functions):
             valid_hook_functions.append(hook_functions)
 
         if hook_name not in cls._settings.post_hooks:
             cls._settings.post_hooks[hook_name] = []
 
         if overwrite:
+            # If `overwrite` is set to `True`, we overwrite all existing hook functions for the given hook
             logger.debug("Overwriting %s existing post-hook functions", len(cls._settings.post_hooks[hook_name]))
             cls._settings.post_hooks[hook_name] = valid_hook_functions
         else:
             logger.debug("Adding %s post-hook functions", len(valid_hook_functions))
             for hook_function in valid_hook_functions:
                 cls._settings.post_hooks[hook_name].append(hook_function)
 
@@ -728,19 +785,21 @@
             deflated (Dict[str, Any]): The model to deflate.
 
         Returns:
             Dict[str, Any]: The model model.
         """
         logger.debug("Deflating model %s to storable dictionary", self)
 
-        # Serialize nested BaseModel or dict instances to JSON strings
         for field_name, field in deepcopy(deflated).items():
             if isinstance(field, (dict, BaseModel)):
+                # If the field is a dictionary or a Pydantic model, we deflate it by serializing it to a JSON string
                 deflated[field_name] = json.dumps(field)
             elif isinstance(field, list):
+                # If the field is a list, we deflate it by serializing each item to a JSON string
+                # This adds the constraint that all items in the list must be encodable to a JSON string
                 for index, item in enumerate(field):
                     if not isinstance(item, (int, float, str, bool)):
                         try:
                             deflated[field_name][index] = json.dumps(item)
                         except TypeError as exc:
                             raise ListItemNotEncodable from exc
 
@@ -766,15 +825,19 @@
             try:
                 return json.loads(property_value)
             except:
                 return property_value
 
         logger.debug("Inflating node %s to model instance", graph_entity)
         for node_property in graph_entity.items():
+            # Inflate each property of the node
+            # If the property is a JSON string, we try to parse it to a dictionary. If the parsing fails, we know
+            # that the property is a string and we can use it as is
             property_name, property_value = node_property
+            logger.debug("Inflating property %s with value %s", property_name, property_value)
 
             if isinstance(property_value, str):
                 inflated[property_name] = try_property_parsing(property_value)
             elif isinstance(property_value, list):
                 inflated[property_name] = [
                     try_property_parsing(item) if isinstance(item, str) else item for item in property_value
                 ]
@@ -826,15 +889,11 @@
             "validate_default": True,
             "validate_assignment": True,
             "revalidate_instances": "always",
         }
     else:
 
         class Config:
-            """
-            Pydantic configuration options.
-            """
-
             validate_all = True
             validate_assignment = True
             revalidate_instances = "always"
             underscore_attrs_are_private = True
```

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/core/client.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """
 Pyneo4j database client class for running operations on the database.
 """
+
 import os
 from enum import Enum
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union, cast
 
 from neo4j import AsyncDriver, AsyncGraphDatabase, AsyncSession, AsyncTransaction
 from neo4j.exceptions import DatabaseError
 from neo4j.graph import Node, Path, Relationship
 from typing_extensions import LiteralString
 
 from pyneo4j_ogm.core.node import NodeModel
 from pyneo4j_ogm.core.relationship import RelationshipModel
 from pyneo4j_ogm.exceptions import (
+    AlreadyRegistered,
     InvalidBookmark,
     InvalidEntityType,
     InvalidLabelOrType,
     MissingDatabaseURI,
     NotConnectedToDatabase,
     TransactionInProgress,
     UnsupportedNeo4jVersion,
 )
+from pyneo4j_ogm.fields.settings import NodeModelSettings, RelationshipModelSettings
 from pyneo4j_ogm.logger import logger
 from pyneo4j_ogm.pydantic_utils import get_field_type, get_model_fields
 from pyneo4j_ogm.queries.query_builder import QueryBuilder
 
 
 class EntityType(str, Enum):
     """
@@ -119,14 +122,15 @@
         self.uri = db_uri
         self._skip_constraints = skip_constraints
         self._skip_indexes = skip_indexes
 
         logger.debug("Connecting to database %s", self.uri)
         self._driver = AsyncGraphDatabase.driver(uri=self.uri, *args, **kwargs)
 
+        # Get server info to check the Neo4j version since versions prior to 5 are not tested yet
         logger.debug("Checking if neo4j version is supported")
         server_info = await self._driver.get_server_info()
 
         version = server_info.agent.split("/")[1]
 
         if int(version.split(".")[0]) < 5:
             raise UnsupportedNeo4jVersion()
@@ -145,35 +149,57 @@
 
         Args:
             models (List[Type[NodeModel | RelationshipModel]]): A list of models to register.
         """
         logger.info("Registering models %s with client %s", models, self)
 
         for model in models:
+            for registered_model in self.models:
+                registered_model_settings = registered_model.model_settings()
+                model_settings = model.model_settings()
+
+                if (
+                    isinstance(registered_model_settings, RelationshipModelSettings)
+                    and isinstance(model_settings, RelationshipModelSettings)
+                    and registered_model_settings.type == model_settings.type
+                ):
+                    raise AlreadyRegistered(cast(str, model_settings.type))
+                elif (
+                    isinstance(registered_model_settings, NodeModelSettings)
+                    and isinstance(model_settings, NodeModelSettings)
+                    and set(registered_model_settings.labels) == set(model_settings.labels)
+                ):
+                    raise AlreadyRegistered(cast(str, model_settings.labels))
+
             if issubclass(model, (NodeModel, RelationshipModel)):
+                logger.debug("Found valid mode %s, registering with client", model.__name__)
+
+                # If the model is a valid model, add it to the set of models stored by the client
                 self.models.add(model)
                 setattr(model, "_client", self)
 
                 for property_name, property_definition in get_model_fields(model).items():
                     entity_type = EntityType.NODE if issubclass(model, NodeModel) else EntityType.RELATIONSHIP
                     labels_or_type = (
                         list(getattr(model._settings, "labels"))
                         if issubclass(model, NodeModel)
                         else getattr(model._settings, "type")
                     )
 
+                    # Check if we need to create any constraints
                     if not self._skip_constraints:
                         if getattr(get_field_type(property_definition), "_unique", False):
                             await self.create_uniqueness_constraint(
                                 name=model.__name__,
                                 entity_type=entity_type,
                                 properties=[property_name],
                                 labels_or_type=labels_or_type,
                             )
 
+                    # Check if we need to create any indexes
                     if not self._skip_indexes:
                         if getattr(get_field_type(property_definition), "_range_index", False):
                             await self.create_range_index(
                                 name=model.__name__,
                                 entity_type=entity_type,
                                 properties=[property_name],
                                 labels_or_type=labels_or_type,
@@ -227,44 +253,51 @@
                 of the returned variables.
         """
         if parameters is None:
             parameters = {}
 
         logger.debug("Checking for open transaction")
         if getattr(self, "_session", None) is None or getattr(self, "_transaction", None) is None:
+            # Begin a new transaction if none is open
             await self._begin_transaction()
 
         try:
             parameters = parameters if parameters is not None else {}
 
+            # Run the query and get the results and result keys used in the query
             logger.debug("Running query \n%s \nwith parameters %s", query, parameters)
             result_data = await cast(AsyncTransaction, self._transaction).run(
                 query=cast(LiteralString, query), parameters=parameters
             )
 
             results = [list(r.values()) async for r in result_data]
             meta = list(result_data.keys())
 
             if resolve_models:
+                # If model resolution has been enabled, try to resolve the query results
+                # If this fails, the raw result will be returned instead
                 logger.debug("`resolve_models` is set to True, trying to resolve query results")
                 for list_index, result_list in enumerate(results):
                     for result_index, result in enumerate(result_list):
                         resolved = self._resolve_database_model(result)
 
                         if resolved is not None:
                             results[list_index][result_index] = resolved
 
             if self._batch_enabled is False:
+                # If batching is enabled, we don't want to commit the transaction yet as
+                # we might have more queries to run
                 logger.debug("No batching enabled, committing transaction")
                 await self._commit_transaction()
 
             return results, meta
         except Exception as exc:
             logger.error("Error running query %s", exc)
             if self._batch_enabled is False:
+                # The same goes for rolling back the transaction when batching is enabled
                 await self._rollback_transaction()
 
             raise exc
 
     @ensure_connection
     async def create_uniqueness_constraint(
         self,
@@ -654,46 +687,44 @@
 
     @ensure_connection
     async def _commit_transaction(self) -> None:
         """
         Commits the currently active transaction and closes it.
         """
         logger.debug("Committing transaction %s", self._transaction)
-        try:
-            await cast(AsyncTransaction, self._transaction).commit()  # type: ignore
-            bookmarks = await cast(AsyncSession, self._session).last_bookmarks()
-            self.last_bookmarks = set(bookmarks.raw_values)
-        finally:
-            self._session = None
-            self._transaction = None
+        await cast(AsyncTransaction, self._transaction).commit()  # type: ignore
+        bookmarks = await cast(AsyncSession, self._session).last_bookmarks()
+        self.last_bookmarks = set(bookmarks.raw_values)
+
+        self._session = None
+        self._transaction = None
 
     @ensure_connection
     async def _rollback_transaction(self) -> None:
         """
         Rolls back the currently active transaction and closes it.
         """
         logger.debug("Rolling back transaction %s", self._transaction)
-        try:
-            await cast(AsyncTransaction, self._transaction).rollback()  # type: ignore
-        finally:
-            self._session = None
-            self._transaction = None
+        await cast(AsyncTransaction, self._transaction).rollback()  # type: ignore
+        self._session = None
+        self._transaction = None
 
     def _resolve_database_model(self, query_result: Any) -> Optional[Any]:
         """
         Resolves a query result to the corresponding database model, if one is registered.
 
         Args:
             query_result (Any): The query result to try to resolve.
 
         Returns:
             Optional[Any]: The database model, if one is registered. If a path is the result, returns the `Path` class
                 with `Path.nodes` and `Path.relationships` resolved to the database models.
         """
         if isinstance(query_result, Path):
+            # If the result is a path, resolve the nodes and relationships inside the path
             logger.debug("Query result %s is a path, resolving nodes and relationship", query_result)
             nodes = []
             relationships = []
 
             logger.debug("Resolving nodes")
             for node in query_result.nodes:
                 resolved = self._resolve_database_model(node)
@@ -705,14 +736,15 @@
                 relationships.append(resolved if resolved is not None else relationship)
 
             setattr(query_result, "_nodes", tuple(nodes))
             setattr(query_result, "_relationships", tuple(relationships))
 
             return query_result
         elif isinstance(query_result, (Node, Relationship)):
+            # Get type or labels and try to resolve the query result to a registered model
             logger.debug("Query result %s is a node or relationship, resolving", query_result)
             labels = set(query_result.labels) if isinstance(query_result, Node) else {query_result.type}
 
             for model in list(self.models):
                 model_labels: set[str] = set()
 
                 if issubclass(model, NodeModel):
```

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/core/node.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Holds the base node class `NodeModel` which is used to define database models for nodes.
 It provides base functionality like de-/inflation, validation and methods for interacting with
 the database for CRUD operations on nodes.
 """
+
 import json
 from copy import deepcopy
 from functools import wraps
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
@@ -95,15 +96,15 @@
     model.
 
     Provides methods for interacting with the database for CRUD operations on nodes. Settings can
     be defined by providing an inner class `Settings`. Settings can control the behavior of the
     model and are defined in `pyneo4j_ogm.fields.settings.NodeModelSettings`.
     """
 
-    _settings: NodeModelSettings
+    _settings: NodeModelSettings = PrivateAttr()
     _relationship_properties: Set[str] = PrivateAttr()
     Settings: ClassVar[Type[NodeModelSettings]]
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         # Build relationship properties
@@ -191,14 +192,16 @@
             parameters=deflated_properties,
         )
 
         logger.debug("Checking if query returned a result")
         if len(results) == 0 or len(results[0]) == 0 or results[0][0] is None:
             raise UnexpectedEmptyResult()
 
+        # Since the instance is now hydrated, we can set the element id and id and reset the modified properties
+        # to the current instance values
         logger.debug("Hydrating instance values")
         setattr(self, "_element_id", getattr(cast(T, results[0][0]), "_element_id"))
         setattr(self, "_id", getattr(cast(T, results[0][0]), "_id"))
 
         logger.debug("Resetting modified properties")
         self._db_properties = get_model_dump(self, exclude={*self._relationship_properties, "element_id", "id"})
         logger.debug("Created new node %s", self)
@@ -225,14 +228,16 @@
             [
                 f"n.{property_name} = ${property_name}"
                 for property_name in deflated
                 if property_name in self.modified_properties
             ]
         )
 
+        # We return the updated node to check if the query was successful
+        # since Neo4j does not raise any exceptions if the node does not exist
         results, _ = await self._client.cypher(
             query=f"""
                 MATCH {self._query_builder.node_match(list(self._settings.labels))}
                 WHERE elementId(n) = $element_id
                 {f"SET {set_query}" if set_query != "" else ""}
                 RETURN n
             """,
@@ -264,14 +269,15 @@
                 WHERE elementId(n) = $element_id
                 DETACH DELETE n
                 RETURN count(n)
             """,
             parameters={"element_id": self._element_id},
         )
 
+        # If the returned value is empty, the node does not exist and the query failed
         logger.debug("Checking if query returned a result")
         if len(results) == 0 or len(results[0]) == 0 or results[0][0] is None:
             raise UnexpectedEmptyResult()
 
         logger.debug("Marking instance as destroyed")
         setattr(self, "_destroyed", True)
         logger.debug("Deleted node %s", self)
@@ -291,14 +297,16 @@
                 MATCH {self._query_builder.node_match(list(self._settings.labels))}
                 WHERE elementId(n) = $element_id
                 RETURN n
             """,
             parameters={"element_id": self._element_id},
         )
 
+        # If the returned value is empty, we can not refresh the instance
+        # since the node does not exist anymore
         logger.debug("Checking if query returned a result")
         if len(results) == 0 or len(results[0]) == 0 or results[0][0] is None:
             raise UnexpectedEmptyResult()
 
         logger.debug("Updating current instance")
         self.__dict__.update(results[0][0].__dict__)
         logger.debug("Refreshed node %s", self)
@@ -359,20 +367,24 @@
         )
 
         if auto_fetch_nodes or (auto_fetch_nodes is not False and self._settings.auto_fetch_nodes):
             logger.debug("Auto-fetching nodes is enabled, checking if model with target labels is registered")
             if "$node" not in filters or "$labels" not in filters["$node"]:
                 raise InvalidFilters()
 
-            labels = cast(List[str], filters["$node"]["$labels"])
+            labels = set(filters["$node"]["$labels"])
 
             # Get target node model from the models registered with the client
             # If no model is found, someone forgot to register it
             for model in self._client.models:
-                if hasattr(model._settings, "labels") and list(getattr(model._settings, "labels", [])) == labels:
+                if not issubclass(model, NodeModel):
+                    continue
+
+                model_labels = set(getattr(model._settings, "labels", []))
+                if not model_labels.difference(labels):
                     target_node_model = cast("NodeModel", model)
                     break
 
             if target_node_model is None:
                 raise UnregisteredModel(f"with labels {labels}")
 
             logger.debug("Model with labels %s is registered, building auto-fetch query", labels)
@@ -511,14 +523,15 @@
                 projections is None,
                 auto_fetch_nodes or (auto_fetch_nodes is not False and cls._settings.auto_fetch_nodes),
                 cls._query_builder.query["projections"] == "",
             ]
         )
 
         if do_auto_fetch:
+            # If auto-fetch is enabled, we need to build the auto-fetch queries in addition to the normal query
             logger.debug("Querying database with auto-fetch enabled")
             projection_query = (
                 "RETURN n" if cls._query_builder.query["projections"] == "" else cls._query_builder.query["projections"]
             )
             match_queries, return_queries = cls._build_auto_fetch(nodes_to_fetch=auto_fetch_models)
 
             results, meta = await cls._client.cypher(
@@ -553,18 +566,20 @@
         logger.debug("Checking if query returned a result")
         if (
             len(results) == 0
             or len(results[0]) == 0
             or results[0][0] is None
             or (isinstance(results[0][0], dict) and len(results[0][0]) == 0)
         ):
+            # If no results are found, we return None or raise an exception
             if raise_on_empty:
                 raise NoResultFound(filters)
             return None
 
+        # Normalize results to a single instance
         if isinstance(results[0][0], Node):
             instance = cls._inflate(graph_entity=results[0][0])
         elif isinstance(results[0][0], list):
             instance = results[0][0][0]
         else:
             instance = results[0][0]
```

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/core/relationship.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/core/relationship.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Holds the base relationship class `RelationshipModel` which is used to define database models for
 relationships. It provides base functionality like de-/inflation and validation and methods for interacting with
 the database for CRUD operations on relationships.
 """
+
 import json
 import re
 from functools import wraps
 from typing import Any, ClassVar, Dict, List, Optional, Type, TypeVar, Union, cast
 
 from neo4j.graph import Node, Relationship
 from pydantic import PrivateAttr
@@ -79,15 +80,15 @@
     functionality like de-/inflation and validation.
 
     Provides methods for interacting with the database for CRUD operations on relationships. Settings can be defined
     by the inner class `Settings`. Settings control the behavior of the model and are defined in
     `pyneo4j_ogm.fields.settings.RelationshipModelSettings`.
     """
 
-    _settings: RelationshipModelSettings
+    _settings: RelationshipModelSettings = PrivateAttr()
     _start_node_element_id: Optional[str] = PrivateAttr(default=None)
     _start_node_id: Optional[int] = PrivateAttr(default=None)
     _end_node_element_id: Optional[str] = PrivateAttr(default=None)
     _end_node_id: Optional[int] = PrivateAttr(default=None)
     Settings: ClassVar[Type[RelationshipModelSettings]]
 
     def __init__(self, *args, **kwargs) -> None:
@@ -423,14 +424,15 @@
                 WITH DISTINCT r
                 {cls._query_builder.query['options']}
                 {projection_query}
             """,
             parameters=cls._query_builder.parameters,
         )
 
+        # Normalize results to instance classes
         logger.debug("Building instances from query results")
         for result_list in results:
             for result in result_list:
                 if result is None:
                     continue
 
                 if isinstance(result, Relationship):
```

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/exceptions.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
-Pyneo4j exceptions raised by the client or model classes.
+Exceptions module for Pyneo4j OGM.
 """
-from typing import Any, List
+
+from typing import Any, List, Set, Union
 
 
 class Pyneo4jException(Exception):
     """
-    Base exception for all Pyneo4j exceptions
+    Base exception for all Pyneo4j exceptions.
     """
 
 
 class NotConnectedToDatabase(Pyneo4jException):
     """
     A client tried to run a query without being connected to a database.
     """
@@ -210,7 +211,18 @@
 class ListItemNotEncodable(Pyneo4jException):
     """
     A list item is not JSON encodable and can thus not be stored.
     """
 
     def __init__(self, *args: object) -> None:
         super().__init__("List item is not JSON encodable and can not be stored inside the database", *args)
+
+
+class AlreadyRegistered(Pyneo4jException):
+    """
+    Multiple models are using the same labels/type as a already registered model.
+    """
+
+    def __init__(self, labels_or_type: Union[Set[str], str], *args: object) -> None:
+        received = f"[{', '.join(labels_or_type)}]" if isinstance(labels_or_type, set) else f"[{labels_or_type}]"
+        label_or_type = "labels" if isinstance(labels_or_type, set) else "type"
+        super().__init__(f"A model is using the same {label_or_type} as another model. Got {received}", *args)
```

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/fields/property_options.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/fields/property_options.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/fields/relationship_property.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/fields/relationship_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """
 Relationship property class used to define relationships between the model this class is used on and a target model,
 which defines the other end of the relationship.
 """
 
-# pyright: reportUnboundVariable=false
-
 import asyncio
 from asyncio import iscoroutinefunction
 from enum import Enum
 from functools import wraps
 from typing import (
     TYPE_CHECKING,
     Any,
```

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/fields/settings.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/fields/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """
 Settings for model classes.
 """
 
-# pyright: reportUnboundVariable=false
-
 from typing import Callable, Dict, List, Optional, Set, Union
 
 from pydantic import BaseModel
 from pydantic.class_validators import validator
 
 from pyneo4j_ogm.pydantic_utils import IS_PYDANTIC_V2
```

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/logger.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Logging configuration for pyneo4j-ogm
+Logging module.
 
 Logging is controlled by two environment variables:
 - PYNEO4J_OGM_LOG_LEVEL: the log level to use. Defaults to `WARNING`.
 - PYNEO4J_OGM_ENABLE_LOGGING: whether to enable logging. Defaults to `True`.
 """
 import logging
 from os import environ
```

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/actions/create.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/create.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/actions/down.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/down.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,22 +31,25 @@
     logger.info("Rolling back %s migrations", down_count)
     async with MigrationClient(config) as migration_client:
         migration_files = get_migration_files(config.migration_dir)
         migration_node = await migration_client.get_migration_node()
 
         logger.debug("Filtering migration files for applied migrations")
         applied_migration_identifiers = migration_node.get_applied_migration_identifiers
+        # Remove all migration files that have not been applied
         for identifier in deepcopy(migration_files).keys():
             if identifier not in applied_migration_identifiers:
                 migration_files.pop(identifier, None)
 
         for count, _ in enumerate(deepcopy(migration_files).values()):
             if down_count != "all" and count >= down_count:
                 break
 
+            # We can get the current migration by getting the max identifier, which is a
+            # UNIX timestamp meaning the highest value is the most recent migration
             current_migration_identifier = max(migration_files.keys())
             current_migration = migration_files[current_migration_identifier]
 
             logger.debug("Rolling back migration %s", current_migration["name"])
             await current_migration["down"](migration_client.client)
             migration_files.pop(current_migration_identifier)
             migration_node.applied_migrations = [
```

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/actions/init.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/init.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/actions/status.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/status.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/actions/up.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/actions/up.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         for applied_migration in migration_node.get_applied_migration_identifiers:
             migration_files.pop(applied_migration, None)
 
         for count, _ in enumerate(deepcopy(migration_files).values()):
             if up_count != "all" and count >= up_count:
                 break
 
+            # Since the migration files are sorted by identifier, we can get the current migration
+            # by getting the min identifier, which is a UNIX timestamp meaning the lowest value is the oldest migration
             current_migration_identifier = min(migration_files.keys())
             current_migration = migration_files[current_migration_identifier]
 
             logger.debug("Applying migration %s", current_migration["name"])
             await current_migration["up"](migration_client.client)
             migration_files.pop(current_migration_identifier)
             migration_node.applied_migrations.append(AppliedMigration(name=current_migration["name"]))
```

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/cli.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/cli.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/utils/client.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/client.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/utils/defaults.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/utils/migration.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/migration.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/migrations/utils/models.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/migrations/utils/models.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/pydantic_utils.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/pydantic_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """
-Utility functions for staying compatible with Pydantic V1 and V2
+Pydantic compatibility utility module.
 """
 
-# pyright: reportUnboundVariable=false
-
 from typing import Any, Type, Union
 
 import pydantic
 from pydantic import BaseModel
 
 IS_PYDANTIC_V2 = int(pydantic.VERSION.split(".", maxsplit=1)[0]) >= 2
```

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/queries/operators.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/operators.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/queries/query_builder.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/query_builder.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/queries/types.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/types.py`

 * *Files identical despite different names*

### Comparing `pyneo4j_ogm-0.5.2/pyneo4j_ogm/queries/validators.py` & `pyneo4j_ogm-0.5.3/pyneo4j_ogm/queries/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Pydantic validators for query operators and filters.
 """
 
-# pyright: reportUnboundVariable=false
 # pylint: disable=unused-argument
 
 from typing import Any, Dict, List, Literal, Optional, Type, Union
 
 from pydantic import BaseModel, Field, ValidationError
 
 from pyneo4j_ogm.logger import logger
```

