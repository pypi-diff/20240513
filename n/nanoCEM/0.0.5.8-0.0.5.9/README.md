# Comparing `tmp/nanoCEM-0.0.5.8.tar.gz` & `tmp/nanoCEM-0.0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.5.8.tar", last modified: Wed Apr 17 04:26:00 2024, max compression
+gzip compressed data, was "nanoCEM-0.0.5.9.tar", last modified: Mon May 13 03:58:27 2024, max compression
```

## Comparing `nanoCEM-0.0.5.8.tar` & `nanoCEM-0.0.5.9.tar`

### file list

```diff
@@ -1,34 +1,26 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-17 04:26:00.445337 nanoCEM-0.0.5.8/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.5.8/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2730 2024-04-17 04:26:00.445337 nanoCEM-0.0.5.8/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2100 2024-03-07 07:08:59.000000 nanoCEM-0.0.5.8/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-17 04:26:00.441338 nanoCEM-0.0.5.8/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    15656 2024-04-17 03:28:08.000000 nanoCEM-0.0.5.8/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5416 2023-12-21 04:37:40.000000 nanoCEM-0.0.5.8/nanoCEM/NEW_TRAINER.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.5.8/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4547 2023-12-10 10:36:58.000000 nanoCEM-0.0.5.8/nanoCEM/alignment_feature_camera.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3946 2024-04-17 04:24:54.000000 nanoCEM-0.0.5.8/nanoCEM/alignment_magnifier
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    14691 2024-04-16 13:13:00.000000 nanoCEM-0.0.5.8/nanoCEM/cem_utils.py
--rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    10833 2024-04-16 13:13:00.000000 nanoCEM-0.0.5.8/nanoCEM/current_events_magnifier
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5903 2024-03-27 13:32:46.000000 nanoCEM-0.0.5.8/nanoCEM/de_novo.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3137 2023-12-15 14:01:45.000000 nanoCEM-0.0.5.8/nanoCEM/density_2d.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4083 2024-02-22 02:44:17.000000 nanoCEM-0.0.5.8/nanoCEM/extract_sub_fast5_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1868 2023-07-24 04:48:56.000000 nanoCEM-0.0.5.8/nanoCEM/extract_sub_fastq_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2160 2024-03-27 13:32:46.000000 nanoCEM-0.0.5.8/nanoCEM/kmer_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1988 2024-02-23 07:56:30.000000 nanoCEM-0.0.5.8/nanoCEM/kmer_test_pr.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3600 2024-03-27 13:32:45.000000 nanoCEM-0.0.5.8/nanoCEM/machine_learning_trainer.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4427 2024-03-27 13:32:45.000000 nanoCEM-0.0.5.8/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11200 2024-02-23 10:21:22.000000 nanoCEM-0.0.5.8/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10253 2024-04-16 13:13:00.000000 nanoCEM-0.0.5.8/nanoCEM/read_f5c_eventalign.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6807 2024-04-16 13:13:00.000000 nanoCEM-0.0.5.8/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6866 2024-04-16 13:13:00.000000 nanoCEM-0.0.5.8/nanoCEM/read_move_table.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13342 2024-02-26 08:39:30.000000 nanoCEM-0.0.5.8/nanoCEM/read_tombo_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8548 2024-04-09 09:41:06.000000 nanoCEM-0.0.5.8/nanoCEM/squigualiser_utils.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-17 04:26:00.445337 nanoCEM-0.0.5.8/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2730 2024-04-17 04:26:00.000000 nanoCEM-0.0.5.8/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      755 2024-04-17 04:26:00.000000 nanoCEM-0.0.5.8/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2024-04-17 04:26:00.000000 nanoCEM-0.0.5.8/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      178 2024-04-17 04:26:00.000000 nanoCEM-0.0.5.8/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2024-04-17 04:26:00.000000 nanoCEM-0.0.5.8/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2024-04-17 04:26:00.445337 nanoCEM-0.0.5.8/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1295 2024-04-17 04:25:17.000000 nanoCEM-0.0.5.8/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-13 03:58:27.013821 nanoCEM-0.0.5.9/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2024-04-30 05:56:15.000000 nanoCEM-0.0.5.9/LICENSE
+-rw-r--r--   0 zhguo     (1000) zhguo     (1000)     3073 2024-05-13 03:58:27.013821 nanoCEM-0.0.5.9/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2100 2024-04-30 05:56:15.000000 nanoCEM-0.0.5.9/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-13 03:58:27.013821 nanoCEM-0.0.5.9/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    15657 2024-04-30 05:57:13.000000 nanoCEM-0.0.5.9/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3973 2024-05-03 02:57:20.000000 nanoCEM-0.0.5.9/nanoCEM/alignment_magnifier
+-rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    14799 2024-05-13 03:24:07.000000 nanoCEM-0.0.5.9/nanoCEM/cem_utils.py
+-rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    10833 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/current_events_magnifier
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4083 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/extract_sub_fast5_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3597 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/machine_learning_trainer.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4427 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11200 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10253 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/read_f5c_eventalign.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6807 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6866 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/read_move_table.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13342 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-13 03:58:27.013821 nanoCEM-0.0.5.9/nanoCEM.egg-info/
+-rw-r--r--   0 zhguo     (1000) zhguo     (1000)     3073 2024-05-13 03:58:27.000000 nanoCEM-0.0.5.9/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      545 2024-05-13 03:58:27.000000 nanoCEM-0.0.5.9/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2024-05-13 03:58:27.000000 nanoCEM-0.0.5.9/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      178 2024-05-13 03:58:27.000000 nanoCEM-0.0.5.9/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2024-05-13 03:58:27.000000 nanoCEM-0.0.5.9/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2024-05-13 03:58:27.013821 nanoCEM-0.0.5.9/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1295 2024-05-13 03:57:30.000000 nanoCEM-0.0.5.9/setup.py
```

### Comparing `nanoCEM-0.0.5.8/LICENSE` & `nanoCEM-0.0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.8/PKG-INFO` & `nanoCEM-0.0.5.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: nanoCEM
-Version: 0.0.5.8
-Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).
-Home-page: https://github.com/lrslab/nanoCEM
-Author: GUO Zhihao
-Author-email: qhuozhihao@icloud.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0,<=3.11.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nanoCEM ![logo](docs/logo_tiny.png "nanoCEM")
 <a href="https://pypi.python.org/pypi/nanoCEM" rel="pypi">![PyPI](https://img.shields.io/pypi/v/nanoCEM?color=green) </a>
 <a href="https://opensource.org/license/mit/" rel="license">![License](https://img.shields.io/pypi/l/nanoCEM?color=orange)</a>
 
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 NanoCEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
```

#### html2text {}

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.8 Summary: A simple tool
-designed to visualize the features that distinguish between two groups of ONT
-data at the site level. It supports 4 re-squiggle program(tombo resquiggle/f5c
-resquiggle/f5c eventalign/move_table). Home-page: https://github.com/lrslab/
-nanoCEM Author: GUO Zhihao Author-email: qhuozhihao@icloud.com Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python:
->=3.7.0,<=3.11.7 Description-Content-Type: text/markdown License-File: LICENSE
 # nanoCEM ![logo](docs/logo_tiny.png "nanoCEM") _!_[_P_y_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _p_y_p_i_/_v_/_n_a_n_o_C_E_M_?_c_o_l_o_r_=_g_r_e_e_n_)_ _!_[_L_i_c_e_n_s_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/
 _n_a_n_o_C_E_M_?_c_o_l_o_r_=_o_r_a_n_g_e_) The nanopore current events magnifier (`nanoCEM`) is a
 python command line to facilitate the analysis of DNA/RNA modification sites by
 visualizing statistical features of current events. NanoCEM can be used to
 showcase high confidence sites and observe the difference based on the
 modification sample and the low or no modification sample. It supports two re-
```

### Comparing `nanoCEM-0.0.5.8/README.md` & `nanoCEM-0.0.5.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: nanoCEM
+Version: 0.0.5.9
+Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).
+Home-page: https://github.com/lrslab/nanoCEM
+Author: GUO Zhihao
+Author-email: qhuozhihao@icloud.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7.0,<=3.11.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: h5py>=3.8.0
+Requires-Dist: numpy>=1.23.0
+Requires-Dist: pandas>=1.5.0
+Requires-Dist: plotnine==0.12.4
+Requires-Dist: tqdm>=4.62.0
+Requires-Dist: pysam>=0.21.0
+Requires-Dist: pyslow5>=1.0.0
+Requires-Dist: vbz_h5py_plugin>=1.0.1
+Requires-Dist: biopython>=1.80
+Requires-Dist: scikit-learn>=1.2.2
+Requires-Dist: squigualiser==0.5.1
+
 # nanoCEM ![logo](docs/logo_tiny.png "nanoCEM")
 <a href="https://pypi.python.org/pypi/nanoCEM" rel="pypi">![PyPI](https://img.shields.io/pypi/v/nanoCEM?color=green) </a>
 <a href="https://opensource.org/license/mit/" rel="license">![License](https://img.shields.io/pypi/l/nanoCEM?color=orange)</a>
 
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 NanoCEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
```

#### html2text {}

```diff
@@ -1,9 +1,22 @@
-# nanoCEM ![logo](docs/logo_tiny.png "nanoCEM") _!_[_P_y_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_p_y_p_i_/_v_/_n_a_n_o_C_E_M_?_c_o_l_o_r_=_g_r_e_e_n_)_ _!_[_L_i_c_e_n_s_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/
+Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.9 Summary: A simple tool
+designed to visualize the features that distinguish between two groups of ONT
+data at the site level. It supports 4 re-squiggle program(tombo resquiggle/f5c
+resquiggle/f5c eventalign/move_table). Home-page: https://github.com/lrslab/
+nanoCEM Author: GUO Zhihao Author-email: qhuozhihao@icloud.com Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python:
+>=3.7.0,<=3.11.7 Description-Content-Type: text/markdown License-File: LICENSE
+Requires-Dist: h5py>=3.8.0 Requires-Dist: numpy>=1.23.0 Requires-Dist:
+pandas>=1.5.0 Requires-Dist: plotnine==0.12.4 Requires-Dist: tqdm>=4.62.0
+Requires-Dist: pysam>=0.21.0 Requires-Dist: pyslow5>=1.0.0 Requires-Dist:
+vbz_h5py_plugin>=1.0.1 Requires-Dist: biopython>=1.80 Requires-Dist: scikit-
+learn>=1.2.2 Requires-Dist: squigualiser==0.5.1 # nanoCEM ![logo](docs/
+logo_tiny.png "nanoCEM") _!_[_P_y_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
+_n_a_n_o_C_E_M_?_c_o_l_o_r_=_g_r_e_e_n_)_ _!_[_L_i_c_e_n_s_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/
 _n_a_n_o_C_E_M_?_c_o_l_o_r_=_o_r_a_n_g_e_) The nanopore current events magnifier (`nanoCEM`) is a
 python command line to facilitate the analysis of DNA/RNA modification sites by
 visualizing statistical features of current events. NanoCEM can be used to
 showcase high confidence sites and observe the difference based on the
 modification sample and the low or no modification sample. It supports two re-
 squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`. If you want to
 view single read signal or raw signal, [Squigualiser](https://github.com/
```

### Comparing `nanoCEM-0.0.5.8/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.5.9/nanoCEM/CE_magnifier_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,16 +119,16 @@
     #                     control='/hdd_data/download/23s_rRNA_A2030/ivt/file', output='f5c_result_rna_re_2524',
     #                     subsample_ratio=1,rna=True,
     #                     ref="../example/data/23S_rRNA.fasta", pore='r9')
     # parser.set_defaults(function='f5c_re', chrom="NR_103073.1", pos=875, len=10, strand='-', cpu=8,norm=True,base_shift='auto',pore='r9',
     #                     input='../example/data/wt/file', control='../example/data/ivt/file', output='f5c_result_rna_re_re',
     #                     subsample_ratio=1,kmer_size=3,
     #                     ref="../example/data/reverse/23S_rRNA_re.fasta", rna=True)
-    parser.set_defaults(function='f5c_ev', chrom="NR_103073.1", pos=2524, len=5, strand='+', cpu=8,norm=True,base_shift='auto',pore='r9',
-                        input='../example/data/wt/file', control='../example/data/ivt/file', output='f5c_result_rna_ev_2524',kmer_size=5,
+    parser.set_defaults(function='f5c_re', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=8,norm=True,base_shift='auto',pore='r9',
+                        input='../example/data/wt/file', control='../example/data/ivt/file', output='f5c_result_rna_re_2030',kmer_size=3,
                         subsample_ratio=1,
                         ref="../example/data/23S_rRNA.fasta", rna=True)
     return parser
 
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
```

### Comparing `nanoCEM-0.0.5.8/nanoCEM/alignment_feature_camera.py` & `nanoCEM-0.0.5.9/nanoCEM/alignment_magnifier`

 * *Files 21% similar despite different names*

```diff
@@ -23,40 +23,34 @@
     parser.add_argument("--pos", type=int, help="site of your interest")
     parser.add_argument("--len", default=10, type=int, help="region around the position")
     parser.add_argument('-t',"--cpu", default=4, type=int, help="region around the position")
     parser.add_argument("--strand", default="+", help="Strand of your interest")
     parser.add_argument('--rna', action='store_true', help='Turn on the RNA mode')
     parser.add_argument('-r', "--ref", help="fasta file")
     parser.add_argument('-i', "--input_fastq",
-                        help="input_bam_file")
+                        help="input_fastq_file")
     parser.add_argument('-c', "--control_fastq",
-                        help="control_bam_file")
+                        help="control_fastq_file")
     # parser_tombo.add_argument('-b', "--bam", help="bam file to help index to speed up")
     parser.add_argument('-o', "--output", default="nanoCEM_result", help="output_file")
 
-    parser.set_defaults(chrom="NR_103073.1", pos=2030, len=10, strand='+', input_fastq='../example/data/wt/file.fastq',
-                        control_fastq='../example/data/ivt/file.fastq', output='tombo_result_rna', rna=True,cpu=16,
-                        ref='../example/data/23S_rRNA.fasta')
-    # parser.set_defaults(chrom="NR_103073.1", pos=875, len=10, strand='-', input_bam='../example/data/reverse/wt.bam',
-    #                     control_bam='../example/data/reverse/ivt.bam', output='tombo_result_rna_re', rna=True,
-    #                     ref='../example/data/reverse/23S_rRNA_re.fasta')
     return parser
 
 
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
     input_fastq = args.input_fastq
     control_fastq = args.control_fastq
     ref = args.ref
     cpu = str(args.cpu)
     # check input file
     identify_file_path(input_fastq)
-
+    identify_file_path(ref)
     # prepare title
     location = args.chrom + ':' + str(args.pos - args.len) + '-' + str(args.pos + args.len)
     title = location + ':' + args.strand
     # check output path
     results_path = args.output
     build_out_path(results_path)
 
@@ -91,15 +85,15 @@
 
 
     final_feature = final_feature.apply(lambda x: count_mis(x, feature_matrix), axis=1)
     final_feature['Match'] = final_feature[feature_matrix[0]]
     final_feature.drop(feature_matrix[0], inplace=True, axis=1)
     final_feature.columns = ['Chrom', 'Position', 'Base', 'Coverage', 'Align string', 'Q string', 'Group', 'A', 'T',
                              'C', 'G', 'Match']
-    final_feature.to_csv(results_path + '/alignment_feature.csv', index=None)
+    final_feature.to_csv(results_path + '/alignment_feature.csv', index=False)
     print("Alignment feature file saved as "+results_path + '/alignment_feature.csv')
 
     final_feature = pd.melt(final_feature, id_vars=['Position', 'Group'], value_vars=['A', 'T', 'C', 'G', 'Match'])
 
     print("Start to plot ...")
     alignment_plot(final_feature, pos_list, base_list, title, args.pos, results_path)
     print('Finished')
```

### Comparing `nanoCEM-0.0.5.8/nanoCEM/cem_utils.py` & `nanoCEM-0.0.5.9/nanoCEM/cem_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 base_shift_dict ={
     'r9RNA+': -1,
     'r9RNA-': -3,
     'r9DNA+': -2,
     'r9DNA-': -3,
     'r10DNA+': -6,
     'r10DNA-': -2,
-    'rna004RNA+': -6,
-    'rna004RNA-': -2,
+    'rna004RNA+': -2,
+    'rna004RNA-': -6,
 }
 
 def caculate_base_shift_size(kmer_model,strand):
     def is_odd(number):
         if number % 2 == 0:
             return False
         else:
@@ -99,51 +99,52 @@
     if subsample_ratio < 1:
         new_bam = '.'.join(fastq_file.split('.')[:-1]) + '_sub.bam'
         cmds = "samtools view -hbS -s " +str(subsample_ratio) +' ' + bam_file +' > ' + new_bam
         print(cmds)
         run_cmd(cmds)
         bam_file = new_bam
 
-    # if not os.path.exists(bam_file+'.bai'):
-    cmds = 'samtools index ' + bam_file
-    run_cmd(cmds)
+    if not os.path.exists(bam_file+'.bai'):
+        cmds = 'samtools index ' + bam_file
+        run_cmd(cmds)
 
     new_fastq_file = '.'.join(bam_file.split('.')[:-1]) + '.fastq'
     if not os.path.exists(new_fastq_file):
         cmds = 'samtools bam2fq ' + bam_file + ' > '+ new_fastq_file
         run_cmd(cmds)
     return new_fastq_file,bam_file
 
 def generate_paf_file_eventalign(fastq_file, blow5_file,bam_file,fasta_file,pore,rna,cpu):
     paf_file =  '.'.join(fastq_file.split('.')[:-1]) + '_ev.paf'
     if not os.path.exists(paf_file):
-        cmds = 'slow5tools index ' + blow5_file
-        run_cmd(cmds)
+        if not os.path.exists(blow5_file+'.idx'):
+            cmds = 'slow5tools index ' + blow5_file
+            run_cmd(cmds)
 
         cmds = 'f5c index --slow5 ' +blow5_file+' '+ fastq_file
         run_cmd(cmds)
 
         cmds = 'f5c eventalign -r '+ fastq_file +" -g "+fasta_file+ ' --slow5 ' + blow5_file + ' --pore '+ pore+' -b ' + bam_file +' -c --min-mapq 0' + ' -t ' + str(cpu)
-        print()
         if rna:
             cmds =cmds +' --rna'
         cmds =cmds +' > '+ paf_file
         print(cmds)
         print('Start to eventalign ...')
         run_cmd(cmds)
         print('Generated paf file : ' + paf_file)
     else:
         print(paf_file + ' existed. Will skip the f5c eventalign ... ')
     return paf_file
 
 def generate_paf_file_resquiggle(fastq_file, blow5_file,pore,rna,cpu):
     paf_file =  '.'.join(fastq_file.split('.')[:-1]) + '_re.paf'
     if not os.path.exists(paf_file):
-        cmds = 'slow5tools index ' + blow5_file
-        run_cmd(cmds)
+        if not os.path.exists(blow5_file + '.idx'):
+            cmds = 'slow5tools index ' + blow5_file
+            run_cmd(cmds)
 
         cmds = 'f5c index --slow5 ' +blow5_file+' '+ fastq_file
         run_cmd(cmds)
 
         cmds = 'f5c resquiggle -c ' + fastq_file + ' ' + blow5_file + ' --pore ' + pore + ' -o ' + paf_file +' -t '+ str(cpu)
         if rna:
             cmds =cmds +' --rna'
```

### Comparing `nanoCEM-0.0.5.8/nanoCEM/current_events_magnifier` & `nanoCEM-0.0.5.9/nanoCEM/current_events_magnifier`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.8/nanoCEM/de_novo.py` & `nanoCEM-0.0.5.9/nanoCEM/read_move_table.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,157 +1,181 @@
-import pandas as pd
 import re
 import numpy as np
-from cem_utils import *
-from normalization import normalize_signal_with_lim
-import pysam
+import pandas as pd
 import pyslow5
-
-def extract_feature(line, strand, base_shift=2, norm=True):
-    global nucleotide_type
+import pysam
+from tqdm import tqdm
+from nanoCEM.normalization import normalize_signal,normalize_signal_with_lim
+from nanoCEM.cem_utils import generate_bam_file,identify_file_path,prepare_move_table_file
+# from nanoCEM.plot import draw_signal
+import os
+import argparse
+score_dict={}
+nucleotide_type=None
+def extract_feature(line,strand,sig_move_offset,norm=True):
+    pbar.update(1)
     read_id = line[0]
-    # if read_id !='562eeb47-2b86-4fc7-abfc-5dce62f511ed':
-    #     return None
-
+    # if read_id =='dd49b363-ab1e-45c0-ae06-7d7a06452f4c':
+    #     print(1)
+    if read_id not in info_dict:
+        return None
     # tackle moves tag
-    moves_string = line[14]
+    moves_string = line[12]
     moves_string = re.sub('ss:Z:', '', moves_string)
     moves_string = re.sub('D', 'D,', moves_string)
     moves_string = re.sub('I', 'I,', moves_string)
     # print(moves_string)
     moves = re.split(r',+', moves_string)
     moves = moves[:-1]
     # extract index and generate event_length and event_start
     insertion = 0
     event_length = []
-    for i, item in enumerate(moves):
+    for i,item in enumerate(moves):
         if 'D' in item:
             deletion = int(item[:-1])
             for i in range(deletion):
                 event_length.append(0)
         elif 'I' in item:
-            if i == 0:
+            if i == 0 :
                 continue
             else:
                 return None
         elif '=' in item:
             return None
         else:
             event_length.append(int(item))
     # build event_length from move table
-    read = s5.get_read(read_id, aux=["read_number", "start_mux"], pA=True)
+
+    if read_id not in read_ids:
+        return None
+    read = s5.get_read(read_id, aux=["read_number", "start_mux"],pA=True)
     start_index = line[2]
     end_index = line[3]
     event_length = np.array(event_length)
+    # assert len_raw_signal in paf and blow5
 
-    # identify RNA or DNA
-    if nucleotide_type is None:
-        if line[7] > line[8]:
-            nucleotide_type = 'RNA'
-        else:
-            nucleotide_type = 'DNA'
-    #  assert len_raw_signal in paf and blow5
     try:
-        assert end_index - start_index == np.sum(event_length)
         assert read['len_raw_signal'] == line[1]
     except Exception:
         print("Warning: 1 read's length of signal is not equal between blow5 and paf")
         return None
-
     signal = read['signal']
 
     # create event start and flip all table
     signal = signal[start_index:end_index]
-    if nucleotide_type == 'RNA':
-        signal = np.flip(signal)
-        event_length = np.flip(event_length)
 
     event_starts = event_length.cumsum()
     event_starts = np.insert(event_starts, 0, 0)[:-1]
     if norm:
-        signal = normalize_signal_with_lim(signal)
+        signal,shift,scale = normalize_signal_with_lim(signal)
 
     # index query and reference
-    aligned_pair = info_dict[read_id]['pairs']
+    aligned_pair=info_dict[read_id]['pairs']
     qlen = info_dict[read_id]['query_length']
+    try:
+        assert qlen == len(event_length) + sig_move_offset
+    except Exception:
+        print("Warning: 1 read's length of event is not equal between bam and paf file")
+        return None
     # correct index about DNA and RNA
-    if nucleotide_type == 'RNA':
-        if strand == '+':
-            gap = qlen - event_length.shape[0]
-            aligned_pair[0] = aligned_pair[0] - gap
-            aligned_pair = aligned_pair[aligned_pair[0] >= 0]
-        elif strand == '-':
-            aligned_pair[0] = event_length.shape[0] - aligned_pair[0] - 1
-    else:
-        if strand == '-':
-            aligned_pair[0] = qlen - aligned_pair[0] - 1
-        aligned_pair = aligned_pair[aligned_pair[0] < event_length.shape[0]]
-    # base shift
-    if nucleotide_type == 'RNA':
-        aligned_pair[0] = aligned_pair[0].values + base_shift
-        aligned_pair = aligned_pair[aligned_pair[0] < event_length.shape[0]]
-    else:
-        aligned_pair[0] = aligned_pair[0].values - base_shift
-        aligned_pair = aligned_pair[aligned_pair[0] >= 0]
+    if (nucleotide_type == 'RNA' and strand == '+') or (nucleotide_type == 'DNA' and strand == '-'):
+        aligned_pair[0] = qlen - aligned_pair[0] - 1
 
-    if aligned_pair.shape[0] == 0:
+    if aligned_pair.shape[0]==0:
         return None
     read_pos = aligned_pair[0].values
     ref_pos = aligned_pair[1].values
 
     # extract raw signal by event length and event start
     total_feature_per_reads = []
-    try:
-        raw_signal_every = [signal[event_starts[x]:event_starts[x] + event_length[x]] for x in
-                            read_pos]
-        # if aligned_pair.shape[0] < 11:
-        #     draw_signal(signal[event_starts[read_pos[0]]:event_starts[read_pos[-1]+1]], event_starts[read_pos[0]:read_pos[-1]+1]-event_starts[read_pos[0]], base_list)
-    except Exception:
-        print(1)
+    raw_signal_every = [signal[event_starts[x]:event_starts[x] + event_length[x]] for x in
+                        read_pos]
     # calculate mean median and dwell time
     for i, element in enumerate(raw_signal_every):
-        if event_length[read_pos[i]] == 0:
+        if len(element) == 0:
             continue
-        temp = [read_id, np.mean(element), np.std(element), np.median(element), event_length[read_pos[i]], ref_pos[i]]
+        temp = [read_id,np.mean(element), np.std(element), np.median(element), event_length[read_pos[i]],ref_pos[i]]
         total_feature_per_reads.append(temp)
     return total_feature_per_reads
 
+def extract_pairs_pos(bam_file,position,length,chromosome,strand):
+
+    result_dict={}
+    for read in bam_file.fetch(chromosome,position-length, position+length+1):
+        if strand == '+' and read.is_reverse:
+            continue
+        if strand == '-' and not read.is_reverse:
+            continue
+        # if read.qname == '7dcec2bc-65f3-41fe-8981-dd3af9fa6e67':
+        #     print(1)
+        start_position=read.reference_start
+        end_position=read.reference_end
+        if position < start_position or position > end_position:
+            continue
+        # unit
+        aligned_pair = pd.DataFrame(np.array(read.aligned_pairs)).dropna().reset_index(drop=True)
+        aligned_pair = aligned_pair[(aligned_pair[1] >= position - length) & (aligned_pair[1] <= position + length)]
+
+        temp={}
+        temp['pairs']=aligned_pair
+        temp['query_length'] = read.query_length
+        result_dict[read.qname] = temp
+    return result_dict
 
-def read_blow5(path, reference, pore, subsample_ratio=1, base_shift=2, norm=True,
-               cpu=4, rna=True):
-    global info_dict, s5, pbar
+
+
+def read_basecall_bam(path,position,reference,length,chrom,strand,sig_move_offset,kmer_length,subsample_ratio=1,norm=True,cpu=4,rna=True):
+    global info_dict, s5,pbar,nucleotide_type,read_ids
     slow5_file = path + ".blow5"
-    fastq_file = path + ".fastq"
-    identify_file_path(fastq_file)
+    bam_file = path + ".bam"
+    identify_file_path(bam_file)
     identify_file_path(slow5_file)
-    paf_file = generate_paf_file(fastq_file, slow5_file, pore, rna)
-    bam_file = generate_bam_file(fastq_file, reference, cpu)
-    bam_file = pysam.AlignmentFile(bam_file, 'rb')
+    align_bam_file, paf_file = prepare_move_table_file(bam_file,reference,cpu,str(sig_move_offset),str(kmer_length))
 
-    s5 = pyslow5.Open(slow5_file, 'r')
+    if rna:
+        nucleotide_type ='RNA'
+    else:
+        nucleotide_type = 'DNA'
+    bam_file = pysam.AlignmentFile(align_bam_file,'rb')
 
-    df = pd.read_csv(paf_file, sep='\t', header=None)
-    df = pd.merge(df, info_df, how='inner', on=0)
+    info_dict=extract_pairs_pos(bam_file,position,length,chrom,strand)
+    if info_dict == {}:
+        raise RuntimeError("There is no read aligned on this position")
+    info_df = pd.DataFrame(list(info_dict.keys()))
+
+    s5 = pyslow5.Open(slow5_file, 'r')
+    read_ids, num_reads = s5.get_read_ids()
+    df=pd.read_csv(paf_file,sep='\t',header=None)
+    df=pd.merge(df,info_df,how='inner',on=0)
     if df.shape[0] == 0:
         raise RuntimeError("cannot found the record from bam in your paf file. Please check your f5c command ... ")
     if df.shape[0] / info_df.shape[0] < 0.8:
-        print('There are ' + str(info_df.shape[0] - df.shape[0]) + " reads not found in your paf file ...")
+        print('There are '+str(info_df.shape[0]-df.shape[0])+" reads not found in your paf file ...")
     pbar = tqdm(total=df.shape[0], position=0, leave=True)
-    df["feature"] = df.apply(extract_feature, strand=strand, base_shift=base_shift, norm=norm, axis=1)
+    df["feature"] = df.apply(extract_feature,strand=strand,norm=norm,sig_move_offset=sig_move_offset,axis=1)
     pbar.close()
 
     df.dropna(inplace=True)
     num_aligned = df.shape[0]
-    if subsample_ratio < 1:
-        df = df.sample(frac=subsample_ratio)
-    final_feature = []
+    if subsample_ratio<1:
+        df=df.sample(frac=subsample_ratio)
+    final_feature=[]
     for item in df["feature"]:
         final_feature.extend(item)
-    final_feature = pd.DataFrame(final_feature)
-    final_feature.columns = ['Read ID', 'Mean', 'STD', 'Median', 'Dwell time', 'Position']
+    final_feature=pd.DataFrame(final_feature)
+    final_feature.columns=['Read ID','Mean','STD','Median','Dwell time','Position']
+    # if rna_mode:
+    #     if strand == '+':
+    #         final_feature['position']=final_feature['position'] - (kmer_model-1)
+    #     else:
+    #         final_feature['position']=final_feature['position'] + (kmer_model-1)
 
     final_feature['Position'] = final_feature['Position'].astype(int).astype(str)
     print('Extracted ', num_aligned, ' aligned reads from blow5 files')
 
-    return final_feature, num_aligned, nucleotide_type
+    # if num_aligned>50:
+    #     dwell_filter_pctls = (0.5, 99.5)
+    #     dwell_min, dwell_max = np.percentile(final_feature['Dwell time'].values, dwell_filter_pctls)
+    #     final_feature = final_feature[(final_feature['Dwell time'] > dwell_min) & (final_feature['Dwell time'] < dwell_max)]
+
+    return final_feature,num_aligned
 
-read_blow5('/t1/zhguo/Data/ASFV_RNA/ASFV_go/WGS1','/t1/zhguo/Data/ASFV_RNA/asfv.fa','r10')
```

### Comparing `nanoCEM-0.0.5.8/nanoCEM/extract_sub_fast5_from_bam` & `nanoCEM-0.0.5.9/nanoCEM/extract_sub_fast5_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.8/nanoCEM/machine_learning_trainer.py` & `nanoCEM-0.0.5.9/nanoCEM/machine_learning_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 import numpy as np
 from matplotlib import pyplot as plt
 import pandas as pd
 import xgboost
 from nanoCEM.cem_utils import  extract_kmer_feature
 plt.rcParams['pdf.fonttype'] = 42
-results_path='f5c_result_rna_re'
+results_path='f5c_result_rna'
 df = pd.read_csv(results_path+'/current_feature.csv')
 
-feature_matrix, label = extract_kmer_feature( df, 5, 2030)
+feature_matrix, label = extract_kmer_feature( df, 7, 2030)
 
 label[0] = label[0].apply(lambda x: 1 if x == 'Sample' else 0)
 
 X = feature_matrix.values
 y = label.values
 
 from sklearn.metrics import accuracy_score
```

### Comparing `nanoCEM-0.0.5.8/nanoCEM/normalization.py` & `nanoCEM-0.0.5.9/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.8/nanoCEM/plot.py` & `nanoCEM-0.0.5.9/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.8/nanoCEM/read_f5c_eventalign.py` & `nanoCEM-0.0.5.9/nanoCEM/read_f5c_eventalign.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.8/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.5.9/nanoCEM/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.8/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.5.9/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.8/setup.py` & `nanoCEM-0.0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.5.8",
+    version="0.0.5.9",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/nanoCEM",
```

