# Comparing `tmp/anycrc-0.6.2.tar.gz` & `tmp/anycrc-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.6.2.tar", last modified: Sun May 12 15:55:06 2024, max compression
+gzip compressed data, was "anycrc-0.6.3.tar", last modified: Mon May 13 16:49:28 2024, max compression
```

## Comparing `anycrc-0.6.2.tar` & `anycrc-0.6.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:55:06.949481 anycrc-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-12 15:55:00.000000 anycrc-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-12 15:55:06.949481 anycrc-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-12 15:55:00.000000 anycrc-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:55:06.945481 anycrc-0.6.2/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:55:06.945481 anycrc-0.6.2/lib/crcany/
--rw-r--r--   0 runner    (1001) docker     (127)    25327 2024-05-12 15:55:00.000000 anycrc-0.6.2/lib/crcany/crc.c
--rw-r--r--   0 runner    (1001) docker     (127)    18945 2024-05-12 15:55:00.000000 anycrc-0.6.2/lib/crcany/model.c
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-12 15:55:00.000000 anycrc-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 15:55:06.949481 anycrc-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 15:55:00.000000 anycrc-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:55:06.945481 anycrc-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:55:06.945481 anycrc-0.6.2/src/anycrc/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-12 15:55:00.000000 anycrc-0.6.2/src/anycrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-12 15:55:00.000000 anycrc-0.6.2/src/anycrc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-12 15:55:00.000000 anycrc-0.6.2/src/anycrc/anycrc.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    17619 2024-05-12 15:55:00.000000 anycrc-0.6.2/src/anycrc/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:55:06.949481 anycrc-0.6.2/src/anycrc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-12 15:55:06.000000 anycrc-0.6.2/src/anycrc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-12 15:55:06.000000 anycrc-0.6.2/src/anycrc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 15:55:06.000000 anycrc-0.6.2/src/anycrc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-12 15:55:06.000000 anycrc-0.6.2/src/anycrc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:28.148919 anycrc-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-13 16:49:23.000000 anycrc-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-13 16:49:28.148919 anycrc-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-13 16:49:23.000000 anycrc-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:28.144919 anycrc-0.6.3/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:28.144919 anycrc-0.6.3/lib/crcany/
+-rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-05-13 16:49:23.000000 anycrc-0.6.3/lib/crcany/crc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18945 2024-05-13 16:49:23.000000 anycrc-0.6.3/lib/crcany/model.c
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-13 16:49:23.000000 anycrc-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:49:28.148919 anycrc-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-13 16:49:23.000000 anycrc-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:28.144919 anycrc-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:28.144919 anycrc-0.6.3/src/anycrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 16:49:23.000000 anycrc-0.6.3/src/anycrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-13 16:49:23.000000 anycrc-0.6.3/src/anycrc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-13 16:49:23.000000 anycrc-0.6.3/src/anycrc/anycrc.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    17619 2024-05-13 16:49:23.000000 anycrc-0.6.3/src/anycrc/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:28.148919 anycrc-0.6.3/src/anycrc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-13 16:49:28.000000 anycrc-0.6.3/src/anycrc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-13 16:49:28.000000 anycrc-0.6.3/src/anycrc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:49:28.000000 anycrc-0.6.3/src/anycrc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 16:49:28.000000 anycrc-0.6.3/src/anycrc.egg-info/top_level.txt
```

### Comparing `anycrc-0.6.2/LICENSE` & `anycrc-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anycrc-0.6.2/PKG-INFO` & `anycrc-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time. It takes advantage of crcany's ability to efficiently combine multiple CRCs to parallelize the CRC's calculation.
```

### Comparing `anycrc-0.6.2/README.md` & `anycrc-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `anycrc-0.6.2/lib/crcany/crc.c` & `anycrc-0.6.3/lib/crcany/crc.c`

 * *Files 0% similar despite different names*

```diff
@@ -143,30 +143,32 @@
 // call, and then only on little-endian machines if the CRC is not reflected,
 // or on big-endian machines if the CRC is reflected.
 static inline word_t swap(word_t x) {
     return swaplow(x, WORDCHARS);
 }
 
 int crc_table_wordwise(model_t *model, unsigned little, unsigned word_bits) {
+    unsigned word_bytes = word_bits >> 3;
+    
     if(model->table_word == NULL) {
-        model->table_word = (word_t*) malloc(WORDCHARS * 256);
+        model->table_word = (word_t*) malloc(WORDCHARS * word_bytes * 256);
         
         if(model->table_word == NULL) {
             return 1;
         }
     }
     
     unsigned opp = little ^ model->ref;
     unsigned top =
         model->ref ? 0 :
                      word_bits - (model->width > 8 ? model->width : 8);
     word_t xor = model->xorout;
     if (model->width < 8 && !model->ref)
         xor <<= 8 - model->width;
-    unsigned word_bytes = word_bits >> 3;
+    
     for (unsigned k = 0; k < 256; k++) {
         word_t crc = model->table_byte[k];
         model->table_word[k] = opp ? swaplow(crc << top, word_bytes) :
                                         crc << top;
         for (unsigned n = 1; n < (word_bits >> 3); n++) {
             crc ^= xor;
             if (model->ref)
@@ -248,19 +250,19 @@
                     ^ model->table_word[(WORDCHARS - 7) * 256 + ((crc >> 48) & 0xff)]
                     ^ model->table_word[(WORDCHARS - 8) * 256 + ((crc >> 56) & 0xff)
 #if WORDCHARS > 8
                                                                    ]
                     ^ model->table_word[(WORDCHARS - 9) * 256 + ((crc >> 64) & 0xff)]
                     ^ model->table_word[(WORDCHARS - 10) * 256 + ((crc >> 72) & 0xff)]
                     ^ model->table_word[(WORDCHARS - 11) * 256 + ((crc >> 80) & 0xff)]
-                    ^ model->table_word[WORDCHARS - 12 * 256 + ((crc >> 88) & 0xff)]
-                    ^ model->table_word[WORDCHARS - 13 * 256 + ((crc >> 96) & 0xff)]
-                    ^ model->table_word[WORDCHARS - 14 * 256 + ((crc >> 104) & 0xff)]
-                    ^ model->table_word[WORDCHARS - 15 * 256 + ((crc >> 112) & 0xff)]
-                    ^ model->table_word[WORDCHARS - 16 * 256 + (crc >> 120)
+                    ^ model->table_word[(WORDCHARS - 12) * 256 + ((crc >> 88) & 0xff)]
+                    ^ model->table_word[(WORDCHARS - 13) * 256 + ((crc >> 96) & 0xff)]
+                    ^ model->table_word[(WORDCHARS - 14) * 256 + ((crc >> 104) & 0xff)]
+                    ^ model->table_word[(WORDCHARS - 15) * 256 + ((crc >> 112) & 0xff)]
+                    ^ model->table_word[(WORDCHARS - 16) * 256 + (crc >> 120)
 #endif
 #endif
 #endif
                                                                     ];
                 buf += WORDCHARS;
                 len -= WORDCHARS;
             } while (len >= WORDCHARS);
@@ -501,15 +503,15 @@
         crc = reverse(crc, model->width);
     return crc;
 }
 
 word_t crc_parallel(model_t *model, word_t crc, void const *dat, size_t len, int *error) {
     short nthreads = omp_get_max_threads();
     
-    word_t* crc_p = (word_t*)malloc((nthreads - 1) * sizeof(word_t));
+    word_t* crc_p = (word_t*)malloc((nthreads - 1) * WORDCHARS);
     
     if(crc_p == NULL) {
         error = 1;
         return crc;
     }
     
     size_t block_len = len / nthreads;
```

### Comparing `anycrc-0.6.2/lib/crcany/model.c` & `anycrc-0.6.3/lib/crcany/model.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.6.2/setup.py` & `anycrc-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         
 else:
     compile_args = ['-fopenmp', '-O2']
     link_args = ['-fopenmp', '-O2']
     
 setup(
     name = 'anycrc',
-    version = '0.6.2',
+    version = '0.6.3',
     package_dir = {"": "src"},
     cmdclass={"build_ext": Build},
     ext_modules = [
         Extension(
             name='anycrc.anycrc',
             extra_compile_args=compile_args,
             extra_link_args=link_args,
```

### Comparing `anycrc-0.6.2/src/anycrc/anycrc.pyx` & `anycrc-0.6.3/src/anycrc/anycrc.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # Copyright (c) 2024 Hussain Al Marzooq
 
 from libc.stdint cimport uintmax_t
 from .models import models, aliases
 import sys
 
 ctypedef uintmax_t word_t
-cdef bint parallel = True
 
 cdef extern from '../../lib/crcany/model.h':
-    cdef const unsigned char WORDCHARS
-    
     ctypedef struct model_t:
         unsigned short width
         short cycle
         short back
         char ref
         char rev
         char *name
@@ -39,26 +36,27 @@
     cdef word_t crc_slice16(model_t *model, word_t crc, const void* dat, size_t len)
     
     cdef word_t crc_parallel(model_t *model, word_t crc, const void *dat, size_t len, int *error)
     
     cdef int crc_table_combine(model_t *model)
     cdef word_t crc_combine(model_t *model, word_t crc1, word_t crc2, uintmax_t len2);
     
+cdef bint parallel = True
+word_width = 64 if sys.maxsize > 2 ** 32 else 32
+
 cdef class CRC:
     cdef model_t model
     cdef word_t register
-    cdef unsigned word_width
     
     def __init__(self, width, poly, init, ref_in, ref_out, xor_out, check=0, residue=0):
         cdef unsigned endian = 1 if sys.byteorder == 'little' else 0
-        self.word_width = 64 if sys.maxsize > 2 ** 32 else 32
         refin = 'true' if ref_in else 'false'
         refout = 'true' if ref_out else 'false'
         
-        if width > self.word_width:
+        if width > word_width:
             raise ValueError('CRC width is larger than the system\'s (or python\'s) maximum integer size')
             
         string = f'width={width} poly={poly} init={init} refin={refin} refout={refout} xorout={xor_out} check={check} residue={residue} name=""'.encode('utf-8')
         
         cdef int error_code = read_model(&self.model, string, 0)
         
         if error_code != 0:
@@ -67,15 +65,15 @@
         process_model(&self.model)
         
         error_code = crc_table_bytewise(&self.model)
         
         if error_code == 1:
             raise MemoryError('Out of memory error')
             
-        error_code = crc_table_slice16(&self.model, endian, self.word_width)
+        error_code = crc_table_slice16(&self.model, endian, word_width)
         
         if error_code == 1:
             raise MemoryError('Out of memory error')
             
         error_code = crc_table_combine(&self.model)
         
         if error_code == 1:
```

### Comparing `anycrc-0.6.2/src/anycrc/models.py` & `anycrc-0.6.3/src/anycrc/models.py`

 * *Files identical despite different names*

### Comparing `anycrc-0.6.2/src/anycrc.egg-info/PKG-INFO` & `anycrc-0.6.3/src/anycrc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time. It takes advantage of crcany's ability to efficiently combine multiple CRCs to parallelize the CRC's calculation.
```

