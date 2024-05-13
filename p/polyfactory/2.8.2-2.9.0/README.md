# Comparing `tmp/polyfactory-2.8.2.tar.gz` & `tmp/polyfactory-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.8.2.tar", max compression
+gzip compressed data, was "polyfactory-2.9.0.tar", max compression
```

## Comparing `polyfactory-2.8.2.tar` & `polyfactory-2.9.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1092 2023-09-16 02:56:34.460504 polyfactory-2.8.2/LICENSE
--rw-r--r--   0        0        0    24136 2023-09-16 02:56:34.460504 polyfactory-2.8.2/docs/PYPI_README.md
--rw-r--r--   0        0        0      425 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/__init__.py
--rw-r--r--   0        0        0     2525 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/collection_extender.py
--rw-r--r--   0        0        0      912 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0     2147 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/factories/attrs_factory.py
--rw-r--r--   0        0        0    34575 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2758 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1912 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     2751 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/factories/msgspec_factory.py
--rw-r--r--   0        0        0     2192 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0    15976 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1699 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     8689 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3317 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/fields.py
--rw-r--r--   0        0        0     1192 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/py.typed
--rw-r--r--   0        0        0     2850 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     3885 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     4097 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     1948 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     3048 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1125 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13429 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0      433 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/value_generators/constrained_path.py
--rw-r--r--   0        0        0     3846 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0      440 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/value_generators/constrained_url.py
--rw-r--r--   0        0        0      446 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/value_generators/constrained_uuid.py
--rw-r--r--   0        0        0     3678 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6172 2023-09-16 02:56:34.464504 polyfactory-2.8.2/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6647 2023-09-16 02:56:34.464504 polyfactory-2.8.2/pyproject.toml
--rw-r--r--   0        0        0    26144 1970-01-01 00:00:00.000000 polyfactory-2.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-09-19 03:09:22.334563 polyfactory-2.9.0/LICENSE
+-rw-r--r--   0        0        0    24136 2023-09-19 03:09:22.334563 polyfactory-2.9.0/docs/PYPI_README.md
+-rw-r--r--   0        0        0      425 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/__init__.py
+-rw-r--r--   0        0        0     2525 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/collection_extender.py
+-rw-r--r--   0        0        0      912 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0     2622 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/factories/attrs_factory.py
+-rw-r--r--   0        0        0    34783 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2758 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     2254 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     2751 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/factories/msgspec_factory.py
+-rw-r--r--   0        0        0     2192 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0    15976 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     7194 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/factories/sqlalchemy_factory.py
+-rw-r--r--   0        0        0     1699 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     8689 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3329 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/fields.py
+-rw-r--r--   0        0        0     1192 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/py.typed
+-rw-r--r--   0        0        0     2850 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     4221 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     4097 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     1948 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     3048 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1125 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13429 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0      433 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/value_generators/constrained_path.py
+-rw-r--r--   0        0        0     3846 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0      440 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/value_generators/constrained_url.py
+-rw-r--r--   0        0        0      446 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/value_generators/constrained_uuid.py
+-rw-r--r--   0        0        0     3678 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6172 2023-09-19 03:09:22.338563 polyfactory-2.9.0/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6868 2023-09-19 03:09:22.338563 polyfactory-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0    26264 1970-01-01 00:00:00.000000 polyfactory-2.9.0/PKG-INFO
```

### Comparing `polyfactory-2.8.2/LICENSE` & `polyfactory-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/docs/PYPI_README.md` & `polyfactory-2.9.0/docs/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/collection_extender.py` & `polyfactory-2.9.0/polyfactory/collection_extender.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/constants.py` & `polyfactory-2.9.0/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/decorators.py` & `polyfactory-2.9.0/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/exceptions.py` & `polyfactory-2.9.0/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/factories/attrs_factory.py` & `polyfactory-2.9.0/polyfactory/factories/msgspec_factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,82 @@
 from __future__ import annotations
 
 from inspect import isclass
-from typing import TYPE_CHECKING, TypeVar
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Generic,
+    TypeVar,
+    cast,
+)
+
+from typing_extensions import get_type_hints
 
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.base import BaseFactory
 from polyfactory.field_meta import FieldMeta, Null
+from polyfactory.value_generators.constrained_numbers import handle_constrained_int
+from polyfactory.value_generators.primitives import create_random_bytes
 
 if TYPE_CHECKING:
-    from typing import Any, TypeGuard
-
+    from typing_extensions import TypeGuard
 
 try:
-    import attrs
-    from attr._make import Factory
-except ImportError as ex:
-    raise MissingDependencyException("attrs is not installed") from ex
+    import msgspec
+    from msgspec import inspect
+except ImportError as e:
+    raise MissingDependencyException("msgspec is not installed") from e
 
-T = TypeVar("T", bound=attrs.AttrsInstance)
+T = TypeVar("T", bound=msgspec.Struct)
 
 
-class AttrsFactory(BaseFactory[T]):
-    """Base factory for attrs classes."""
+class MsgspecFactory(Generic[T], BaseFactory[T]):
+    """Base factory for msgspec Structs."""
 
     __is_base_factory__ = True
 
     @classmethod
+    def get_provider_map(cls) -> dict[Any, Callable[[], Any]]:
+        def get_msgpack_ext() -> msgspec.msgpack.Ext:
+            code = handle_constrained_int(cls.__random__, ge=-128, le=127)
+            data = create_random_bytes(cls.__random__)
+            return msgspec.msgpack.Ext(code, data)
+
+        msgspec_provider_map = {msgspec.UnsetType: lambda: msgspec.UNSET, msgspec.msgpack.Ext: get_msgpack_ext}
+
+        provider_map = super().get_provider_map()
+        provider_map.update(msgspec_provider_map)
+
+        return provider_map
+
+    @classmethod
     def is_supported_type(cls, value: Any) -> TypeGuard[type[T]]:
-        return isclass(value) and hasattr(value, "__attrs_attrs__")
+        return isclass(value) and hasattr(value, "__struct_fields__")
 
     @classmethod
     def get_model_fields(cls) -> list[FieldMeta]:
-        field_metas: list[FieldMeta] = []
-        fields = attrs.fields(cls.__model__)
-        none_type = type(None)
-
-        for field in fields:
-            annotation = none_type if field.type is None else field.type
-
-            default = field.default
-            if isinstance(default, Factory):
-                # The default value is not currently being used when generating
-                # the field values. When that is implemented, this would need
-                # to be handled differently since the `default.factory` could
-                # take a `self` argument.
-                default_value = default.factory
-            elif default is None:
-                default_value = Null
+        type_info = cast(inspect.StructType, inspect.type_info(cls.__model__))
+
+        fields_meta: list[FieldMeta] = []
+
+        for field in type_info.fields:
+            annotation = get_type_hints(cls.__model__, include_extras=True)[field.name]
+            if field.default is not msgspec.NODEFAULT:
+                default_value = field.default
+            elif field.default_factory is not msgspec.NODEFAULT:
+                default_value = field.default_factory()
             else:
-                default_value = default
+                default_value = Null
 
-            field_metas.append(
+            fields_meta.append(
                 FieldMeta.from_type(
                     annotation=annotation,
-                    name=field.alias,
+                    name=field.name,
                     default=default_value,
                     random=cls.__random__,
                     randomize_collection_length=cls.__randomize_collection_length__,
                     min_collection_length=cls.__min_collection_length__,
                     max_collection_length=cls.__max_collection_length__,
                 )
             )
-
-        return field_metas
+        return fields_meta
```

### Comparing `polyfactory-2.8.2/polyfactory/factories/base.py` & `polyfactory-2.9.0/polyfactory/factories/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,15 @@
     except ImportError:
         mapping = {}
 
     return mapping
 
 
 T = TypeVar("T")
+F = TypeVar("F", bound="BaseFactory[Any]")
 
 
 class BaseFactory(ABC, Generic[T]):
     """Base Factory class - this class holds the main logic of the library"""
 
     # configuration attributes
     __model__: type[T]
@@ -483,30 +484,30 @@
             abc.Callable: _create_generic_fn,
             Counter: lambda: Counter(cls.__faker__.pystr()),
             **_create_pydantic_type_map(cls),
         }
 
     @classmethod
     def create_factory(
-        cls,
-        model: type,
+        cls: type[F],
+        model: type[T],
         bases: tuple[type[BaseFactory[Any]], ...] | None = None,
         **kwargs: Any,
-    ) -> type[BaseFactory[Any]]:
+    ) -> type[F]:
         """Generate a factory for the given type dynamically.
 
         :param model: A type to model.
         :param bases: Base classes to use when generating the new class.
         :param kwargs: Any kwargs.
 
         :returns: A 'ModelFactory' subclass.
 
         """
         return cast(
-            "Type[BaseFactory[Any]]",
+            "Type[F]",
             type(
                 f"{model.__name__}Factory",
                 (*(bases or ()), cls),
                 {"__model__": model, **kwargs},
             ),
         )
 
@@ -844,15 +845,17 @@
     import polyfactory.factories.typed_dict_factory  # noqa: F401
 
     for module in [
         "polyfactory.factories.pydantic_factory",
         "polyfactory.factories.beanie_odm_factory",
         "polyfactory.factories.odmantic_odm_factory",
         "polyfactory.factories.msgspec_factory",
-        "polyfactory.factories.attrs_factory",
+        # `AttrsFactory` is not being registered by default since not all versions of `attrs` are supported.
+        # Issue: https://github.com/litestar-org/polyfactory/issues/356
+        # "polyfactory.factories.attrs_factory",
     ]:
         try:
             import_module(module)
         except ImportError:
             continue
```

### Comparing `polyfactory-2.8.2/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.9.0/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.9.0/polyfactory/factories/dataclass_factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 from dataclasses import MISSING, fields, is_dataclass
-from typing import Any, Generic
-
-from typing_extensions import TypeGuard, get_type_hints
+from typing import TYPE_CHECKING, Any, ForwardRef, Generic
 
 from polyfactory.factories.base import BaseFactory, T
 from polyfactory.field_meta import FieldMeta, Null
+from polyfactory.utils.helpers import evaluate_forwardref
+
+if TYPE_CHECKING:
+    from typing_extensions import TypeGuard
 
 
 class DataclassFactory(Generic[T], BaseFactory[T]):
     """Dataclass base factory"""
 
     __is_base_factory__ = True
 
@@ -29,27 +31,32 @@
 
 
         :returns: A list of field MetaData instances.
 
         """
         fields_meta: list["FieldMeta"] = []
 
-        model_type_hints = get_type_hints(cls.__model__, include_extras=True)
-
         for field in fields(cls.__model__):  # type: ignore[arg-type]
             if field.default_factory and field.default_factory is not MISSING:
                 default_value = field.default_factory()
             elif field.default is not MISSING:
                 default_value = field.default
             else:
                 default_value = Null
 
+            if isinstance(field.type, ForwardRef):
+                annotation = evaluate_forwardref(field.type)  # type: ignore[unreachable]
+            elif isinstance(field.type, str):
+                annotation = evaluate_forwardref(ForwardRef(field.type))  # type: ignore[unreachable]
+            else:
+                annotation = field.type
+
             fields_meta.append(
                 FieldMeta.from_type(
-                    annotation=model_type_hints[field.name],
+                    annotation=annotation,
                     name=field.name,
                     default=default_value,
                     random=cls.__random__,
                     randomize_collection_length=cls.__randomize_collection_length__,
                     min_collection_length=cls.__min_collection_length__,
                     max_collection_length=cls.__max_collection_length__,
                 )
```

### Comparing `polyfactory-2.8.2/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.9.0/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.9.0/polyfactory/factories/pydantic_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.9.0/polyfactory/factories/typed_dict_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/field_meta.py` & `polyfactory-2.9.0/polyfactory/field_meta.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/fields.py` & `polyfactory-2.9.0/polyfactory/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,12 +104,12 @@
         :raises: ParameterException
 
         :returns: The build result.
         """
         from polyfactory.pytest_plugin import FactoryFixture
 
         if factory := FactoryFixture.factory_class_map.get(self.ref["value"]):
-            if self.size:
+            if self.size is not None:
                 return factory.batch(self.size, **self.kwargs)
             return factory.build(**self.kwargs)
 
         raise ParameterException("fixture has not been registered using the register_factory decorator")
```

### Comparing `polyfactory-2.8.2/polyfactory/persistence.py` & `polyfactory-2.9.0/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/pytest_plugin.py` & `polyfactory-2.9.0/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/utils/helpers.py` & `polyfactory-2.9.0/polyfactory/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import sys
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, ForwardRef
 
 from typing_extensions import get_args, get_origin
 
 from polyfactory.constants import TYPE_MAPPING
 from polyfactory.utils.predicates import (
     is_annotated,
     is_new_type,
@@ -126,7 +126,21 @@
         origin = TYPE_MAPPING[origin]
 
     if args := get_args(annotation):
         args = tuple(normalize_annotation(arg, random=random) for arg in args)
         return origin[args] if origin is not type else annotation
 
     return origin
+
+
+def evaluate_forwardref(ref: ForwardRef) -> Any:
+    """Evaluate ForwardRef to get type annotation
+
+    :param ref: A ForwardRef object
+
+    :returns: A type annotation
+
+    """
+    if sys.version_info < (3, 9):
+        return ref._evaluate(globals(), locals())
+
+    return ref._evaluate(globals(), locals(), frozenset())
```

### Comparing `polyfactory-2.8.2/polyfactory/utils/predicates.py` & `polyfactory-2.9.0/polyfactory/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/value_generators/complex_types.py` & `polyfactory-2.9.0/polyfactory/value_generators/complex_types.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.9.0/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.9.0/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.9.0/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.9.0/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/value_generators/primitives.py` & `polyfactory-2.9.0/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/polyfactory/value_generators/regex.py` & `polyfactory-2.9.0/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.8.2/pyproject.toml` & `polyfactory-2.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.8.2"
+version = "2.9.0"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
 ]
 maintainers = [
-    "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
+    "Visakh Unnikrishnan <guacs.guacs@gmail.com>",
 ]
 license = "MIT"
 readme = "docs/PYPI_README.md"
 homepage = "https://github.com/litestar-org/polyfactory"
 repository = "https://github.com/litestar-org/polyfactory"
 documentation = "https://github.com/litestar-org/polyfactory"
-keywords = ["dataclasses", "factory", "msgspec", "pydantic", "testing"]
+keywords = ["dataclasses", "factory", "msgspec", "pydantic", "attrs", "sqlalchemy", "testing"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Framework :: Pytest",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
@@ -41,21 +41,23 @@
 beanie = { version = "*", optional = true }
 faker = "*"
 msgspec = { version = "*", optional = true }
 odmantic = { version = "*", optional = true }
 pydantic = { version = "*", optional = true, extras = ["email"] }
 typing-extensions = "*"
 attrs = {version = ">=22.2.0", optional = true}
+sqlalchemy = { version = ">=2", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "*"
 mongomock-motor = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
+aiosqlite = "^0.19.0"
 
 [tool.poetry.group.docs.dependencies]
 auto-pytabs = "*"
 blacken-docs = "*"
 litestar-sphinx-theme = { git = "https://github.com/litestar-org/litestar-sphinx-theme.git" }
 sphinx = "*"
 sphinx-autobuild = "*"
@@ -71,20 +73,21 @@
 mypy = "*"
 pre-commit = "*"
 pyright = "*"
 ruff = '*'
 sourcery = "*"
 
 [tool.poetry.extras]
+sqlalchemy = ["sqlalchemy"]
 pydantic = ["pydantic"]
 msgspec = ["msgspec"]
 odmantic = ["odmantic", "pydantic"]
 beanie = ["beanie", "pydantic"]
 attrs = ["attrs"]
-full = ["pydantic", "odmantic", "msgspec", "beanie", "attrs"]
+full = ["pydantic", "odmantic", "msgspec", "beanie", "attrs", "sqlalchemy"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
@@ -93,22 +96,26 @@
 [tool.pyright]
 include = ["polyfactory", "tests", "examples"]
 
 [tool.coverage.run]
 omit = ["*/tests/*"]
 
 [tool.pytest.ini_options]
-addopts = "tests docs/examples"
+addopts = "--strict-config --strict-markers"
 asyncio_mode = "auto"
 filterwarnings = [
     "ignore:.*pkg_resources.declare_namespace\\('sphinxcontrib'\\).*:DeprecationWarning",
     "ignore:pkg_resources is deprecated as an API:DeprecationWarning",
     # Get rid those above once sphinxcontrib-mermaid doesn't use pkg_resources anymore
     # https://github.com/mgaitan/sphinxcontrib-mermaid/issues/119
 ]
+markers = [
+    # Marks tests that use `attrs` library
+    "attrs",
+]
 
 [tool.coverage.report]
 exclude_lines = [
     'pragma: no cover',
     'if TYPE_CHECKING:',
     'except ImportError:',
     'except ImportError as e:',
```

### Comparing `polyfactory-2.8.2/PKG-INFO` & `polyfactory-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.8.2
+Version: 2.9.0
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
-Keywords: dataclasses,factory,msgspec,pydantic,testing
+Keywords: dataclasses,factory,msgspec,pydantic,attrs,sqlalchemy,testing
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
-Maintainer: Na'aman Hirschfeld
-Maintainer-email: nhirschfeld@gmail.com
+Maintainer: Visakh Unnikrishnan
+Maintainer-email: guacs.guacs@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -31,20 +31,22 @@
 Classifier: Typing :: Typed
 Provides-Extra: attrs
 Provides-Extra: beanie
 Provides-Extra: full
 Provides-Extra: msgspec
 Provides-Extra: odmantic
 Provides-Extra: pydantic
+Provides-Extra: sqlalchemy
 Requires-Dist: attrs (>=22.2.0) ; extra == "attrs" or extra == "full"
 Requires-Dist: beanie ; extra == "beanie" or extra == "full"
 Requires-Dist: faker
 Requires-Dist: msgspec ; extra == "msgspec" or extra == "full"
 Requires-Dist: odmantic ; extra == "odmantic" or extra == "full"
 Requires-Dist: pydantic[email] ; extra == "pydantic" or extra == "odmantic" or extra == "beanie" or extra == "full"
+Requires-Dist: sqlalchemy (>=2) ; extra == "sqlalchemy" or extra == "full"
 Requires-Dist: typing-extensions
 Project-URL: Documentation, https://github.com/litestar-org/polyfactory
 Project-URL: Repository, https://github.com/litestar-org/polyfactory
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable -->
 <p align="center">
```

