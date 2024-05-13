# Comparing `tmp/dcw-finder-0.0.5.tar.gz` & `tmp/dcw-finder-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcw-finder-0.0.5.tar", last modified: Mon May 13 18:09:49 2024, max compression
+gzip compressed data, was "dcw-finder-0.0.6.tar", last modified: Mon May 13 18:17:51 2024, max compression
```

## Comparing `dcw-finder-0.0.5.tar` & `dcw-finder-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:09:49.658986 dcw-finder-0.0.5/
--rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:09:49.658774 dcw-finder-0.0.5/PKG-INFO
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:09:49.658528 dcw-finder-0.0.5/dcw_finder.egg-info/
--rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:09:49.000000 dcw-finder-0.0.5/dcw_finder.egg-info/PKG-INFO
--rw-r--r--   0 jrim       (501) staff       (20)      407 2024-05-13 18:09:49.000000 dcw-finder-0.0.5/dcw_finder.egg-info/SOURCES.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 18:09:49.000000 dcw-finder-0.0.5/dcw_finder.egg-info/dependency_links.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 17:52:51.000000 dcw-finder-0.0.5/dcw_finder.egg-info/not-zip-safe
--rw-r--r--   0 jrim       (501) staff       (20)        7 2024-05-13 18:09:49.000000 dcw-finder-0.0.5/dcw_finder.egg-info/requires.txt
--rw-r--r--   0 jrim       (501) staff       (20)        4 2024-05-13 18:09:49.000000 dcw-finder-0.0.5/dcw_finder.egg-info/top_level.txt
--rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-13 18:09:49.659044 dcw-finder-0.0.5/setup.cfg
--rw-r--r--   0 jrim       (501) staff       (20)      650 2024-05-13 18:09:46.000000 dcw-finder-0.0.5/setup.py
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:09:49.658334 dcw-finder-0.0.5/src/
--rw-r--r--   0 jrim       (501) staff       (20)      280 2024-05-13 18:09:42.000000 dcw-finder-0.0.5/src/__init__.py
--rw-r--r--   0 jrim       (501) staff       (20)     7746 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_accessory.py
--rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_blast.py
--rw-r--r--   0 jrim       (501) staff       (20)    11473 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_cluster.py
--rw-r--r--   0 jrim       (501) staff       (20)    10164 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_count.py
--rw-r--r--   0 jrim       (501) staff       (20)     7797 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_parse.py
--rw-r--r--   0 jrim       (501) staff       (20)     2667 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_profile.py
--rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_search.py
--rw-r--r--   0 jrim       (501) staff       (20)     4183 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_seqlib.py
--rw-r--r--   0 jrim       (501) staff       (20)     4337 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_target.py
--rw-r--r--   0 jrim       (501) staff       (20)     5582 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_utils.py
--rw-r--r--   0 jrim       (501) staff       (20)     6629 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/_visualize.py
--rw-r--r--   0 jrim       (501) staff       (20)     1971 2024-05-13 17:40:31.000000 dcw-finder-0.0.5/src/main.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:17:51.076161 dcw-finder-0.0.6/
+-rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:17:51.075932 dcw-finder-0.0.6/PKG-INFO
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:17:51.075663 dcw-finder-0.0.6/dcw_finder.egg-info/
+-rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:17:51.000000 dcw-finder-0.0.6/dcw_finder.egg-info/PKG-INFO
+-rw-r--r--   0 jrim       (501) staff       (20)      407 2024-05-13 18:17:51.000000 dcw-finder-0.0.6/dcw_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 18:17:51.000000 dcw-finder-0.0.6/dcw_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 17:52:51.000000 dcw-finder-0.0.6/dcw_finder.egg-info/not-zip-safe
+-rw-r--r--   0 jrim       (501) staff       (20)        7 2024-05-13 18:17:51.000000 dcw-finder-0.0.6/dcw_finder.egg-info/requires.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        4 2024-05-13 18:17:51.000000 dcw-finder-0.0.6/dcw_finder.egg-info/top_level.txt
+-rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-13 18:17:51.076216 dcw-finder-0.0.6/setup.cfg
+-rw-r--r--   0 jrim       (501) staff       (20)      650 2024-05-13 18:17:49.000000 dcw-finder-0.0.6/setup.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:17:51.075426 dcw-finder-0.0.6/src/
+-rw-r--r--   0 jrim       (501) staff       (20)      280 2024-05-13 18:17:46.000000 dcw-finder-0.0.6/src/__init__.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7747 2024-05-13 18:17:38.000000 dcw-finder-0.0.6/src/_accessory.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-13 17:40:31.000000 dcw-finder-0.0.6/src/_blast.py
+-rw-r--r--   0 jrim       (501) staff       (20)    11475 2024-05-13 18:17:38.000000 dcw-finder-0.0.6/src/_cluster.py
+-rw-r--r--   0 jrim       (501) staff       (20)    10166 2024-05-13 18:17:38.000000 dcw-finder-0.0.6/src/_count.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7797 2024-05-13 17:40:31.000000 dcw-finder-0.0.6/src/_parse.py
+-rw-r--r--   0 jrim       (501) staff       (20)     2668 2024-05-13 18:17:38.000000 dcw-finder-0.0.6/src/_profile.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-13 17:40:31.000000 dcw-finder-0.0.6/src/_search.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4184 2024-05-13 18:17:38.000000 dcw-finder-0.0.6/src/_seqlib.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4337 2024-05-13 17:40:31.000000 dcw-finder-0.0.6/src/_target.py
+-rw-r--r--   0 jrim       (501) staff       (20)     5582 2024-05-13 17:40:31.000000 dcw-finder-0.0.6/src/_utils.py
+-rw-r--r--   0 jrim       (501) staff       (20)     6629 2024-05-13 17:40:31.000000 dcw-finder-0.0.6/src/_visualize.py
+-rw-r--r--   0 jrim       (501) staff       (20)     1984 2024-05-13 18:17:38.000000 dcw-finder-0.0.6/src/main.py
```

### Comparing `dcw-finder-0.0.5/setup.py` & `dcw-finder-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dcw-finder',
-    version='0.0.5',
+    version='0.0.6',
     description='Package for detecting dcw gene cluster',
     author='jsrim',
     author_email='comfortindex@naver.com',
     url='https://github.com/jrim42/gene-cluster',
     install_requires=['pandas'],
     packages=find_packages(exclude=[]),
     keywords=[],
```

### Comparing `dcw-finder-0.0.5/src/_accessory.py` & `dcw-finder-0.0.6/src/_accessory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import time
 import pandas as pd
 import ast
-from _utils import remove_non_numeric
+from ._utils import remove_non_numeric
 
 def collect_accessory(project_info):
     print("<< collecting accessory genes...")
     input_dir = project_info['input']
     output_dir = project_info['output']
     seqlib_dir = project_info['seqlib']
     data_dir = project_info['data']
```

### Comparing `dcw-finder-0.0.5/src/_blast.py` & `dcw-finder-0.0.6/src/_blast.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.5/src/_cluster.py` & `dcw-finder-0.0.6/src/_cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 '''
 
 import os
 import pandas as pd
 import time
 
-from _visualize import visualize_cluster
-from _visualize import visualize_cluster_type
+from ._visualize import visualize_cluster
+from ._visualize import visualize_cluster_type
 
 #===============================================================================
 def cluster_target(project_info):
     print("<< clustering target genes...")
     input_dir = project_info['input']
     input_len = project_info['input_len']
     output_dir = project_info['output']
```

### Comparing `dcw-finder-0.0.5/src/_count.py` & `dcw-finder-0.0.6/src/_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import pandas as pd
 import sys
 import time
 
 sys.path.append('./info/')
 from target_info import target_list
 
-from _visualize import visualize_heatmap
-from _visualize import visualize_freq
+from ._visualize import visualize_heatmap
+from ._visualize import visualize_freq
 
 #===============================================================================
 def count_blastp_result(project_info):
     output_dir = project_info['output']
 
     result_df = pd.read_csv(f"{project_info['seqlib']}/blast_output1.tsv", sep='\t')
     target_df = pd.read_csv(f"{project_info['data']}/metadata_target.tsv", sep='\t')
```

### Comparing `dcw-finder-0.0.5/src/_parse.py` & `dcw-finder-0.0.6/src/_parse.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.5/src/_profile.py` & `dcw-finder-0.0.6/src/_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 import os
-from _visualize import visualize_heatmap
+from ._visualize import visualize_heatmap
 
 def final_profile(project_info):
 	input_dir = project_info['input']
 	seqlib_dir = project_info['seqlib']
 	output_dir = project_info['output']
 
 	seqlib = pd.read_csv(f"{seqlib_dir}/seqlib.tsv", sep='\t', comment='#')
```

### Comparing `dcw-finder-0.0.5/src/_search.py` & `dcw-finder-0.0.6/src/_search.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.5/src/_seqlib.py` & `dcw-finder-0.0.6/src/_seqlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 	│  													 by using result cluster from mmseq2 and blast output
 	└── construct_seqlib  ˑˑˑˑˑ  to create sequence library using representative sequences
 
 '''
 
 import time
 import pandas as pd
-from _utils import remove_non_numeric
+from ._utils import remove_non_numeric
 
 #===============================================================================
 def create_seqlib(project_info):
 	print("<< creating seqlib...")
 	start_time = time.time()
 
 	search_repseq(project_info)
```

### Comparing `dcw-finder-0.0.5/src/_target.py` & `dcw-finder-0.0.6/src/_target.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.5/src/_utils.py` & `dcw-finder-0.0.6/src/_utils.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.5/src/_visualize.py` & `dcw-finder-0.0.6/src/_visualize.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.5/src/main.py` & `dcw-finder-0.0.6/src/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import time
 import subprocess
 import os
 
-from _utils import sum_assembly_report
-from _utils import organize_input_dir
-from _parse import parse_genome
-from _blast import run_blastp
-from _count import count_blastp_result
-from _seqlib import create_seqlib
-from _search import search_target
-from _count import count_mmseq_result
-from _cluster import cluster_target
-from _cluster import classify_cluster_type
-from _accessory import collect_accessory
-from _profile import final_profile
-from _target import process_target_data
+from ._utils import sum_assembly_report
+from ._utils import organize_input_dir
+from ._parse import parse_genome
+from ._blast import run_blastp
+from ._count import count_blastp_result
+from ._seqlib import create_seqlib
+from ._search import search_target
+from ._count import count_mmseq_result
+from ._cluster import cluster_target
+from ._cluster import classify_cluster_type
+from ._accessory import collect_accessory
+from ._profile import final_profile
+from ._target import process_target_data
 
 def find_gene_cluster(TAXON, target_path):
     if not os.path.exists(target_path):
         print("<< Target file does not exist. Please provide a valid file path.")
         return
 
     start_time = time.time()
```

