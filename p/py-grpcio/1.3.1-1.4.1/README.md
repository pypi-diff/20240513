# Comparing `tmp/py_grpcio-1.3.1.tar.gz` & `tmp/py_grpcio-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_grpcio-1.3.1.tar", max compression
+gzip compressed data, was "py_grpcio-1.4.1.tar", max compression
```

## Comparing `py_grpcio-1.3.1.tar` & `py_grpcio-1.4.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1076 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/LICENSE
--rw-r--r--   0        0        0     4581 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/README.md
--rw-r--r--   0        0        0      119 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/__init__.py
--rw-r--r--   0        0        0      750 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/exceptions.py
--rw-r--r--   0        0        0     1809 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/interceptor.py
--rw-r--r--   0        0        0     4190 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/method.py
--rw-r--r--   0        0        0     4639 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/models.py
--rw-r--r--   0        0        0      114 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/proto/__init__.py
--rw-r--r--   0        0        0      483 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/proto/enums.py
--rw-r--r--   0        0        0     3818 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/proto/parser.py
--rw-r--r--   0        0        0      682 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/proto/templates/service.proto.template
--rw-r--r--   0        0        0     1873 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/server.py
--rw-r--r--   0        0        0      924 2024-05-09 22:05:04.790626 py_grpcio-1.3.1/py_grpcio/service.py
--rw-r--r--   0        0        0     2417 2024-05-09 22:05:04.794626 py_grpcio-1.3.1/py_grpcio/service_meta.py
--rw-r--r--   0        0        0      582 2024-05-09 22:05:04.794626 py_grpcio-1.3.1/py_grpcio/utils.py
--rw-r--r--   0        0        0      573 2024-05-09 22:05:04.794626 py_grpcio-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 py_grpcio-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/LICENSE
+-rw-r--r--   0        0        0     4581 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/README.md
+-rw-r--r--   0        0        0      167 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/__init__.py
+-rw-r--r--   0        0        0      750 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/exceptions.py
+-rw-r--r--   0        0        0     1826 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/interceptor.py
+-rw-r--r--   0        0        0     4977 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/method.py
+-rw-r--r--   0        0        0     1148 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/middleware.py
+-rw-r--r--   0        0        0     4810 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/models.py
+-rw-r--r--   0        0        0      114 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/proto/__init__.py
+-rw-r--r--   0        0        0      483 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/proto/enums.py
+-rw-r--r--   0        0        0     3818 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/proto/parser.py
+-rw-r--r--   0        0        0      687 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/proto/templates/service.proto.template
+-rw-r--r--   0        0        0     1921 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/server.py
+-rw-r--r--   0        0        0      924 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/service.py
+-rw-r--r--   0        0        0     2727 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/service_meta.py
+-rw-r--r--   0        0        0      582 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/py_grpcio/utils.py
+-rw-r--r--   0        0        0      573 2024-05-13 20:12:35.281000 py_grpcio-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 py_grpcio-1.4.1/PKG-INFO
```

### Comparing `py_grpcio-1.3.1/LICENSE` & `py_grpcio-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.3.1/README.md` & `py_grpcio-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.3.1/py_grpcio/exceptions.py` & `py_grpcio-1.4.1/py_grpcio/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.3.1/py_grpcio/interceptor.py` & `py_grpcio-1.4.1/py_grpcio/interceptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self: 'ServerInterceptor',
         route: ServerMethodGRPC,
         message: Message,
         context: ServicerContext,
         method_name: str,
     ) -> Message | None:
         try:
-            response: Message | None = await route(message=message)
+            response: Message | None = await route(message=message, context=context)
             logger.info(f'{context.peer()} - {route.__qualname__}')
             return response
         except GrpcException as grpc_exc:
             logger.error(
                 f'{context.peer()} - {route.__qualname__} | '
                 f'{grpc_exc.__class__.__name__} | {grpc_exc.status_code} | {grpc_exc.details}'
             )
```

### Comparing `py_grpcio-1.3.1/py_grpcio/models.py` & `py_grpcio-1.4.1/py_grpcio/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from inspect import isclass
-from typing import Type, Any, Callable
+from functools import partial
+from typing import Type, Any, TypeVar
 from typing_extensions import Annotated
 from types import FunctionType, ModuleType
 
-from pydantic import BaseModel, Field as PyField
+from pydantic import BaseModel, ConfigDict, Field as PyField
 from pydantic.fields import FieldInfo  # noqa: FieldInfo
 from pydantic_core.core_schema import CoreSchema, no_info_wrap_validator_function, str_schema, to_string_ser_schema
 
 from google.protobuf.message import Message as ProtoMessage
 
 from py_grpcio.exceptions import MethodSignatureException
 
 from py_grpcio.proto import ProtoBufTypes, parse_field_type
 
+Target: 'Target' = TypeVar('Target', bound=partial)
+
 
 class Field(BaseModel):
     name: str
     type: ProtoBufTypes | str
     repeated: bool = False
     map_key: str | None = None
     map_value: str | None = None
@@ -63,31 +66,33 @@
             serialization=to_string_ser_schema(),
         )
 
 
 class Method(BaseModel):
     request: Type[Message]
     response: Type[Message]
-    target: Callable[..., Message]
+    target: Target
     protos: Annotated[ModuleType, ModuleTypePydanticAnnotation] | None = None
     services: Annotated[ModuleType, ModuleTypePydanticAnnotation] | None = None
     additional_messages: dict[str, Type[Message]] = PyField(default_factory=dict)
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     @classmethod
     def from_target(cls, target: FunctionType) -> 'Method':
         annotations: dict[str, Any] = target.__annotations__
         if not (requst_message := annotations.get('request')) or not issubclass(requst_message, Message):
             raise MethodSignatureException(
                 text=f'Method `{target.__qualname__}` must receive a request parameter of type subclass `Message`'
             )
         if not (response_message := annotations.get('return')) or not issubclass(response_message, Message):
             raise MethodSignatureException(
                 text=f'The `{target.__qualname__}` method should return an object of type subclass `Message`'
             )
-        return cls(target=target, request=requst_message, response=response_message)
+        return cls(target=partial(target, self=target.__class__), request=requst_message, response=response_message)
 
     @property
     def messages(self: 'Method') -> dict[str, Type[Message]]:
         self.additional_messages.update(self.request.get_additional_messages_from_fields())
         self.additional_messages.update(self.response.get_additional_messages_from_fields())
         return {
             **self.additional_messages,
```

### Comparing `py_grpcio-1.3.1/py_grpcio/proto/parser.py` & `py_grpcio-1.4.1/py_grpcio/proto/parser.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.3.1/py_grpcio/proto/templates/service.proto.template` & `py_grpcio-1.4.1/py_grpcio/proto/templates/service.proto.template`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 //Automatically generated
 
 syntax = "proto3";
 package {{ camel_to_snake(string=service.name) }};
 
 service {{ service.name }} {
 {% for method in service.methods.values() %}
-    rpc {{ snake_to_camel(string=method.target.__name__) }}({{ method.request.__name__ }}) returns ({{ method.response.__name__}}) {}
+    rpc {{ snake_to_camel(string=method.target.func.__name__) }}({{ method.request.__name__ }}) returns ({{ method.response.__name__}}) {}
 {% endfor %}
 }
 
 {% for message in service.messages.values() %}
 message {{ message.__name__ }} {
 {% for field in message.fields() %}
     {% if field.repeated %}repeated {% endif -%}
```

### Comparing `py_grpcio-1.3.1/py_grpcio/server.py` & `py_grpcio-1.4.1/py_grpcio/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 from types import ModuleType
 
 from asyncio import AbstractEventLoop, get_event_loop
 
 from grpc.aio import server
 from grpc.aio._server import Server  # noqa: _server
 
-from grpc_interceptor.server import AsyncServerInterceptor
-
 from py_grpcio.service import BaseService
+from py_grpcio.middleware import BaseMiddleware
 from py_grpcio.interceptor import ServerInterceptor
 
 
 class BaseServer:
     def __init__(
         self: 'BaseServer',
         port: int = 50051,
-        interceptors: list[AsyncServerInterceptor] | None = None,
-        proto_dir: Path = Path('proto')
+        proto_dir: Path = Path('proto'),
+        middlewares: set[Type[BaseMiddleware]] | None = None
     ):
         self.port: int = port
-        self.interceptors: list = interceptors or []
         self.proto_dir: Path = proto_dir
         self.proto_dir.mkdir(exist_ok=True)
 
         self.loop: AbstractEventLoop = get_event_loop()
 
-        self.server: Server = server(interceptors=[ServerInterceptor(), *self.interceptors])
+        self.server: Server = server(interceptors=[ServerInterceptor()])
         self.server._loop = self.loop
 
         self.services: dict[str, Type[BaseService]] = {}
 
         self.__protos: dict[str, ModuleType] = {}
         self.__services: dict[str, ModuleType] = {}
+        self.middlewares: set[Type[BaseMiddleware]] = middlewares or set()
 
     def add_service(self: 'BaseServer', service: Type[BaseService]):
         self.services[service.name]: Type[BaseService] = service
+        service.set_middlewares(middlewares=self.middlewares)
         service.init_protos_and_services(proto_dir=self.proto_dir)
         self.__protos[service.name], self.__services[service.name] = service.protos, service.services
         getattr(service.services, f'add_{service.name}Servicer_to_server')(servicer=service, server=self.server)
 
     async def start_server(self: 'BaseServer') -> None:
         await self.server.start()
         await self.server.wait_for_termination()
```

### Comparing `py_grpcio-1.3.1/py_grpcio/service.py` & `py_grpcio-1.4.1/py_grpcio/service.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.3.1/py_grpcio/service_meta.py` & `py_grpcio-1.4.1/py_grpcio/service_meta.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from pathlib import Path
 
-from types import ModuleType
 from typing import Any, Type
+from types import ModuleType
 
 from jinja2 import Environment, FileSystemLoader, Template
 
 from grpc import protos_and_services
 
 from py_grpcio.models import Message, Method
 from py_grpcio.method import ServerMethodGRPC
+from py_grpcio.middleware import BaseMiddleware
+
 from py_grpcio.utils import is_method, camel_to_snake, snake_to_camel
 
 environment: Environment = Environment(
     loader=FileSystemLoader(searchpath=Path(__file__).parent / 'proto/templates'),
     trim_blocks=True
 )
 
@@ -21,20 +23,24 @@
     def __init__(cls: 'BaseServiceMeta', name: str, *args):
         super().__init__(name, *args)
         cls.name: str = name
         cls.methods: dict[str, Method] = {}
         cls.messages: dict[str, Type[Message]] = {}
         cls.protos: ModuleType | None = None
         cls.services: ModuleType | None = None
+        cls.middlewares: set[Type[BaseMiddleware]] = set()
 
     def __getattr__(cls: 'BaseServiceMeta', attr_name: str) -> ServerMethodGRPC | Any:
         if method := cls.methods.get(camel_to_snake(string=attr_name)):
-            return ServerMethodGRPC(method=method)
+            return ServerMethodGRPC(method=method, middlewares=cls.middlewares)
         return getattr(cls, attr_name)
 
+    def set_middlewares(cls, middlewares: set[Type[BaseMiddleware]]) -> None:
+        cls.middlewares: set[Type[BaseMiddleware]] = middlewares
+
     def methods_and_messages(cls: 'BaseServiceMeta') -> None:
         for method_name, target in cls.__dict__.items():
             if is_method(method=target):
                 method: Method = Method.from_target(target=target)
                 cls.methods[method_name]: Method = method
                 cls.messages.update(method.messages)
 
@@ -49,13 +55,13 @@
 
     def gen_proto(cls: 'BaseServiceMeta', proto_dir: Path) -> Path:
         path: Path = proto_dir / f'{camel_to_snake(string=cls.name)}.proto'
         path.write_text(data=cls.get_proto())
         return path
 
     def get_method(cls: 'BaseServiceMeta', method_name: str) -> ServerMethodGRPC:
-        return ServerMethodGRPC(method=getattr(cls, method_name))
+        return ServerMethodGRPC(method=getattr(cls, method_name), middlewares=cls.middlewares)
 
     def init_protos_and_services(cls: 'BaseServiceMeta', proto_dir: Path) -> None:
         cls.protos, cls.services = protos_and_services(protobuf_path=str(cls.gen_proto(proto_dir=proto_dir)))
         for method in cls.methods.values():
             method.protos, method.services = cls.protos, cls.services
```

### Comparing `py_grpcio-1.3.1/py_grpcio/utils.py` & `py_grpcio-1.4.1/py_grpcio/utils.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.3.1/pyproject.toml` & `py_grpcio-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-grpcio"
-version = "1.3.1"
+version = "1.4.1"
 description = "gRPC with autogen by Pydantic models"
 authors = ["Yurii <ykolibroda@lytvynov-production.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "py_grpcio" },
 ]
```

### Comparing `py_grpcio-1.3.1/PKG-INFO` & `py_grpcio-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-grpcio
-Version: 1.3.1
+Version: 1.4.1
 Summary: gRPC with autogen by Pydantic models
 License: MIT
 Author: Yurii
 Author-email: ykolibroda@lytvynov-production.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

