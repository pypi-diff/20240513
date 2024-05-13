# Comparing `tmp/jaxfi-0.7.1-py3-none-any.whl.zip` & `tmp/jaxfi-0.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 16182 bytes, number of entries: 15
--rw-rw-r--  2.0 unx      524 b- defN 24-May-01 17:37 jaxfi/__init__.py
+Zip file size: 17144 bytes, number of entries: 16
+-rw-rw-r--  2.0 unx      576 b- defN 24-May-13 17:48 jaxfi/__init__.py
 -rw-rw-r--  2.0 unx     7166 b- defN 24-May-01 17:37 jaxfi/api.py
 -rw-rw-r--  2.0 unx     2679 b- defN 24-May-01 17:37 jaxfi/dynamic_lib_loading.py
 -rw-rw-r--  2.0 unx    16362 b- defN 24-May-01 17:37 jaxfi/enumerated_jnp_members.py
 -rw-rw-r--  2.0 unx      114 b- defN 23-Apr-26 03:31 jaxfi/globals.py
 -rw-rw-r--  2.0 unx      169 b- defN 24-Jan-24 19:31 jaxfi/types.py
 -rw-rw-r--  2.0 unx     6345 b- defN 24-May-01 17:37 jaxfi/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Jan-24 19:29 jaxfi/experimental/__init__.py
+-rw-rw-r--  2.0 unx      104 b- defN 24-May-13 17:56 jaxfi/experimental/__init__.py
 -rw-rw-r--  2.0 unx     3035 b- defN 24-Jan-03 16:31 jaxfi/experimental/auto_pmap.py
+-rw-rw-r--  2.0 unx     2098 b- defN 24-May-13 17:49 jaxfi/experimental/device_cond.py
 -rw-rw-r--  2.0 unx     3517 b- defN 23-Nov-10 18:47 jaxfi/experimental/jit.py
--rw-rw-r--  2.0 unx     1068 b- defN 24-May-01 17:38 jaxfi-0.7.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6223 b- defN 24-May-01 17:38 jaxfi-0.7.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-01 17:38 jaxfi-0.7.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 24-May-01 17:38 jaxfi-0.7.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1158 b- defN 24-May-01 17:38 jaxfi-0.7.1.dist-info/RECORD
-15 files, 48458 bytes uncompressed, 14286 bytes compressed:  70.5%
+-rw-rw-r--  2.0 unx     1068 b- defN 24-May-13 19:50 jaxfi-0.7.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6223 b- defN 24-May-13 19:50 jaxfi-0.7.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-13 19:50 jaxfi-0.7.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 24-May-13 19:50 jaxfi-0.7.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1250 b- defN 24-May-13 19:50 jaxfi-0.7.2.dist-info/RECORD
+16 files, 50804 bytes uncompressed, 15106 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -21,26 +21,29 @@
 
 Filename: jaxfi/experimental/__init__.py
 Comment: 
 
 Filename: jaxfi/experimental/auto_pmap.py
 Comment: 
 
+Filename: jaxfi/experimental/device_cond.py
+Comment: 
+
 Filename: jaxfi/experimental/jit.py
 Comment: 
 
-Filename: jaxfi-0.7.1.dist-info/LICENSE
+Filename: jaxfi-0.7.2.dist-info/LICENSE
 Comment: 
 
-Filename: jaxfi-0.7.1.dist-info/METADATA
+Filename: jaxfi-0.7.2.dist-info/METADATA
 Comment: 
 
-Filename: jaxfi-0.7.1.dist-info/WHEEL
+Filename: jaxfi-0.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: jaxfi-0.7.1.dist-info/top_level.txt
+Filename: jaxfi-0.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: jaxfi-0.7.1.dist-info/RECORD
+Filename: jaxfi-0.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jaxfi/__init__.py

```diff
@@ -2,14 +2,15 @@
 
 from .api import * # noqa: F403
 
 from .utils import resolve_device, resolve_dtype, default_dtype_for_device  # noqa: F401
 from .utils import get_default_device, get_default_dtype  # noqa: F401
 from .utils import set_default_dtype, set_default_device  # noqa: F401
 from .experimental.jit import autojit, nestedautojit  # noqa: F401
+from .experimental.device_cond import device_select
 
 jaxm = sys.modules[__name__]
 try:
     from importlib.metadata import version
 except ModuleNotFoundError:
     from importlib_metadata import version
 __version__ = version(__name__)
```

## jaxfi/experimental/__init__.py

```diff
@@ -0,0 +1,7 @@
+00000000: 6672 6f6d 202e 6465 7669 6365 5f63 6f6e  from .device_con
+00000010: 6420 696d 706f 7274 2064 6576 6963 655f  d import device_
+00000020: 7365 6c65 6374 2023 206e 6f71 613a 2046  select # noqa: F
+00000030: 3430 310a 6672 6f6d 202e 6a69 7420 696d  401.from .jit im
+00000040: 706f 7274 206e 6573 7465 6461 7574 6f6a  port nestedautoj
+00000050: 6974 2c20 6175 746f 6a69 7420 2320 6e6f  it, autojit # no
+00000060: 7161 3a20 4634 3031                      qa: F401
```

## Comparing `jaxfi-0.7.1.dist-info/LICENSE` & `jaxfi-0.7.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jaxfi-0.7.1.dist-info/METADATA` & `jaxfi-0.7.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxfi
-Version: 0.7.1
+Version: 0.7.2
 Summary: Friendly Interface to JAX, that behaves similar to PyTorch while maintaining compatibility.
 Author: Robert Dyro
 Author-email: Robert Dyro <robert.dyro@gmail.com>
 Project-URL: Homepage, https://github.com/rdyro/jaxfi-JAXFriendlyInterface
 Project-URL: Bug Tracker, https://github.com/rdyro/jaxfi-JAXFriendlyInterface
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `jaxfi-0.7.1.dist-info/RECORD` & `jaxfi-0.7.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-jaxfi/__init__.py,sha256=qPGWAslLYk2I2asB8P4G93Si6RNqjlW4kzIzkrNYP8c,524
+jaxfi/__init__.py,sha256=CY5U8e9dnR87WvmUs-wZvtQy4fWKqVWc6oeKWiFfg4w,576
 jaxfi/api.py,sha256=g8491iuPez1pKHLTsc7CWK3G3Ny9JHvvJgX_1SLX0ro,7166
 jaxfi/dynamic_lib_loading.py,sha256=vka7l2bbUwfGIZZsoWWHwEGUHVE21mwilUZqPB2r7do,2679
 jaxfi/enumerated_jnp_members.py,sha256=8i7LPXSwF5y8Ps-XRhXg8c90E4w1aJKK0MDF3KOtyKg,16362
 jaxfi/globals.py,sha256=PVptT3X5WjKXe3SO6yPkbBQ-1nIKpRHu5ehue2fS5JQ,114
 jaxfi/types.py,sha256=g6QfE9scN3B-YsVMtX35rJlZj-z99zN-MgD19mXHExU,169
 jaxfi/utils.py,sha256=hoDvWxfg7j5TOaIaibxNCDEKHz1DZ5EZN-DxIpfs0x4,6345
-jaxfi/experimental/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+jaxfi/experimental/__init__.py,sha256=Q8Iy9k57bPB2M0FXW0kY94zamVsDRKkhWvqR3sPun7k,104
 jaxfi/experimental/auto_pmap.py,sha256=gZlWfEcKjApYu6yfkefKukc7ORFdIMe1uf7USxazPx8,3035
+jaxfi/experimental/device_cond.py,sha256=XhzteS01y0plG-Th2h_5jECLh5KbJumbbXN_5zJWKhA,2098
 jaxfi/experimental/jit.py,sha256=jDwrcaAHWRxQHZxHiBTzBP56lvRH4rRCKotZOYvg5bQ,3517
-jaxfi-0.7.1.dist-info/LICENSE,sha256=Y_vRJ8ePCccT_XKyn3V3moM24W2NoXqcKq0cSeZhCng,1068
-jaxfi-0.7.1.dist-info/METADATA,sha256=PcOUo2GSU8RBXJ2c_IWNFFW_tHcCQCC7JJ5WHr95Y9o,6223
-jaxfi-0.7.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-jaxfi-0.7.1.dist-info/top_level.txt,sha256=pMa_rDYgwq1q_ibjcWBU-h-oDQfzeSB_5UZ_I-76Pdw,6
-jaxfi-0.7.1.dist-info/RECORD,,
+jaxfi-0.7.2.dist-info/LICENSE,sha256=Y_vRJ8ePCccT_XKyn3V3moM24W2NoXqcKq0cSeZhCng,1068
+jaxfi-0.7.2.dist-info/METADATA,sha256=ucACEFj1DdtaOMygB_2JsTnSboceLakB_QF-b0rAyuU,6223
+jaxfi-0.7.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+jaxfi-0.7.2.dist-info/top_level.txt,sha256=pMa_rDYgwq1q_ibjcWBU-h-oDQfzeSB_5UZ_I-76Pdw,6
+jaxfi-0.7.2.dist-info/RECORD,,
```

