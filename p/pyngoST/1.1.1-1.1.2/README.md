# Comparing `tmp/pyngoST-1.1.1.tar.gz` & `tmp/pyngoST-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyngoST-1.1.1.tar", last modified: Tue Jan 16 08:33:13 2024, max compression
+gzip compressed data, was "dist/pyngoST-1.1.2.tar", last modified: Mon May 13 13:31:48 2024, max compression
```

## Comparing `pyngoST-1.1.1.tar` & `pyngoST-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 leosanbu   (501) staff       (20)        0 2024-01-16 08:33:13.363808 pyngoST-1.1.1/
--rw-r--r--   0 leosanbu   (501) staff       (20)      345 2024-01-16 08:33:13.363559 pyngoST-1.1.1/PKG-INFO
--rw-r--r--   0 leosanbu   (501) staff       (20)    16881 2023-10-18 14:21:01.000000 pyngoST-1.1.1/README.md
-drwxr-xr-x   0 leosanbu   (501) staff       (20)        0 2024-01-16 08:33:13.360574 pyngoST-1.1.1/pyngoST/
--rwxr-xr-x   0 leosanbu   (501) staff       (20)     7616 2024-01-15 21:49:48.000000 pyngoST-1.1.1/pyngoST/pyngoST.py
--rwxr-xr-x   0 leosanbu   (501) staff       (20)    26850 2024-01-15 22:08:12.000000 pyngoST-1.1.1/pyngoST/pyngoST_utils.py
-drwxr-xr-x   0 leosanbu   (501) staff       (20)        0 2024-01-16 08:33:13.363171 pyngoST-1.1.1/pyngoST.egg-info/
--rw-r--r--   0 leosanbu   (501) staff       (20)      345 2024-01-16 08:33:13.000000 pyngoST-1.1.1/pyngoST.egg-info/PKG-INFO
--rw-r--r--   0 leosanbu   (501) staff       (20)      216 2024-01-16 08:33:13.000000 pyngoST-1.1.1/pyngoST.egg-info/SOURCES.txt
--rw-r--r--   0 leosanbu   (501) staff       (20)        1 2024-01-16 08:33:13.000000 pyngoST-1.1.1/pyngoST.egg-info/dependency_links.txt
--rw-r--r--   0 leosanbu   (501) staff       (20)       73 2024-01-16 08:33:13.000000 pyngoST-1.1.1/pyngoST.egg-info/requires.txt
--rw-r--r--   0 leosanbu   (501) staff       (20)        8 2024-01-16 08:33:13.000000 pyngoST-1.1.1/pyngoST.egg-info/top_level.txt
--rw-r--r--   0 leosanbu   (501) staff       (20)       38 2024-01-16 08:33:13.363884 pyngoST-1.1.1/setup.cfg
--rw-r--r--   0 leosanbu   (501) staff       (20)      545 2024-01-16 08:33:07.000000 pyngoST-1.1.1/setup.py
+drwxr-xr-x   0 leosanbu   (501) staff       (20)        0 2024-05-13 13:31:48.691228 pyngoST-1.1.2/
+-rw-r--r--   0 leosanbu   (501) staff       (20)      345 2024-05-13 13:31:48.690962 pyngoST-1.1.2/PKG-INFO
+-rw-r--r--   0 leosanbu   (501) staff       (20)    17883 2024-05-13 13:29:32.000000 pyngoST-1.1.2/README.md
+drwxr-xr-x   0 leosanbu   (501) staff       (20)        0 2024-05-13 13:31:48.688266 pyngoST-1.1.2/pyngoST/
+-rwxr-xr-x   0 leosanbu   (501) staff       (20)     7597 2024-05-13 13:26:58.000000 pyngoST-1.1.2/pyngoST/pyngoST.py
+-rwxr-xr-x   0 leosanbu   (501) staff       (20)    27204 2024-05-13 10:32:52.000000 pyngoST-1.1.2/pyngoST/pyngoST_utils.py
+drwxr-xr-x   0 leosanbu   (501) staff       (20)        0 2024-05-13 13:31:48.690377 pyngoST-1.1.2/pyngoST.egg-info/
+-rw-r--r--   0 leosanbu   (501) staff       (20)      345 2024-05-13 13:31:48.000000 pyngoST-1.1.2/pyngoST.egg-info/PKG-INFO
+-rw-r--r--   0 leosanbu   (501) staff       (20)      216 2024-05-13 13:31:48.000000 pyngoST-1.1.2/pyngoST.egg-info/SOURCES.txt
+-rw-r--r--   0 leosanbu   (501) staff       (20)        1 2024-05-13 13:31:48.000000 pyngoST-1.1.2/pyngoST.egg-info/dependency_links.txt
+-rw-r--r--   0 leosanbu   (501) staff       (20)       73 2024-05-13 13:31:48.000000 pyngoST-1.1.2/pyngoST.egg-info/requires.txt
+-rw-r--r--   0 leosanbu   (501) staff       (20)        8 2024-05-13 13:31:48.000000 pyngoST-1.1.2/pyngoST.egg-info/top_level.txt
+-rw-r--r--   0 leosanbu   (501) staff       (20)       38 2024-05-13 13:31:48.691319 pyngoST-1.1.2/setup.cfg
+-rw-r--r--   0 leosanbu   (501) staff       (20)      545 2024-05-13 13:31:29.000000 pyngoST-1.1.2/setup.py
```

### Comparing `pyngoST-1.1.1/README.md` & `pyngoST-1.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,19 @@
 
 ## Run pyngSTar
 
 ## Exit virtualenv
 deactivate
 ```
 
+**NOTE**: After installing with `pip`, the package can be run from `/Users/username/venv/lib/python3.X/site-packages/pyngoST/pyngoST.py`. You can add it to your PATH or create an alias to use it more easily, as in:
+```
+alias pyngoST.py="/Users/username/venv/bin/python3 /Users/username/venv/lib/python3.X/site-packages/pyngoST/pyngoST.py"
+```
+
 ## Bulding the database
 
 You can download updated allele and profiles files for the three schemes using `-d`. NG-STAR alleles and profiles will be downloaded and adapted from [NG-STAR Canada](https://ngstar.canada.ca/)). MLST and NG-MAST alleles and profiles will be downloaded from [PubMLST Neisseria](https://pubmlst.org/bigsdb?db=pubmlst_mlst_seqdef). By default, it will create the database under the `allelesDB` folder if it does not exist in the working directory. You can provide a database name with `-n`. If a CSV file containing NG-STAR CCs is included with `-cc`, CCs will be integrated into the database.
 ```
 ## Create the database as 'allelesDB'
 pyngoST.py -d
 
@@ -59,45 +64,47 @@
 ## Incorporate NG-STAR CCs and update the pickle file in the database
 pyngoST.py -u -p /path/to/allelesDB -cc NGSTAR_CCs.csv
 ```
 
 ## Available options
 
 ```
-usage: pyngoST.py [options]
+usage: pyngoST [options]
 
 pyngoST: fast, simultaneous and accurate multiple sequence typing of Neisseria gonorrhoeae genome collections
 
 Citation:
     Sanchez-Buso L, Sanchez-Serrano A, Golparian D and Unemo M.
     pyngoST: fast, simultaneous and accurate multiple sequence typing of Neisseria gonorrhoeae genome collections.
+    Preprint: https://doi.org/10.1099/mgen.0.001189
     GitHub: https://github.com/leosanbu/pyngoST
 
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT [INPUT ...], --input INPUT [INPUT ...]
                         Input files (fasta or tab/csv)
   -r READ_FILE, --read_file READ_FILE
                         File containing the paths to the input files
   -s SCHEMES, --schemes SCHEMES
                         Typing schemes to query separated by commas (options: NG-STAR, MLST, NG-MAST) (default=NG-STAR)
   -g, --genogroups      Calculate NG-MAST genogroups from NG-MAST types (default=False)
   -c, --ngstarccs       Include NG-STAR CCs in output table (default=False)
+  -m, --mosaic_pena     Report if the penA allele sequence is a mosaic or semimosaic (default=False)
   -b, --blast_new_alleles
-                        Use blastn to find the closest alleles to new ones (default: False)
-  -a, --alleles_out     Print fasta files with new alleles (optional, default: False)
+                        Use blastn to find the closest alleles to new ones (default=False)
+  -a, --alleles_out     Print fasta files with new alleles (optional, default=False)
   -q OUT_PATH, --out_path OUT_PATH
                         Path used to save output files (default: current directory)
   -o OUT_FILENAME, --out_filename OUT_FILENAME
-                        Name of file to print the results table to (optional, default: screen output)
+                        Name of file to print the results table to (optional, default=screen output)
   -y ONLY_ASSIGNCCS, --only_assignccs ONLY_ASSIGNCCS
-                        Only assign CCs from a table with NG-STAR STs. Indicate as value the number of the column that contains the STs (optional, default: None)
-  -z, --only_assignsts  Only assign STs from a table with NG-STAR, MLST and/or NG-MAST profiles (optional, default: None)
+                        Only assign CCs from a table with NG-STAR STs. Indicate as value the number of the column that contains the STs (optional, default=None)
+  -z, --only_assignsts  Only assign STs from a table with NG-STAR, MLST and/or NG-MAST profiles (optional, default=None)
   -t NUM_THREADS, --num_threads NUM_THREADS
-                        Number of processes to use for computation (optional, default: 1)
+                        Number of processes to use for computation (optional, default=1)
   -p PATH, --path PATH  Path to database containing MLST/NG-STAR alleles and profiles. If not available, use -d to create an updated database
   -d, --download_db     Download updated allele and profile files and create database
   -n DB_NAME, --db_name DB_NAME
                         Name of the folder that will contain the database in case a download is requested with -d (default=allelesDB in working directory)
   -u, --update          Only recreate the database pickle file
   -cc NGSTARCCSFILE, --ngstarccsfile NGSTARCCSFILE
                         File with the NG-STAR clonal complexes (NG-STAR CCs) database (csv) to integrate to NG-STAR profiles
@@ -106,14 +113,15 @@
 | Option | Description |
 | :---: | :--- |
 | -i | list of assembly files (* can be used to input multiple files in a directory). |
 | -r | text file containing a list of paths to assembly files. |
 | -s | schemes to query and report: NG-STAR,MLST,NG-STAR or any combination/order separated by commas. |
 | -g | calculate NG-MAST genogroups from NG-MAST typing using the rules described in [Harris et al, 2018](https://doi.org/10.1016/S1473-3099(18)30225-1). |
 | -c | report NG-STAR Clonal Complexes from NG-STAR STs in the final results table. |
+| -m | report the type of penA mosaicism (mosaic, semi-mosaic or non-mosaic). |
 | -b | blast new alleles to identify the closest among the known ones. |
 | -a | save new alleles to output fasta files. |
 | -o | name of output file where to save the results table. By default, results will print to the screen. |
 | -q | path where to save results if different from the working directory. |
 | -y | only call NG-STAR Clonal Complexes from a table of NG-STAR STs. Specify the number of column containing the STs. |
 | -z | only assign STs from a table containing allelic profiles of any of NG-STAR, MLST and NG-STAR (specify with -s). |
 | -t | number of threads for multithreading the main processing function from fasta files. |
@@ -236,7 +244,15 @@
 
 Please note that only computationally intensive tasks are worth multithreading, such as combining the blasting of new alleles with the calculation of NG-MAST genogroups. You can multithread using `-t <number of threads`, i.e:
 ```
 ## Run pyngoST on 400 FASTA files requesting the blasting of new alleles with -b and genogroups calculation with -g on 8 threads
 pyngoST.py -i /path/to/400genomes/*.fasta -p /path/to/allelesDB -s MLST,NG-MAST,NG-STAR -c -g -b -t 8
 ```
 The request of NG-STAR CCs with `-c` is not a calculation but only a query of the existing database and it does not add significantly more computation time compared to not requesting CCs.
+
+## Citation
+
+If you use `pyngoST` or integrate it into your pipelines and use it in a scientific publication, we would appreciate if you could cite our work:
+
+Sánchez-Busó L, Sánchez-Serrano A, Golparian D, Unemo M. pyngoST: fast, simultaneous and accurate multiple sequence typing of Neisseria gonorrhoeae genome collections. Microb Genom. 2024 Jan;10(1):001189. doi: 10.1099/mgen.0.001189. PMID: 38288762; PMCID: PMC10868605.
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyngoST-1.1.1/pyngoST/pyngoST.py` & `pyngoST-1.1.2/pyngoST/pyngoST.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ## Script parameters
 parser = arg.ArgumentParser(prog="pyngoST",
 	formatter_class=RawTextHelpFormatter,
 	description='pyngoST: fast, simultaneous and accurate multiple sequence typing of Neisseria gonorrhoeae genome collections\n'
 	'\nCitation:\n'
 	'    Sanchez-Buso L, Sanchez-Serrano A, Golparian D and Unemo M.\n'
 	'    pyngoST: fast, simultaneous and accurate multiple sequence typing of Neisseria gonorrhoeae genome collections.\n'
-	'    Preprint: https://www.biorxiv.org/content/10.1101/2023.10.23.563537v2\n'
+	'    Publication: https://doi.org/10.1099/mgen.0.001189\n'
 	'    GitHub: https://github.com/leosanbu/pyngoST\n',
 	usage = '%(prog)s [options]')
 
 parser.add_argument('-i', '--input', help='Input files (fasta or tab/csv)', required=False, nargs='+')
 parser.add_argument('-r', '--read_file', help='File containing the paths to the input files', required=False)
 parser.add_argument('-s', '--schemes', help='Typing schemes to query separated by commas (options: NG-STAR, MLST, NG-MAST) (default=NG-STAR)', required=False, default='NG-STAR')
 parser.add_argument('-g', '--genogroups', help='Calculate NG-MAST genogroups from NG-MAST types (default=False)', required=False, action='store_true')
```

### Comparing `pyngoST-1.1.1/pyngoST/pyngoST_utils.py` & `pyngoST-1.1.2/pyngoST/pyngoST_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,19 +99,19 @@
 
 def download_updated_dbs(db_path, ccsfile):
 	if ccsfile:
 		ngstarccsfile = read_ngstar_ccs(ccsfile)
 	# MLST and NG-MAST v2 from PubMLST
 	print('## Downloading MLST and NG-MAST v2 alleles and Sequence Type profiles from https://pubmlst.org')
 	loci = ['abcZ', 'adk', 'aroE', 'fumC', 'gdh', 'pdhC', 'pgm', 'NG-MAST_porB', 'NG-MAST_tbpB']
-	pubmlstURLloci = 'https://pubmlst.org/bigsdb?db=pubmlst_neisseria_seqdef&page=downloadAlleles&locus='
-	pubmlstMLSTs = 'https://pubmlst.org/bigsdb?db=pubmlst_neisseria_seqdef&page=downloadProfiles&scheme_id=1'
-	pubmlstNGMASTs = 'https://pubmlst.org/bigsdb?db=pubmlst_neisseria_seqdef&page=downloadProfiles&scheme_id=71'
+	pubmlstURLloci = 'https://rest.pubmlst.org/db/pubmlst_neisseria_seqdef/loci/'#abcZ/alleles_fasta'
+	pubmlstMLSTs = 'https://rest.pubmlst.org/db/pubmlst_neisseria_seqdef/schemes/1/profiles_csv'
+	pubmlstNGMASTs = 'https://rest.pubmlst.org/db/pubmlst_neisseria_seqdef/schemes/71/profiles_csv'
 	for g in loci:
-		r = requests.get(pubmlstURLloci+g, allow_redirects=True)
+		r = requests.get(pubmlstURLloci+g+'/alleles_fasta', allow_redirects=True)
 		open(db_path+'/'+g+'.fas', 'wb').write(r.content)
 	m = requests.get(pubmlstMLSTs, allow_redirects=True)
 	open(db_path+'/MLST_profiles.tab', 'wb').write(m.content)
 	n = requests.get(pubmlstNGMASTs, allow_redirects=True)
 	open(db_path+'/NGMAST_profiles.tab', 'wb').write(n.content)
 	# Formatting NG-MAST files
 	por_fas = open(db_path+'/POR.fas', 'w+')
@@ -141,15 +141,15 @@
 	# Download allele fasta files
 	for g in locistar:
 		r = requests.get(ngstarURLloci+g, allow_redirects=True, verify=False)
 		open(db_path+'/'+g+'.fas', 'wb').write(r.content)
 	# Download and process profiles
 	s = requests.get(ngstarNGSTARs, allow_redirects=True, verify=False)
 	open(db_path+'/NGSTAR_profiles.xlsx', 'wb').write(s.content)
-	df = pd.read_excel(db_path+'/NGSTAR_profiles.xlsx', sheet_name='Sheet 1')
+	df = pd.read_excel(db_path+'/NGSTAR_profiles.xlsx', sheet_name='Sheet 1', engine='openpyxl')
 	with open(db_path+'/NGSTAR_profiles.tmp.tab', 'w') as outfile:
 		df.to_string(outfile, index=None)
 	outfile = open(db_path+'/NGSTAR_profiles.tab', 'w+')
 	with open(db_path+'/NGSTAR_profiles.tmp.tab', 'r') as profiles:
 		for line in profiles:
 			if 'Sequence Type':
 				line=line.replace('Sequence Type', 'ST')
@@ -164,15 +164,15 @@
 						linesplit.append('-')
 			outfile.write('\t'.join(linesplit)+'\n')
 	if 'NGSTAR_profiles.tmp.tab' in os.listdir(db_path):
 		subprocess.call(['rm', db_path+'/NGSTAR_profiles.tmp.tab'])
 	# Download penA alleles metadata to extract mosaic information
 	r = requests.get(ngstarMOSAIC, allow_redirects=True, verify=False)
 	open(db_path+'/penA_alleles_metadata.xlsx', 'wb').write(r.content)
-	df2 = pd.read_excel(db_path+'/penA_alleles_metadata.xlsx', sheet_name='Sheet 1')
+	df2 = pd.read_excel(db_path+'/penA_alleles_metadata.xlsx', sheet_name='Sheet 1', engine='openpyxl')
 	with open(db_path+'/penA_metadata.tmp.tab', 'w') as outfile2:
 		df2.to_string(outfile2, index=None)
 	outmeta = open(db_path+'/penA_mosaics.tab', 'w+')
 	outmeta.write('penA_allele'+'\t'+'mosaic_type'+'\n')
 	with open(db_path+'/penA_metadata.tmp.tab', 'r') as metadata:
 		for line in metadata:
 			linesplit=re.split(' |;|,|:', line)
@@ -293,15 +293,20 @@
 			for line in tab:
 				linesplit = line.rstrip().split(sep)
 				st = linesplit[int(column)-1]
 				if st in ngstarCCsdic:
 					cc = ngstarCCsdic[st]
 				else:
 					cc = '-'
-				ngstarccsvec.append(sep.join(linesplit)+sep+'CC'+cc)
+				if cc=='Ungroupable':
+					ngstarccsvec.append(sep.join(linesplit)+sep+cc)
+				elif cc=='-':
+					st_list['NG-STAR'] = st+'\t'+prof+'\t-'
+				else:
+					ngstarccsvec.append(sep.join(linesplit)+sep+'CC'+cc)
 		# Print results
 		if outfilename:
 			outfilehandle = open(outfilename, 'w+')
 			for v in ngstarccsvec: 
 				outfilehandle.write(v+'\n')
 			outfilehandle.close()
 		else:
@@ -369,15 +374,20 @@
 					to_join.append(ngmast)
 					to_join.append(sep.join(NGMASTprof))
 				elif s=='NG-STAR':
 					to_join.append(ngstar)
 					to_join.append(sep.join(NGSTARprof))
 					if ngstarccs:
 						if ngstar in ngstarCCsdic:
-							cc = 'CC'+ngstarCCsdic[ngstar]
+							if ngstarCCsdic[ngstar]=="Ungroupable":
+								cc = 'Ungroupable'
+							elif ngstarCCsdic[ngstar]=='-':
+								cc = '-'
+							else:
+								cc = 'CC'+ngstarCCsdic[ngstar]
 						else:
 							cc = '-'
 						to_join.append(cc)
 					if mosaic_pena:
 						penA_al = NGSTARprof[0]
 						if penA_al in penAmosaicsdic:
 							penmos = penAmosaicsdic[penA_al]
@@ -648,16 +658,16 @@
 
 def process_files(args):
 	fpath, order, MLSTorder, NGSTARorder, NGMASTorder, profilesDB, allelesDB, allelesAC, schemes, \
     ngstarCCsdic, penAmosaicsdic, genogroups, db_path, PORout_results, TBPBout_results, allout, blast_new_alleles, out_path, \
     new_alleles, indices_new_alleles = args
 	fname = fpath.split('/').pop()
 	blast_hit = 0
-	if not fpath.endswith('.fasta') or fpath.endswith('.fas') or fpath.endswith('.fa'):
-		print('## Input file is not recognised as a fasta file. Please, include fasta files ending in .fasta, .fas or .fa')
+	if not fpath.endswith('.fasta') or fpath.endswith('.fas') or fpath.endswith('.fa') or fpath.endswith('.fna'):
+		print('## Input file is not recognised as a fasta file. Please, include fasta files ending in .fasta, .fas, .fa or .fna')
 		sys.exit()
 	with open(fpath, 'r') as fasta:
 		concat = ''
 		for record in SeqIO.parse(fasta, 'fasta'):
 			concat += record.seq
 	#AC algorithm:
 	resultsDB = ac_fast(fname, str(concat), order, allelesDB, allelesAC, genogroups, out_path, PORout_results, TBPBout_results)
```

### Comparing `pyngoST-1.1.1/setup.py` & `pyngoST-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='pyngoST',
-    version='1.1.1',
+    version='1.1.2',
     author='Leonor Sanchez-Buso',
     author_email='leonor.sanchez@fisabio.es',
     description='pyngoST: fast, simultaneous and accurate and multiple sequence typing of Neisseria gonorrhoeae genome collections',
     url='https://github.com/leosanbu/pyngoST',
     packages=['pyngoST'],
     install_requires=[
         'urllib3==1.26.6',
```

