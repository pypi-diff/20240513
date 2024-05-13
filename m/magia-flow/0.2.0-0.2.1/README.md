# Comparing `tmp/magia_flow-0.2.0.tar.gz` & `tmp/magia_flow-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magia_flow-0.2.0.tar", max compression
+gzip compressed data, was "magia_flow-0.2.1.tar", max compression
```

## Comparing `magia_flow-0.2.0.tar` & `magia_flow-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1069 2024-05-11 21:00:55.314060 magia_flow-0.2.0/LICENSE
--rw-r--r--   0        0        0      472 2024-05-11 21:00:55.314060 magia_flow-0.2.0/README.md
--rw-r--r--   0        0        0      104 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/__init__.py
--rw-r--r--   0        0        0     1302 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/__main__.py
--rw-r--r--   0        0        0       89 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/formal/__init__.py
--rw-r--r--   0        0        0     7828 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/formal/sby.py
--rw-r--r--   0        0        0      487 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/online/__init__.py
--rw-r--r--   0        0        0     1374 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/online/digitaljs/Dockerfile
--rw-r--r--   0        0        0      224 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/online/digitaljs/docker-compose.yml
--rw-r--r--   0        0        0      232 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/online/digitaljs/nginx.conf
--rw-r--r--   0        0        0     2861 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/online/digitaljs.py
--rw-r--r--   0        0        0     1863 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/oss_cad.py
--rw-r--r--   0        0        0      126 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/simulation/__init__.py
--rw-r--r--   0        0        0     3808 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/simulation/general.py
--rw-r--r--   0        0        0     2782 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/simulation/surfer.py
--rw-r--r--   0        0        0     1888 2024-05-11 21:00:55.314060 magia_flow-0.2.0/magia_flow/simulation/verilator.py
--rw-r--r--   0        0        0     1557 2024-05-11 21:00:55.314060 magia_flow-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 magia_flow-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-13 15:04:40.552307 magia_flow-0.2.1/LICENSE
+-rw-r--r--   0        0        0      472 2024-05-13 15:04:40.552307 magia_flow-0.2.1/README.md
+-rw-r--r--   0        0        0      104 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/__init__.py
+-rw-r--r--   0        0        0     1302 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/__main__.py
+-rw-r--r--   0        0        0       89 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/formal/__init__.py
+-rw-r--r--   0        0        0     7697 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/formal/sby.py
+-rw-r--r--   0        0        0      487 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/online/__init__.py
+-rw-r--r--   0        0        0     1374 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/online/digitaljs/Dockerfile
+-rw-r--r--   0        0        0      224 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/online/digitaljs/docker-compose.yml
+-rw-r--r--   0        0        0      232 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/online/digitaljs/nginx.conf
+-rw-r--r--   0        0        0     2861 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/online/digitaljs.py
+-rw-r--r--   0        0        0     1863 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/oss_cad.py
+-rw-r--r--   0        0        0      126 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/simulation/__init__.py
+-rw-r--r--   0        0        0     3808 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/simulation/general.py
+-rw-r--r--   0        0        0     2782 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/simulation/surfer.py
+-rw-r--r--   0        0        0     1888 2024-05-13 15:04:40.552307 magia_flow-0.2.1/magia_flow/simulation/verilator.py
+-rw-r--r--   0        0        0     1557 2024-05-13 15:04:40.552307 magia_flow-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 magia_flow-0.2.1/PKG-INFO
```

### Comparing `magia_flow-0.2.0/LICENSE` & `magia_flow-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magia_flow-0.2.0/magia_flow/__main__.py` & `magia_flow-0.2.1/magia_flow/__main__.py`

 * *Files identical despite different names*

### Comparing `magia_flow-0.2.0/magia_flow/formal/sby.py` & `magia_flow-0.2.1/magia_flow/formal/sby.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,62 +27,64 @@
 EXTRA_FILE_TEMPLATE = string.Template("[file $fname]\n$code\n")
 READ_FILE_TEMPLATE = string.Template('read -formal "$fname"\n')
 SECTION_TEMPLATE = string.Template("[$section]\n$content\n")
 
 CMD_TEMPLATE = string.Template('sby -f -d "$workdir" "$sby_file"')
 
 
+@dataclass
+class SbyTaskSpec:
+    """Describes a SymbiYosys task to be executed."""
+
+    name: str = "default"
+    top_module: str = None
+    mode: Literal["prove", "cover", "bmc", "live"] = "bmc"
+    engines: list[str] = field(default_factory=list)
+    options: list[str] = field(default_factory=list)
+    script: list[str] = field(default_factory=list)
+    files: list[str] = field(default_factory=list)
+    extra_code: dict[str, str] = field(default_factory=dict)
+
+    def __post_init__(self):
+        if self.top_module is None:
+            raise ValueError("top_module is required")
+        self.script.append(f"prep -top {self.top_module}")
+
+        if len(self.engines) == 0:
+            if self.mode == "live":
+                self.engines.append("aiger suprove")
+            else:
+                self.engines.append("smtbmc boolector")
+
+        self.options = [f"mode {self.mode}"] + self.options
+
+
+@dataclass
+class SbyTaskResult:
+    """Describes the result of a SymbiYosys task."""
+
+    passed: bool
+    raw_result: str = field(repr=False)
+    stdout: str = field(repr=False)
+    stderr: str = field(repr=False)
+    tests: list[dict] = field(repr=False)
+    test_count: int
+    failures: int
+    errors: int
+    skipped: int
+
+
 class SbyTask:
     extra_code_counter = 0
 
-    @dataclass
-    class SbyTaskSpec:
-        """Describes a SymbiYosys task to be executed."""
-
-        name: str = "default"
-        top_module: str = None
-        mode: Literal["prove", "cover", "bmc", "live"] = "bmc"
-        engines: list[str] = field(default_factory=list)
-        options: list[str] = field(default_factory=list)
-        script: list[str] = field(default_factory=list)
-        files: list[str] = field(default_factory=list)
-        extra_code: dict[str, str] = field(default_factory=dict)
-
-        def __post_init__(self):
-            if self.top_module is None:
-                raise ValueError("top_module is required")
-            self.script.append(f"prep -top {self.top_module}")
-
-            if len(self.engines) == 0:
-                if self.mode == "live":
-                    self.engines.append("aiger suprove")
-                else:
-                    self.engines.append("smtbmc boolector")
-
-            self.options = [f"mode {self.mode}"] + self.options
-
-    @dataclass
-    class SbyTaskResult:
-        """Describes the result of a SymbiYosys task."""
-
-        passed: bool
-        raw_result: str = field(repr=False)
-        stdout: str = field(repr=False)
-        stderr: str = field(repr=False)
-        tests: list[dict] = field(repr=False)
-        test_count: int
-        failures: int
-        errors: int
-        skipped: int
-
     def __init__(self, top_module: str, mode="bmc", work_dir=None, **kwargs):
-        self.spec = self.SbyTaskSpec(top_module=top_module, mode=mode)
+        self.spec = SbyTaskSpec(top_module=top_module, mode=mode)
         self.work_dir = Path.cwd().absolute() if work_dir is None else Path(work_dir).absolute()
         self._task_executed = False
-        self._result = None
+        self._result: None | SbyTaskResult = None
 
     def add_file(self, *files: Iterable[os.PathLike]):
         """Add files to the task."""
         self.spec.files += [
             str(Path(file).absolute())
             for file in files
         ]
@@ -102,34 +104,33 @@
 
     def add_script(self, *script: Iterable[str]):
         """Add script lines to the task."""
         self.spec.script += list(script)
 
     def _generate_script(self):
         """Generate the SymbiYosys script."""
-        extra_code = [
-            EXTRA_FILE_TEMPLATE.substitute(fname=fname, code=code)
-            for fname, code in self.spec.extra_code.items()
-        ]
-        flist = self.spec.files + list(self.spec.extra_code.keys())
+        for fname, code in self.spec.extra_code.items():
+            (self.work_dir / fname).write_text(code)
+        flist = self.spec.files + [str((self.work_dir / fname).absolute()) for fname in self.spec.extra_code]
         read_file_scripts = [
             READ_FILE_TEMPLATE.substitute(fname=fname)
             for fname in flist
         ]
 
         section_formation = {
             "tasks": [f"{self.spec.name}"],
             "options": self.spec.options,
             "engines": self.spec.engines,
+            "files": ["\n".join(flist)],
             "script": read_file_scripts + self.spec.script,
         }
         sections = [
-                       SECTION_TEMPLATE.substitute(section=section, content="\n".join(content))
-                       for section, content in section_formation.items()
-                   ] + extra_code
+            SECTION_TEMPLATE.substitute(section=section, content="\n".join(content))
+            for section, content in section_formation.items()
+        ]
 
         return "\n".join(sections)
 
     def run(self):
         """Run the task. Override work_dir if it is provided."""
         work_dir = self.work_dir / self.spec.top_module
         with NamedTemporaryFile("w", suffix=".sby") as sby_file:
@@ -183,15 +184,15 @@
                     new_test["status"] = "error"
                     new_test["info"] = {
                         "type": node.get("type", ""),
                         "message": node.get("message", ""),
                     }
                 tests.append(new_test)
 
-        self._result = self.SbyTaskResult(
+        self._result = SbyTaskResult(
             passed=errors == 0 and failures == 0,
             raw_result=raw_xml,
             stdout=stdout, stderr=stderr,
             test_count=len(tests),
             tests=tests,
             failures=failures, errors=errors, skipped=skipped,
         )
```

### Comparing `magia_flow-0.2.0/magia_flow/online/digitaljs/Dockerfile` & `magia_flow-0.2.1/magia_flow/online/digitaljs/Dockerfile`

 * *Files identical despite different names*

### Comparing `magia_flow-0.2.0/magia_flow/online/digitaljs.py` & `magia_flow-0.2.1/magia_flow/online/digitaljs.py`

 * *Files identical despite different names*

### Comparing `magia_flow-0.2.0/magia_flow/oss_cad.py` & `magia_flow-0.2.1/magia_flow/oss_cad.py`

 * *Files identical despite different names*

### Comparing `magia_flow-0.2.0/magia_flow/simulation/general.py` & `magia_flow-0.2.1/magia_flow/simulation/general.py`

 * *Files identical despite different names*

### Comparing `magia_flow-0.2.0/magia_flow/simulation/surfer.py` & `magia_flow-0.2.1/magia_flow/simulation/surfer.py`

 * *Files identical despite different names*

### Comparing `magia_flow-0.2.0/magia_flow/simulation/verilator.py` & `magia_flow-0.2.1/magia_flow/simulation/verilator.py`

 * *Files identical despite different names*

### Comparing `magia_flow-0.2.0/pyproject.toml` & `magia_flow-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 [tool.ruff.lint.per-file-ignores]
 
 "tests/**" = ["S101", "S311"]
 
 [tool.poetry]
 name = "magia-flow"
-version = "0.2.0"
+version = "0.2.1"
 description = "Design flow integration and automation with Magia"
 readme = "README.md"
 authors = ["khwong-c64 <kin.hin.wong.c@gmail.com>"]
 license = "LICENSE"
 
 packages = [
     { include = "magia_flow" },
```

### Comparing `magia_flow-0.2.0/PKG-INFO` & `magia_flow-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magia-flow
-Version: 0.2.0
+Version: 0.2.1
 Summary: Design flow integration and automation with Magia
 License: LICENSE
 Keywords: Verilog HDL,SystemVerilog,Synthesizable,RTL,HDL,Hardware Description Language,Code Generation,FPGA,ASIC,EDA,RTL Design
 Author: khwong-c64
 Author-email: kin.hin.wong.c@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

