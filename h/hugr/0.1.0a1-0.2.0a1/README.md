# Comparing `tmp/hugr-0.1.0a1.tar.gz` & `tmp/hugr-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugr-0.1.0a1.tar", max compression
+gzip compressed data, was "hugr-0.2.0a1.tar", max compression
```

## Comparing `hugr-0.1.0a1.tar` & `hugr-0.2.0a1.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1446 2024-04-03 17:19:08.176174 hugr-0.1.0a1/README.md
--rw-r--r--   0        0        0     1132 2024-04-03 17:19:08.176174 hugr-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      209 2024-04-03 17:19:08.176174 hugr-0.1.0a1/src/hugr/__init__.py
--rw-r--r--   0        0        0       62 2024-04-03 17:19:08.176174 hugr-0.1.0a1/src/hugr/serialization/__init__.py
--rw-r--r--   0        0        0    17296 2024-04-03 17:19:08.176174 hugr-0.1.0a1/src/hugr/serialization/ops.py
--rw-r--r--   0        0        0      894 2024-04-03 17:19:08.176174 hugr-0.1.0a1/src/hugr/serialization/serial_hugr.py
--rw-r--r--   0        0        0     8041 2024-04-03 17:19:08.176174 hugr-0.1.0a1/src/hugr/serialization/tys.py
--rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 hugr-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1446 2024-05-13 10:18:47.630760 hugr-0.2.0a1/README.md
+-rw-r--r--   0        0        0     1217 2024-05-13 10:18:47.630760 hugr-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0      234 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/py.typed
+-rw-r--r--   0        0        0       62 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/serialization/__init__.py
+-rw-r--r--   0        0        0    15478 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/serialization/ops.py
+-rw-r--r--   0        0        0     1392 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/serialization/serial_hugr.py
+-rw-r--r--   0        0        0      971 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/serialization/testing_hugr.py
+-rw-r--r--   0        0        0     9457 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/serialization/tys.py
+-rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 hugr-0.2.0a1/PKG-INFO
```

### Comparing `hugr-0.1.0a1/README.md` & `hugr-0.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `hugr-0.1.0a1/pyproject.toml` & `hugr-0.2.0a1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,24 +9,28 @@
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
 ]
 name = "hugr"
-version = "0.1.0a1"
+version = "0.2.0a1"
 description = "Quantinuum's common representation for quantum programs"
 #keywords = []
 authors = ["TKET development team <tket-support@cambridgequantum.com>"]
 maintainers = ["TKET development team <tket-support@cambridgequantum.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/CQCL/hugr"
 repository = "https://github.com/CQCL/hugr"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
-pydantic = "^2.6.4"
+pydantic = "~2.7.0"
 
 [tool.pytest.ini_options]
 # Lark throws deprecation warnings for `src_parse` and `src_constants`.
 filterwarnings = "ignore::DeprecationWarning:lark.*"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `hugr-0.1.0a1/src/hugr/serialization/ops.py` & `hugr-0.2.0a1/src/hugr/serialization/ops.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import inspect
 import sys
 from abc import ABC
-from typing import Any, Literal, cast
+from typing import Any, Literal
 
-from pydantic import BaseModel, Field, RootModel
+from pydantic import Field, RootModel
 
 from . import tys
 from .tys import (
     ExtensionId,
     ExtensionSet,
     FunctionType,
     PolyFuncType,
     Type,
     TypeRow,
+    SumType,
+    TypeBound,
+    ConfiguredBaseModel,
+    classes as tys_classes,
+    model_rebuild as tys_model_rebuild,
 )
 
 NodeID = int
 
 
-class BaseOp(ABC, BaseModel):
+class BaseOp(ABC, ConfiguredBaseModel):
     """Base class for ops that store their node's input/output types"""
 
     # Parent node index of node the op belongs to, used only at serialization time
     parent: NodeID
-    input_extensions: ExtensionSet = Field(default_factory=ExtensionSet)
+    input_extensions: ExtensionSet | None = Field(default=None)
 
     def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
         """Hook to insert type information from the input and output ports into the
         op"""
 
     def insert_child_dfg_signature(self, inputs: TypeRow, outputs: TypeRow) -> None:
         """Hook to insert type information from a child dataflow graph"""
@@ -50,169 +55,141 @@
 
 class FuncDefn(BaseOp):
     """A function definition. Children nodes are the body of the definition."""
 
     op: Literal["FuncDefn"] = "FuncDefn"
 
     name: str
-    signature: PolyFuncType = Field(default_factory=PolyFuncType.empty)
-
-    def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
-        assert len(in_types) == 0
-        assert len(out_types) == 1
-        out = out_types[0]
-        assert isinstance(out, PolyFuncType)
-        self.signature = out  # TODO: Extensions
+    signature: PolyFuncType
 
 
 class FuncDecl(BaseOp):
     """External function declaration, linked at runtime."""
 
     op: Literal["FuncDecl"] = "FuncDecl"
     name: str
-    signature: PolyFuncType = Field(default_factory=PolyFuncType.empty)
-
-    def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
-        assert len(in_types) == 0
-        assert len(out_types) == 1
-        out = out_types[0]
-        assert isinstance(out, PolyFuncType)
-        self.signature = out
+    signature: PolyFuncType
 
 
-class ConstBase(BaseOp):
-    """A constant operation definition."""
-
-    op: Literal["Const"] = "Const"
-
-
-CustomConst = Any  # TODO
+class CustomConst(ConfiguredBaseModel):
+    c: str
+    v: Any
 
 
-class ExtensionConst(ConstBase):
+class ExtensionValue(ConfiguredBaseModel):
     """An extension constant value, that can check it is of a given [CustomType]."""
 
-    c: Literal["Extension"] = Field("Extension", title="ConstTag")
-    e: CustomConst = Field(title="CustomConst")
-
-    class Config:
-        json_schema_extra = {
-            "required": ["parent", "op", "c", "e"],
-        }
+    v: Literal["Extension"] = Field("Extension", title="ValueTag")
+    extensions: ExtensionSet
+    typ: Type
+    value: CustomConst
 
 
-class FunctionConst(ConstBase):
+class FunctionValue(ConfiguredBaseModel):
     """A higher-order function value."""
 
-    c: Literal["Function"] = Field("Function", title="ConstTag")
+    v: Literal["Function"] = Field("Function", title="ValueTag")
     hugr: Any  # TODO
 
-    class Config:
-        json_schema_extra = {
-            "required": ["parent", "op", "c", "hugr"],
-        }
-
 
-class Tuple(ConstBase):
+class TupleValue(ConfiguredBaseModel):
     """A constant tuple value."""
 
-    c: Literal["Tuple"] = Field("Tuple", title="ConstTag")
-    vs: list["Const"]
-
-    class Config:
-        json_schema_extra = {
-            "required": ["parent", "op", "c", "vs"],
-        }
+    v: Literal["Tuple"] = Field("Tuple", title="ValueTag")
+    vs: list["Value"]
 
 
-class Sum(ConstBase):
+class SumValue(ConfiguredBaseModel):
     """A Sum variant
 
     For any Sum type where this value meets the type of the variant indicated by the tag
     """
 
-    c: Literal["Sum"] = Field("Sum", title="ConstTag")
+    v: Literal["Sum"] = Field("Sum", title="ValueTag")
     tag: int
-    typ: Type
-    vs: list["Const"]
+    typ: SumType
+    vs: list["Value"]
 
     class Config:
         # Needed to avoid random '\n's in the pydantic description
         json_schema_extra = {
             "description": (
                 "A Sum variant For any Sum type where this value meets the type "
                 "of the variant indicated by the tag."
             ),
-            "required": ["parent", "op", "c", "tag", "typ", "vs"],
         }
 
 
-class Const(RootModel):
-    """A constant operation."""
+class Value(RootModel):
+    """A constant Value."""
+
+    root: ExtensionValue | FunctionValue | TupleValue | SumValue = Field(
+        discriminator="v"
+    )
+
+    class Config:
+        json_schema_extra = {"required": ["v"]}
 
-    root: ExtensionConst | FunctionConst | Tuple | Sum = Field(discriminator="c")
+
+class Const(BaseOp):
+    """A Const operation definition."""
+
+    op: Literal["Const"] = "Const"
+    v: Value = Field()
 
 
 # -----------------------------------------------
 # --------------- BasicBlock types ------------------
 # -----------------------------------------------
 
 
 class DataflowBlock(BaseOp):
     """A CFG basic block node. The signature is that of the internal Dataflow
     graph."""
 
     op: Literal["DataflowBlock"] = "DataflowBlock"
     inputs: TypeRow = Field(default_factory=list)
     other_outputs: TypeRow = Field(default_factory=list)
-    sum_rows: list[TypeRow] = Field(default_factory=list)
+    sum_rows: list[TypeRow]
     extension_delta: ExtensionSet = Field(default_factory=list)
 
     def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
         num_cases = len(out_types)
         self.sum_rows = [[] for _ in range(num_cases)]
 
     def insert_child_dfg_signature(self, inputs: TypeRow, outputs: TypeRow) -> None:
         self.inputs = inputs
-        pred = outputs[0]
-        assert isinstance(pred, tys.UnitSum | tys.GeneralSum)
-        if isinstance(pred, tys.UnitSum):
-            self.sum_rows = [[] for _ in range(cast(tys.UnitSum, pred).size)]
+        pred = outputs[0].root
+        assert isinstance(pred, tys.SumType)
+        if isinstance(pred.root, tys.UnitSum):
+            self.sum_rows = [[] for _ in range(pred.root.size)]
         else:
             self.sum_rows = []
-            for variant in pred.rows:
+            for variant in pred.root.rows:
                 self.sum_rows.append(variant)
         self.other_outputs = outputs[1:]
 
     class Config:
         # Needed to avoid random '\n's in the pydantic description
         json_schema_extra = {
-            "required": [
-                "parent",
-                "op",
-                "inputs",
-                "other_outputs",
-                "sum_rows",
-                "extension_delta",
-            ],
             "description": "A CFG basic block node. The signature is that of the internal Dataflow graph.",
         }
 
 
 class ExitBlock(BaseOp):
     """The single exit node of the CFG, has no children, stores the types of
     the CFG node output."""
 
     op: Literal["ExitBlock"] = "ExitBlock"
     cfg_outputs: TypeRow
 
     class Config:
-        # Needed to avoid random '\n's in the pydantic description
         json_schema_extra = {
-            "description": "The single exit node of the CFG, has no children, stores the types of the CFG node output."
+            # Needed to avoid random '\n's in the pydantic description
+            "description": "The single exit node of the CFG, has no children, stores the types of the CFG node output.",
         }
 
 
 # ---------------------------------------------
 # --------------- DataflowOp ------------------
 # ---------------------------------------------
 
@@ -249,23 +226,17 @@
 
     The first port is connected to the def/declare of the function being called
     directly, with a `ConstE<Graph>` edge. The signature of the remaining ports matches
     the function being called.
     """
 
     op: Literal["Call"] = "Call"
-    signature: FunctionType = Field(default_factory=FunctionType.empty)
-
-    def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
-        # The constE edge comes after the value inputs
-        fun_ty = in_types[-1]
-        assert isinstance(fun_ty, PolyFuncType)
-        poly_func = cast(PolyFuncType, fun_ty)
-        assert len(poly_func.params) == 0
-        self.signature = poly_func.body
+    func_sig: PolyFuncType
+    type_args: list[tys.TypeArg]
+    instantiation: FunctionType
 
     class Config:
         # Needed to avoid random '\n's in the pydantic description
         json_schema_extra = {
             "description": (
                 "Operation to call a function directly. The first port is "
                 "connected to the def/declare of the function being called directly, "
@@ -274,41 +245,42 @@
             )
         }
 
 
 class CallIndirect(DataflowOp):
     """Call a function indirectly.
 
-    Like call, but the first input is a standard dataflow graph type."""
+    Like call, but the first input is a standard dataflow graph type.
+    """
 
     op: Literal["CallIndirect"] = "CallIndirect"
     signature: FunctionType = Field(default_factory=FunctionType.empty)
 
     def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
-        fun_ty = in_types[0]
-        assert isinstance(fun_ty, PolyFuncType)
-        poly_func = cast(PolyFuncType, fun_ty)
-        assert len(poly_func.params) == 0
-        assert len(poly_func.body.input) == len(in_types) - 1
-        assert len(poly_func.body.output) == len(out_types)
-        self.signature = poly_func.body
+        fun_ty = in_types[0].root
+        assert isinstance(fun_ty, FunctionType)
+        assert len(fun_ty.input) == len(in_types) - 1
+        assert len(fun_ty.output) == len(out_types)
+        self.signature = fun_ty
 
 
 class LoadConstant(DataflowOp):
     """An operation that loads a static constant in to the local dataflow graph."""
 
     op: Literal["LoadConstant"] = "LoadConstant"
     datatype: Type
 
 
-class LeafOpBase(DataflowOp):
-    """Simple operation that has only value inputs+outputs and (potentially) StateOrder
-    edges."""
+class LoadFunction(DataflowOp):
+    """Load a static function in to the local dataflow graph."""
 
-    op: Literal["LeafOp"] = "LeafOp"
+    op: Literal["LoadFunction"] = "LoadFunction"
+    func_sig: PolyFuncType
+    type_args: list[tys.TypeArg]
+    signature: FunctionType
 
 
 class DFG(DataflowOp):
     """A simply nested dataflow graph."""
 
     op: Literal["DFG"] = "DFG"
     signature: FunctionType = Field(default_factory=FunctionType.empty)
@@ -326,28 +298,32 @@
 
 class Conditional(DataflowOp):
     """Conditional operation, defined by child `Case` nodes for each branch."""
 
     op: Literal["Conditional"] = "Conditional"
     other_inputs: TypeRow = Field(default_factory=list)  # Remaining input types
     outputs: TypeRow = Field(default_factory=list)  # Output types
-    sum_rows: list[TypeRow] = Field(description="The possible rows of the Sum input")
+    sum_rows: list[TypeRow] = Field(
+        description="The possible rows of the Sum input", default_factory=list
+    )
     # Extensions used to produce the outputs
     extension_delta: ExtensionSet = Field(default_factory=list)
 
     def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
         # First port is a predicate, i.e. a sum of tuple types. We need to unpack
         # those into a list of type rows
         pred = in_types[0]
-        if isinstance(pred, tys.UnitSum):
-            self.sum_rows = [[] for _ in range(cast(tys.UnitSum, pred).size)]
+        assert isinstance(pred.root, tys.SumType)
+        sum = pred.root.root
+        if isinstance(sum, tys.UnitSum):
+            self.sum_rows = [[] for _ in range(sum.size)]
         else:
-            assert isinstance(pred, tys.GeneralSum)
+            assert isinstance(sum, tys.GeneralSum)
             self.sum_rows = []
-            for ty in pred.rows:
+            for ty in sum.rows:
                 self.sum_rows.append(ty)
         self.other_inputs = list(in_types[1:])
         self.outputs = list(out_types)
 
 
 class Case(BaseOp):
     """Case ops - nodes valid inside Conditional nodes."""
@@ -389,24 +365,19 @@
             input=list(inputs), output=list(outputs), extension_reqs=ExtensionSet([])
         )
 
 
 ControlFlowOp = Conditional | TailLoop | CFG
 
 
-# -----------------------------------------
-# --------------- LeafOp ------------------
-# -----------------------------------------
-
-
-class CustomOp(LeafOpBase):
+class CustomOp(DataflowOp):
     """A user-defined operation that can be downcasted by the extensions that define
     it."""
 
-    lop: Literal["CustomOp"] = "CustomOp"
+    op: Literal["CustomOp"] = "CustomOp"
     extension: ExtensionId
     op_name: str
     signature: tys.FunctionType = Field(default_factory=tys.FunctionType.empty)
     description: str = ""
     args: list[tys.TypeArg] = Field(default_factory=list)
 
     def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
@@ -421,90 +392,76 @@
             "description": (
                 "A user-defined operation that can be downcasted by the extensions that "
                 "define it."
             )
         }
 
 
-class Noop(LeafOpBase):
+class Noop(DataflowOp):
     """A no-op operation."""
 
-    lop: Literal["Noop"] = "Noop"
+    op: Literal["Noop"] = "Noop"
     ty: Type
 
     def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
         assert len(in_types) == 1
         assert len(out_types) == 1
         assert in_types[0] == out_types[0]
         self.ty = in_types[0]
 
 
-class MakeTuple(LeafOpBase):
+class MakeTuple(DataflowOp):
     """An operation that packs all its inputs into a tuple."""
 
-    lop: Literal["MakeTuple"] = "MakeTuple"
+    op: Literal["MakeTuple"] = "MakeTuple"
     tys: TypeRow = Field(default_factory=list)
 
     def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
         # If we have a single order edge as input, this is a unit
         if in_types == [None]:
             in_types = []
         self.tys = list(in_types)
 
 
-class UnpackTuple(LeafOpBase):
+class UnpackTuple(DataflowOp):
     """An operation that packs all its inputs into a tuple."""
 
-    lop: Literal["UnpackTuple"] = "UnpackTuple"
+    op: Literal["UnpackTuple"] = "UnpackTuple"
     tys: TypeRow = Field(default_factory=list)
 
     def insert_port_types(self, in_types: TypeRow, out_types: TypeRow) -> None:
         self.tys = list(out_types)
 
 
-class Tag(LeafOpBase):
+class Tag(DataflowOp):
     """An operation that creates a tagged sum value from one of its variants."""
 
-    lop: Literal["Tag"] = "Tag"
+    op: Literal["Tag"] = "Tag"
     tag: int  # The variant to create.
-    variants: TypeRow  # The variants of the sum type.
+    variants: list[TypeRow]  # The variants of the sum type.
 
 
-class TypeApply(LeafOpBase):
+class Lift(DataflowOp):
     """Fixes some TypeParams of a polymorphic type by providing TypeArgs."""
 
-    lop: Literal["TypeApply"] = "TypeApply"
-    ta: "TypeApplication"
-
-
-class TypeApplication(BaseModel):
-    """Records details of an application of a PolyFuncType to some TypeArgs and the
-    result (a less-, but still potentially-, polymorphic type).
-    """
+    op: Literal["Lift"] = "Lift"
+    type_row: TypeRow
+    new_extension: ExtensionId
 
-    input: PolyFuncType
-    args: list[tys.TypeTypeArg]
-    output: PolyFuncType
-
-    class Config:
-        # Needed to avoid random '\n's in the pydantic description
-        json_schema_extra = {
-            "description": (
-                "Records details of an application of a PolyFuncType to some TypeArgs "
-                "and the result (a less-, but still potentially-, polymorphic type)."
-            )
-        }
 
+class AliasDecl(BaseOp):
+    op: Literal["AliasDecl"] = "AliasDecl"
+    name: str
+    bound: TypeBound
 
-class LeafOp(RootModel):
-    """A constant operation."""
 
-    root: CustomOp | Noop | MakeTuple | UnpackTuple | Tag | TypeApply = Field(
-        discriminator="lop"
-    )
+class AliasDefn(BaseOp):
+    op: Literal["AliasDefn"] = "AliasDefn"
+    name: str
+    definition: Type
 
 
 class OpType(RootModel):
     """A constant operation."""
 
     root: (
         Module
@@ -518,40 +475,55 @@
         | TailLoop
         | CFG
         | Input
         | Output
         | Call
         | CallIndirect
         | LoadConstant
-        | LeafOp
+        | LoadFunction
+        | CustomOp
+        | Noop
+        | MakeTuple
+        | UnpackTuple
+        | Tag
+        | Lift
         | DFG
+        | AliasDecl
+        | AliasDefn
     ) = Field(discriminator="op")
 
+    class Config:
+        json_schema_extra = {"required": ["parent", "op"]}
+
 
 # --------------------------------------
 # --------------- OpDef ----------------
 # --------------------------------------
 
 
-class OpDef(BaseOp, populate_by_name=True):
+class FixedHugr(ConfiguredBaseModel):
+    extensions: ExtensionSet
+    hugr: Any
+
+
+class OpDef(ConfiguredBaseModel, populate_by_name=True):
     """Serializable definition for dynamically loaded operations."""
 
+    extension: ExtensionId
     name: str  # Unique identifier of the operation.
     description: str  # Human readable description of the operation.
-    inputs: list[tuple[str | None, Type]]
-    outputs: list[tuple[str | None, Type]]
-    misc: dict[str, Any]  # Miscellaneous data associated with the operation.
-    def_: str | None = Field(
-        ..., alias="def"
-    )  # (YAML?)-encoded definition of the operation.
-    extension_reqs: ExtensionSet  # Resources required to execute this operation.
+    misc: dict[str, Any] | None = None
+    signature: PolyFuncType | None = None
+    lower_funcs: list[FixedHugr]
 
 
 # Now that all classes are defined, we need to update the ForwardRefs in all type
 # annotations. We use some inspect magic to find all classes defined in this file.
-classes = inspect.getmembers(
-    sys.modules[__name__],
-    lambda member: inspect.isclass(member) and member.__module__ == __name__,
+classes = (
+    inspect.getmembers(
+        sys.modules[__name__],
+        lambda member: inspect.isclass(member) and member.__module__ == __name__,
+    )
+    + tys_classes
 )
-for _, c in classes:
-    if issubclass(c, BaseModel):
-        c.model_rebuild()
+
+tys_model_rebuild(dict(classes))
```

### Comparing `hugr-0.1.0a1/src/hugr/serialization/serial_hugr.py` & `hugr-0.2.0a1/src/hugr/serialization/serial_hugr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 from typing import Any, Literal
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field, ConfigDict
 
-from .ops import NodeID, OpType
+from .ops import NodeID, OpType, classes as ops_classes
+from .tys import model_rebuild
+import hugr
 
 Port = tuple[NodeID, int | None]  # (node, offset)
 Edge = tuple[Port, Port]
 
 
 class SerialHugr(BaseModel):
     """A serializable representation of a Hugr."""
 
     version: Literal["v1"] = "v1"
     nodes: list[OpType]
     edges: list[Edge]
+    encoder: str | None = Field(
+        default=None, description="The name of the encoder used to generate the Hugr."
+    )
 
     def to_json(self) -> str:
         """Return a JSON representation of the Hugr."""
+        self.encoder = f"hugr-py v{hugr.__version__}"
         return self.model_dump_json()
 
     @classmethod
     def load_json(cls, json: dict[Any, Any]) -> "SerialHugr":
         """Decode a JSON-encoded Hugr."""
         return cls(**json)
 
     @classmethod
     def get_version(cls) -> str:
         """Return the version of the schema."""
         return cls(nodes=[], edges=[]).version
 
+    @classmethod
+    def _pydantic_rebuild(cls, config: ConfigDict = ConfigDict(), **kwargs):
+        my_classes = dict(ops_classes)
+        my_classes[cls.__name__] = cls
+        model_rebuild(my_classes, config=config, **kwargs)
+
     class Config:
         title = "Hugr"
         json_schema_extra = {
             "required": ["version", "nodes", "edges"],
         }
```

### Comparing `hugr-0.1.0a1/PKG-INFO` & `hugr-0.2.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugr
-Version: 0.1.0a1
+Version: 0.2.0a1
 Summary: Quantinuum's common representation for quantum programs
 Home-page: https://github.com/CQCL/hugr
 License: Apache-2.0
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 Maintainer: TKET development team
 Maintainer-email: tket-support@cambridgequantum.com
@@ -17,15 +17,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pydantic (>=2.7.0,<2.8.0)
 Project-URL: Repository, https://github.com/CQCL/hugr
 Description-Content-Type: text/markdown
 
 hugr
 ===============
 
 [![build_status][]](https://github.com/CQCL/hugr/actions)
```

