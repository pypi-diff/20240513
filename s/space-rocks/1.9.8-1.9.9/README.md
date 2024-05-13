# Comparing `tmp/space_rocks-1.9.8.tar.gz` & `tmp/space_rocks-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_rocks-1.9.8.tar", max compression
+gzip compressed data, was "space_rocks-1.9.9.tar", max compression
```

## Comparing `space_rocks-1.9.8.tar` & `space_rocks-1.9.9.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rwxr-xr-x   0        0        0     1067 2024-04-01 10:44:27.849527 space_rocks-1.9.8/LICENSE
--rw-r--r--   0        0        0     1986 2024-04-15 15:14:00.101493 space_rocks-1.9.8/README.md
--rw-r--r--   0        0        0     1478 2024-04-22 12:54:19.721550 space_rocks-1.9.8/pyproject.toml
--rwxr-xr-x   0        0        0      520 2024-04-22 12:54:02.881550 space_rocks-1.9.8/rocks/__init__.py
--rw-r--r--   0        0        0     2191 2024-04-22 12:53:02.141549 space_rocks-1.9.8/rocks/bft.py
--rwxr-xr-x   0        0        0     5033 2024-04-01 10:44:28.129532 space_rocks-1.9.8/rocks/cache.py
--rw-r--r--   0        0        0    13323 2024-04-22 12:53:02.141549 space_rocks-1.9.8/rocks/cli.py
--rwxr-xr-x   0        0        0     7850 2024-04-01 10:44:28.101531 space_rocks-1.9.8/rocks/config.py
--rw-r--r--   0        0        0    44752 2024-04-22 12:53:02.141549 space_rocks-1.9.8/rocks/core.py
--rwxr-xr-x   0        0        0    33041 2024-04-01 10:44:28.129532 space_rocks-1.9.8/rocks/datacloud.py
--rw-r--r--   0        0        0    15355 2024-04-22 12:53:02.141549 space_rocks-1.9.8/rocks/index.py
--rwxr-xr-x   0        0        0      982 2024-04-01 10:44:28.105531 space_rocks-1.9.8/rocks/logging.py
--rw-r--r--   0        0        0     6430 2024-04-22 12:53:04.993549 space_rocks-1.9.8/rocks/metadata.py
--rwxr-xr-x   0        0        0     6300 2024-04-01 10:44:28.105531 space_rocks-1.9.8/rocks/plots.py
--rw-r--r--   0        0        0    13343 2024-04-22 12:53:02.141549 space_rocks-1.9.8/rocks/resolve.py
--rw-r--r--   0        0        0    13547 2024-04-22 12:53:02.141549 space_rocks-1.9.8/rocks/ssodnet.py
--rw-r--r--   0        0        0     3298 1970-01-01 00:00:00.000000 space_rocks-1.9.8/setup.py
--rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 space_rocks-1.9.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1067 2024-04-01 10:44:27.849527 space_rocks-1.9.9/LICENSE
+-rw-r--r--   0        0        0     1986 2024-04-15 15:14:00.101493 space_rocks-1.9.9/README.md
+-rw-r--r--   0        0        0     1478 2024-05-11 14:48:13.468866 space_rocks-1.9.9/pyproject.toml
+-rw-r--r--   0        0        0      520 2024-05-11 14:44:36.547858 space_rocks-1.9.9/rocks/__init__.py
+-rw-r--r--   0        0        0     2191 2024-05-01 11:56:14.028320 space_rocks-1.9.9/rocks/bft.py
+-rwxr-xr-x   0        0        0     5033 2024-04-01 10:44:28.129532 space_rocks-1.9.9/rocks/cache.py
+-rw-r--r--   0        0        0    13323 2024-05-01 11:56:14.028858 space_rocks-1.9.9/rocks/cli.py
+-rwxr-xr-x   0        0        0     7850 2024-04-01 10:44:28.101531 space_rocks-1.9.9/rocks/config.py
+-rw-r--r--   0        0        0    44752 2024-05-12 20:17:20.577352 space_rocks-1.9.9/rocks/core.py
+-rw-r--r--   0        0        0    33049 2024-04-30 19:21:22.619602 space_rocks-1.9.9/rocks/datacloud.py
+-rw-r--r--   0        0        0    15375 2024-05-11 14:43:22.929031 space_rocks-1.9.9/rocks/index.py
+-rwxr-xr-x   0        0        0      982 2024-04-01 10:44:28.105531 space_rocks-1.9.9/rocks/logging.py
+-rw-r--r--   0        0        0     6556 2024-05-11 14:46:30.924054 space_rocks-1.9.9/rocks/metadata.py
+-rwxr-xr-x   0        0        0     6300 2024-04-01 10:44:28.105531 space_rocks-1.9.9/rocks/plots.py
+-rw-r--r--   0        0        0    13343 2024-05-01 11:56:14.030522 space_rocks-1.9.9/rocks/resolve.py
+-rw-r--r--   0        0        0    13547 2024-05-01 11:56:14.031001 space_rocks-1.9.9/rocks/ssodnet.py
+-rw-r--r--   0        0        0     3413 1970-01-01 00:00:00.000000 space_rocks-1.9.9/PKG-INFO
```

### Comparing `space_rocks-1.9.8/LICENSE` & `space_rocks-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `space_rocks-1.9.8/README.md` & `space_rocks-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `space_rocks-1.9.8/pyproject.toml` & `space_rocks-1.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "space-rocks"
-version = "1.9.8"
+version = "1.9.9"
 description = "Python client for SsODNet data access."
 authors = ["Max Mahlke <max.mahlke@oca.eu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://rocks.readthedocs.io/en/latest/"
 documentation = "https://rocks.readthedocs.io/en/latest/"
 repository = "https://github.com/maxmahlke/rocks.git"
```

### Comparing `space_rocks-1.9.8/rocks/__init__.py` & `space_rocks-1.9.9/rocks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """For space rocks."""
 
 import inspect
 
 # Welcome to rocks
-__version__ = "1.9.8"
+__version__ = "1.9.9"
 
 # Only define user API if rocks is not called via command line
 context = inspect.stack()[-1].code_context
 if context is None or "rocks.cli" not in context[0]:
     # Expose API to user
     from .bft import load_bft  # noqa
     from .core import Rock  # noqa
```

### Comparing `space_rocks-1.9.8/rocks/bft.py` & `space_rocks-1.9.9/rocks/bft.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.9.8/rocks/cache.py` & `space_rocks-1.9.9/rocks/cache.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.9.8/rocks/cli.py` & `space_rocks-1.9.9/rocks/cli.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.9.8/rocks/config.py` & `space_rocks-1.9.9/rocks/config.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.9.8/rocks/core.py` & `space_rocks-1.9.9/rocks/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,15 +484,15 @@
 
     _convert_list_to_parameterlist: classmethod = pydantic.field_validator(
         "bibref", mode="before"
     )(lambda list_: ListWithAttributes([Bibref(**element) for element in list_]))
 
 
 class Yarkovsky(Parameter):
-    s: FloatValue = FloatValue(**{})
+    S: FloatValue = FloatValue(**{})
     a2: FloatValue = FloatValue(**{})
     snr: FloatValue = FloatValue(**{})
     dadt: FloatValue = FloatValue(**{})
     links: LinksParameter = LinksParameter(**{})
     bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
     method: List[Method] = [Method(**{})]
```

### Comparing `space_rocks-1.9.8/rocks/datacloud.py` & `space_rocks-1.9.9/rocks/datacloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -746,16 +746,16 @@
     number: List[Optional[int]] = pydantic.Field([None], alias="num")
     name: List[Optional[str]] = [""]
     color: List[Optional[str]] = [""]
     value: List[Optional[float]] = [np.nan]
     uncertainty: List[Optional[float]] = [np.nan]
     facility: List[Optional[str]] = [""]
     observer: List[Optional[str]] = [""]
-    epoch: List[Optional[float]] = [""]
-    delta_time: List[Optional[float]] = [""]
+    epoch: List[Optional[float]] = [np.nan]
+    delta_time: List[Optional[float]] = [np.nan]
     color_type: List[Optional[str]] = [""]
     id_filter_1: List[Optional[str]] = [""]
     id_filter_2: List[Optional[str]] = [""]
     phot_sys: List[Optional[str]] = [""]
     selection: List[Optional[int]] = [None]
     iddataset: List[Optional[int]] = [None]
```

### Comparing `space_rocks-1.9.8/rocks/index.py` & `space_rocks-1.9.9/rocks/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,14 +516,15 @@
                 "\n    Not using a cache. Set [dim]ROCKS_CACHE_DIR='no-cache'[/dim] to make this\n"
                 "    decision permanent.\n"
             )
             config.CACHELESS = True
             return
 
         config.PATH_CACHE.mkdir(parents=True)
+        print("\n")
 
     # Cache exists but index is missing
     else:
         logger.warning(
             "The local asteroid name-number index is missing. Downloading it now."
         )
```

### Comparing `space_rocks-1.9.8/rocks/logging.py` & `space_rocks-1.9.9/rocks/logging.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.9.8/rocks/metadata.py` & `space_rocks-1.9.9/rocks/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functionality for SsODNet metadata interaction with rocks."""
+
 from functools import lru_cache
 import html
 import json
 import re
 import unicodedata
 from urllib.request import urlretrieve, urlopen
 from urllib.error import HTTPError
@@ -10,14 +11,15 @@
 import requests
 import rich
 
 from rocks import config
 from rocks.logging import logger
 from rocks import ssodnet
 from rocks import __version__
+from rocks import index
 
 
 @lru_cache(None)
 def load_mappings():
     """Load SsODNet metadata mappings file from cache."""
 
     if config.CACHELESS or not config.PATH_MAPPINGS.is_file():
@@ -39,14 +41,16 @@
     """Retrieve the metadata JSON files from SsODNet to the cache directory.
 
     Parameter
     ---------
     which : str
         Which metadata to retrieve. Choose from ['mappings', 'authors'].
     """
+    if not config.PATH_INDEX.is_dir() and not config.CACHELESS:
+        index._ensure_index_exists()
 
     if which not in ["mappings", "authors", "citations"]:
         raise ValueError(
             f"'which' has to be in ['mappings', 'authors', 'citations'], received {which}."
         )
 
     if which == "citations":
```

### Comparing `space_rocks-1.9.8/rocks/plots.py` & `space_rocks-1.9.9/rocks/plots.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.9.8/rocks/resolve.py` & `space_rocks-1.9.9/rocks/resolve.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.9.8/rocks/ssodnet.py` & `space_rocks-1.9.9/rocks/ssodnet.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.9.8/setup.py` & `space_rocks-1.9.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,117 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: space-rocks
+Version: 1.9.9
+Summary: Python client for SsODNet data access.
+Home-page: https://rocks.readthedocs.io/en/latest/
+License: MIT
+Author: Max Mahlke
+Author-email: max.mahlke@oca.eu
+Requires-Python: >=3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: docs
+Requires-Dist: Levenshtein (>=0.16.0)
+Requires-Dist: aiodns (>=3.1.0)
+Requires-Dist: aiohttp (>=3.9.2)
+Requires-Dist: click (>=8.1.2)
+Requires-Dist: faust-cchardet (>=2.1.7)
+Requires-Dist: matplotlib (>=3.4.3)
+Requires-Dist: nest-asyncio (>=1.5.1,<2.0.0)
+Requires-Dist: numpy (>=1.21) ; python_version >= "3.7" and python_version < "3.11"
+Requires-Dist: numpy (>=1.24) ; python_version >= "3.11" and python_version < "4.0"
+Requires-Dist: pandas (>=1.3.5)
+Requires-Dist: platformdirs (>=2.6.2,<3.0.0)
+Requires-Dist: pydantic (>=2.0)
+Requires-Dist: rapidfuzz (>=3,<4)
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: rich (>=12.2.0)
+Project-URL: Documentation, https://rocks.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/maxmahlke/rocks.git
+Description-Content-Type: text/markdown
+
+<p align="center">
+  <img width="260" src="https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/logo_rocks.svg">
+</p>
+
+<p align="center">
+  <a href="https://github.com/maxmahlke/rocks#features"> Features </a> - <a href="https://github.com/maxmahlke/rocks#install"> Install </a> - <a href="https://github.com/maxmahlke/rocks#documentation"> Documentation </a>
+</p>
+
+<div align="center">
+  <a href="https://img.shields.io/pypi/pyversions/space-rocks">
+    <img src="https://img.shields.io/pypi/pyversions/space-rocks"/>
+  </a>
+  <a href="https://img.shields.io/pypi/v/space-rocks">
+    <img src="https://img.shields.io/pypi/v/space-rocks"/>
+  </a>
+  <a href="https://readthedocs.org/projects/rocks/badge/?version=latest">
+    <img src="https://readthedocs.org/projects/rocks/badge/?version=latest"/>
+  </a>
+  <a href="https://arxiv.org/abs/2209.10697">
+    <img src="https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg"/>
+  </a>
+</div>
+
+
+## Features
+
+Explore asteroid data on the command-line...
+
+``` sh
+$ rocks id 221
+(221) Eos
+
+$ rocks class Eos
+MB>Outer
+
+$ rocks albedo Eos
+0.136 +- 0.004
+
+$ rocks taxonomy Eos
+K
+
+$ rocks density Eos
+4.559e+03 +- 1.139e+03 kg/m$^3$
+```
+
+... and in a `python` script.
+
+``` python
+>>> import rocks
+>>> rocks.identify("1902ug")
+('Fortuna', 19)
+>>> ceres = rocks.Rock("ceres")
+>>> ceres.diameter.value
+848.4
+>>> ceres.diameter.unit
+'km'
+>>> ceres.mass.value
+9.384e+20
+>>> ceres.mass.error
+6.711e+17
+```
+
+## Install
+
+Install from PyPi using `pip`:
+
+     $ pip install space-rocks
+
+The minimum required `python` version is 3.8.
+
+
+## Documentation
 
-packages = \
-['rocks']
+Check out the documentation at [rocks.readthedocs.io](https://rocks.readthedocs.io/en/latest/) or run
 
-package_data = \
-{'': ['*']}
+     $ rocks docs
 
-install_requires = \
-['Levenshtein>=0.16.0',
- 'aiodns>=3.1.0',
- 'aiohttp>=3.9.2',
- 'click>=8.1.2',
- 'faust-cchardet>=2.1.7',
- 'matplotlib>=3.4.3',
- 'nest-asyncio>=1.5.1,<2.0.0',
- 'pandas>=1.3.5',
- 'platformdirs>=2.6.2,<3.0.0',
- 'pydantic>=2.0',
- 'rapidfuzz>=3,<4',
- 'requests>=2.26.0,<3.0.0',
- 'rich>=12.2.0']
-
-extras_require = \
-{':python_version >= "3.11" and python_version < "4.0"': ['numpy>=1.24'],
- ':python_version >= "3.7" and python_version < "3.11"': ['numpy>=1.21']}
-
-entry_points = \
-{'console_scripts': ['rocks = rocks.cli:cli_rocks']}
-
-setup_kwargs = {
-    'name': 'space-rocks',
-    'version': '1.9.8',
-    'description': 'Python client for SsODNet data access.',
-    'long_description': '<p align="center">\n  <img width="260" src="https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/logo_rocks.svg">\n</p>\n\n<p align="center">\n  <a href="https://github.com/maxmahlke/rocks#features"> Features </a> - <a href="https://github.com/maxmahlke/rocks#install"> Install </a> - <a href="https://github.com/maxmahlke/rocks#documentation"> Documentation </a>\n</p>\n\n<div align="center">\n  <a href="https://img.shields.io/pypi/pyversions/space-rocks">\n    <img src="https://img.shields.io/pypi/pyversions/space-rocks"/>\n  </a>\n  <a href="https://img.shields.io/pypi/v/space-rocks">\n    <img src="https://img.shields.io/pypi/v/space-rocks"/>\n  </a>\n  <a href="https://readthedocs.org/projects/rocks/badge/?version=latest">\n    <img src="https://readthedocs.org/projects/rocks/badge/?version=latest"/>\n  </a>\n  <a href="https://arxiv.org/abs/2209.10697">\n    <img src="https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg"/>\n  </a>\n</div>\n\n\n## Features\n\nExplore asteroid data on the command-line...\n\n``` sh\n$ rocks id 221\n(221) Eos\n\n$ rocks class Eos\nMB>Outer\n\n$ rocks albedo Eos\n0.136 +- 0.004\n\n$ rocks taxonomy Eos\nK\n\n$ rocks density Eos\n4.559e+03 +- 1.139e+03 kg/m$^3$\n```\n\n... and in a `python` script.\n\n``` python\n>>> import rocks\n>>> rocks.identify("1902ug")\n(\'Fortuna\', 19)\n>>> ceres = rocks.Rock("ceres")\n>>> ceres.diameter.value\n848.4\n>>> ceres.diameter.unit\n\'km\'\n>>> ceres.mass.value\n9.384e+20\n>>> ceres.mass.error\n6.711e+17\n```\n\n## Install\n\nInstall from PyPi using `pip`:\n\n     $ pip install space-rocks\n\nThe minimum required `python` version is 3.8.\n\n\n## Documentation\n\nCheck out the documentation at [rocks.readthedocs.io](https://rocks.readthedocs.io/en/latest/) or run\n\n     $ rocks docs\n\nFor a quick overview, check out the jupyter notebooks:\n\n[Basic Usage](https://github.com/maxmahlke/rocks/blob/master/docs/tutorials/rocks_basic_usage.ipynb) - [Bibliography Management](https://github.com/maxmahlke/rocks/blob/master/docs/tutorials/literature.ipynb)\n',
-    'author': 'Max Mahlke',
-    'author_email': 'max.mahlke@oca.eu',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://rocks.readthedocs.io/en/latest/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8',
-}
+For a quick overview, check out the jupyter notebooks:
 
+[Basic Usage](https://github.com/maxmahlke/rocks/blob/master/docs/tutorials/rocks_basic_usage.ipynb) - [Bibliography Management](https://github.com/maxmahlke/rocks/blob/master/docs/tutorials/literature.ipynb)
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,41 +1,39 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['rocks']
-package_data = \ {'': ['*']} install_requires = \ ['Levenshtein>=0.16.0',
-'aiodns>=3.1.0', 'aiohttp>=3.9.2', 'click>=8.1.2', 'faust-cchardet>=2.1.7',
-'matplotlib>=3.4.3', 'nest-asyncio>=1.5.1,<2.0.0', 'pandas>=1.3.5',
-'platformdirs>=2.6.2,<3.0.0', 'pydantic>=2.0', 'rapidfuzz>=3,<4',
-'requests>=2.26.0,<3.0.0', 'rich>=12.2.0'] extras_require = \ {':python_version
->= "3.11" and python_version < "4.0"': ['numpy>=1.24'], ':python_version >=
-"3.7" and python_version < "3.11"': ['numpy>=1.21']} entry_points = \
-{'console_scripts': ['rocks = rocks.cli:cli_rocks']} setup_kwargs = { 'name':
-'space-rocks', 'version': '1.9.8', 'description': 'Python client for SsODNet
-data access.', 'long_description': '
-  \n [https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/
-                               logo_rocks.svg]\n
-\n\n
-                   \n _F_e_a_t_u_r_e_s_ - _I_n_s_t_a_l_l_ - _D_o_c_u_m_e_n_t_a_t_i_o_n_ \n
-\n\n
- \n _\_n_ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_s_p_a_c_e_-_r_o_c_k_s_]_\_n_ \n _\_n_ _[_h_t_t_p_s_:_/_/
- _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_s_p_a_c_e_-_r_o_c_k_s_]_\_n_ \n _\_n_ _[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/
-   _r_o_c_k_s_/_b_a_d_g_e_/_?_v_e_r_s_i_o_n_=_l_a_t_e_s_t_]_\_n_ \n _\_n_ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_r_X_i_v_-
-                          _2_2_0_9_._1_0_6_9_7_-_f_9_f_1_0_7_._s_v_g_]_\_n_ \n
-\n\n\n## Features\n\nExplore asteroid data on the command-line...\n\n``` sh\n$
-rocks id 221\n(221) Eos\n\n$ rocks class Eos\nMB>Outer\n\n$ rocks albedo
-Eos\n0.136 +- 0.004\n\n$ rocks taxonomy Eos\nK\n\n$ rocks density
-Eos\n4.559e+03 +- 1.139e+03 kg/m$^3$\n```\n\n... and in a `python`
-script.\n\n``` python\n>>> import rocks\n>>> rocks.identify("1902ug")\n
-(\'Fortuna\', 19)\n>>> ceres = rocks.Rock("ceres")\n>>>
-ceres.diameter.value\n848.4\n>>> ceres.diameter.unit\n\'km\'\n>>>
-ceres.mass.value\n9.384e+20\n>>> ceres.mass.error\n6.711e+17\n```\n\n##
-Install\n\nInstall from PyPi using `pip`:\n\n $ pip install space-rocks\n\nThe
-minimum required `python` version is 3.8.\n\n\n## Documentation\n\nCheck out
-the documentation at [rocks.readthedocs.io](https://rocks.readthedocs.io/en/
-latest/) or run\n\n $ rocks docs\n\nFor a quick overview, check out the jupyter
-notebooks:\n\n[Basic Usage](https://github.com/maxmahlke/rocks/blob/master/
-docs/tutorials/rocks_basic_usage.ipynb) - [Bibliography Management](https://
-github.com/maxmahlke/rocks/blob/master/docs/tutorials/literature.ipynb)\n',
-'author': 'Max Mahlke', 'author_email': 'max.mahlke@oca.eu', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://rocks.readthedocs.io/en/
-latest/', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'extras_require': extras_require,
-'entry_points': entry_points, 'python_requires': '>=3.8', } setup
-(**setup_kwargs)
+Metadata-Version: 2.1 Name: space-rocks Version: 1.9.9 Summary: Python client
+for SsODNet data access. Home-page: https://rocks.readthedocs.io/en/latest/
+License: MIT Author: Max Mahlke Author-email: max.mahlke@oca.eu Requires-
+Python: >=3.8 Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Provides-
+Extra: docs Requires-Dist: Levenshtein (>=0.16.0) Requires-Dist: aiodns
+(>=3.1.0) Requires-Dist: aiohttp (>=3.9.2) Requires-Dist: click (>=8.1.2)
+Requires-Dist: faust-cchardet (>=2.1.7) Requires-Dist: matplotlib (>=3.4.3)
+Requires-Dist: nest-asyncio (>=1.5.1,<2.0.0) Requires-Dist: numpy (>=1.21) ;
+python_version >= "3.7" and python_version < "3.11" Requires-Dist: numpy
+(>=1.24) ; python_version >= "3.11" and python_version < "4.0" Requires-Dist:
+pandas (>=1.3.5) Requires-Dist: platformdirs (>=2.6.2,<3.0.0) Requires-Dist:
+pydantic (>=2.0) Requires-Dist: rapidfuzz (>=3,<4) Requires-Dist: requests
+(>=2.26.0,<3.0.0) Requires-Dist: rich (>=12.2.0) Project-URL: Documentation,
+https://rocks.readthedocs.io/en/latest/ Project-URL: Repository, https://
+github.com/maxmahlke/rocks.git Description-Content-Type: text/markdown
+    [https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/
+                                logo_rocks.svg]
+                      _F_e_a_t_u_r_e_s_ - _I_n_s_t_a_l_l_ - _D_o_c_u_m_e_n_t_a_t_i_o_n
+ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_s_p_a_c_e_-_r_o_c_k_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+       _p_y_p_i_/_v_/_s_p_a_c_e_-_r_o_c_k_s_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_r_o_c_k_s_/_b_a_d_g_e_/
+  _?_v_e_r_s_i_o_n_=_l_a_t_e_s_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_r_X_i_v_-_2_2_0_9_._1_0_6_9_7_-_f_9_f_1_0_7_._s_v_g_]
+## Features Explore asteroid data on the command-line... ``` sh $ rocks id 221
+(221) Eos $ rocks class Eos MB>Outer $ rocks albedo Eos 0.136 +- 0.004 $ rocks
+taxonomy Eos K $ rocks density Eos 4.559e+03 +- 1.139e+03 kg/m$^3$ ``` ... and
+in a `python` script. ``` python >>> import rocks >>> rocks.identify("1902ug")
+('Fortuna', 19) >>> ceres = rocks.Rock("ceres") >>> ceres.diameter.value 848.4
+>>> ceres.diameter.unit 'km' >>> ceres.mass.value 9.384e+20 >>>
+ceres.mass.error 6.711e+17 ``` ## Install Install from PyPi using `pip`: $ pip
+install space-rocks The minimum required `python` version is 3.8. ##
+Documentation Check out the documentation at [rocks.readthedocs.io](https://
+rocks.readthedocs.io/en/latest/) or run $ rocks docs For a quick overview,
+check out the jupyter notebooks: [Basic Usage](https://github.com/maxmahlke/
+rocks/blob/master/docs/tutorials/rocks_basic_usage.ipynb) - [Bibliography
+Management](https://github.com/maxmahlke/rocks/blob/master/docs/tutorials/
+literature.ipynb)
```

