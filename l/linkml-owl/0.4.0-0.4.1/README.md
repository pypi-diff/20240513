# Comparing `tmp/linkml_owl-0.4.0.tar.gz` & `tmp/linkml_owl-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_owl-0.4.0.tar", max compression
+gzip compressed data, was "linkml_owl-0.4.1.tar", max compression
```

## Comparing `linkml_owl-0.4.0.tar` & `linkml_owl-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      141 2024-02-27 00:34:58.202462 linkml_owl-0.4.0/README.md
--rw-r--r--   0        0        0      301 2024-02-27 00:34:58.210462 linkml_owl-0.4.0/linkml_owl/__init__.py
--rw-r--r--   0        0        0        0 2024-02-27 00:34:58.210462 linkml_owl-0.4.0/linkml_owl/crossproducts/__init__.py
--rw-r--r--   0        0        0     5407 2024-02-27 00:34:58.210462 linkml_owl-0.4.0/linkml_owl/crossproducts/cross_product_generator.py
--rw-r--r--   0        0        0        0 2024-02-27 00:34:58.210462 linkml_owl-0.4.0/linkml_owl/dumpers/__init__.py
--rw-r--r--   0        0        0    37629 2024-02-27 00:34:58.210462 linkml_owl-0.4.0/linkml_owl/dumpers/owl_dumper.py
--rw-r--r--   0        0        0        0 2024-02-27 00:34:58.210462 linkml_owl-0.4.0/linkml_owl/util/__init__.py
--rw-r--r--   0        0        0      659 2024-02-27 00:34:58.210462 linkml_owl-0.4.0/linkml_owl/util/csv_converter.py
--rw-r--r--   0        0        0     7763 2024-02-27 00:34:58.210462 linkml_owl-0.4.0/linkml_owl/util/loader_wrapper.py
--rw-r--r--   0        0        0      454 2024-02-27 00:34:58.210462 linkml_owl-0.4.0/linkml_owl/util/trim_yaml.py
--rw-r--r--   0        0        0     1412 2024-02-27 00:35:12.558415 linkml_owl-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 linkml_owl-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      141 2024-05-13 02:49:29.345132 linkml_owl-0.4.1/README.md
+-rw-r--r--   0        0        0      301 2024-05-13 02:49:29.349132 linkml_owl-0.4.1/linkml_owl/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 02:49:29.349132 linkml_owl-0.4.1/linkml_owl/crossproducts/__init__.py
+-rw-r--r--   0        0        0     5407 2024-05-13 02:49:29.349132 linkml_owl-0.4.1/linkml_owl/crossproducts/cross_product_generator.py
+-rw-r--r--   0        0        0        0 2024-05-13 02:49:29.349132 linkml_owl-0.4.1/linkml_owl/dumpers/__init__.py
+-rw-r--r--   0        0        0    38550 2024-05-13 02:49:29.353132 linkml_owl-0.4.1/linkml_owl/dumpers/owl_dumper.py
+-rw-r--r--   0        0        0        0 2024-05-13 02:49:29.353132 linkml_owl-0.4.1/linkml_owl/util/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-13 02:49:29.353132 linkml_owl-0.4.1/linkml_owl/util/csv_converter.py
+-rw-r--r--   0        0        0     7763 2024-05-13 02:49:29.353132 linkml_owl-0.4.1/linkml_owl/util/loader_wrapper.py
+-rw-r--r--   0        0        0      454 2024-05-13 02:49:29.353132 linkml_owl-0.4.1/linkml_owl/util/trim_yaml.py
+-rw-r--r--   0        0        0     1412 2024-05-13 02:49:42.109131 linkml_owl-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 linkml_owl-0.4.1/PKG-INFO
```

### Comparing `linkml_owl-0.4.0/linkml_owl/crossproducts/cross_product_generator.py` & `linkml_owl-0.4.1/linkml_owl/crossproducts/cross_product_generator.py`

 * *Files identical despite different names*

### Comparing `linkml_owl-0.4.0/linkml_owl/dumpers/owl_dumper.py` & `linkml_owl-0.4.1/linkml_owl/dumpers/owl_dumper.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 AXIOM_TYPE_NAME = str
 OPERAND = str  ## e.g IntersectionOf, UnionOf
 
 LEVEL = int
 OP_KEY = Tuple[LEVEL, OPERAND, AXIOM_TYPE_NAME]
 
 
+def _skip_key_in_element(k: str, element: YAMLRoot) -> bool:
+    return k.startswith("unknown_") and k.replace("unknown_", "") in vars(element)
+
 @dataclass
 class EntityAxiomIndex:
     """
     An index of axioms (plus annotations), indexed by entity, plus aggregate grouping criteria (intersection, union)
 
     Motivation: any entity (such as a class) might have an arbitrary number of equivalence, disjointness, etc axioms
     associated with it; e.g.
@@ -244,18 +247,20 @@
             self.add_axioms_from_template(tmpl_str, element, schema=schema)
         cls_interps = self._get_class_interpretations(c)
         subj = None
         eai = EntityAxiomIndex()
         unprocessed_parents = []
         # set subj = IRI for element
         for k, v in vars(element).items():
+            if _skip_key_in_element(k, element):
+                continue
             slot: SlotDefinition
             slot = self._lookup_slot(c, k)
             if slot is None:
-                raise ValueError(f'Lookup slot in {c.name} failed for {k} // element={element}')
+                raise ValueError(f'Cannot find slot {c.name}.{k} // {vars(element)} element={element}')
             if slot.identifier:
                 subj = URIRef(self._get_IRI_str(v))
                 logging.debug(f"set subj from {slot.name}={v} asURI: {subj}")
         if AnonymousIndividual.__name__ in cls_interps or (subj is None and "Individual" in cls_interps):
             subj = AnonymousIndividual()
             logging.debug(f"No identifier slot; Creating anon individual for element = {subj}")
         else:
@@ -271,14 +276,16 @@
                     o.axioms.append(decl)
         logging.info(f"Subject={subj}")
         expression_termset = {"IntersectionOf", "UnionOf", "ComplementOf", "OneOf", "SomeValuesFrom", "AllValuesFrom"}
         is_returns_expression = len(expression_termset.intersection(cls_interps)) > 0
         # iterate through all slot-value assignments for element;
         # generate axioms or add axioms to EntityAxiomIndex for each
         for k, v in vars(element).items():
+            if _skip_key_in_element(k, element):
+                continue
             slot: SlotDefinition
             # TODO: unify slot/schema_level_slot
             slot = self._lookup_slot(c, k)
             if slot is None:
                 logging.error(f'No slot for {k}')
                 continue
             if slot.identifier:
@@ -514,14 +521,17 @@
         try:
             if type(v).class_name:
                 return True
         except Exception:
             return False
 
     def _lookup_slot(self, cls: ClassDefinition, field: str) -> SlotDefinition:
+        """
+        Lookup a slot in a class by name
+        """
         matching_slot = None
         for s in self.schemaview.class_induced_slots(cls.name):
             if underscore(s.name) == field:
                 matching_slot = s
                 break
             if s.alias and underscore(s.alias) == field:
                 matching_slot = s
@@ -794,30 +804,39 @@
         linkml-data2owl -s owl_dumper_test.yaml owl_dumper_test_data.yaml -o ont.ofn
 
     More documentation:
 
         https://linkml.io/linkml-owl/
     """
     logger = logging.getLogger()
+    # Set handler for the root logger to output to the console
+    console_handler = logging.StreamHandler()
+    console_handler.setFormatter(logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s"))
+    # Clear existing handlers to avoid duplicate messages if function runs multiple times
+    logger.handlers = []
+    # Add the newly created console handler to the logger
+    logger.addHandler(console_handler)
     if verbose >= 2:
         logger.setLevel(level=logging.DEBUG)
     elif verbose == 1:
         logger.setLevel(level=logging.INFO)
     else:
         logger.setLevel(level=logging.WARNING)
     if quiet:
         logger.setLevel(level=logging.ERROR)
+    logger.info(f"Loading and compiling schema {schema}")
     if module is None:
         if schema is None:
             raise Exception('must pass one of module OR schema')
         else:
             python_module = PythonGenerator(schema).compile_module()
     else:
         python_module = compile_python(module)
     sv = SchemaView(schema)
+    logger.info(f"Loading {inputfile} into schema {sv.schema.name}")
     element = load_structured_file(inputfile, target_class=target_class, python_module=python_module, schemaview=sv, fmt=format)
 
     dumper = OWLDumper()
     if autofill:
         dumper.autofill = True
     doc = dumper.dumps(element, schemaview=sv, output_type=output_type)
     output.write(str(doc))
```

### Comparing `linkml_owl-0.4.0/linkml_owl/util/csv_converter.py` & `linkml_owl-0.4.1/linkml_owl/util/csv_converter.py`

 * *Files identical despite different names*

### Comparing `linkml_owl-0.4.0/linkml_owl/util/loader_wrapper.py` & `linkml_owl-0.4.1/linkml_owl/util/loader_wrapper.py`

 * *Files identical despite different names*

### Comparing `linkml_owl-0.4.0/pyproject.toml` & `linkml_owl-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml_owl"
-version = "0.4.0"
+version = "0.4.1"
 description = "OWL mappings for Linked Open Data Modeling Language"
 authors = ["Chris Mungall <cjmungall@lbl.gov>"]
 
 readme = "README.md"
 
 homepage = "https://github.com/linkml/linkml-owl"
 repository = "https://github.com/linkml/linkml-owl"
```

### Comparing `linkml_owl-0.4.0/PKG-INFO` & `linkml_owl-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml_owl
-Version: 0.4.0
+Version: 0.4.1
 Summary: OWL mappings for Linked Open Data Modeling Language
 Home-page: https://github.com/linkml/linkml-owl
 Keywords: linkml,owl
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

