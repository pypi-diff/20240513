# Comparing `tmp/hmmix-0.6.9.tar.gz` & `tmp/hmmix-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hmmix-0.6.9.tar", last modified: Tue Dec  5 21:58:45 2023, max compression
+gzip compressed data, was "dist/hmmix-0.7.0.tar", last modified: Mon May 13 01:32:28 2024, max compression
```

## Comparing `hmmix-0.6.9.tar` & `hmmix-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-12-05 21:58:45.000000 hmmix-0.6.9/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    35149 2022-05-11 17:42:22.000000 hmmix-0.6.9/LICENSE.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34593 2023-12-05 21:58:45.000000 hmmix-0.6.9/PKG-INFO
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34059 2023-12-05 21:58:05.000000 hmmix-0.6.9/README.md
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       38 2023-12-05 21:58:45.000000 hmmix-0.6.9/setup.cfg
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      994 2023-12-05 21:11:35.000000 hmmix-0.6.9/setup.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-12-05 21:58:45.000000 hmmix-0.6.9/src/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     8599 2023-06-24 23:31:27.000000 hmmix-0.6.9/src/bcf_vcf.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    15596 2023-10-26 21:24:32.000000 hmmix-0.6.9/src/helper_functions.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    14421 2023-12-05 20:59:49.000000 hmmix-0.6.9/src/hmm_functions.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-12-05 21:58:45.000000 hmmix-0.6.9/src/hmmix.egg-info/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    34593 2023-12-05 21:58:45.000000 hmmix-0.6.9/src/hmmix.egg-info/PKG-INFO
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      411 2023-12-05 21:58:45.000000 hmmix-0.6.9/src/hmmix.egg-info/SOURCES.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        1 2023-12-05 21:58:45.000000 hmmix-0.6.9/src/hmmix.egg-info/dependency_links.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       36 2023-12-05 21:58:45.000000 hmmix-0.6.9/src/hmmix.egg-info/entry_points.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       29 2023-12-05 21:58:45.000000 hmmix-0.6.9/src/hmmix.egg-info/requires.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       77 2023-12-05 21:58:45.000000 hmmix-0.6.9/src/hmmix.egg-info/top_level.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    16030 2023-12-05 20:26:40.000000 hmmix-0.6.9/src/main.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2007 2022-10-25 01:10:14.000000 hmmix-0.6.9/src/make_mutationrate.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     4281 2022-10-25 01:10:46.000000 hmmix-0.6.9/src/make_test_data.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2023-12-05 21:58:45.000000 hmmix-0.6.9/test/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2725 2022-05-26 04:20:02.000000 hmmix-0.6.9/test/test.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     3106 2022-06-02 06:35:33.000000 hmmix-0.6.9/test/test2.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      541 2022-06-08 21:55:04.000000 hmmix-0.6.9/test/test_main.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        0 2022-07-12 05:40:51.000000 hmmix-0.6.9/test/testfred.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-13 01:32:28.000000 hmmix-0.7.0/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    35149 2022-05-11 17:42:22.000000 hmmix-0.7.0/LICENSE.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    37194 2024-05-13 01:32:28.000000 hmmix-0.7.0/PKG-INFO
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    36660 2024-05-13 00:59:09.000000 hmmix-0.7.0/README.md
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       38 2024-05-13 01:32:28.000000 hmmix-0.7.0/setup.cfg
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      994 2024-05-13 01:32:07.000000 hmmix-0.7.0/setup.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-13 01:32:28.000000 hmmix-0.7.0/src/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     8599 2024-05-10 23:31:25.000000 hmmix-0.7.0/src/bcf_vcf.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    17028 2024-05-13 01:21:08.000000 hmmix-0.7.0/src/helper_functions.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    18509 2024-05-13 01:27:31.000000 hmmix-0.7.0/src/hmm_functions.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-13 01:32:28.000000 hmmix-0.7.0/src/hmmix.egg-info/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    37194 2024-05-13 01:32:27.000000 hmmix-0.7.0/src/hmmix.egg-info/PKG-INFO
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      411 2024-05-13 01:32:28.000000 hmmix-0.7.0/src/hmmix.egg-info/SOURCES.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        1 2024-05-13 01:32:27.000000 hmmix-0.7.0/src/hmmix.egg-info/dependency_links.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       36 2024-05-13 01:32:28.000000 hmmix-0.7.0/src/hmmix.egg-info/entry_points.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       29 2024-05-13 01:32:28.000000 hmmix-0.7.0/src/hmmix.egg-info/requires.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       77 2024-05-13 01:32:28.000000 hmmix-0.7.0/src/hmmix.egg-info/top_level.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    21088 2024-05-13 01:31:55.000000 hmmix-0.7.0/src/main.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2007 2022-10-25 01:10:14.000000 hmmix-0.7.0/src/make_mutationrate.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     4560 2024-05-12 23:11:55.000000 hmmix-0.7.0/src/make_test_data.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-13 01:32:28.000000 hmmix-0.7.0/test/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     1280 2024-05-13 00:59:38.000000 hmmix-0.7.0/test/test.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     3106 2022-06-02 06:35:33.000000 hmmix-0.7.0/test/test2.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      541 2022-06-08 21:55:04.000000 hmmix-0.7.0/test/test_main.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        0 2022-07-12 05:40:51.000000 hmmix-0.7.0/test/testfred.py
```

### Comparing `hmmix-0.6.9/LICENSE.txt` & `hmmix-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.9/PKG-INFO` & `hmmix-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,61 @@
 Metadata-Version: 2.1
 Name: hmmix
-Version: 0.6.9
+Version: 0.7.0
 Summary: Find introgressed segments
 Home-page: https://github.com/LauritsSkov/Introgression-detection
 Author: Laurits Skov and Moises Coll Macia
 Author-email: lauritsskov2@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+# Contact
+https://sites.google.com/view/laurits-skov
+
+---
+
+# Helpful files
+The outgroup files, mutation rate files and callability files and ancestral allele files are now premade! 
+
+https://doi.org/10.5281/zenodo.10806733 (hg19 and hg38)
+
+VCF file containing 4 high coverage archaic genomes (Altai, Vindija and Chagyrskaya Neanderthals and Denisovan) here: 
+
+https://zenodo.org/records/7246376 (hg19)
+
+https://zenodo.org/records/10806726 (hg38)
+
+---
 
 # Introgression detection
 
+If you are working with archaic introgression into present-day humans of non-African ancestry you can use these files and skip the following steps:
+Find derived variants in outgroup and Estimate local mutation rate. 
+
 These are the scripts needed to infere archaic introgression in modern populations using an unadmixed outgroup.
 
 1. [Installation](#installation)
 2. [Usage](#usage)
 3. [Quick tutorial](#quick-tutorial)
 4. [1000 genomes tutorial](#example-with-1000-genomes-data)
       - [Get data](#getting-data)
       - [Find derived variants in outgroup](#finding-snps-which-are-derived-in-the-outgroup)
       - [Estimate local mutation rate](#estimating-mutation-rate-across-genome)
       - [Find variants in ingroup](#find-a-set-of-variants-which-are-not-derived-in-the-outgroup)
       - [Train the HMM](#training)
       - [Decoding](#decoding)
       - [Phased data](#training-and-decoding-with-phased-data)
       - [Annotate](#annotate-with-known-admixing-population)
-      - [Run in python](#annotate-with-known-admixing-population)
+5. [Run in python](#annotate-with-known-admixing-population)
 
 ---
 
 ## Installation
 
 Run the following command to install:
 
@@ -72,15 +92,16 @@
 hmmix make_test_data 
 hmmix train  -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=Initialguesses.json -out=trained.json 
 hmmix decode -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=trained.json
 
 
 Different modes (you can also see the options for each by writing hmmix make_test_data -h):
 > make_test_data        
-    -windows            Number of Kb windows to create (defaults to 50,000)
+    -windows            Number of Kb windows to create (defaults to 50,000 per chromosome)
+    -chromosomes        Number of chromosomes to simulate (defaults to 2)
     -nooutfiles         Don't create obs.txt, mutrates.bed, weights.bed, Initialguesses.json (defaults to yes)
 
 > mutation_rate         
     -outgroup           [required] path to variants found in outgroup
     -out                outputfile (defaults to mutationrate.bed)
     -weights            file with callability (defaults to all positions being called)
     -window_size        size of bins (defaults to 1 Mb)
@@ -99,30 +120,45 @@
     -outgroup           [required] path to variant found in outgroup
     -weights            file with callability (defaults to all positions being called)
     -out                outputfile prefix (default is a file named obs.<ind>.txt where ind is the name of individual in ingroup/outgrop list)
     -ancestral          fasta file with ancestral information - comma-separated list or wildcards like vcf argument (default none)
 
 > train                 
     -obs                [required] file with observation data
+    -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
     -weights            file with callability (defaults to all positions being called)
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
     -out                outputfile (default is a file named trained.json)
     -window_size        size of bins (default is 1000 bp)
     -haploid            Change from using diploid data to haploid data (default is diploid)
 
 > decode                
     -obs                [required] file with observation data
+    -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
+    -weights            file with callability (defaults to all positions being called)
+    -mutrates           file with mutation rates (default is mutation rate is uniform)
+    -param              markov parameters file (default is human/neanderthal like parameters)
+    -out                outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)
+    -window_size        size of bins (default is 1000 bp)
+    -haploid            Change from using diploid data to haploid data (default is diploid)
+    -admixpop           Annotate using vcffile with admixing population (default is none)
+    -extrainfo          Add variant position for each SNP (default is off)
+
+> inhomogeneous                
+    -obs                [required] file with observation data
+    -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
     -weights            file with callability (defaults to all positions being called)
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
     -out                outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)
     -window_size        size of bins (default is 1000 bp)
     -haploid            Change from using diploid data to haploid data (default is diploid)
-    -admixpop ADMIXPOP  Annotate using vcffile with admixing population (default is none)
+    -samples            Number of simulated paths for the inhomogeneous markov chain (default is 100)
+    -admixpop           Annotate using vcffile with admixing population (default is none)
     -extrainfo          Add variant position for each SNP (default is off)
 ```
 
 ---
 
 ## Quick tutorial
 
@@ -156,27 +192,19 @@
 weights.bed. This is the parts of the genome that we can accurately map to - in this case we have simulated the data and can accurately access the entire genome.
 
 ```note
 chr1   0   50000000
 chr2   0   50000000
 ```
 
-mutrates.bed. This is the normalized mutation rate across the genome (in bins of 1 Mb).
+mutrates.bed. This is the normalized mutation rate across the genome.
 
 ```note
-chr1  0        1000000   1
-chr1  1000000  2000000   1
-chr1  2000000  3000000   1
-chr1  3000000  4000000   1
-chr1  4000000  5000000   1
-chr1  5000000  6000000   1
-chr1  6000000  7000000   1
-chr1  7000000  8000000   1
-chr1  8000000  9000000   1
-chr1  9000000  10000000  1
+chr1   0   50000000   1
+chr2   0   50000000   1
 ```
 
 Initialguesses.json. This is our initial guesses when training the model - note these are different from those we simulated from.
 
 ```json
 {
   "state_names": ["Human","Archaic"],
@@ -191,29 +219,30 @@
 ```note
 > hmmix train  -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=Initialguesses.json -out=trained.json
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.5, 0.5]
 > transitions = [[0.99, 0.01], [0.02, 0.98]]
 > emissions = [0.03, 0.3]
+> chromosomes to use: All
 > number of windows: 99970 . Number of snps =  4230
 > total callability: 1.0
 > average mutation rate per bin: 1.0
 > Output is trained.json
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -18123.4432    0.5     0.5     0.03    0.3     0.99      0.98
-1          -17506.017     0.96    0.04    0.035   0.2202  0.9969    0.9242
-2          -17487.7921    0.971   0.029   0.0369  0.2235  0.9974    0.9141
+0          -18123.4598    0.5     0.5     0.03    0.3     0.99      0.98
+1          -17506.0258    0.96    0.04    0.035   0.2202  0.9969    0.9242
+2          -17487.8       0.971   0.029   0.0369  0.2235  0.9974    0.9141
 ...
-16         -17401.3802    0.994   0.006   0.0398  0.4584  0.9999    0.9806
-17         -17401.3786    0.994   0.006   0.0398  0.4586  0.9999    0.9807
-18         -17401.3783    0.994   0.006   0.0398  0.4587  0.9999    0.9808
+16         -17401.3853    0.994   0.006   0.0398  0.4584  0.9999    0.9806
+17         -17401.3838    0.994   0.006   0.0398  0.4586  0.9999    0.9807
+18         -17401.3835    0.994   0.006   0.0398  0.4587  0.9999    0.9808
 
 
 # run without mutrate and weights (only do this for simulated data)
 > hmmix train  -obs=obs.txt -param=Initialguesses.json -out=trained.json
 ```
 
 We can now decode the data with the best parameters that maximize the likelihood and find the archaic segments:
@@ -221,53 +250,56 @@
 ```note
 > hmmix decode -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=trained.json
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.994, 0.006]
 > transitions = [[1.0, 0.0], [0.019, 0.981]]
 > emissions = [0.04, 0.459]
+> chromosomes to use: All
 > number of windows: 99970 . Number of snps =  4230
 > total callability: 1.0
 > average mutation rate per bin: 1.0
-> Output is /dev/stdout
+> Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 chrom  start     end       length    state    mean_prob  snps
-chr1   0         7233000   7234000   Human    0.9995     287
-chr1   7234000   7246000   13000     Archaic  0.90427    9
-chr1   7247000   21618000  14372000  Human    0.99946    610
-chr1   21619000  21673000  55000     Archaic  0.9697     22
-chr1   21674000  26859000  5186000   Human    0.99878    204
-chr1   26860000  26941000  82000     Archaic  0.971      36
-chr1   26942000  49989000  23048000  Human    0.99982    863
-chr2   0         6793000   6794000   Human    0.99972    237
-chr2   6794000   6822000   29000     Archaic  0.95461    14
-chr2   6823000   12646000  5824000   Human    0.99927    244
-chr2   12647000  12745000  99000     Archaic  0.97413    55
-chr2   12746000  15461000  2716000   Human    0.99881    125
-chr2   15462000  15547000  86000     Archaic  0.93728    38
-chr2   15548000  32626000  17079000  Human    0.99951    709
-chr2   32627000  32695000  69000     Archaic  0.98305    31
-chr2   32696000  41087000  8392000   Human    0.9995     360
-chr2   41088000  41178000  91000     Archaic  0.96092    43
-chr2   41179000  49952000  8774000   Human    0.99789    328
-chr2   49953000  49977000  25000     Archaic  0.98501    13
+chr1   0         7234000   7234000   Human    0.9995     287
+chr1   7234000   7247000   13000     Archaic  0.90427    9
+chr1   7247000   21619000  14372000  Human    0.99946    610
+chr1   21619000  21674000  55000     Archaic  0.9697     22
+chr1   21674000  26860000  5186000   Human    0.99878    204
+chr1   26860000  26942000  82000     Archaic  0.971      36
+chr1   26942000  49991000  23049000  Human    0.99982    864
+chr2   0         6794000   6794000   Human    0.99972    237
+chr2   6794000   6823000   29000     Archaic  0.95461    14
+chr2   6823000   12647000  5824000   Human    0.99927    244
+chr2   12647000  12746000  99000     Archaic  0.97413    55
+chr2   12746000  15462000  2716000   Human    0.99881    125
+chr2   15462000  15548000  86000     Archaic  0.93728    38
+chr2   15548000  32627000  17079000  Human    0.99951    709
+chr2   32627000  32696000  69000     Archaic  0.98305    31
+chr2   32696000  41088000  8392000   Human    0.9995     360
+chr2   41088000  41179000  91000     Archaic  0.96092    43
+chr2   41179000  49953000  8774000   Human    0.99789    328
+chr2   49953000  49979000  26000     Archaic  0.98515    14
 
 # Again here you could ommit weights and mutationrates. Actually one could also ommit trained.json because then the model defaults to using the parameters we used the generated the data
-> hmmix decode -obs=obs.txt
+> hmmix decode -obs=obs.txt -param=trained.json
 ```
 
 ---
 
 ## Example with 1000 genomes data
 
 ---
 
 The whole pipeline we will run looks like this. In the following section we will go through all the steps on the way
+NOTE: The outgroup files, mutation rate files and callability files are now premade! They can be downloaded in hg38 and hg19 here: https://doi.org/10.5281/zenodo.10806733
+But keep reading along if you want to know HOW the files were generated!
 
 ```note
 hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa -refgenome=referencegenome/*fa
 hmmix mutation_rate -outgroup=outgroup.txt  -weights=strickmask.bed -window_size=1000000 -out mutationrate.bed
 hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
 hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json 
@@ -301,15 +333,16 @@
 # Ancestral information
 ftp://ftp.ensembl.org/pub/release-74/fasta/ancestral_alleles/homo_sapiens_ancestor_GRCh37_e71.tar.bz2
 
 # Reference genome
 wget 'ftp://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/chromFa.tar.gz' -O chromFa.tar.gz
 
 # Archaic variants (Altai, Vindija, Chagyrskaya and Denisova in hg19)
-https://zenodo.org/record/7246376#.Y1cRBkrMJH4
+https://zenodo.org/records/7246376
+
 ```
 
 For this example we will use all individuals from 'YRI','MSL' and 'ESN' as outgroup individuals. While we will only be decoding hG00096 in this example you can add as many individuals as you want to the ingroup.  
 
 ```json
 {
   "ingroup": [
@@ -328,32 +361,32 @@
 ---
 
 ### Finding snps which are derived in the outgroup
 
 First we need to find a set of variants found in the outgroup. We can use the wildcard character to loop through all bcf files. If you dont have ancestral information you can skip the ancestral argument.
 
 ```bash
-(took an hour) > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+(took an hour) > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa 
 
 # Alternative usage (if you only have a few individual in the outgroup you can also provide a comma separated list)
-> hmmix create_outgroup -ind=HG02922,HG02923,HG02938 -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+> hmmix create_outgroup -ind=HG02922,HG02923,HG02938 -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa 
 
 # Alternative usage (if you have no ancestral information)
 > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt 
 
 # Alternative usage (if you only want to run the model on a subset of chromosomes, with or without ancestral information)
 > hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf -weights=strickmask.bed -out=outgroup.txt
 
 > hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_1.fa,homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_2.fa
 ```
 
 Something to note is that if you use an outgroup vcffile (like 1000 genomes) and an ingroup vcf file from a different dataset (like SGDP) there is an edge case which could occur. There could be recurrent mutations where every individual in 1000 genome has the derived variant and one individual in SGDP where the derived variant has mutated back to the ancestral allele. This means that this position will not be present in the outgroup file. However if a recurrent mutation occurs it will look like multiple individuals in the ingroup file have the mutation. This does not happen often but just in case you can create the outgroup file and adding the sites which are fixed derived in all individuals using the reference genome:
 
 ```bash
-# Alternative usage (if you want to remove sites which are fixed derived in your outgroup/ingroup)
+# Recommended usage (if you want to remove sites which are fixed derived in your outgroup/ingroup)
 > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa -refgenome=*fa
 ```
 
 ---
 
 ### Estimating mutation rate across genome
 
@@ -427,148 +460,160 @@
 ```note
 (took 2 min) > hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.98, 0.02]
 > transitions = [[1.0, 0.0], [0.02, 0.98]]
 > emissions = [0.04, 0.4]
+> chromosomes to use: All
 > number of windows: 2877010 . Number of snps =  129734
 > total callability: 0.72
 > average mutation rate per bin: 1.0
-> Output is trained.HG00096_new.json
+> Output is trained.HG00096.json
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -492288.9165   0.98    0.02    0.04    0.4     0.9999    0.98
-1          -488899.7271   0.961   0.039   0.0483  0.3913  0.9994    0.986
-2          -488755.4068   0.958   0.042   0.0481  0.3911  0.9993    0.9835
+0          -492287.8643   0.98    0.02    0.04    0.4     0.9999    0.98
+1          -488898.6051   0.961   0.039   0.0483  0.3913  0.9994    0.986
+2          -488754.2455   0.958   0.042   0.0481  0.3911  0.9993    0.9835
 ...
-19         -488642.2737   0.954   0.046   0.047   0.3862  0.9989    0.9771
-20         -488642.2723   0.954   0.046   0.047   0.3862  0.9989    0.9771
-21         -488642.2716   0.954   0.046   0.047   0.3862  0.9989    0.9771
+19         -488641.0769   0.954   0.046   0.047   0.3862  0.9989    0.9771
+20         -488641.0755   0.954   0.046   0.047   0.3862  0.9989    0.9771
+21         -488641.0748   0.954   0.046   0.047   0.3862  0.9989    0.9771
 ```
 
 ---
 
 ### Decoding
 
 ```note
 (took 30 sec) > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json 
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.954, 0.046]
 > transitions = [[0.999, 0.001], [0.023, 0.977]]
 > emissions = [0.047, 0.386]
+> chromosomes to use: All
 > number of windows: 2877010 . Number of snps =  129734
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 chrom  start    end      length   state    mean_prob  snps
-1      0        2987000  2988000  Human    0.98484    91
-1      2988000  2996000  9000     Archaic  0.71815    6
-1      2997000  3424000  428000   Human    0.98944    30
-1      3425000  3451000  27000    Archaic  0.95652    22
-1      3452000  4301000  850000   Human    0.98203    36
-1      4302000  4360000  59000    Archaic  0.84636    20
-1      4361000  4499000  139000   Human    0.97136    4
-1      4500000  4509000  10000    Archaic  0.84456    7
+1      0        2988000  2988000  Human    0.98484    91
+1      2988000  2997000  9000     Archaic  0.71819    6
+1      2997000  3425000  428000   Human    0.98944    30
+1      3425000  3452000  27000    Archaic  0.95652    22
+1      3452000  4302000  850000   Human    0.98203    36
+1      4302000  4361000  59000    Archaic  0.84636    20
+1      4361000  4500000  139000   Human    0.97136    4
+1      4500000  4510000  10000    Archaic  0.84457    7
 ```
 
 You can also save to an output file with the command:
 
 ```note
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json -out=HG00096.decoded
 ```
 
 This will create a file named HG00096.decoded.diploid.txt because the default option is treating the data as diploid (more on haploid decoding in next chapter)
 
 ---
 
 ### Training and decoding with phased data
 
-It is also possible to tell the model that the data is phased with the -haploid parameter. For that we first need to train the parameters for haploid data and then decode. Training the model on phased data is done like this - and we also remember to change the name of the parameter file to include phased so future versions of ourselves don't forget. Another thing to note is that the number of snps is bigger than before 134799 vs 129149. This is because the program is counting snps on both haplotypes and homozygotes will be counted twice!
+It is also possible to tell the model that the data is phased with the -haploid parameter. For that we first need to train the parameters for haploid data and then decode. Training the model on phased data is done like this - and we also remember to change the name of the parameter file to include phased so future versions of ourselves don't forget. Another thing to note is that the number of snps is bigger than before 135411 vs 129734. This is because the program is counting snps on both haplotypes and homozygotes will be counted twice!
 
 ```note
 (took 4 min) > hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.phased.json -haploid
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.98, 0.02]
 > transitions = [[1.0, 0.0], [0.02, 0.98]]
 > emissions = [0.04, 0.4]
+> chromosomes to use: All
 > number of windows: 5754020 . Number of snps =  135411
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output is trained.HG00096.phased.json
 > Window size is 1000 bp
 > Haploid True
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -597753.9141   0.98    0.02    0.04    0.4     0.9999    0.98
-1          -585032.3914   0.983   0.017   0.0261  0.4026  0.9998    0.9853
-2          -584451.0968   0.979   0.021   0.0252  0.373   0.9996    0.9826
+0          -597750.7043   0.98    0.02    0.04    0.4     0.9999    0.98
+1          -585028.8828   0.983   0.017   0.0261  0.4026  0.9998    0.9853
+2          -584447.5809   0.979   0.021   0.0252  0.373   0.9996    0.9826
 ...
-19         -584134.532    0.972   0.028   0.0241  0.3367  0.9993    0.9758
-20         -584134.5305   0.972   0.028   0.0241  0.3366  0.9993    0.9758
-21         -584134.5297   0.972   0.028   0.0241  0.3366  0.9993    0.975
+19         -584131.0153   0.972   0.028   0.0241  0.3367  0.9993    0.9758
+20         -584131.0138   0.972   0.028   0.0241  0.3367  0.9993    0.9758
+21         -584131.013    0.972   0.028   0.0241  0.3366  0.9993    0.9758
 ```
 
 Below I am only showing the first archaic segments on chromosome 1 for each haplotype (note you have to scroll down after chrom 22 before the new haplotype begins). The seem to fall more or less in the same places as when we used diploid data.
 
 ```note
 (took 30 sec) > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.phased.json -haploid
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.972, 0.028]
 > transitions = [[0.999, 0.001], [0.024, 0.976]]
 > emissions = [0.024, 0.337]
+> chromosomes to use: All
 > number of windows: 5754020 . Number of snps =  135411
 > total callability: 0.72
 > average mutation rate per bin: 1.0
-> Output prefix is HG00096.decoded
+> Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid True
 ----------------------------------------
 hap1
 chrom  start    end      length  state    mean_prob  snps
-1      2162000  2184000  23000   Archaic  0.61055    6
-1      3425000  3451000  27000   Archaic  0.96595    22
+1      2162000  2185000  23000   Archaic  0.61054    6
+1      3425000  3452000  27000   Archaic  0.96595    22
 
 ...
 hap2
-1      2780000  2802000  23000   Archaic  0.61948    7
-1      4302000  4336000  35000   Archaic  0.94008    13
-1      4500000  4510000  11000   Archaic  0.87592    7
-1      4989000  4999000  11000   Archaic  0.57897    4
+1      2780000  2803000  23000   Archaic  0.61948    7
+1      4302000  4337000  35000   Archaic  0.94008    13
+1      4500000  4511000  11000   Archaic  0.87592    7
+1      4989000  5000000  11000   Archaic  0.579      4
 ```
 
 You can also save to an output file with the command:
 
 ```note
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.phased.json -haploid -out=HG00096.decoded
 ```
 
 This will create two files named HG00096.decoded.hap1.txt and HG00096.decoded.hap2.txt
 
 ---
 
 ### Annotate with known admixing population
 
-Even though this method does not use archaic reference genomes for finding segments you can still use them to annotate your segments. If you have a vcf from the population that admixed in VCF/BCF format you can write this:
+Even though this method does not use archaic reference genomes for finding segments you can still use them to annotate your segments. 
+I have uploaded a VCF file containing 4 high coverage archaic genomes (3 Neanderthals and 1 Denisovan) here:
+
+https://zenodo.org/records/7246376 (hg19 - the one I use in this example)
+
+https://zenodo.org/records/10806726 (hg38)
+
+If you have a vcf from the population that admixed in VCF/BCF format you can write this:
 
 ```note
 > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json -admixpop=archaicvar/*bcf
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.954, 0.046]
 > transitions = [[0.999, 0.001], [0.023, 0.977]]
 > emissions = [0.047, 0.386]
+> chromosomes to use: All
 > number of windows: 2877010 . Number of snps =  129734
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
@@ -593,21 +638,21 @@
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_5.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_8.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_11.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_12.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_13.bcf
 
 chrom  start     end       length  state    mean_prob  snps  admixpopvariants  AltaiNeandertal  Vindija33.19  Denisova  Chagyrskaya-Phalanx
-1      2988000   2996000   9000    Archaic  0.71815    6     4                 4                4             1         4
-1      3425000   3451000   27000   Archaic  0.95652    22    17                17               15            3         17
-1      4302000   4360000   59000   Archaic  0.84636    20    12                11               12            11        11
-1      4500000   4509000   10000   Archaic  0.84456    7     5                 4                5             4         5
-1      5339000   5346000   8000    Archaic  0.58909    4     3                 2                3             0         3
-1      9322000   9354000   33000   Archaic  0.8475     9     0                 0                0             0         0
-1      12599000  12653000  55000   Archaic  0.9142     18    11                4                11            0         10
+1      2988000   2997000   9000    Archaic  0.71819    6     4                 4                4             1         4
+1      3425000   3452000   27000   Archaic  0.95652    22    17                17               15            3         17
+1      4302000   4361000   59000   Archaic  0.84636    20    12                11               12            11        11
+1      4500000   4510000   10000   Archaic  0.84457    7     5                 4                5             4         5
+1      5339000   5347000   8000    Archaic  0.58914    4     3                 2                3             0         3
+1      9322000   9355000   33000   Archaic  0.84751    9     0                 0                0             0         0
+1      12599000  12654000  55000   Archaic  0.9142     18    11                4                11            0         10
 
 ```
 
 For the first segment there are 6 derived snps. Of these snps 4 are shared with Altai,Vindija, Denisova and Chagyrskaya. Only 1 is shared with Denisova so this segment likeli introgressed from Neanderthals
 
 ---
 
@@ -627,24 +672,24 @@
 # Initial HMM guess
 initial_hmm_params = HMMParam(state_names = ['Human', 'Archaic'], 
                               starting_probabilities = [0.5, 0.5], 
                               transitions = [[0.99,0.01],[0.02,0.98]], 
                               emissions = [0.03, 0.3]) 
 
 # Create test data
-obs, chroms, starts, variants, weights, mutrates  = create_test_data(50000, write_out_files = False)
+obs, chroms, starts, variants, mutrates, weights  = create_test_data(50000, write_out_files = False)
 
 # Train model
 hmm_parameters = TrainModel(obs, mutrates, weights, initial_hmm_params)
 
 # Decode model
 segments = DecodeModel(obs, chroms, starts, variants, mutrates, weights, hmm_parameters)
 
 for segment_info in segments:
-    chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, variants = segment_info
+    chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, called_sequence, average_mutation_rate, variants = segment_info
     print(chrom, genome_start,  genome_end, genome_length, state, mean_prob, snp_counter, sep = '\t')
 
 
 
 # -----------------------------------------------------------------------------
 # Running on an individual from 1000 genomes
 # -----------------------------------------------------------------------------
@@ -655,23 +700,19 @@
                                                                                       mutrates_file = 'mutationrate.bed', 
                                                                                       window_size = 1000, 
                                                                                       haploid = False)
 
 segments = DecodeModel(obs, chroms, starts, variants, mutrates, weights, hmm_parameters)
 
 for segment_info in segments:  
-    chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, variants = segment_info
+    chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, called_sequence, average_mutation_rate, variants = segment_info
     print(chrom, genome_start,  genome_end, genome_length, state, mean_prob, snp_counter, sep = '\t')
 
 
 ```
 
 And that is it! Now you have run the model and gotten a set of parameters that you can interpret biologically (see my paper) and you have a list of segments that belong to the human and Archaic state.
 
 If you have any questions about the use of the scripts, if you find errors or if you have feedback you can contact my here (make an issue) or write to:
-
----
-Contact:
-
 lauritsskov2@gmail.com
```

### Comparing `hmmix-0.6.9/README.md` & `hmmix-0.7.0/src/hmmix.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,61 @@
+Metadata-Version: 2.1
+Name: hmmix
+Version: 0.7.0
+Summary: Find introgressed segments
+Home-page: https://github.com/LauritsSkov/Introgression-detection
+Author: Laurits Skov and Moises Coll Macia
+Author-email: lauritsskov2@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Contact
+https://sites.google.com/view/laurits-skov
+
+---
+
+# Helpful files
+The outgroup files, mutation rate files and callability files and ancestral allele files are now premade! 
+
+https://doi.org/10.5281/zenodo.10806733 (hg19 and hg38)
+
+VCF file containing 4 high coverage archaic genomes (Altai, Vindija and Chagyrskaya Neanderthals and Denisovan) here: 
+
+https://zenodo.org/records/7246376 (hg19)
+
+https://zenodo.org/records/10806726 (hg38)
+
+---
 
 # Introgression detection
 
+If you are working with archaic introgression into present-day humans of non-African ancestry you can use these files and skip the following steps:
+Find derived variants in outgroup and Estimate local mutation rate. 
+
 These are the scripts needed to infere archaic introgression in modern populations using an unadmixed outgroup.
 
 1. [Installation](#installation)
 2. [Usage](#usage)
 3. [Quick tutorial](#quick-tutorial)
 4. [1000 genomes tutorial](#example-with-1000-genomes-data)
       - [Get data](#getting-data)
       - [Find derived variants in outgroup](#finding-snps-which-are-derived-in-the-outgroup)
       - [Estimate local mutation rate](#estimating-mutation-rate-across-genome)
       - [Find variants in ingroup](#find-a-set-of-variants-which-are-not-derived-in-the-outgroup)
       - [Train the HMM](#training)
       - [Decoding](#decoding)
       - [Phased data](#training-and-decoding-with-phased-data)
       - [Annotate](#annotate-with-known-admixing-population)
-      - [Run in python](#annotate-with-known-admixing-population)
+5. [Run in python](#annotate-with-known-admixing-population)
 
 ---
 
 ## Installation
 
 Run the following command to install:
 
@@ -56,15 +92,16 @@
 hmmix make_test_data 
 hmmix train  -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=Initialguesses.json -out=trained.json 
 hmmix decode -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=trained.json
 
 
 Different modes (you can also see the options for each by writing hmmix make_test_data -h):
 > make_test_data        
-    -windows            Number of Kb windows to create (defaults to 50,000)
+    -windows            Number of Kb windows to create (defaults to 50,000 per chromosome)
+    -chromosomes        Number of chromosomes to simulate (defaults to 2)
     -nooutfiles         Don't create obs.txt, mutrates.bed, weights.bed, Initialguesses.json (defaults to yes)
 
 > mutation_rate         
     -outgroup           [required] path to variants found in outgroup
     -out                outputfile (defaults to mutationrate.bed)
     -weights            file with callability (defaults to all positions being called)
     -window_size        size of bins (defaults to 1 Mb)
@@ -83,30 +120,45 @@
     -outgroup           [required] path to variant found in outgroup
     -weights            file with callability (defaults to all positions being called)
     -out                outputfile prefix (default is a file named obs.<ind>.txt where ind is the name of individual in ingroup/outgrop list)
     -ancestral          fasta file with ancestral information - comma-separated list or wildcards like vcf argument (default none)
 
 > train                 
     -obs                [required] file with observation data
+    -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
     -weights            file with callability (defaults to all positions being called)
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
     -out                outputfile (default is a file named trained.json)
     -window_size        size of bins (default is 1000 bp)
     -haploid            Change from using diploid data to haploid data (default is diploid)
 
 > decode                
     -obs                [required] file with observation data
+    -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
     -weights            file with callability (defaults to all positions being called)
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
     -out                outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)
     -window_size        size of bins (default is 1000 bp)
     -haploid            Change from using diploid data to haploid data (default is diploid)
-    -admixpop ADMIXPOP  Annotate using vcffile with admixing population (default is none)
+    -admixpop           Annotate using vcffile with admixing population (default is none)
+    -extrainfo          Add variant position for each SNP (default is off)
+
+> inhomogeneous                
+    -obs                [required] file with observation data
+    -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
+    -weights            file with callability (defaults to all positions being called)
+    -mutrates           file with mutation rates (default is mutation rate is uniform)
+    -param              markov parameters file (default is human/neanderthal like parameters)
+    -out                outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)
+    -window_size        size of bins (default is 1000 bp)
+    -haploid            Change from using diploid data to haploid data (default is diploid)
+    -samples            Number of simulated paths for the inhomogeneous markov chain (default is 100)
+    -admixpop           Annotate using vcffile with admixing population (default is none)
     -extrainfo          Add variant position for each SNP (default is off)
 ```
 
 ---
 
 ## Quick tutorial
 
@@ -140,27 +192,19 @@
 weights.bed. This is the parts of the genome that we can accurately map to - in this case we have simulated the data and can accurately access the entire genome.
 
 ```note
 chr1   0   50000000
 chr2   0   50000000
 ```
 
-mutrates.bed. This is the normalized mutation rate across the genome (in bins of 1 Mb).
+mutrates.bed. This is the normalized mutation rate across the genome.
 
 ```note
-chr1  0        1000000   1
-chr1  1000000  2000000   1
-chr1  2000000  3000000   1
-chr1  3000000  4000000   1
-chr1  4000000  5000000   1
-chr1  5000000  6000000   1
-chr1  6000000  7000000   1
-chr1  7000000  8000000   1
-chr1  8000000  9000000   1
-chr1  9000000  10000000  1
+chr1   0   50000000   1
+chr2   0   50000000   1
 ```
 
 Initialguesses.json. This is our initial guesses when training the model - note these are different from those we simulated from.
 
 ```json
 {
   "state_names": ["Human","Archaic"],
@@ -175,29 +219,30 @@
 ```note
 > hmmix train  -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=Initialguesses.json -out=trained.json
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.5, 0.5]
 > transitions = [[0.99, 0.01], [0.02, 0.98]]
 > emissions = [0.03, 0.3]
+> chromosomes to use: All
 > number of windows: 99970 . Number of snps =  4230
 > total callability: 1.0
 > average mutation rate per bin: 1.0
 > Output is trained.json
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -18123.4432    0.5     0.5     0.03    0.3     0.99      0.98
-1          -17506.017     0.96    0.04    0.035   0.2202  0.9969    0.9242
-2          -17487.7921    0.971   0.029   0.0369  0.2235  0.9974    0.9141
+0          -18123.4598    0.5     0.5     0.03    0.3     0.99      0.98
+1          -17506.0258    0.96    0.04    0.035   0.2202  0.9969    0.9242
+2          -17487.8       0.971   0.029   0.0369  0.2235  0.9974    0.9141
 ...
-16         -17401.3802    0.994   0.006   0.0398  0.4584  0.9999    0.9806
-17         -17401.3786    0.994   0.006   0.0398  0.4586  0.9999    0.9807
-18         -17401.3783    0.994   0.006   0.0398  0.4587  0.9999    0.9808
+16         -17401.3853    0.994   0.006   0.0398  0.4584  0.9999    0.9806
+17         -17401.3838    0.994   0.006   0.0398  0.4586  0.9999    0.9807
+18         -17401.3835    0.994   0.006   0.0398  0.4587  0.9999    0.9808
 
 
 # run without mutrate and weights (only do this for simulated data)
 > hmmix train  -obs=obs.txt -param=Initialguesses.json -out=trained.json
 ```
 
 We can now decode the data with the best parameters that maximize the likelihood and find the archaic segments:
@@ -205,53 +250,56 @@
 ```note
 > hmmix decode -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=trained.json
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.994, 0.006]
 > transitions = [[1.0, 0.0], [0.019, 0.981]]
 > emissions = [0.04, 0.459]
+> chromosomes to use: All
 > number of windows: 99970 . Number of snps =  4230
 > total callability: 1.0
 > average mutation rate per bin: 1.0
-> Output is /dev/stdout
+> Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 chrom  start     end       length    state    mean_prob  snps
-chr1   0         7233000   7234000   Human    0.9995     287
-chr1   7234000   7246000   13000     Archaic  0.90427    9
-chr1   7247000   21618000  14372000  Human    0.99946    610
-chr1   21619000  21673000  55000     Archaic  0.9697     22
-chr1   21674000  26859000  5186000   Human    0.99878    204
-chr1   26860000  26941000  82000     Archaic  0.971      36
-chr1   26942000  49989000  23048000  Human    0.99982    863
-chr2   0         6793000   6794000   Human    0.99972    237
-chr2   6794000   6822000   29000     Archaic  0.95461    14
-chr2   6823000   12646000  5824000   Human    0.99927    244
-chr2   12647000  12745000  99000     Archaic  0.97413    55
-chr2   12746000  15461000  2716000   Human    0.99881    125
-chr2   15462000  15547000  86000     Archaic  0.93728    38
-chr2   15548000  32626000  17079000  Human    0.99951    709
-chr2   32627000  32695000  69000     Archaic  0.98305    31
-chr2   32696000  41087000  8392000   Human    0.9995     360
-chr2   41088000  41178000  91000     Archaic  0.96092    43
-chr2   41179000  49952000  8774000   Human    0.99789    328
-chr2   49953000  49977000  25000     Archaic  0.98501    13
+chr1   0         7234000   7234000   Human    0.9995     287
+chr1   7234000   7247000   13000     Archaic  0.90427    9
+chr1   7247000   21619000  14372000  Human    0.99946    610
+chr1   21619000  21674000  55000     Archaic  0.9697     22
+chr1   21674000  26860000  5186000   Human    0.99878    204
+chr1   26860000  26942000  82000     Archaic  0.971      36
+chr1   26942000  49991000  23049000  Human    0.99982    864
+chr2   0         6794000   6794000   Human    0.99972    237
+chr2   6794000   6823000   29000     Archaic  0.95461    14
+chr2   6823000   12647000  5824000   Human    0.99927    244
+chr2   12647000  12746000  99000     Archaic  0.97413    55
+chr2   12746000  15462000  2716000   Human    0.99881    125
+chr2   15462000  15548000  86000     Archaic  0.93728    38
+chr2   15548000  32627000  17079000  Human    0.99951    709
+chr2   32627000  32696000  69000     Archaic  0.98305    31
+chr2   32696000  41088000  8392000   Human    0.9995     360
+chr2   41088000  41179000  91000     Archaic  0.96092    43
+chr2   41179000  49953000  8774000   Human    0.99789    328
+chr2   49953000  49979000  26000     Archaic  0.98515    14
 
 # Again here you could ommit weights and mutationrates. Actually one could also ommit trained.json because then the model defaults to using the parameters we used the generated the data
-> hmmix decode -obs=obs.txt
+> hmmix decode -obs=obs.txt -param=trained.json
 ```
 
 ---
 
 ## Example with 1000 genomes data
 
 ---
 
 The whole pipeline we will run looks like this. In the following section we will go through all the steps on the way
+NOTE: The outgroup files, mutation rate files and callability files are now premade! They can be downloaded in hg38 and hg19 here: https://doi.org/10.5281/zenodo.10806733
+But keep reading along if you want to know HOW the files were generated!
 
 ```note
 hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa -refgenome=referencegenome/*fa
 hmmix mutation_rate -outgroup=outgroup.txt  -weights=strickmask.bed -window_size=1000000 -out mutationrate.bed
 hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
 hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json 
@@ -285,15 +333,16 @@
 # Ancestral information
 ftp://ftp.ensembl.org/pub/release-74/fasta/ancestral_alleles/homo_sapiens_ancestor_GRCh37_e71.tar.bz2
 
 # Reference genome
 wget 'ftp://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/chromFa.tar.gz' -O chromFa.tar.gz
 
 # Archaic variants (Altai, Vindija, Chagyrskaya and Denisova in hg19)
-https://zenodo.org/record/7246376#.Y1cRBkrMJH4
+https://zenodo.org/records/7246376
+
 ```
 
 For this example we will use all individuals from 'YRI','MSL' and 'ESN' as outgroup individuals. While we will only be decoding hG00096 in this example you can add as many individuals as you want to the ingroup.  
 
 ```json
 {
   "ingroup": [
@@ -312,32 +361,32 @@
 ---
 
 ### Finding snps which are derived in the outgroup
 
 First we need to find a set of variants found in the outgroup. We can use the wildcard character to loop through all bcf files. If you dont have ancestral information you can skip the ancestral argument.
 
 ```bash
-(took an hour) > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+(took an hour) > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa 
 
 # Alternative usage (if you only have a few individual in the outgroup you can also provide a comma separated list)
-> hmmix create_outgroup -ind=HG02922,HG02923,HG02938 -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+> hmmix create_outgroup -ind=HG02922,HG02923,HG02938 -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa 
 
 # Alternative usage (if you have no ancestral information)
 > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt 
 
 # Alternative usage (if you only want to run the model on a subset of chromosomes, with or without ancestral information)
 > hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf -weights=strickmask.bed -out=outgroup.txt
 
 > hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_1.fa,homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_2.fa
 ```
 
 Something to note is that if you use an outgroup vcffile (like 1000 genomes) and an ingroup vcf file from a different dataset (like SGDP) there is an edge case which could occur. There could be recurrent mutations where every individual in 1000 genome has the derived variant and one individual in SGDP where the derived variant has mutated back to the ancestral allele. This means that this position will not be present in the outgroup file. However if a recurrent mutation occurs it will look like multiple individuals in the ingroup file have the mutation. This does not happen often but just in case you can create the outgroup file and adding the sites which are fixed derived in all individuals using the reference genome:
 
 ```bash
-# Alternative usage (if you want to remove sites which are fixed derived in your outgroup/ingroup)
+# Recommended usage (if you want to remove sites which are fixed derived in your outgroup/ingroup)
 > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa -refgenome=*fa
 ```
 
 ---
 
 ### Estimating mutation rate across genome
 
@@ -411,148 +460,160 @@
 ```note
 (took 2 min) > hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.98, 0.02]
 > transitions = [[1.0, 0.0], [0.02, 0.98]]
 > emissions = [0.04, 0.4]
+> chromosomes to use: All
 > number of windows: 2877010 . Number of snps =  129734
 > total callability: 0.72
 > average mutation rate per bin: 1.0
-> Output is trained.HG00096_new.json
+> Output is trained.HG00096.json
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -492288.9165   0.98    0.02    0.04    0.4     0.9999    0.98
-1          -488899.7271   0.961   0.039   0.0483  0.3913  0.9994    0.986
-2          -488755.4068   0.958   0.042   0.0481  0.3911  0.9993    0.9835
+0          -492287.8643   0.98    0.02    0.04    0.4     0.9999    0.98
+1          -488898.6051   0.961   0.039   0.0483  0.3913  0.9994    0.986
+2          -488754.2455   0.958   0.042   0.0481  0.3911  0.9993    0.9835
 ...
-19         -488642.2737   0.954   0.046   0.047   0.3862  0.9989    0.9771
-20         -488642.2723   0.954   0.046   0.047   0.3862  0.9989    0.9771
-21         -488642.2716   0.954   0.046   0.047   0.3862  0.9989    0.9771
+19         -488641.0769   0.954   0.046   0.047   0.3862  0.9989    0.9771
+20         -488641.0755   0.954   0.046   0.047   0.3862  0.9989    0.9771
+21         -488641.0748   0.954   0.046   0.047   0.3862  0.9989    0.9771
 ```
 
 ---
 
 ### Decoding
 
 ```note
 (took 30 sec) > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json 
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.954, 0.046]
 > transitions = [[0.999, 0.001], [0.023, 0.977]]
 > emissions = [0.047, 0.386]
+> chromosomes to use: All
 > number of windows: 2877010 . Number of snps =  129734
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 chrom  start    end      length   state    mean_prob  snps
-1      0        2987000  2988000  Human    0.98484    91
-1      2988000  2996000  9000     Archaic  0.71815    6
-1      2997000  3424000  428000   Human    0.98944    30
-1      3425000  3451000  27000    Archaic  0.95652    22
-1      3452000  4301000  850000   Human    0.98203    36
-1      4302000  4360000  59000    Archaic  0.84636    20
-1      4361000  4499000  139000   Human    0.97136    4
-1      4500000  4509000  10000    Archaic  0.84456    7
+1      0        2988000  2988000  Human    0.98484    91
+1      2988000  2997000  9000     Archaic  0.71819    6
+1      2997000  3425000  428000   Human    0.98944    30
+1      3425000  3452000  27000    Archaic  0.95652    22
+1      3452000  4302000  850000   Human    0.98203    36
+1      4302000  4361000  59000    Archaic  0.84636    20
+1      4361000  4500000  139000   Human    0.97136    4
+1      4500000  4510000  10000    Archaic  0.84457    7
 ```
 
 You can also save to an output file with the command:
 
 ```note
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json -out=HG00096.decoded
 ```
 
 This will create a file named HG00096.decoded.diploid.txt because the default option is treating the data as diploid (more on haploid decoding in next chapter)
 
 ---
 
 ### Training and decoding with phased data
 
-It is also possible to tell the model that the data is phased with the -haploid parameter. For that we first need to train the parameters for haploid data and then decode. Training the model on phased data is done like this - and we also remember to change the name of the parameter file to include phased so future versions of ourselves don't forget. Another thing to note is that the number of snps is bigger than before 134799 vs 129149. This is because the program is counting snps on both haplotypes and homozygotes will be counted twice!
+It is also possible to tell the model that the data is phased with the -haploid parameter. For that we first need to train the parameters for haploid data and then decode. Training the model on phased data is done like this - and we also remember to change the name of the parameter file to include phased so future versions of ourselves don't forget. Another thing to note is that the number of snps is bigger than before 135411 vs 129734. This is because the program is counting snps on both haplotypes and homozygotes will be counted twice!
 
 ```note
 (took 4 min) > hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.phased.json -haploid
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.98, 0.02]
 > transitions = [[1.0, 0.0], [0.02, 0.98]]
 > emissions = [0.04, 0.4]
+> chromosomes to use: All
 > number of windows: 5754020 . Number of snps =  135411
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output is trained.HG00096.phased.json
 > Window size is 1000 bp
 > Haploid True
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -597753.9141   0.98    0.02    0.04    0.4     0.9999    0.98
-1          -585032.3914   0.983   0.017   0.0261  0.4026  0.9998    0.9853
-2          -584451.0968   0.979   0.021   0.0252  0.373   0.9996    0.9826
+0          -597750.7043   0.98    0.02    0.04    0.4     0.9999    0.98
+1          -585028.8828   0.983   0.017   0.0261  0.4026  0.9998    0.9853
+2          -584447.5809   0.979   0.021   0.0252  0.373   0.9996    0.9826
 ...
-19         -584134.532    0.972   0.028   0.0241  0.3367  0.9993    0.9758
-20         -584134.5305   0.972   0.028   0.0241  0.3366  0.9993    0.9758
-21         -584134.5297   0.972   0.028   0.0241  0.3366  0.9993    0.975
+19         -584131.0153   0.972   0.028   0.0241  0.3367  0.9993    0.9758
+20         -584131.0138   0.972   0.028   0.0241  0.3367  0.9993    0.9758
+21         -584131.013    0.972   0.028   0.0241  0.3366  0.9993    0.9758
 ```
 
 Below I am only showing the first archaic segments on chromosome 1 for each haplotype (note you have to scroll down after chrom 22 before the new haplotype begins). The seem to fall more or less in the same places as when we used diploid data.
 
 ```note
 (took 30 sec) > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.phased.json -haploid
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.972, 0.028]
 > transitions = [[0.999, 0.001], [0.024, 0.976]]
 > emissions = [0.024, 0.337]
+> chromosomes to use: All
 > number of windows: 5754020 . Number of snps =  135411
 > total callability: 0.72
 > average mutation rate per bin: 1.0
-> Output prefix is HG00096.decoded
+> Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid True
 ----------------------------------------
 hap1
 chrom  start    end      length  state    mean_prob  snps
-1      2162000  2184000  23000   Archaic  0.61055    6
-1      3425000  3451000  27000   Archaic  0.96595    22
+1      2162000  2185000  23000   Archaic  0.61054    6
+1      3425000  3452000  27000   Archaic  0.96595    22
 
 ...
 hap2
-1      2780000  2802000  23000   Archaic  0.61948    7
-1      4302000  4336000  35000   Archaic  0.94008    13
-1      4500000  4510000  11000   Archaic  0.87592    7
-1      4989000  4999000  11000   Archaic  0.57897    4
+1      2780000  2803000  23000   Archaic  0.61948    7
+1      4302000  4337000  35000   Archaic  0.94008    13
+1      4500000  4511000  11000   Archaic  0.87592    7
+1      4989000  5000000  11000   Archaic  0.579      4
 ```
 
 You can also save to an output file with the command:
 
 ```note
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.phased.json -haploid -out=HG00096.decoded
 ```
 
 This will create two files named HG00096.decoded.hap1.txt and HG00096.decoded.hap2.txt
 
 ---
 
 ### Annotate with known admixing population
 
-Even though this method does not use archaic reference genomes for finding segments you can still use them to annotate your segments. If you have a vcf from the population that admixed in VCF/BCF format you can write this:
+Even though this method does not use archaic reference genomes for finding segments you can still use them to annotate your segments. 
+I have uploaded a VCF file containing 4 high coverage archaic genomes (3 Neanderthals and 1 Denisovan) here:
+
+https://zenodo.org/records/7246376 (hg19 - the one I use in this example)
+
+https://zenodo.org/records/10806726 (hg38)
+
+If you have a vcf from the population that admixed in VCF/BCF format you can write this:
 
 ```note
 > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json -admixpop=archaicvar/*bcf
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.954, 0.046]
 > transitions = [[0.999, 0.001], [0.023, 0.977]]
 > emissions = [0.047, 0.386]
+> chromosomes to use: All
 > number of windows: 2877010 . Number of snps =  129734
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
@@ -577,21 +638,21 @@
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_5.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_8.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_11.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_12.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_13.bcf
 
 chrom  start     end       length  state    mean_prob  snps  admixpopvariants  AltaiNeandertal  Vindija33.19  Denisova  Chagyrskaya-Phalanx
-1      2988000   2996000   9000    Archaic  0.71815    6     4                 4                4             1         4
-1      3425000   3451000   27000   Archaic  0.95652    22    17                17               15            3         17
-1      4302000   4360000   59000   Archaic  0.84636    20    12                11               12            11        11
-1      4500000   4509000   10000   Archaic  0.84456    7     5                 4                5             4         5
-1      5339000   5346000   8000    Archaic  0.58909    4     3                 2                3             0         3
-1      9322000   9354000   33000   Archaic  0.8475     9     0                 0                0             0         0
-1      12599000  12653000  55000   Archaic  0.9142     18    11                4                11            0         10
+1      2988000   2997000   9000    Archaic  0.71819    6     4                 4                4             1         4
+1      3425000   3452000   27000   Archaic  0.95652    22    17                17               15            3         17
+1      4302000   4361000   59000   Archaic  0.84636    20    12                11               12            11        11
+1      4500000   4510000   10000   Archaic  0.84457    7     5                 4                5             4         5
+1      5339000   5347000   8000    Archaic  0.58914    4     3                 2                3             0         3
+1      9322000   9355000   33000   Archaic  0.84751    9     0                 0                0             0         0
+1      12599000  12654000  55000   Archaic  0.9142     18    11                4                11            0         10
 
 ```
 
 For the first segment there are 6 derived snps. Of these snps 4 are shared with Altai,Vindija, Denisova and Chagyrskaya. Only 1 is shared with Denisova so this segment likeli introgressed from Neanderthals
 
 ---
 
@@ -611,24 +672,24 @@
 # Initial HMM guess
 initial_hmm_params = HMMParam(state_names = ['Human', 'Archaic'], 
                               starting_probabilities = [0.5, 0.5], 
                               transitions = [[0.99,0.01],[0.02,0.98]], 
                               emissions = [0.03, 0.3]) 
 
 # Create test data
-obs, chroms, starts, variants, weights, mutrates  = create_test_data(50000, write_out_files = False)
+obs, chroms, starts, variants, mutrates, weights  = create_test_data(50000, write_out_files = False)
 
 # Train model
 hmm_parameters = TrainModel(obs, mutrates, weights, initial_hmm_params)
 
 # Decode model
 segments = DecodeModel(obs, chroms, starts, variants, mutrates, weights, hmm_parameters)
 
 for segment_info in segments:
-    chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, variants = segment_info
+    chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, called_sequence, average_mutation_rate, variants = segment_info
     print(chrom, genome_start,  genome_end, genome_length, state, mean_prob, snp_counter, sep = '\t')
 
 
 
 # -----------------------------------------------------------------------------
 # Running on an individual from 1000 genomes
 # -----------------------------------------------------------------------------
@@ -639,21 +700,19 @@
                                                                                       mutrates_file = 'mutationrate.bed', 
                                                                                       window_size = 1000, 
                                                                                       haploid = False)
 
 segments = DecodeModel(obs, chroms, starts, variants, mutrates, weights, hmm_parameters)
 
 for segment_info in segments:  
-    chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, variants = segment_info
+    chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, called_sequence, average_mutation_rate, variants = segment_info
     print(chrom, genome_start,  genome_end, genome_length, state, mean_prob, snp_counter, sep = '\t')
 
 
 ```
 
 And that is it! Now you have run the model and gotten a set of parameters that you can interpret biologically (see my paper) and you have a list of segments that belong to the human and Archaic state.
 
 If you have any questions about the use of the scripts, if you find errors or if you have feedback you can contact my here (make an issue) or write to:
+lauritsskov2@gmail.com
 
----
-Contact:
 
-lauritsskov2@gmail.com
```

### Comparing `hmmix-0.6.9/setup.py` & `hmmix-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='hmmix', 
-    version = '0.6.9',
+    version = '0.7.0',
     description='Find introgressed segments',
     py_modules=['bcf_vcf', 'helper_functions', 'hmm_functions', 'main', 'make_mutationrate', 'make_test_data'],
     package_dir={'': 'src'},
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `hmmix-0.6.9/src/bcf_vcf.py` & `hmmix-0.7.0/src/bcf_vcf.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.9/src/helper_functions.py` & `hmmix-0.7.0/src/helper_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,53 +45,78 @@
                     for window_tofil in range(firstwindow + window_size, lastwindow, window_size):
                         callability[chrom][window_tofil] += window_size * value
 
     return callability
 
 
 
-def Load_observations_weights_mutrates(obs_file, weights_file, mutrates_file, window_size = 1000, haploid = False):
+def Load_observations_weights_mutrates(obs_file, weights_file, mutrates_file, window_size = 1000, haploid = False, chrom_to_look_for = 'All'):
 
     obs_counter = defaultdict(lambda: defaultdict(lambda: defaultdict(list)))
     haplotypes = defaultdict(int)
 
+    if chrom_to_look_for != 'All':
+        chromosome_list = chrom_to_look_for.split(',')
+
     with open(obs_file) as data:
         for line in data:
             if not line.startswith('chrom'):
                 chrom, pos, ancestral_base, genotype = line.strip().split()
-                rounded_pos = int(pos) - int(pos) % window_size
 
-                if haploid:  
-                    for i, base in enumerate(genotype):
-                        if base != ancestral_base:
-                            obs_counter[chrom][rounded_pos][f'_hap{i+1}'].append(pos)
-                            haplotypes[f'_hap{i+1}'] += 1
+               
+                
+                keep_chromosome = False
+                if chrom_to_look_for == 'All':
+                    keep_chromosome = True
                 else:
-                    obs_counter[chrom][rounded_pos][''].append(pos)
-                    haplotypes[''] += 1
+                    if chrom in chromosome_list:
+                        keep_chromosome = True
+
+                if keep_chromosome:
+                     # convert 1-indexed position to 0-indexed position
+                    zero_based_pos = int(pos) - 1
+                    rounded_pos = zero_based_pos - zero_based_pos % window_size
+
+                    if haploid:  
+                        for i, base in enumerate(genotype):
+                            if base != ancestral_base:
+                                obs_counter[chrom][rounded_pos][f'_hap{i+1}'].append(pos)
+                                haplotypes[f'_hap{i+1}'] += 1
+                    else:
+                        obs_counter[chrom][rounded_pos][''].append(pos)
+                        haplotypes[''] += 1
 
 
     chroms, starts, variants, obs = [], [], [], []
     # In the case that there are NO derived variants - use weights to make list of zeros
     if len(obs_counter) == 0:
 
         if weights_file is None:
             sys.exit(f'{obs_file} is empty! You need to provide a bed file!')
 
         haplotypes[''] += 1
         callability = make_callability_from_bed(weights_file, window_size)
         for chrom in sorted(callability, key=sortby):
-            lastwindow = max(callability[chrom]) + window_size
 
-            for window in range(0, lastwindow, window_size):
-                obs_counter[chrom][window][''].append('')
-                chroms.append(f'{chrom}')   
-                starts.append(window)
-                variants.append('')  
-                obs.append(0) 
+            keep_variant = False
+            if chrom_to_look_for == 'All':
+                keep_variant = True
+            else:
+                if chrom in chromosome_list:
+                    keep_variant = True
+
+            if keep_variant:
+                lastwindow = max(callability[chrom]) + window_size
+
+                for window in range(0, lastwindow, window_size):
+                    obs_counter[chrom][window][''].append('')
+                    chroms.append(f'{chrom}')   
+                    starts.append(window)
+                    variants.append('')  
+                    obs.append(0) 
 
     # Otherwise fill out as normal
     else:
         for haplotype in sorted(haplotypes, key=sortby_haplotype):
             
             for chrom in sorted(obs_counter, key=sortby):
                 lastwindow = max(obs_counter[chrom]) + window_size
@@ -135,21 +160,21 @@
     # Make sure there are no places with obs > 0 and 0 in mutation rate or weight
     for index, (observation, w, m) in enumerate(zip(obs, weights, mutrates)):
         if w*m == 0 and observation != 0:
             print(f'warning, you had {observation} observations but no called bases/no mutation rate at index:{index}. weights:{w}, mutrates:{m}')
             obs[index] = 0
             
 
-
     return np.array(obs).astype(int), chroms, starts, variants, np.array(mutrates).astype(float), np.array(weights).astype(float)
 
 
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
 # For decoding/training
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
+
 def find_runs(inarray):
     """ run length encoding. Partial credit to R rle function. 
         Multi datatype arrays catered for including non Numpy
         returns: tuple (runlengths, startpositions, values) """
     ia = np.asarray(inarray)                # force numpy
     n = len(ia)
     if n == 0: 
@@ -269,24 +294,40 @@
 
 
 def Annotate_with_ref_genome(vcffiles, obsfile):
     obs = defaultdict(list)
     shared_with = defaultdict(str)
 
     tempobsfile = obsfile + 'temp'
-
     with open(obsfile) as data, open(tempobsfile,'w') as out:
         for line in data:
             if not line.startswith('chrom'):
                 out.write(line)
                 chrom, pos, ancestral_base, genotype = line.strip().split()
                 derived_variant = genotype.replace(ancestral_base, '')[0]
                 ID = f'{chrom}_{pos}'
                 obs[ID] = [ancestral_base, derived_variant]
 
+    # handle case with 0 SNPs
+    if len(obs) == 0:
+        for vcffile in handle_infiles(vcffiles):
+            command = f'bcftools view -h {vcffile}'
+            print('You have no observations!')
+
+            for line in os.popen(command):
+                if line.startswith('#CHROM'):
+                    individuals_in_vcffile = line.strip().split()[9:]
+
+            # Clean log files generated by vcf and bcf tools
+            clean_files('out.log')
+            clean_files(tempobsfile)
+
+            return shared_with, individuals_in_vcffile
+
+
     print('Loading in admixpop snp information')
     for vcffile in handle_infiles(vcffiles):
         command = f'bcftools view -a -R {tempobsfile} {vcffile}'
         print(command)
 
         for line in os.popen(command):
             if line.startswith('#CHROM'):
```

### Comparing `hmmix-0.6.9/src/hmm_functions.py` & `hmmix-0.7.0/src/hmm_functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from collections import defaultdict
 import numpy as np
 from numba import njit
 import json
-import math
 
 from helper_functions import find_runs, Annotate_with_ref_genome, Make_folder_if_not_exists, flatten_list
 
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
 # HMM Parameter Class
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
 class HMMParam:
@@ -75,34 +74,17 @@
 
 
 
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
 # HMM functions
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-
-# def Emission_probs_poisson(emissions, observations, weights, mutrates):
-#     n = len(observations)
-#     n_states = len(emissions)
-    
-#     # observations values
-#     fractorials = np.zeros(n)
-#     for i, obs in enumerate(observations):
-#         fractorials[i] = math.factorial(obs)
-
-#     probabilities = np.zeros( (n, n_states) ) 
-#     for state in range(n_states): 
-#         probabilities[:,state] = (np.exp( - emissions[state] * weights * mutrates) *  ((emissions[state] * weights * mutrates )**observations )) / fractorials
-
-#     return probabilities
-
-
 @njit
 def poisson_probability_underflow_safe(n, lam):
-    # naive:   math.exp(-lam) * lam**n / factorial(n)
+    # naive:   np.exp(-lam) * lam**n / factorial(n)
 
     # iterative, to keep the components from getting too large or small:
     p = np.exp(-lam)
     for i in range(n):
         p *= lam
         p /= i+1
     return p
@@ -119,33 +101,32 @@
             probabilities[index,state] = poisson_probability_underflow_safe(observations[index], lam)
 
     return probabilities
 
 
 
 
-
 @njit
 def fwd_step(alpha_prev, E, trans_mat):
     alpha_new = (alpha_prev @ trans_mat) * E
     n = np.sum(alpha_new)
     return alpha_new / n, n
 
+
 @njit
 def forward(probabilities, transitions, init_start):
-
     n = len(probabilities)
     forwards_in = np.zeros( (n, len(init_start)) ) 
     scale_param = np.ones(n)
 
     for t in range(n):
         if t == 0:
             forwards_in[t,:] = init_start  * probabilities[t,:]
             scale_param[t] = np.sum( forwards_in[t,:])
-            forwards_in[t,:] = forwards_in[t,:] / scale_param[t]
+            forwards_in[t,:] = forwards_in[t,:] / scale_param[t]  
         else:
             forwards_in[t,:], scale_param[t] =  fwd_step(forwards_in[t-1,:], probabilities[t,:], transitions) 
 
     return forwards_in, scale_param
     
 
 @njit
@@ -202,14 +183,123 @@
         for state2 in range(n_states):
             new_transitions_matrix[state1,state2] = np.sum( forward_probs[:-1,state1]  * hmm_parameters.transitions[state1, state2] * emissions[1:,state2] * backward_probs[1:,state2] / scales[1:] )
 
     new_transitions_matrix /=  new_transitions_matrix.sum(axis=1)[:,np.newaxis]
 
     return HMMParam(hmm_parameters.state_names,new_starting_probabilities, new_transitions_matrix, new_emissions_matrix)
 
+
+
+
+
+
+
+# ----------------------------------------------------------------------------------------------------------------------------------------------------------------
+# inhomogeneous markov chain
+# ----------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+
+@njit
+def Simulate_values(n_states, p):
+    return np.random.binomial(1, p)
+
+
+
+def Simulate_transition(n_states, matrix, current_state):
+
+    # prob of statying (can be done with numba so its quick)
+    next_state = Simulate_values(n_states, matrix[current_state])
+    if next_state == 1:
+        return current_state
+    
+    else:
+        if n_states == 2:
+            return abs(current_state - 1)
+        
+        else:
+            new_matrix = [matrix[x] for x in range(n_states) if current_state != x]
+            new_matrix /= np.sum(new_matrix)
+            new_states = [x for x in range(n_states) if current_state != x]
+
+            return np.random.choice(new_states, p=new_matrix)
+
+
+
+def inhomogeneous(hmm_parameters, weights, obs, mutrates, samples, chroms, starts, variants):
+    """
+    Calculate transition matrix for each position in the sequence (given the data)
+    """ 
+
+    n_states = len(hmm_parameters.starting_probabilities)
+    number_observations = len(obs)
+    emissions = Emission_probs_poisson(hmm_parameters.emissions, obs, weights, mutrates)   
+    window_size = starts[2] - starts[1] 
+
+    _, scales = forward(emissions, hmm_parameters.transitions, hmm_parameters.starting_probabilities)
+    backward_probs = backward(emissions, hmm_parameters.transitions, scales)
+
+    # Make and initialise new transition matrix
+    new_transition_matrix = np.zeros((number_observations, n_states, n_states))
+
+    for state in range(n_states):
+        for otherstate in range(n_states):
+            new_transition_matrix[1:, otherstate, state] = (backward_probs[1:, state] ) / (backward_probs[:-1, otherstate] * scales[1:]) * hmm_parameters.transitions[otherstate, state] * emissions[1:, state]
+    
+
+
+    segments = []
+    for sim_number in range(samples):
+        print(f'Running inhomogen markov chain simulation {sim_number + 1}/{samples}')
+
+        sim_path = np.zeros(number_observations, dtype=int)
+        
+        # set start state
+        current_state = np.random.choice(n_states, p=hmm_parameters.starting_probabilities)
+        sim_path[0] = current_state
+
+        CHROMOSOME_BREAKPOINTS = [x for x in find_runs(chroms)]
+
+        for t in range(1, number_observations):
+            #next_state = np.random.choice(n_states, p=new_transition_matrix[t][current_state])
+            next_state = Simulate_transition(n_states, new_transition_matrix[t,current_state,:], current_state)
+            sim_path[t] = next_state
+            current_state = next_state
+
+        for (chrom, chrom_start_index, chrom_length_index) in CHROMOSOME_BREAKPOINTS:
+            state_with_highest_prob = sim_path[chrom_start_index:chrom_start_index + chrom_length_index]
+
+            # Diploid or haploid
+            if '_hap' in chrom:
+                newchrom, ploidity = chrom.split('_')
+            else:
+                ploidity = 'diploid'
+                newchrom = chrom
+
+
+            for (state, start_index, length_index) in find_runs(state_with_highest_prob):
+            
+                start_index = start_index + chrom_start_index
+                end_index = start_index + length_index
+
+                genome_start = starts[start_index]
+                genome_length =  length_index * window_size
+                genome_end = genome_start + genome_length
+
+                called_sequence = int(np.sum(weights[start_index:end_index]) * window_size)
+                average_mutation_rate = round(np.mean(mutrates[start_index:end_index]), 3)
+
+                snp_counter = np.sum(obs[start_index:end_index])
+                mean_prob = 1.0
+                variants_segment = flatten_list(variants[start_index:end_index])
+
+                if called_sequence > 0:
+                    segments.append([newchrom, genome_start,  genome_end, genome_length, hmm_parameters.state_names[state], mean_prob, snp_counter, f'{ploidity}_sim_{sim_number}', called_sequence, average_mutation_rate, variants_segment]) 
+
+    return segments
+
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
 # Train
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
 def TrainModel(obs, mutrates, weights, hmm_parameters, epsilon = 1e-3, maxiterations = 1000):
 
     # Get probability of sequece with start parameters
     previous_loglikelihood = GetProbability(hmm_parameters, weights, obs, mutrates)
@@ -231,64 +321,69 @@
     
 
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
 # Decode
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def DecodeModel(obs, chroms, starts, variants, mutrates, weights, hmm_parameters):
+
     
     # Posterior decode the file
     emissions = Emission_probs_poisson(hmm_parameters.emissions, obs, weights, mutrates)
     forward_probs, scales = forward(emissions, hmm_parameters.transitions, hmm_parameters.starting_probabilities)
     backward_probs = backward(emissions, hmm_parameters.transitions, scales)
     post_seq = (forward_probs * backward_probs).T
 
     window_size = starts[2] - starts[1]
 
     segments = []
     for (chrom, chrom_start_index, chrom_length_index) in find_runs(chroms):
-        state_with_highest_prob = np.argmax(post_seq[:,chrom_start_index:chrom_start_index + chrom_length_index-1], axis = 0)
-        for (state, start_index, length_index) in find_runs(state_with_highest_prob):
 
+        # Diploid or haploid
+        if '_hap' in chrom:
+            newchrom, ploidity = chrom.split('_')
+        else:
+            ploidity = 'diploid'
+            newchrom = chrom
+
+        state_with_highest_prob = np.argmax(post_seq[:,chrom_start_index:chrom_start_index + chrom_length_index], axis = 0)
+
+        for (state, start_index, length_index) in find_runs(state_with_highest_prob):
+            
             start_index = start_index + chrom_start_index
             end_index = start_index + length_index
 
             genome_start = starts[start_index]
-            genome_end = starts[start_index + length_index - 1]
             genome_length =  length_index * window_size
+            genome_end = genome_start + genome_length
+
+            called_sequence = int(np.sum(weights[start_index:end_index]) * window_size)
+            average_mutation_rate = round(np.mean(mutrates[start_index:end_index]), 3)
 
             snp_counter = np.sum(obs[start_index:end_index])
             mean_prob = round(np.mean(post_seq[state, start_index:end_index]), 5)
             variants_segment = flatten_list(variants[start_index:end_index])
 
-            
-            # Diploid or haploid
-            if '_hap' in chrom:
-                newchrom, ploidity = chrom.split('_')
-            else:
-                ploidity = 'diploid'
-                newchrom = chrom
-
-            segments.append([newchrom, genome_start,  genome_end, genome_length, hmm_parameters.state_names[state], mean_prob, snp_counter, ploidity, variants_segment]) 
-        
+            segments.append([newchrom, genome_start,  genome_end, genome_length, hmm_parameters.state_names[state], mean_prob, snp_counter, ploidity, called_sequence, average_mutation_rate, variants_segment]) 
+    
     return segments
 
 
 
 
 
 def Write_Decoded_output(outputprefix, segments, obs_file = None, admixpop_file = None, extrainfo = False):
 
     # Load archaic data
     if admixpop_file is not None:
         admix_pop_variants, admixpop_names = Annotate_with_ref_genome(admixpop_file, obs_file)
 
     # Are we doing haploid/diploid?
     outfile_mapper = {}
-    for _, _, _, _, _, _, _, ploidity, _ in segments:
+    for _, _, _, _, _, _, _, ploidity, _, _, _ in segments:
         if outputprefix == '/dev/stdout':
             outfile_mapper[ploidity] = '/dev/stdout'
         else:
             outfile_mapper[ploidity] = f'{outputprefix}.{ploidity}.txt'
 
 
     # Make output files and write headers
@@ -297,25 +392,25 @@
        
         Make_folder_if_not_exists(output)
         outputfiles_handlers[ploidity] = open(output, 'w')
         out = outputfiles_handlers[ploidity]
 
         if admixpop_file is not None:
             if extrainfo:
-                out.write('chrom\tstart\tend\tlength\tstate\tmean_prob\tsnps\tadmixpopvariants\t{}\tvariants\n'.format('\t'.join(admixpop_names)))
+                out.write('chrom\tstart\tend\tlength\tstate\tmean_prob\tsnps\tadmixpopvariants\t{}\tcalled_sequence\tmutationrate\tvariants\n'.format('\t'.join(admixpop_names)))
             else:
                 out.write('chrom\tstart\tend\tlength\tstate\tmean_prob\tsnps\tadmixpopvariants\t{}\n'.format('\t'.join(admixpop_names)))
         else:
             if extrainfo:
-                out.write('chrom\tstart\tend\tlength\tstate\tmean_prob\tsnps\tvariants\n')
+                out.write('chrom\tstart\tend\tlength\tstate\tmean_prob\tsnps\tcalled_sequence\tmutationrate\tvariants\n')
             else:
                 out.write('chrom\tstart\tend\tlength\tstate\tmean_prob\tsnps\n')
 
     # Go through segments and write to output
-    for chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, variants in segments:
+    for chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, called_sequence, average_mutation_rate, variants  in segments:
 
         out = outputfiles_handlers[ploidity]
 
         if admixpop_file is not None:
             archiac_variants_dict = defaultdict(int)
             for snp_position in variants.split(','):
                 variant = admix_pop_variants[f'{chrom}_{snp_position}']
@@ -327,22 +422,22 @@
                         archiac_variants_dict[variant] += 1
 
                     archiac_variants_dict['total'] += 1
 
             archaic_variants = '\t'.join([str(archiac_variants_dict[x]) for x in ['total'] + admixpop_names])
 
             if extrainfo:
-                print(chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, archaic_variants, variants, sep = '\t', file = out)
+                print(chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, archaic_variants, called_sequence, average_mutation_rate, variants, sep = '\t', file = out)
             else:
                 print(chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, archaic_variants, sep = '\t', file = out)
 
         else:
 
             if extrainfo:
-                print(chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, variants, sep = '\t', file = out)
+                print(chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, called_sequence, average_mutation_rate, variants, sep = '\t', file = out)
             else:    
                 print(chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, sep = '\t', file = out)
 
 
     # Close output files
     for ploidity, out in outputfiles_handlers.items():
         out.close()
```

### Comparing `hmmix-0.6.9/src/hmmix.egg-info/PKG-INFO` & `hmmix-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-Metadata-Version: 2.1
-Name: hmmix
-Version: 0.6.9
-Summary: Find introgressed segments
-Home-page: https://github.com/LauritsSkov/Introgression-detection
-Author: Laurits Skov and Moises Coll Macia
-Author-email: lauritsskov2@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+# Contact
+https://sites.google.com/view/laurits-skov
 
+---
+
+# Helpful files
+The outgroup files, mutation rate files and callability files and ancestral allele files are now premade! 
+
+https://doi.org/10.5281/zenodo.10806733 (hg19 and hg38)
+
+VCF file containing 4 high coverage archaic genomes (Altai, Vindija and Chagyrskaya Neanderthals and Denisovan) here: 
+
+https://zenodo.org/records/7246376 (hg19)
+
+https://zenodo.org/records/10806726 (hg38)
+
+---
 
 # Introgression detection
 
+If you are working with archaic introgression into present-day humans of non-African ancestry you can use these files and skip the following steps:
+Find derived variants in outgroup and Estimate local mutation rate. 
+
 These are the scripts needed to infere archaic introgression in modern populations using an unadmixed outgroup.
 
 1. [Installation](#installation)
 2. [Usage](#usage)
 3. [Quick tutorial](#quick-tutorial)
 4. [1000 genomes tutorial](#example-with-1000-genomes-data)
       - [Get data](#getting-data)
       - [Find derived variants in outgroup](#finding-snps-which-are-derived-in-the-outgroup)
       - [Estimate local mutation rate](#estimating-mutation-rate-across-genome)
       - [Find variants in ingroup](#find-a-set-of-variants-which-are-not-derived-in-the-outgroup)
       - [Train the HMM](#training)
       - [Decoding](#decoding)
       - [Phased data](#training-and-decoding-with-phased-data)
       - [Annotate](#annotate-with-known-admixing-population)
-      - [Run in python](#annotate-with-known-admixing-population)
+5. [Run in python](#annotate-with-known-admixing-population)
 
 ---
 
 ## Installation
 
 Run the following command to install:
 
@@ -72,15 +76,16 @@
 hmmix make_test_data 
 hmmix train  -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=Initialguesses.json -out=trained.json 
 hmmix decode -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=trained.json
 
 
 Different modes (you can also see the options for each by writing hmmix make_test_data -h):
 > make_test_data        
-    -windows            Number of Kb windows to create (defaults to 50,000)
+    -windows            Number of Kb windows to create (defaults to 50,000 per chromosome)
+    -chromosomes        Number of chromosomes to simulate (defaults to 2)
     -nooutfiles         Don't create obs.txt, mutrates.bed, weights.bed, Initialguesses.json (defaults to yes)
 
 > mutation_rate         
     -outgroup           [required] path to variants found in outgroup
     -out                outputfile (defaults to mutationrate.bed)
     -weights            file with callability (defaults to all positions being called)
     -window_size        size of bins (defaults to 1 Mb)
@@ -99,30 +104,45 @@
     -outgroup           [required] path to variant found in outgroup
     -weights            file with callability (defaults to all positions being called)
     -out                outputfile prefix (default is a file named obs.<ind>.txt where ind is the name of individual in ingroup/outgrop list)
     -ancestral          fasta file with ancestral information - comma-separated list or wildcards like vcf argument (default none)
 
 > train                 
     -obs                [required] file with observation data
+    -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
     -weights            file with callability (defaults to all positions being called)
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
     -out                outputfile (default is a file named trained.json)
     -window_size        size of bins (default is 1000 bp)
     -haploid            Change from using diploid data to haploid data (default is diploid)
 
 > decode                
     -obs                [required] file with observation data
+    -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
     -weights            file with callability (defaults to all positions being called)
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
     -out                outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)
     -window_size        size of bins (default is 1000 bp)
     -haploid            Change from using diploid data to haploid data (default is diploid)
-    -admixpop ADMIXPOP  Annotate using vcffile with admixing population (default is none)
+    -admixpop           Annotate using vcffile with admixing population (default is none)
+    -extrainfo          Add variant position for each SNP (default is off)
+
+> inhomogeneous                
+    -obs                [required] file with observation data
+    -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
+    -weights            file with callability (defaults to all positions being called)
+    -mutrates           file with mutation rates (default is mutation rate is uniform)
+    -param              markov parameters file (default is human/neanderthal like parameters)
+    -out                outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)
+    -window_size        size of bins (default is 1000 bp)
+    -haploid            Change from using diploid data to haploid data (default is diploid)
+    -samples            Number of simulated paths for the inhomogeneous markov chain (default is 100)
+    -admixpop           Annotate using vcffile with admixing population (default is none)
     -extrainfo          Add variant position for each SNP (default is off)
 ```
 
 ---
 
 ## Quick tutorial
 
@@ -156,27 +176,19 @@
 weights.bed. This is the parts of the genome that we can accurately map to - in this case we have simulated the data and can accurately access the entire genome.
 
 ```note
 chr1   0   50000000
 chr2   0   50000000
 ```
 
-mutrates.bed. This is the normalized mutation rate across the genome (in bins of 1 Mb).
+mutrates.bed. This is the normalized mutation rate across the genome.
 
 ```note
-chr1  0        1000000   1
-chr1  1000000  2000000   1
-chr1  2000000  3000000   1
-chr1  3000000  4000000   1
-chr1  4000000  5000000   1
-chr1  5000000  6000000   1
-chr1  6000000  7000000   1
-chr1  7000000  8000000   1
-chr1  8000000  9000000   1
-chr1  9000000  10000000  1
+chr1   0   50000000   1
+chr2   0   50000000   1
 ```
 
 Initialguesses.json. This is our initial guesses when training the model - note these are different from those we simulated from.
 
 ```json
 {
   "state_names": ["Human","Archaic"],
@@ -191,29 +203,30 @@
 ```note
 > hmmix train  -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=Initialguesses.json -out=trained.json
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.5, 0.5]
 > transitions = [[0.99, 0.01], [0.02, 0.98]]
 > emissions = [0.03, 0.3]
+> chromosomes to use: All
 > number of windows: 99970 . Number of snps =  4230
 > total callability: 1.0
 > average mutation rate per bin: 1.0
 > Output is trained.json
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -18123.4432    0.5     0.5     0.03    0.3     0.99      0.98
-1          -17506.017     0.96    0.04    0.035   0.2202  0.9969    0.9242
-2          -17487.7921    0.971   0.029   0.0369  0.2235  0.9974    0.9141
+0          -18123.4598    0.5     0.5     0.03    0.3     0.99      0.98
+1          -17506.0258    0.96    0.04    0.035   0.2202  0.9969    0.9242
+2          -17487.8       0.971   0.029   0.0369  0.2235  0.9974    0.9141
 ...
-16         -17401.3802    0.994   0.006   0.0398  0.4584  0.9999    0.9806
-17         -17401.3786    0.994   0.006   0.0398  0.4586  0.9999    0.9807
-18         -17401.3783    0.994   0.006   0.0398  0.4587  0.9999    0.9808
+16         -17401.3853    0.994   0.006   0.0398  0.4584  0.9999    0.9806
+17         -17401.3838    0.994   0.006   0.0398  0.4586  0.9999    0.9807
+18         -17401.3835    0.994   0.006   0.0398  0.4587  0.9999    0.9808
 
 
 # run without mutrate and weights (only do this for simulated data)
 > hmmix train  -obs=obs.txt -param=Initialguesses.json -out=trained.json
 ```
 
 We can now decode the data with the best parameters that maximize the likelihood and find the archaic segments:
@@ -221,53 +234,56 @@
 ```note
 > hmmix decode -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=trained.json
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.994, 0.006]
 > transitions = [[1.0, 0.0], [0.019, 0.981]]
 > emissions = [0.04, 0.459]
+> chromosomes to use: All
 > number of windows: 99970 . Number of snps =  4230
 > total callability: 1.0
 > average mutation rate per bin: 1.0
-> Output is /dev/stdout
+> Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 chrom  start     end       length    state    mean_prob  snps
-chr1   0         7233000   7234000   Human    0.9995     287
-chr1   7234000   7246000   13000     Archaic  0.90427    9
-chr1   7247000   21618000  14372000  Human    0.99946    610
-chr1   21619000  21673000  55000     Archaic  0.9697     22
-chr1   21674000  26859000  5186000   Human    0.99878    204
-chr1   26860000  26941000  82000     Archaic  0.971      36
-chr1   26942000  49989000  23048000  Human    0.99982    863
-chr2   0         6793000   6794000   Human    0.99972    237
-chr2   6794000   6822000   29000     Archaic  0.95461    14
-chr2   6823000   12646000  5824000   Human    0.99927    244
-chr2   12647000  12745000  99000     Archaic  0.97413    55
-chr2   12746000  15461000  2716000   Human    0.99881    125
-chr2   15462000  15547000  86000     Archaic  0.93728    38
-chr2   15548000  32626000  17079000  Human    0.99951    709
-chr2   32627000  32695000  69000     Archaic  0.98305    31
-chr2   32696000  41087000  8392000   Human    0.9995     360
-chr2   41088000  41178000  91000     Archaic  0.96092    43
-chr2   41179000  49952000  8774000   Human    0.99789    328
-chr2   49953000  49977000  25000     Archaic  0.98501    13
+chr1   0         7234000   7234000   Human    0.9995     287
+chr1   7234000   7247000   13000     Archaic  0.90427    9
+chr1   7247000   21619000  14372000  Human    0.99946    610
+chr1   21619000  21674000  55000     Archaic  0.9697     22
+chr1   21674000  26860000  5186000   Human    0.99878    204
+chr1   26860000  26942000  82000     Archaic  0.971      36
+chr1   26942000  49991000  23049000  Human    0.99982    864
+chr2   0         6794000   6794000   Human    0.99972    237
+chr2   6794000   6823000   29000     Archaic  0.95461    14
+chr2   6823000   12647000  5824000   Human    0.99927    244
+chr2   12647000  12746000  99000     Archaic  0.97413    55
+chr2   12746000  15462000  2716000   Human    0.99881    125
+chr2   15462000  15548000  86000     Archaic  0.93728    38
+chr2   15548000  32627000  17079000  Human    0.99951    709
+chr2   32627000  32696000  69000     Archaic  0.98305    31
+chr2   32696000  41088000  8392000   Human    0.9995     360
+chr2   41088000  41179000  91000     Archaic  0.96092    43
+chr2   41179000  49953000  8774000   Human    0.99789    328
+chr2   49953000  49979000  26000     Archaic  0.98515    14
 
 # Again here you could ommit weights and mutationrates. Actually one could also ommit trained.json because then the model defaults to using the parameters we used the generated the data
-> hmmix decode -obs=obs.txt
+> hmmix decode -obs=obs.txt -param=trained.json
 ```
 
 ---
 
 ## Example with 1000 genomes data
 
 ---
 
 The whole pipeline we will run looks like this. In the following section we will go through all the steps on the way
+NOTE: The outgroup files, mutation rate files and callability files are now premade! They can be downloaded in hg38 and hg19 here: https://doi.org/10.5281/zenodo.10806733
+But keep reading along if you want to know HOW the files were generated!
 
 ```note
 hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa -refgenome=referencegenome/*fa
 hmmix mutation_rate -outgroup=outgroup.txt  -weights=strickmask.bed -window_size=1000000 -out mutationrate.bed
 hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
 hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json 
@@ -301,15 +317,16 @@
 # Ancestral information
 ftp://ftp.ensembl.org/pub/release-74/fasta/ancestral_alleles/homo_sapiens_ancestor_GRCh37_e71.tar.bz2
 
 # Reference genome
 wget 'ftp://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/chromFa.tar.gz' -O chromFa.tar.gz
 
 # Archaic variants (Altai, Vindija, Chagyrskaya and Denisova in hg19)
-https://zenodo.org/record/7246376#.Y1cRBkrMJH4
+https://zenodo.org/records/7246376
+
 ```
 
 For this example we will use all individuals from 'YRI','MSL' and 'ESN' as outgroup individuals. While we will only be decoding hG00096 in this example you can add as many individuals as you want to the ingroup.  
 
 ```json
 {
   "ingroup": [
@@ -328,32 +345,32 @@
 ---
 
 ### Finding snps which are derived in the outgroup
 
 First we need to find a set of variants found in the outgroup. We can use the wildcard character to loop through all bcf files. If you dont have ancestral information you can skip the ancestral argument.
 
 ```bash
-(took an hour) > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+(took an hour) > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa 
 
 # Alternative usage (if you only have a few individual in the outgroup you can also provide a comma separated list)
-> hmmix create_outgroup -ind=HG02922,HG02923,HG02938 -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+> hmmix create_outgroup -ind=HG02922,HG02923,HG02938 -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa 
 
 # Alternative usage (if you have no ancestral information)
 > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt 
 
 # Alternative usage (if you only want to run the model on a subset of chromosomes, with or without ancestral information)
 > hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf -weights=strickmask.bed -out=outgroup.txt
 
 > hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_1.fa,homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_2.fa
 ```
 
 Something to note is that if you use an outgroup vcffile (like 1000 genomes) and an ingroup vcf file from a different dataset (like SGDP) there is an edge case which could occur. There could be recurrent mutations where every individual in 1000 genome has the derived variant and one individual in SGDP where the derived variant has mutated back to the ancestral allele. This means that this position will not be present in the outgroup file. However if a recurrent mutation occurs it will look like multiple individuals in the ingroup file have the mutation. This does not happen often but just in case you can create the outgroup file and adding the sites which are fixed derived in all individuals using the reference genome:
 
 ```bash
-# Alternative usage (if you want to remove sites which are fixed derived in your outgroup/ingroup)
+# Recommended usage (if you want to remove sites which are fixed derived in your outgroup/ingroup)
 > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa -refgenome=*fa
 ```
 
 ---
 
 ### Estimating mutation rate across genome
 
@@ -427,148 +444,160 @@
 ```note
 (took 2 min) > hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.98, 0.02]
 > transitions = [[1.0, 0.0], [0.02, 0.98]]
 > emissions = [0.04, 0.4]
+> chromosomes to use: All
 > number of windows: 2877010 . Number of snps =  129734
 > total callability: 0.72
 > average mutation rate per bin: 1.0
-> Output is trained.HG00096_new.json
+> Output is trained.HG00096.json
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -492288.9165   0.98    0.02    0.04    0.4     0.9999    0.98
-1          -488899.7271   0.961   0.039   0.0483  0.3913  0.9994    0.986
-2          -488755.4068   0.958   0.042   0.0481  0.3911  0.9993    0.9835
+0          -492287.8643   0.98    0.02    0.04    0.4     0.9999    0.98
+1          -488898.6051   0.961   0.039   0.0483  0.3913  0.9994    0.986
+2          -488754.2455   0.958   0.042   0.0481  0.3911  0.9993    0.9835
 ...
-19         -488642.2737   0.954   0.046   0.047   0.3862  0.9989    0.9771
-20         -488642.2723   0.954   0.046   0.047   0.3862  0.9989    0.9771
-21         -488642.2716   0.954   0.046   0.047   0.3862  0.9989    0.9771
+19         -488641.0769   0.954   0.046   0.047   0.3862  0.9989    0.9771
+20         -488641.0755   0.954   0.046   0.047   0.3862  0.9989    0.9771
+21         -488641.0748   0.954   0.046   0.047   0.3862  0.9989    0.9771
 ```
 
 ---
 
 ### Decoding
 
 ```note
 (took 30 sec) > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json 
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.954, 0.046]
 > transitions = [[0.999, 0.001], [0.023, 0.977]]
 > emissions = [0.047, 0.386]
+> chromosomes to use: All
 > number of windows: 2877010 . Number of snps =  129734
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 chrom  start    end      length   state    mean_prob  snps
-1      0        2987000  2988000  Human    0.98484    91
-1      2988000  2996000  9000     Archaic  0.71815    6
-1      2997000  3424000  428000   Human    0.98944    30
-1      3425000  3451000  27000    Archaic  0.95652    22
-1      3452000  4301000  850000   Human    0.98203    36
-1      4302000  4360000  59000    Archaic  0.84636    20
-1      4361000  4499000  139000   Human    0.97136    4
-1      4500000  4509000  10000    Archaic  0.84456    7
+1      0        2988000  2988000  Human    0.98484    91
+1      2988000  2997000  9000     Archaic  0.71819    6
+1      2997000  3425000  428000   Human    0.98944    30
+1      3425000  3452000  27000    Archaic  0.95652    22
+1      3452000  4302000  850000   Human    0.98203    36
+1      4302000  4361000  59000    Archaic  0.84636    20
+1      4361000  4500000  139000   Human    0.97136    4
+1      4500000  4510000  10000    Archaic  0.84457    7
 ```
 
 You can also save to an output file with the command:
 
 ```note
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json -out=HG00096.decoded
 ```
 
 This will create a file named HG00096.decoded.diploid.txt because the default option is treating the data as diploid (more on haploid decoding in next chapter)
 
 ---
 
 ### Training and decoding with phased data
 
-It is also possible to tell the model that the data is phased with the -haploid parameter. For that we first need to train the parameters for haploid data and then decode. Training the model on phased data is done like this - and we also remember to change the name of the parameter file to include phased so future versions of ourselves don't forget. Another thing to note is that the number of snps is bigger than before 134799 vs 129149. This is because the program is counting snps on both haplotypes and homozygotes will be counted twice!
+It is also possible to tell the model that the data is phased with the -haploid parameter. For that we first need to train the parameters for haploid data and then decode. Training the model on phased data is done like this - and we also remember to change the name of the parameter file to include phased so future versions of ourselves don't forget. Another thing to note is that the number of snps is bigger than before 135411 vs 129734. This is because the program is counting snps on both haplotypes and homozygotes will be counted twice!
 
 ```note
 (took 4 min) > hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.phased.json -haploid
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.98, 0.02]
 > transitions = [[1.0, 0.0], [0.02, 0.98]]
 > emissions = [0.04, 0.4]
+> chromosomes to use: All
 > number of windows: 5754020 . Number of snps =  135411
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output is trained.HG00096.phased.json
 > Window size is 1000 bp
 > Haploid True
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -597753.9141   0.98    0.02    0.04    0.4     0.9999    0.98
-1          -585032.3914   0.983   0.017   0.0261  0.4026  0.9998    0.9853
-2          -584451.0968   0.979   0.021   0.0252  0.373   0.9996    0.9826
+0          -597750.7043   0.98    0.02    0.04    0.4     0.9999    0.98
+1          -585028.8828   0.983   0.017   0.0261  0.4026  0.9998    0.9853
+2          -584447.5809   0.979   0.021   0.0252  0.373   0.9996    0.9826
 ...
-19         -584134.532    0.972   0.028   0.0241  0.3367  0.9993    0.9758
-20         -584134.5305   0.972   0.028   0.0241  0.3366  0.9993    0.9758
-21         -584134.5297   0.972   0.028   0.0241  0.3366  0.9993    0.975
+19         -584131.0153   0.972   0.028   0.0241  0.3367  0.9993    0.9758
+20         -584131.0138   0.972   0.028   0.0241  0.3367  0.9993    0.9758
+21         -584131.013    0.972   0.028   0.0241  0.3366  0.9993    0.9758
 ```
 
 Below I am only showing the first archaic segments on chromosome 1 for each haplotype (note you have to scroll down after chrom 22 before the new haplotype begins). The seem to fall more or less in the same places as when we used diploid data.
 
 ```note
 (took 30 sec) > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.phased.json -haploid
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.972, 0.028]
 > transitions = [[0.999, 0.001], [0.024, 0.976]]
 > emissions = [0.024, 0.337]
+> chromosomes to use: All
 > number of windows: 5754020 . Number of snps =  135411
 > total callability: 0.72
 > average mutation rate per bin: 1.0
-> Output prefix is HG00096.decoded
+> Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid True
 ----------------------------------------
 hap1
 chrom  start    end      length  state    mean_prob  snps
-1      2162000  2184000  23000   Archaic  0.61055    6
-1      3425000  3451000  27000   Archaic  0.96595    22
+1      2162000  2185000  23000   Archaic  0.61054    6
+1      3425000  3452000  27000   Archaic  0.96595    22
 
 ...
 hap2
-1      2780000  2802000  23000   Archaic  0.61948    7
-1      4302000  4336000  35000   Archaic  0.94008    13
-1      4500000  4510000  11000   Archaic  0.87592    7
-1      4989000  4999000  11000   Archaic  0.57897    4
+1      2780000  2803000  23000   Archaic  0.61948    7
+1      4302000  4337000  35000   Archaic  0.94008    13
+1      4500000  4511000  11000   Archaic  0.87592    7
+1      4989000  5000000  11000   Archaic  0.579      4
 ```
 
 You can also save to an output file with the command:
 
 ```note
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.phased.json -haploid -out=HG00096.decoded
 ```
 
 This will create two files named HG00096.decoded.hap1.txt and HG00096.decoded.hap2.txt
 
 ---
 
 ### Annotate with known admixing population
 
-Even though this method does not use archaic reference genomes for finding segments you can still use them to annotate your segments. If you have a vcf from the population that admixed in VCF/BCF format you can write this:
+Even though this method does not use archaic reference genomes for finding segments you can still use them to annotate your segments. 
+I have uploaded a VCF file containing 4 high coverage archaic genomes (3 Neanderthals and 1 Denisovan) here:
+
+https://zenodo.org/records/7246376 (hg19 - the one I use in this example)
+
+https://zenodo.org/records/10806726 (hg38)
+
+If you have a vcf from the population that admixed in VCF/BCF format you can write this:
 
 ```note
 > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json -admixpop=archaicvar/*bcf
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.954, 0.046]
 > transitions = [[0.999, 0.001], [0.023, 0.977]]
 > emissions = [0.047, 0.386]
+> chromosomes to use: All
 > number of windows: 2877010 . Number of snps =  129734
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
@@ -593,21 +622,21 @@
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_5.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_8.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_11.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_12.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_13.bcf
 
 chrom  start     end       length  state    mean_prob  snps  admixpopvariants  AltaiNeandertal  Vindija33.19  Denisova  Chagyrskaya-Phalanx
-1      2988000   2996000   9000    Archaic  0.71815    6     4                 4                4             1         4
-1      3425000   3451000   27000   Archaic  0.95652    22    17                17               15            3         17
-1      4302000   4360000   59000   Archaic  0.84636    20    12                11               12            11        11
-1      4500000   4509000   10000   Archaic  0.84456    7     5                 4                5             4         5
-1      5339000   5346000   8000    Archaic  0.58909    4     3                 2                3             0         3
-1      9322000   9354000   33000   Archaic  0.8475     9     0                 0                0             0         0
-1      12599000  12653000  55000   Archaic  0.9142     18    11                4                11            0         10
+1      2988000   2997000   9000    Archaic  0.71819    6     4                 4                4             1         4
+1      3425000   3452000   27000   Archaic  0.95652    22    17                17               15            3         17
+1      4302000   4361000   59000   Archaic  0.84636    20    12                11               12            11        11
+1      4500000   4510000   10000   Archaic  0.84457    7     5                 4                5             4         5
+1      5339000   5347000   8000    Archaic  0.58914    4     3                 2                3             0         3
+1      9322000   9355000   33000   Archaic  0.84751    9     0                 0                0             0         0
+1      12599000  12654000  55000   Archaic  0.9142     18    11                4                11            0         10
 
 ```
 
 For the first segment there are 6 derived snps. Of these snps 4 are shared with Altai,Vindija, Denisova and Chagyrskaya. Only 1 is shared with Denisova so this segment likeli introgressed from Neanderthals
 
 ---
 
@@ -627,24 +656,24 @@
 # Initial HMM guess
 initial_hmm_params = HMMParam(state_names = ['Human', 'Archaic'], 
                               starting_probabilities = [0.5, 0.5], 
                               transitions = [[0.99,0.01],[0.02,0.98]], 
                               emissions = [0.03, 0.3]) 
 
 # Create test data
-obs, chroms, starts, variants, weights, mutrates  = create_test_data(50000, write_out_files = False)
+obs, chroms, starts, variants, mutrates, weights  = create_test_data(50000, write_out_files = False)
 
 # Train model
 hmm_parameters = TrainModel(obs, mutrates, weights, initial_hmm_params)
 
 # Decode model
 segments = DecodeModel(obs, chroms, starts, variants, mutrates, weights, hmm_parameters)
 
 for segment_info in segments:
-    chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, variants = segment_info
+    chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, called_sequence, average_mutation_rate, variants = segment_info
     print(chrom, genome_start,  genome_end, genome_length, state, mean_prob, snp_counter, sep = '\t')
 
 
 
 # -----------------------------------------------------------------------------
 # Running on an individual from 1000 genomes
 # -----------------------------------------------------------------------------
@@ -655,23 +684,17 @@
                                                                                       mutrates_file = 'mutationrate.bed', 
                                                                                       window_size = 1000, 
                                                                                       haploid = False)
 
 segments = DecodeModel(obs, chroms, starts, variants, mutrates, weights, hmm_parameters)
 
 for segment_info in segments:  
-    chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, variants = segment_info
+    chrom, genome_start, genome_end, genome_length, state, mean_prob, snp_counter, ploidity, called_sequence, average_mutation_rate, variants = segment_info
     print(chrom, genome_start,  genome_end, genome_length, state, mean_prob, snp_counter, sep = '\t')
 
 
 ```
 
 And that is it! Now you have run the model and gotten a set of parameters that you can interpret biologically (see my paper) and you have a list of segments that belong to the human and Archaic state.
 
 If you have any questions about the use of the scripts, if you find errors or if you have feedback you can contact my here (make an issue) or write to:
-
----
-Contact:
-
 lauritsskov2@gmail.com
-
-
```

### Comparing `hmmix-0.6.9/src/main.py` & `hmmix-0.7.0/src/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import argparse
 import numpy as np
 
-from hmm_functions import TrainModel, DecodeModel, write_HMM_to_file, read_HMM_parameters_from_file, Write_Decoded_output
+from hmm_functions import TrainModel, DecodeModel, write_HMM_to_file, read_HMM_parameters_from_file, Write_Decoded_output, inhomogeneous
 from bcf_vcf import make_out_group, make_ingroup_obs
 from make_test_data import create_test_data
 from make_mutationrate import make_mutation_rate
 from helper_functions import Load_observations_weights_mutrates, handle_individuals_input, handle_infiles, combined_files
 
 
-VERSION = '0.6.8'
+VERSION = '0.7.0'
 
 
 def print_script_usage():
     toprint = f'''
 Script for identifying introgressed archaic segments (version: {VERSION})
 
 > Turorial:
 hmmix make_test_data 
 hmmix train  -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=Initialguesses.json -out=trained.json 
 hmmix decode -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=trained.json
 
 
 Different modes (you can also see the options for each by writing hmmix make_test_data -h):
 > make_test_data        
-    -windows            Number of Kb windows to create (defaults to 50,000)
+    -windows            Number of Kb windows to create (defaults to 50,000 per chromosome)
+    -chromosomes        Number of chromosomes to simulate (defaults to 2)
     -nooutfiles         Don't create obs.txt, mutrates.bed, weights.bed, Initialguesses.json (defaults to yes)
 
 > mutation_rate         
     -outgroup           [required] path to variants found in outgroup
     -out                outputfile (defaults to mutationrate.bed)
     -weights            file with callability (defaults to all positions being called)
     -window_size        size of bins (defaults to 1 Mb)
@@ -46,30 +47,45 @@
     -outgroup           [required] path to variant found in outgroup
     -weights            file with callability (defaults to all positions being called)
     -out                outputfile prefix (default is a file named obs.<ind>.txt where ind is the name of individual in ingroup/outgrop list)
     -ancestral          fasta file with ancestral information - comma-separated list or wildcards like vcf argument (default none)
 
 > train                 
     -obs                [required] file with observation data
+    -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
     -weights            file with callability (defaults to all positions being called)
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
     -out                outputfile (default is a file named trained.json)
     -window_size        size of bins (default is 1000 bp)
     -haploid            Change from using diploid data to haploid data (default is diploid)
 
 > decode                
     -obs                [required] file with observation data
+    -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
     -weights            file with callability (defaults to all positions being called)
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
     -out                outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)
     -window_size        size of bins (default is 1000 bp)
     -haploid            Change from using diploid data to haploid data (default is diploid)
-    -admixpop ADMIXPOP  Annotate using vcffile with admixing population (default is none)
+    -admixpop           Annotate using vcffile with admixing population (default is none)
+    -extrainfo          Add variant position for each SNP (default is off)
+
+> inhomogeneous                
+    -obs                [required] file with observation data
+    -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
+    -weights            file with callability (defaults to all positions being called)
+    -mutrates           file with mutation rates (default is mutation rate is uniform)
+    -param              markov parameters file (default is human/neanderthal like parameters)
+    -out                outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)
+    -window_size        size of bins (default is 1000 bp)
+    -haploid            Change from using diploid data to haploid data (default is diploid)
+    -samples            Number of simulated paths for the inhomogeneous markov chain (default is 100)
+    -admixpop           Annotate using vcffile with admixing population (default is none)
     -extrainfo          Add variant position for each SNP (default is off)
     '''
 
     return toprint
 
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
 # Main
@@ -78,15 +94,16 @@
 
     parser = argparse.ArgumentParser(description=print_script_usage(), formatter_class=argparse.RawTextHelpFormatter)
 
     subparser = parser.add_subparsers(dest = 'mode')
 
     # Run test
     test_subparser = subparser.add_parser('make_test_data', help='Create test data')
-    test_subparser.add_argument("-windows", metavar='',help="Number of Kb windows to create (defaults to 50,000)", type=int, default = 50000)
+    test_subparser.add_argument("-windows", metavar='',help="Number of Kb windows to create (defaults to 50,000 per chromosome)", type=int, default = 50000)
+    test_subparser.add_argument("-chromosomes", metavar='',help="Number of chromosomes to simulate (defaults to 2)", type=int, default = 2)
     test_subparser.add_argument("-nooutfiles",help="Don't create obs.txt, mutrates.bed, weights.bed, Initialguesses.json (defaults to yes)", action='store_false', default = True)
 
     # Make outgroup
     outgroup_subparser = subparser.add_parser('create_outgroup', help='Create outgroup information')
     outgroup_subparser.add_argument("-ind",help="[required] ingroup/outgrop list (json file) or comma-separated list e.g. ind1,ind2", type=str, required = True)
     outgroup_subparser.add_argument("-vcf",help="[required] path to list of comma-separated vcf/bcf file(s) or wildcard characters e.g. chr*.bcf", type=str, required = True)
     outgroup_subparser.add_argument("-weights", metavar='',help="file with callability (defaults to all positions being called)")
@@ -109,53 +126,74 @@
     create_obs_subparser.add_argument("-weights", metavar='',help="file with callability (defaults to all positions being called)")
     create_obs_subparser.add_argument("-out", metavar='',help="outputfile prefix (default is a file named obs.<ind>.txt where ind is the name of individual in ingroup/outgrop list)", default = 'obs')
     create_obs_subparser.add_argument("-ancestral", metavar='',help="fasta file with ancestral information - comma-separated list or wildcards like vcf argument (default none)", default='')
 
     # Train model
     train_subparser = subparser.add_parser('train', help='Train HMM')
     train_subparser.add_argument("-obs",help="[required] file with observation data", type=str, required = True)
+    train_subparser.add_argument("-chrom",help="Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3", type=str, default='All')
     train_subparser.add_argument("-weights", metavar='',help="file with callability (defaults to all positions being called)")
     train_subparser.add_argument("-mutrates", metavar='',help="file with mutation rates (default is mutation rate is uniform)")
     train_subparser.add_argument("-param", metavar='',help="markov parameters file (default is human/neanderthal like parameters)", type=str)
     train_subparser.add_argument("-out", metavar='',help="outputfile (default is a file named trained.json)", default = 'trained.json')
     train_subparser.add_argument("-window_size", metavar='',help="size of bins (default is 1000 bp)", type=int, default = 1000)
     train_subparser.add_argument("-haploid",help="Change from using diploid data to haploid data (default is diploid)", action='store_true', default = False)
 
     # Decode model
     decode_subparser = subparser.add_parser('decode', help='Decode HMM')
     decode_subparser.add_argument("-obs",help="[required] file with observation data", type=str, required = True)
+    decode_subparser.add_argument("-chrom",help="Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3", type=str, default='All')
     decode_subparser.add_argument("-weights", metavar='',help="file with callability (defaults to all positions being called)")
     decode_subparser.add_argument("-mutrates", metavar='',help="file with mutation rates (default is mutation rate is uniform)")
     decode_subparser.add_argument("-param", metavar='',help="markov parameters file (default is human/neanderthal like parameters)", type=str)
     decode_subparser.add_argument("-out", metavar='',help="outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)", default = '/dev/stdout')
     decode_subparser.add_argument("-window_size", metavar='',help="size of bins (default is 1000 bp)", type=int, default = 1000)
     decode_subparser.add_argument("-haploid",help="Change from using diploid data to haploid data (default is diploid)", action='store_true', default = False)
     decode_subparser.add_argument("-admixpop",help="Annotate using vcffile with admixing population (default is none)")
     decode_subparser.add_argument("-extrainfo",help="Add archaic information on each SNP", action='store_true', default = False)
 
+    # inhomogeneous markov chain
+    inhomogen_subparser = subparser.add_parser('inhomogeneous', help='Make inhomogen markov chain')
+    inhomogen_subparser.add_argument("-obs",help="[required] file with observation data", type=str, required = True)
+    inhomogen_subparser.add_argument("-chrom",help="Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3", type=str, default='All')
+    inhomogen_subparser.add_argument("-weights", metavar='',help="file with callability (defaults to all positions being called)")
+    inhomogen_subparser.add_argument("-mutrates", metavar='',help="file with mutation rates (default is mutation rate is uniform)")
+    inhomogen_subparser.add_argument("-param", metavar='',help="markov parameters file (default is human/neanderthal like parameters)", type=str)
+    inhomogen_subparser.add_argument("-out", metavar='',help="outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)", default = '/dev/stdout')
+    inhomogen_subparser.add_argument("-window_size", metavar='',help="size of bins (default is 1000 bp)", type=int, default = 1000)
+    inhomogen_subparser.add_argument("-haploid",help="Change from using diploid data to haploid data (default is diploid)", action='store_true', default = False)
+    inhomogen_subparser.add_argument("-samples",help="Number of paths to sample (default is 100)", type=int, default = 100)
+    inhomogen_subparser.add_argument("-admixpop",help="Annotate using vcffile with admixing population (default is none)")
+    inhomogen_subparser.add_argument("-extrainfo",help="Add archaic information on each SNP", action='store_true', default = False)
+
+
+
+
+
 
     args = parser.parse_args()
 
     # Make test data
     # ------------------------------------------------------------------------------------------------------------
     if args.mode == 'make_test_data':
-        create_test_data(data_set_length = args.windows, write_out_files = args.nooutfiles)
+        create_test_data(data_set_length = args.windows, n_chromosomes = args.chromosomes, write_out_files = args.nooutfiles)
 
 
 
 
     # Train parameters
     # ------------------------------------------------------------------------------------------------------------
     elif args.mode == 'train':
 
         hmm_parameters = read_HMM_parameters_from_file(args.param)
-        obs, _, _, _, mutrates, weights = Load_observations_weights_mutrates(args.obs, args.weights, args.mutrates, args.window_size, args.haploid)
+        obs, _, _, _, mutrates, weights = Load_observations_weights_mutrates(args.obs, args.weights, args.mutrates, args.window_size, args.haploid, args.chrom)
         
         print('-' * 40)
         print(hmm_parameters)
+        print(f'> chromosomes to use: {args.chrom}')
         print('> number of windows:', len(obs), '. Number of snps = ', sum(obs))
         print('> total callability:', round(np.sum(weights) / len(obs),2) )
         print('> average mutation rate per bin:', round(np.sum(mutrates * weights) / np.sum(weights), 2) )
         print('> Output is',args.out) 
         print('> Window size is',args.window_size, 'bp') 
         print('> Haploid',args.haploid) 
         print('-' * 40)
@@ -166,32 +204,55 @@
 
 
 
     # Decode observations using parameters
     # ------------------------------------------------------------------------------------------------------------
     elif args.mode == 'decode':
 
-        obs, chroms, starts, variants, mutrates, weights  = Load_observations_weights_mutrates(args.obs, args.weights, args.mutrates, args.window_size, args.haploid)
+        obs, chroms, starts, variants, mutrates, weights  = Load_observations_weights_mutrates(args.obs, args.weights, args.mutrates, args.window_size, args.haploid, args.chrom)
         hmm_parameters = read_HMM_parameters_from_file(args.param)
         
         print('-' * 40)
         print(hmm_parameters)  
+        print(f'> chromosomes to use: {args.chrom}')
         print('> number of windows:', len(obs), '. Number of snps = ', sum(obs))
         print('> total callability:', round(np.sum(weights) / len(obs),2) )
         print('> average mutation rate per bin:', round(np.sum(mutrates * weights) / np.sum(weights), 2) )
         print('> Output prefix is',args.out) 
         print('> Window size is',args.window_size, 'bp') 
         print('> Haploid',args.haploid) 
         print('-' * 40)
 
         # Find segments and write output
         segments = DecodeModel(obs, chroms, starts, variants, mutrates, weights, hmm_parameters)
         Write_Decoded_output(args.out, segments, args.obs, args.admixpop, args.extrainfo)
 
+    # inhomogeneous markov chain
+    # ------------------------------------------------------------------------------------------------------------
+    elif args.mode == 'inhomogeneous':
+
+        obs, chroms, starts, variants, mutrates, weights  = Load_observations_weights_mutrates(args.obs, args.weights, args.mutrates, args.window_size, args.haploid, args.chrom)
+        hmm_parameters = read_HMM_parameters_from_file(args.param)
+        
+        print('-' * 40)
+        print(hmm_parameters)  
+        print(f'> chromosomes to use: {args.chrom}')
+        print('> number of windows:', len(obs), '. Number of snps = ', sum(obs))
+        print('> total callability:', round(np.sum(weights) / len(obs),2) )
+        print('> average mutation rate per bin:', round(np.sum(mutrates * weights) / np.sum(weights), 2) )
+        print('> Output prefix is',args.out) 
+        print('> Window size is',args.window_size, 'bp') 
+        print('> Haploid',args.haploid) 
+        print('-' * 40)
+
+        # Find segments and write output
+        segments = inhomogeneous(hmm_parameters, weights, obs, mutrates, args.samples, chroms, starts, variants)
+        Write_Decoded_output(args.out, segments, args.obs, args.admixpop, args.extrainfo)
 
+            
 
 
 
     # Create outgroup snps (set of snps to be removed)
     # ------------------------------------------------------------------------------------------------------------
     elif args.mode == 'create_outgroup':
```

### Comparing `hmmix-0.6.9/src/make_mutationrate.py` & `hmmix-0.7.0/src/make_mutationrate.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.9/src/make_test_data.py` & `hmmix-0.7.0/src/make_test_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,78 @@
-from wsgiref.simple_server import demo_app
 import numpy as np
 from collections import defaultdict
 
 from hmm_functions import HMMParam, get_default_HMM_parameters, write_HMM_to_file
 
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
 # Make test data
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
-def create_test_data(data_set_length, write_out_files = False):
+def create_test_data(data_set_length, n_chromosomes = 2, write_out_files = False):
     '''Create test data set of size data_set_length. Also create uniform weights and uniform mutation rates'''
     
     # Config
     np.random.seed(42)
     window_size = 1000
-    mutation_rate_window = 1000000
     mutation_matrix = {
         'A': [0, 0.16, 0.68, 0.16],
         'C': [0.16, 0,0.16, 0.68],
         'G': [0.68, 0.16, 0, 0.16],
         'T': [0.16, 0.68, 0.16, 0],
     }
     bases = ['A','C','G','T']
     base_composition = [0.31, 0.19, 0.19, 0.31]
+    CHROMOSOMES = [f'chr{x + 1}' for x in range(n_chromosomes)] 
 
 
     # Initialization HMM parameters, prob of staring in states and print parameters to user
     state_values = [0,1]
-    hmm_parameters = get_default_HMM_parameters()
-
-    print(f'creating 2 chromosomes each with {data_set_length} kb of test data with the following parameters..\n')
+    hmm_parameters = HMMParam(state_names = ['Human', 'Archaic'], 
+                    starting_probabilities = [0.98, 0.02], 
+                    transitions = [[0.9999,0.0001],[0.02,0.98]], 
+                    emissions = [0.04, 0.4])
+    
+    print(f'creating {len(CHROMOSOMES)} chromosomes each with {data_set_length} kb of test data with the following parameters..\n')
     print(hmm_parameters)  
 
     # Initialize data
     observations_for_obsfile = []
     obs_counter = defaultdict(lambda: defaultdict(int))
     variants_dict = defaultdict(lambda: defaultdict(list))   
 
-    initial_guess = HMMParam(['Human', 'Archaic'], [0.5, 0.5], [[0.99,0.01],[0.02,0.98]], [0.03, 0.3]) 
+    
 
-    for chrom in ['chr1', 'chr2']:
+    for chrom in CHROMOSOMES:
         for index in range(data_set_length):
             
             # Use prior dist if starting window
             if index == 0:
                 current_state = np.random.choice(state_values, p=hmm_parameters.starting_probabilities)
             else:
                 current_state = np.random.choice(state_values, p=hmm_parameters.transitions[prevstate] )
 
+            # if 300 < index < 400:
+            #     current_state = 1
+            # else:
+            #     current_state = 0
+
             n_mutations = np.random.poisson(lam=hmm_parameters.emissions[current_state]) 
             for mutation in [int(x) for x in np.random.uniform(low=index*window_size, high=index*window_size + window_size, size=n_mutations)]: 
                 ancestral_base = np.random.choice(bases, p=base_composition)
                 derived_base = np.random.choice(bases, p=mutation_matrix[ancestral_base])
                 observations_for_obsfile.append(f'{chrom}\t{mutation}\t{ancestral_base}\t{ancestral_base + derived_base}') 
                 obs_counter[chrom][index*window_size] += 1
                 variants_dict[chrom][index*window_size].append(str(mutation))
 
             prevstate = current_state
 
     observations = []
     chroms = []
     starts = []
     variants = []
-    for chrom in ['chr1', 'chr2']:
+    for chrom in CHROMOSOMES:
         lastwindow = max(obs_counter[chrom]) + window_size
 
         for window in range(0, lastwindow, window_size):
             observations.append(obs_counter[chrom][window])
             chroms.append(chrom)
             starts.append(window)
             variants.append(','.join(variants_dict[chrom][window]))
@@ -77,22 +84,19 @@
     if write_out_files:
         # Make obs file
         with open('obs.txt','w') as obs_file:
             print('chrom', 'pos', 'ancestral_base', 'genotype', sep = '\t', file = obs_file)
             for line in observations_for_obsfile:
                 print(line, file = obs_file)
 
-        # Make mutation file
-        with open('mutrates.bed','w') as mutrates_file:
-            for chrom in ['chr1', 'chr2']:
-                for start in range(int(data_set_length * window_size / mutation_rate_window)):
-                    print(chrom, start * mutation_rate_window, (start + 1) * mutation_rate_window, 1, sep = '\t', file = mutrates_file)
-
-        # Make weights file
-        with open('weights.bed','w') as weights_file:
-            for chrom in ['chr1', 'chr2']:
+        # Make weights file and mutation file
+        with open('weights.bed','w') as weights_file, open('mutrates.bed','w') as mutrates_file:
+            for chrom in CHROMOSOMES:
                 print(chrom, 0, data_set_length * window_size, sep = '\t', file = weights_file)
+                print(chrom, 0, data_set_length * window_size, 1, sep = '\t', file = mutrates_file)
 
         # Make initial guesses
+        initial_guess = HMMParam(['Human', 'Archaic'], [0.5, 0.5], [[0.99,0.01],[0.02,0.98]], [0.03, 0.3]) 
         write_HMM_to_file(initial_guess, 'Initialguesses.json')
 
-    return observations, chroms, starts, variants, weights, mutrates
+    #return observations, chroms, starts, variants, mutrates, weights
+    return np.array(observations).astype(int), chroms, starts, variants, np.array(mutrates).astype(float), np.array(weights).astype(float)
```

### Comparing `hmmix-0.6.9/test/test2.py` & `hmmix-0.7.0/test/test2.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.6.9/test/test_main.py` & `hmmix-0.7.0/test/test_main.py`

 * *Files identical despite different names*

