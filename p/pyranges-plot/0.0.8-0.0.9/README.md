# Comparing `tmp/pyranges_plot-0.0.8.tar.gz` & `tmp/pyranges_plot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyranges_plot-0.0.8.tar", last modified: Thu Oct 26 09:47:21 2023, max compression
+gzip compressed data, was "pyranges_plot-0.0.9.tar", last modified: Thu Oct 26 12:06:25 2023, max compression
```

## Comparing `pyranges_plot-0.0.8.tar` & `pyranges_plot-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 estermdc  (1002) estermdc  (1002)        0 2023-10-26 09:47:21.813562 pyranges_plot-0.0.8/
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)     1065 2023-10-06 08:27:42.000000 pyranges_plot-0.0.8/LICENSE
--rw-r--r--   0 estermdc  (1002) estermdc  (1002)    11207 2023-10-26 09:47:21.813562 pyranges_plot-0.0.8/PKG-INFO
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)    10439 2023-10-25 12:13:18.000000 pyranges_plot-0.0.8/README.md
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)      977 2023-10-26 09:47:21.813562 pyranges_plot-0.0.8/setup.cfg
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)       69 2023-10-06 08:29:19.000000 pyranges_plot-0.0.8/setup.py
-drwxrwxr-x   0 estermdc  (1002) estermdc  (1002)        0 2023-10-26 09:47:21.813562 pyranges_plot-0.0.8/src/
-drwxrwxr-x   0 estermdc  (1002) estermdc  (1002)        0 2023-10-26 09:47:21.813562 pyranges_plot-0.0.8/src/pyranges_plot/
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)      146 2023-10-25 08:10:33.000000 pyranges_plot-0.0.8/src/pyranges_plot/__init__.py
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)       22 2023-10-26 09:36:45.000000 pyranges_plot-0.0.8/src/pyranges_plot/_version.py
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)     5159 2023-10-26 08:38:18.000000 pyranges_plot-0.0.8/src/pyranges_plot/core.py
-drwxrwxr-x   0 estermdc  (1002) estermdc  (1002)        0 2023-10-26 09:47:21.813562 pyranges_plot-0.0.8/src/pyranges_plot/plot_exons_plt/
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)       44 2023-10-06 10:53:13.000000 pyranges_plot-0.0.8/src/pyranges_plot/plot_exons_plt/__init__.py
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)    21483 2023-10-26 09:09:21.000000 pyranges_plot-0.0.8/src/pyranges_plot/plot_exons_plt/plot_exons_plt.py
-drwxrwxr-x   0 estermdc  (1002) estermdc  (1002)        0 2023-10-26 09:47:21.813562 pyranges_plot-0.0.8/src/pyranges_plot/plot_exons_ply/
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)       43 2023-10-06 10:53:23.000000 pyranges_plot-0.0.8/src/pyranges_plot/plot_exons_ply/__init__.py
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)    20577 2023-10-26 09:15:33.000000 pyranges_plot-0.0.8/src/pyranges_plot/plot_exons_ply/plot_exons_ply.py
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)     1434 2023-10-17 10:48:05.000000 pyranges_plot-0.0.8/src/pyranges_plot/plot_features.py
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)     5779 2023-10-25 08:31:04.000000 pyranges_plot-0.0.8/src/pyranges_plot/plot_generic.py
-drwxrwxr-x   0 estermdc  (1002) estermdc  (1002)        0 2023-10-26 09:47:21.813562 pyranges_plot-0.0.8/src/pyranges_plot.egg-info/
--rw-r--r--   0 estermdc  (1002) estermdc  (1002)    11207 2023-10-26 09:47:21.000000 pyranges_plot-0.0.8/src/pyranges_plot.egg-info/PKG-INFO
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)      587 2023-10-26 09:47:21.000000 pyranges_plot-0.0.8/src/pyranges_plot.egg-info/SOURCES.txt
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)        1 2023-10-26 09:47:21.000000 pyranges_plot-0.0.8/src/pyranges_plot.egg-info/dependency_links.txt
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)      116 2023-10-26 09:47:21.000000 pyranges_plot-0.0.8/src/pyranges_plot.egg-info/requires.txt
--rw-rw-r--   0 estermdc  (1002) estermdc  (1002)       14 2023-10-26 09:47:21.000000 pyranges_plot-0.0.8/src/pyranges_plot.egg-info/top_level.txt
+drwxrwxr-x   0 estermdc  (1002) estermdc  (1002)        0 2023-10-26 12:06:25.074926 pyranges_plot-0.0.9/
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)     1065 2023-10-06 08:27:42.000000 pyranges_plot-0.0.9/LICENSE
+-rw-r--r--   0 estermdc  (1002) estermdc  (1002)    11207 2023-10-26 12:06:25.074926 pyranges_plot-0.0.9/PKG-INFO
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)    10439 2023-10-25 12:13:18.000000 pyranges_plot-0.0.9/README.md
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)      977 2023-10-26 12:06:25.074926 pyranges_plot-0.0.9/setup.cfg
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)       69 2023-10-06 08:29:19.000000 pyranges_plot-0.0.9/setup.py
+drwxrwxr-x   0 estermdc  (1002) estermdc  (1002)        0 2023-10-26 12:06:25.074926 pyranges_plot-0.0.9/src/
+drwxrwxr-x   0 estermdc  (1002) estermdc  (1002)        0 2023-10-26 12:06:25.074926 pyranges_plot-0.0.9/src/pyranges_plot/
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)      146 2023-10-25 08:10:33.000000 pyranges_plot-0.0.9/src/pyranges_plot/__init__.py
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)       22 2023-10-26 12:03:26.000000 pyranges_plot-0.0.9/src/pyranges_plot/_version.py
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)     5159 2023-10-26 08:38:18.000000 pyranges_plot-0.0.9/src/pyranges_plot/core.py
+drwxrwxr-x   0 estermdc  (1002) estermdc  (1002)        0 2023-10-26 12:06:25.074926 pyranges_plot-0.0.9/src/pyranges_plot/plot_exons_plt/
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)       44 2023-10-06 10:53:13.000000 pyranges_plot-0.0.9/src/pyranges_plot/plot_exons_plt/__init__.py
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)    21607 2023-10-26 12:01:38.000000 pyranges_plot-0.0.9/src/pyranges_plot/plot_exons_plt/plot_exons_plt.py
+drwxrwxr-x   0 estermdc  (1002) estermdc  (1002)        0 2023-10-26 12:06:25.074926 pyranges_plot-0.0.9/src/pyranges_plot/plot_exons_ply/
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)       43 2023-10-06 10:53:23.000000 pyranges_plot-0.0.9/src/pyranges_plot/plot_exons_ply/__init__.py
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)    20703 2023-10-26 12:00:17.000000 pyranges_plot-0.0.9/src/pyranges_plot/plot_exons_ply/plot_exons_ply.py
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)     1434 2023-10-17 10:48:05.000000 pyranges_plot-0.0.9/src/pyranges_plot/plot_features.py
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)     5779 2023-10-25 08:31:04.000000 pyranges_plot-0.0.9/src/pyranges_plot/plot_generic.py
+drwxrwxr-x   0 estermdc  (1002) estermdc  (1002)        0 2023-10-26 12:06:25.074926 pyranges_plot-0.0.9/src/pyranges_plot.egg-info/
+-rw-r--r--   0 estermdc  (1002) estermdc  (1002)    11207 2023-10-26 12:06:25.000000 pyranges_plot-0.0.9/src/pyranges_plot.egg-info/PKG-INFO
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)      587 2023-10-26 12:06:25.000000 pyranges_plot-0.0.9/src/pyranges_plot.egg-info/SOURCES.txt
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)        1 2023-10-26 12:06:25.000000 pyranges_plot-0.0.9/src/pyranges_plot.egg-info/dependency_links.txt
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)      116 2023-10-26 12:06:25.000000 pyranges_plot-0.0.9/src/pyranges_plot.egg-info/requires.txt
+-rw-rw-r--   0 estermdc  (1002) estermdc  (1002)       14 2023-10-26 12:06:25.000000 pyranges_plot-0.0.9/src/pyranges_plot.egg-info/top_level.txt
```

### Comparing `pyranges_plot-0.0.8/LICENSE` & `pyranges_plot-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyranges_plot-0.0.8/PKG-INFO` & `pyranges_plot-0.0.9/src/pyranges_plot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyranges_plot
-Version: 0.0.8
+Name: pyranges-plot
+Version: 0.0.9
 Summary: 'Gene visualization package for dataframe objects generated with PyRanges.'
 Home-page: https://github.com/emunozdc/pyranges_plot.git
 Author: Ester Muñoz del Campo, Marco Mariotti
 Author-email: ester.munoz01@estudiant.upf.edu, marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyranges_plot-0.0.8/README.md` & `pyranges_plot-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyranges_plot-0.0.8/setup.cfg` & `pyranges_plot-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyranges_plot-0.0.8/src/pyranges_plot/core.py` & `pyranges_plot-0.0.9/src/pyranges_plot/core.py`

 * *Files identical despite different names*

### Comparing `pyranges_plot-0.0.8/src/pyranges_plot/plot_exons_plt/plot_exons_plt.py` & `pyranges_plot-0.0.9/src/pyranges_plot/plot_exons_plt/plot_exons_plt.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,23 +356,23 @@
             # Connect the on_hover function to the "motion_notify_event" event
             fig.canvas.mpl_connect("motion_notify_event", on_hover)
         
             #remove non-CDS from data
             df = df.groupby('Feature').get_group('CDS')
         
         # transcript only has CDS
-        #elif df.Feature.str.contains('CDS').any() and not df.Feature.str.contains('exon').any():
+        elif df.Feature.str.contains('CDS').any() and not df.Feature.str.contains('exon').any():
+            print()
         
         # transcript only has exon    
         elif not df.Feature.str.contains('CDS').any() and df.Feature.str.contains('exon').any():
-            #plot just as utr and pass gene
+            #plot just as utr 
             df.apply(_apply_gene, args=(fig, ax, strand, genename, gene_ix, exon_color, chrom, chrom_ix, n_exons, 
                      tag_background, geneinfo, transcript_utr_width), axis=1)
-            return
-            
+          
         # transcript has neither, skip it
         else:
             return
     
     
     # Plot the LINE binding the exons    
     gene_line = ax.plot([min(df.Start), max(df.End)], [gene_ix, gene_ix], color=exon_color, linewidth=1, zorder=1)
@@ -397,15 +397,17 @@
             annotation.set_visible(False)
             fig.canvas.draw()
 
     fig.canvas.mpl_connect("motion_notify_event", on_hover) 
     
     
     # Plot the gene rows
-    df.apply(_apply_gene, args=(fig, ax, strand, genename, gene_ix, exon_color, chrom, chrom_ix, n_exons, tag_background, geneinfo, exon_width), axis=1)
+    # trancript does not only have exon    
+    if df.Feature.str.contains('CDS').any() and not df.Feature.str.contains('exon').any():
+        df.apply(_apply_gene, args=(fig, ax, strand, genename, gene_ix, exon_color, chrom, chrom_ix, n_exons, tag_background, geneinfo, exon_width), axis=1)
             
 
     # Plot DIRECTION ARROW in INTRONS if strand is known
     sorted_exons = df[['Start', 'End']].sort_values(by = 'Start')
     
     if strand:
         # evaluate each intron
```

### Comparing `pyranges_plot-0.0.8/src/pyranges_plot/plot_exons_ply/plot_exons_ply.py` & `pyranges_plot-0.0.9/src/pyranges_plot/plot_exons_ply/plot_exons_ply.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         genesmd_df['color'] = genesmd_df['color_tag'].map(colormap)  ## NOTE: when specifying color by dict, careful with color_col
         genesmd_df['color'].fillna('black', inplace=True) # not specified in dict will be colored as black
     
     
     # Create figure and chromosome plots
     titles = ["Chromosome %s" % chrom for chrom in chrmd_df.index]
     fig = sp.make_subplots(rows=nchrs, cols=1, row_heights=chrmd_df.y_height.to_list(), subplot_titles=titles)
-    print('\n\n\n' + str(sum(chrmd_df.y_height)+ nchrs) + '\n\n\n')
+    #print('\n\n\n' + str(sum(chrmd_df.y_height)+ nchrs) + '\n\n\n')
     
     # one subplot per chromosome
     for i in range(nchrs):
         chrom = chrmd_df.index[i]
         fig.add_trace(go.Scatter(x=[], y=[]), row=i+1, col=1)
         
         # set title format
@@ -332,21 +332,21 @@
                            row=chrom_ix+1, 
                            col=1)
                            
             #remove non-CDS from data
             df = df.groupby('Feature').get_group('CDS')
             
         # transcript only has CDS
-        #elif df.Feature.str.contains('CDS').any() and not df.Feature.str.contains('exon').any():
+        elif df.Feature.str.contains('CDS').any() and not df.Feature.str.contains('exon').any():
+            print()
         
         # trancript only has exon    
         elif not df.Feature.str.contains('CDS').any() and df.Feature.str.contains('exon').any():
-            #plot just as utr and pass gene
+            #plot just as utr
             df.apply(_apply_gene, args=(fig, strand, genename, gene_ix, exon_color, chrom, chrom_ix, n_exons, genelabel, geneinfo, transcript_utr_width), axis=1)
-            return
             
         # transcript has neither, skip it
         else:
             return
 
 
     # Plot LINE binding the exons
@@ -359,15 +359,17 @@
         fillcolor=exon_color,
         mode='lines',
         line=dict(color=exon_color, width=0.5),
         name=geneinfo)
     fig.add_trace(exon_line, row=chrom_ix+1, col=1)
     
     # Plot the gene rows
-    df.apply(_apply_gene, args=(fig, strand, genename, gene_ix, exon_color, chrom, chrom_ix, n_exons, genelabel, geneinfo, exon_width), axis=1)
+    # trancript does not only have exon    
+    if df.Feature.str.contains('CDS').any() and not df.Feature.str.contains('exon').any():
+        df.apply(_apply_gene, args=(fig, strand, genename, gene_ix, exon_color, chrom, chrom_ix, n_exons, genelabel, geneinfo, exon_width), axis=1)
     
     # Plot DIRECTION ARROW in INTRONS if strand is known
     sorted_exons = df[['Start', 'End']].sort_values(by = 'Start')
     
     if strand:
         # evaluate  each intron
         for i in range(len(sorted_exons)-1):
```

### Comparing `pyranges_plot-0.0.8/src/pyranges_plot/plot_features.py` & `pyranges_plot-0.0.9/src/pyranges_plot/plot_features.py`

 * *Files identical despite different names*

### Comparing `pyranges_plot-0.0.8/src/pyranges_plot/plot_generic.py` & `pyranges_plot-0.0.9/src/pyranges_plot/plot_generic.py`

 * *Files identical despite different names*

### Comparing `pyranges_plot-0.0.8/src/pyranges_plot.egg-info/PKG-INFO` & `pyranges_plot-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyranges-plot
-Version: 0.0.8
+Name: pyranges_plot
+Version: 0.0.9
 Summary: 'Gene visualization package for dataframe objects generated with PyRanges.'
 Home-page: https://github.com/emunozdc/pyranges_plot.git
 Author: Ester Muñoz del Campo, Marco Mariotti
 Author-email: ester.munoz01@estudiant.upf.edu, marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyranges_plot-0.0.8/src/pyranges_plot.egg-info/SOURCES.txt` & `pyranges_plot-0.0.9/src/pyranges_plot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

