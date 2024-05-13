# Comparing `tmp/pyc4-1.0.0.tar.gz` & `tmp/pyc4-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyc4-1.0.0.tar", last modified: Mon Aug 28 13:20:14 2023, max compression
+gzip compressed data, was "pyc4-1.0.1.tar", last modified: Mon May 13 10:20:50 2024, max compression
```

## Comparing `pyc4-1.0.0.tar` & `pyc4-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:20:14.875779 pyc4-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (999)    18027 2023-08-28 13:19:59.000000 pyc4-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     1058 2023-08-28 13:20:14.875779 pyc4-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      481 2023-08-28 13:19:59.000000 pyc4-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (999)    19962 2023-08-28 13:19:59.000000 pyc4-1.0.0/c4.c
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:20:14.875779 pyc4-1.0.0/pyc4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     1058 2023-08-28 13:20:14.000000 pyc4-1.0.0/pyc4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      170 2023-08-28 13:20:14.000000 pyc4-1.0.0/pyc4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 13:20:14.000000 pyc4-1.0.0/pyc4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 13:20:14.000000 pyc4-1.0.0/pyc4.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)        3 2023-08-28 13:20:14.000000 pyc4-1.0.0/pyc4.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 13:20:14.875779 pyc4-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      814 2023-08-28 13:19:59.000000 pyc4-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:20:50.979135 pyc4-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    18027 2024-05-13 10:20:42.000000 pyc4-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-13 10:20:50.979135 pyc4-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-13 10:20:42.000000 pyc4-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19724 2024-05-13 10:20:42.000000 pyc4-1.0.1/c4.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:20:50.979135 pyc4-1.0.1/pyc4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-13 10:20:50.000000 pyc4-1.0.1/pyc4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 10:20:50.000000 pyc4-1.0.1/pyc4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:20:50.000000 pyc4-1.0.1/pyc4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:20:50.000000 pyc4-1.0.1/pyc4.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-13 10:20:50.000000 pyc4-1.0.1/pyc4.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:20:50.979135 pyc4-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-13 10:20:42.000000 pyc4-1.0.1/setup.py
```

### Comparing `pyc4-1.0.0/LICENSE` & `pyc4-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyc4-1.0.0/PKG-INFO` & `pyc4-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyc4
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python extension to run C code in Python
 Home-page: https://github.com/donno2048/pyc4
 Author: Elisha Hollander
 Author-email: just4now666666@gmail.com
 License: GPL-2.0
 Project-URL: Documentation, https://github.com/donno2048/pyc4#readme
 Project-URL: Bug Reports, https://github.com/donno2048/pyc4/issues
@@ -29,22 +29,22 @@
 The first argument is the code the rest are the `argv`
 
 ```py
 >>> import c4
 >>>
 >>> c4.execute(r"""
 ... int main() {
-...     printf("hi");
+...     printf("hi\n");
 ...     return 0;
 ... }
 ... """)
 hi
-exit code: 0
+0
 >>> c4.execute(r"""
 ... int main(int argc, char **argv) {
-...     printf("%s", argv[0]);
-...     return 0;
+...     printf("%s\n", argv[0]);
+...     return 1;
 ... }
 ... """, "hi")
 hi
-exit code: 0
+1
 ```
```

### Comparing `pyc4-1.0.0/c4.c` & `pyc4-1.0.1/c4.c`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 // identifier offsets (since we can't create an ident struct)
 enum { Tk, Hash, Name, Class, Type, Val, HClass, HType, HVal, Idsz };
 
 void next()
 {
   char *pp;
 
-  while (tk = *p) {
+  while ((tk = *p)) {
     ++p;
-    if (tk == '\n') ++line;
+    if (tk == '\n') line++;
     else if (tk == '#') {
       while (*p != 0 && *p != '\n') ++p;
     }
     else if ((tk >= 'a' && tk <= 'z') || (tk >= 'A' && tk <= 'Z') || tk == '_') {
       pp = p - 1;
       while ((*p >= 'a' && *p <= 'z') || (*p >= 'A' && *p <= 'Z') || (*p >= '0' && *p <= '9') || *p == '_')
         tk = tk * 147 + *p++;
@@ -64,15 +64,15 @@
       }
       id[Name] = (int)pp;
       id[Hash] = tk;
       tk = id[Tk] = Id;
       return;
     }
     else if (tk >= '0' && tk <= '9') {
-      if (ival = tk - '0') { while (*p >= '0' && *p <= '9') ival = ival * 10 + *p++ - '0'; }
+      if ((ival = tk - '0')) { while (*p >= '0' && *p <= '9') ival = ival * 10 + *p++ - '0'; }
       else if (*p == 'x' || *p == 'X') {
         while ((tk = *++p) && ((tk >= '0' && tk <= '9') || (tk >= 'a' && tk <= 'f') || (tk >= 'A' && tk <= 'F')))
           ival = ival * 16 + (tk & 15) + (tk >= 'A' ? 9 : 0);
       }
       else { while (*p >= '0' && *p <= '7') ival = ival * 8 + *p++ - '0'; }
       tk = Num;
       return;
@@ -121,15 +121,15 @@
   int t, *d;
 
   if (!tk) { printf("%d: unexpected eof in expression\n", line); exit(-1); }
   else if (tk == Num) { *++e = IMM; *++e = ival; next(); ty = INT; }
   else if (tk == '"') {
     *++e = IMM; *++e = ival; next();
     while (tk == '"') next();
-    data = (char *)((int)data + sizeof(int) & -sizeof(int)); ty = PTR;
+    data = (char *)(((int)data + sizeof(int)) & -sizeof(int)); ty = PTR;
   }
   else if (tk == Sizeof) {
     next(); if (tk == '(') next(); else { printf("%d: open paren expected in sizeof\n", line); exit(-1); }
     ty = INT; if (tk == Int) next(); else if (tk == Char) { next(); ty = CHAR; }
     while (tk == Mul) { next(); ty = ty + PTR; }
     if (tk == ')') next(); else { printf("%d: close paren expected in sizeof\n", line); exit(-1); }
     *++e = IMM; *++e = (ty == CHAR) ? sizeof(char) : sizeof(int);
@@ -314,15 +314,15 @@
     if (tk == ';') next(); else { printf("%d: semicolon expected\n", line); exit(-1); }
   }
 }
 
 int run(char *code, int argc, char **argv)
 {
   int bt, ty, poolsz, *idmain;
-  int *pc, *sp, *bp, a, cycle; // vm registers
+  int *pc, *sp, *bp, a; // vm registers
   int i, *t; // temps
 
   poolsz = 256*1024; // arbitrary size
   if (!(sym = malloc(poolsz))) { printf("could not malloc(%d) symbol area\n", poolsz); return -1; }
   if (!(le = e = malloc(poolsz))) { printf("could not malloc(%d) text area\n", poolsz); return -1; }
   if (!(data = malloc(poolsz))) { printf("could not malloc(%d) data area\n", poolsz); return -1; }
   if (!(sp = malloc(poolsz))) { printf("could not malloc(%d) stack area\n", poolsz); return -1; }
@@ -334,17 +334,16 @@
   p = "char else enum if int return sizeof while "
       "open read close printf malloc free memset memcmp exit void main";
   i = Char; while (i <= While) { next(); id[Tk] = i++; } // add keywords to symbol table
   i = OPEN; while (i <= EXIT) { next(); id[Class] = Sys; id[Type] = INT; id[Val] = i++; } // add library to symbol table
   next(); id[Tk] = Char; // handle void type
   next(); idmain = id; // keep track of main
 
-  if (!(lp = p = malloc(poolsz))) { printf("could not malloc(%d) source area\n", poolsz); return -1; }
-  for (i = 0; i < poolsz - 1 && (p[i] = code[i]); i++);
-  p[i] = 0;
+  p = code;
+
   // parse declarations
   line = 1;
   next();
   while (tk) {
     bt = INT; // basetype
     if (tk == Int) next();
     else if (tk == Char) { next(); bt = CHAR; }
@@ -443,17 +442,16 @@
   *--sp = EXIT; // call exit if main returns
   *--sp = PSH; t = sp;
   *--sp = argc;
   *--sp = (int)argv;
   *--sp = (int)t;
 
   // run...
-  cycle = 0;
   while (1) {
-    i = *pc++; ++cycle;
+    i = *pc++;
     if      (i == LEA) a = (int)(bp + *pc++);                             // load local address
     else if (i == IMM) a = *pc++;                                         // load global address or immediate
     else if (i == JMP) pc = (int *)*pc;                                   // jump
     else if (i == JSR) { *--sp = (int)(pc + 1); pc = (int *)*pc; }        // jump to subroutine
     else if (i == BZ)  pc = a ? pc + 1 : (int *)*pc;                      // branch if zero
     else if (i == BNZ) pc = a ? (int *)*pc : pc + 1;                      // branch if not zero
     else if (i == ENT) { *--sp = (int)bp; bp = sp; sp = sp - *pc++; }     // enter subroutine
@@ -486,35 +484,34 @@
     else if (i == READ) a = read(sp[2], (char *)sp[1], *sp);
     else if (i == CLOS) a = close(*sp);
     else if (i == PRTF) { t = sp + pc[1]; a = printf((char *)t[-1], t[-2], t[-3], t[-4], t[-5], t[-6]); }
     else if (i == MALC) a = (int)malloc(*sp);
     else if (i == FREE) free((void *)*sp);
     else if (i == MSET) a = (int)memset((char *)sp[2], sp[1], *sp);
     else if (i == MCMP) a = memcmp((char *)sp[2], (char *)sp[1], *sp);
-    else if (i == EXIT) { printf("\nexit code: %d\n", *sp, cycle); return *sp; }
-    else { printf("unknown instruction = %d! cycle = %d\n", i, cycle); return -1; }
+    else if (i == EXIT) return *sp;
+    else { printf("unknown instruction = %d\n", i); return -1; }
   }
 }
 const static inline PyObject *execute(const PyObject * self, const PyObject *const *args, const Py_ssize_t nargs) {
   if (!nargs) {
     PyErr_SetString(PyExc_TypeError, "execute() takes at least 1 positional argument (0 given)");
     return NULL;
   }
   char **argv = malloc(sizeof(char*) * (nargs - 1));
   if (!PyUnicode_Check(args[0])) Error;
   for (int i = 1; i < nargs; i++) {
     if (!PyUnicode_Check(args[i])) Error;
     argv[i - 1] = PyUnicode_AsUTF8(args[i]);
   }
-  run(PyUnicode_AsUTF8(args[0]), nargs - 1, argv);
-  Py_RETURN_NONE;
+  return PyLong_FromLong(run(PyUnicode_AsUTF8(args[0]), nargs - 1, argv));
 }
 static PyMethodDef c4_methods[] = {
   {"execute", execute, METH_FASTCALL, "Execute C code"},
   {NULL, NULL, 0, NULL}
 };
 static struct PyModuleDef c4 = {PyModuleDef_HEAD_INIT, "c4", NULL, -1, c4_methods};
 PyMODINIT_FUNC PyInit_c4(void){return PyModule_Create(&c4);}
 #ifdef __cplusplus
 }
 #endif
-#endif
+#endif
```

### Comparing `pyc4-1.0.0/pyc4.egg-info/PKG-INFO` & `pyc4-1.0.1/pyc4.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyc4
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python extension to run C code in Python
 Home-page: https://github.com/donno2048/pyc4
 Author: Elisha Hollander
 Author-email: just4now666666@gmail.com
 License: GPL-2.0
 Project-URL: Documentation, https://github.com/donno2048/pyc4#readme
 Project-URL: Bug Reports, https://github.com/donno2048/pyc4/issues
@@ -29,22 +29,22 @@
 The first argument is the code the rest are the `argv`
 
 ```py
 >>> import c4
 >>>
 >>> c4.execute(r"""
 ... int main() {
-...     printf("hi");
+...     printf("hi\n");
 ...     return 0;
 ... }
 ... """)
 hi
-exit code: 0
+0
 >>> c4.execute(r"""
 ... int main(int argc, char **argv) {
-...     printf("%s", argv[0]);
-...     return 0;
+...     printf("%s\n", argv[0]);
+...     return 1;
 ... }
 ... """, "hi")
 hi
-exit code: 0
+1
 ```
```

### Comparing `pyc4-1.0.0/setup.py` & `pyc4-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, Extension
 setup(
     name='pyc4',
-    version='1.0.0',
+    version='1.0.1',
     license='GPL-2.0',
     author='Elisha Hollander',
     author_email='just4now666666@gmail.com',
     description='A Python extension to run C code in Python',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url='https://github.com/donno2048/pyc4',
@@ -16,8 +16,8 @@
     },
     ext_modules=[Extension('c4', ['c4.c'])],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3"
     ],
     zip_safe = False,
-)
+)
```

