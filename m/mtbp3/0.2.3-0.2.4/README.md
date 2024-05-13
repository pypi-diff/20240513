# Comparing `tmp/mtbp3-0.2.3-py3-none-any.whl.zip` & `tmp/mtbp3-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 255760 bytes, number of entries: 54
+Zip file size: 255975 bytes, number of entries: 54
 -rw-r--r--  2.0 unx     6148 b- defN 80-Jan-01 00:00 mtbp3/.DS_Store
 -rw-r--r--  2.0 unx      351 b- defN 80-Jan-01 00:00 mtbp3/__init__.py
 -rw-r--r--  2.0 unx     6148 b- defN 80-Jan-01 00:00 mtbp3/data/.DS_Store
 -rw-r--r--  2.0 unx    19789 b- defN 80-Jan-01 00:00 mtbp3/data/supp_ectd/fda_ctoc_v2.3.3.txt
 -rw-r--r--  2.0 unx  1016108 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/FMQ/FMQ_Consolidated_List.csv
 -rw-r--r--  2.0 unx       42 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/MedDRA/!!readme_26_1_English.txt
 -rw-r--r--  2.0 unx     2221 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/MedDRA/MedAscii/hlgt.asc
@@ -42,15 +42,15 @@
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_lsr/testfolder2/testfile20
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_lsr/testfolder2/testfile3
 -rw-r--r--  2.0 unx       19 b- defN 80-Jan-01 00:00 mtbp3/health/__init__.py
 -rw-r--r--  2.0 unx     9095 b- defN 80-Jan-01 00:00 mtbp3/health/clinical.py
 -rw-r--r--  2.0 unx     2113 b- defN 80-Jan-01 00:00 mtbp3/health/ectd.py
 -rw-r--r--  2.0 unx    34117 b- defN 80-Jan-01 00:00 mtbp3/health/emt.py
 -rw-r--r--  2.0 unx       58 b- defN 80-Jan-01 00:00 mtbp3/util/__init__.py
--rw-r--r--  2.0 unx    12727 b- defN 80-Jan-01 00:00 mtbp3/util/cdt.py
+-rw-r--r--  2.0 unx    13604 b- defN 80-Jan-01 00:00 mtbp3/util/cdt.py
 -rw-r--r--  2.0 unx    17343 b- defN 80-Jan-01 00:00 mtbp3/util/cdtg.py
 -rw-r--r--  2.0 unx    11887 b- defN 80-Jan-01 00:00 mtbp3/util/lsr.py
--rw-r--r--  2.0 unx    35107 b- defN 80-Jan-01 00:00 mtbp3-0.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2672 b- defN 80-Jan-01 00:00 mtbp3-0.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mtbp3-0.2.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     5143 b- defN 16-Jan-01 00:00 mtbp3-0.2.3.dist-info/RECORD
-54 files, 1408492 bytes uncompressed, 247254 bytes compressed:  82.4%
+-rw-r--r--  2.0 unx    35107 b- defN 80-Jan-01 00:00 mtbp3-0.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2672 b- defN 80-Jan-01 00:00 mtbp3-0.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mtbp3-0.2.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     5143 b- defN 16-Jan-01 00:00 mtbp3-0.2.4.dist-info/RECORD
+54 files, 1409369 bytes uncompressed, 247469 bytes compressed:  82.4%
```

## zipnote {}

```diff
@@ -144,20 +144,20 @@
 
 Filename: mtbp3/util/cdtg.py
 Comment: 
 
 Filename: mtbp3/util/lsr.py
 Comment: 
 
-Filename: mtbp3-0.2.3.dist-info/LICENSE
+Filename: mtbp3-0.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: mtbp3-0.2.3.dist-info/METADATA
+Filename: mtbp3-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: mtbp3-0.2.3.dist-info/WHEEL
+Filename: mtbp3-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: mtbp3-0.2.3.dist-info/RECORD
+Filename: mtbp3-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mtbp3/util/cdt.py

```diff
@@ -162,16 +162,18 @@
         summary_df.columns = ['Mean', 'SD']
         summary_df['Mean_w_SD'] = summary_df.apply(lambda row: f"{row['Mean']:.1f} ({SD:.1f})", axis=1)
         out = summary_df.reset_index().pivot(index=group_col0, columns=group_col1, values='Mean_w_SD')
 
     return [out, tmp]
 
 class ListTree:
-    def __init__(self, lst=[]):
+    def __init__(self, lst=[], label=[], infmt='path'):
         self.lst = lst
+        self.label = label
+        self.infmt = infmt
         self.df = pd.DataFrame()
         self.prelst = pd.DataFrame()
         self.out = pd.DataFrame()
     
     def __list_tree_df(self):
         if not isinstance(self.lst, list):
             print('Input should be a list.')
@@ -183,15 +185,28 @@
             self.df = pd.DataFrame()
             return
         
         if len(self.lst) <= 1:
             self.df = pd.DataFrame(self.lst, columns=['lst'])
             return
         
-        df0 = pd.DataFrame(self.lst, columns=['lst'])
+        if self.infmt == 'dotspace':
+            df0 = pd.DataFrame([[line.split(' ', 1)[0]]+[line] for line in self.lst], columns=['c1', 'property'])
+            df0['lst'] = df0['c1'].str.replace('.', '/')
+            df0['lst'] = df0['lst'].apply(lambda x: '/'.join([part.zfill(3) for part in x.split('/')]))
+            df0['lst'] = df0['lst'].apply(lambda x: x + '/' if df0['lst'].str.contains(x+'/').any() else x)
+            df0 = df0.drop('c1', axis=1)
+            df0 = df0.sort_values('lst').reset_index(drop=True)
+        else:
+            df0 = pd.DataFrame(self.lst, columns=['lst'])
+            if len(self.label) > 0:
+                df0['property'] = self.label
+            else:
+                df0['property'] = ''
+
         df0['lst'] = df0['lst'].str.replace('^/', '', regex=True)
         df0['type'] = df0['lst'].apply(lambda x: True if x.endswith('/') else False)
         
         for index, row in df0.iterrows():
             r0, r1 = row['lst'].rsplit('/', 1)
             if r1 == "":
                 if '/' in r0:
@@ -209,15 +224,15 @@
         df0['level'] = df0['lst'].str.count('/') + 1
         df0['level'] = df0['level'] - df0['type']
         
         if df0['level'].min() > 0:
             df0['level'] = df0['level'] - df0['level'].min() + 1
         
         df0['row_index'] = df0.index
-        df0['property'] = ""
+        df0 = df0[['lst', 'type', 't1', 't0', 'level', 'row_index', 'property']]
         
         self.df = df0.groupby(df0.columns.difference(['property', 'row_index']).tolist(), sort=False).agg({'row_index': 'max', 'property': lambda x: ''.join(x)}).reset_index().sort_values('row_index')
     
     def __list_tree_pre(self, to_right=False):
         self.__list_tree_df()
         if self.df.empty:
             self.prelst = self.df
@@ -229,15 +244,15 @@
         prelst = pd.concat([prelst, self.df[['t0','property','t1','type','level','row_index']]], axis=1).sort_values('row_index')
         prelst.reset_index(drop=True, inplace=True)
         prelst['row_index'] = prelst.index
         
         if to_right:
             pre = ['', '    ', '   │', ' ──┤', ' ──┘', '  ']
         else:
-            pre  = ['', '    ', '│   ', '├── ', '└── ', '  ']
+            pre = ['', '    ', '│   ', '├── ', '└── ', '  ']
         
         t1_list = prelst[prelst['type'] == True][['t1','level','t0']]
         
         if t1_list.empty:
             self.prelst = self.df['lst']
             return self.prelst
         
@@ -263,14 +278,17 @@
         if to_right:
             prelst['t0'] = prelst.apply(lambda row: row['t0'] if row['type'] == True else row['t0'], axis=1)
             prelst = prelst.loc[:, :'property']
             prelst = prelst.iloc[:, ::-1]
         else:
             prelst['t0'] = prelst.apply(lambda row: row['t0'] + ':' if row['type'] == True else row['t0'], axis=1)
             prelst = prelst.loc[:, :'property']
+
+        if self.infmt == 'dotspace':
+            prelst['t0'] = ''
         
         self.prelst = prelst
     
     def list_tree(self, to_right=False):
         self.__list_tree_pre(to_right=to_right)
         
         if self.prelst.empty:
```

## Comparing `mtbp3-0.2.3.dist-info/LICENSE` & `mtbp3-0.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtbp3-0.2.3.dist-info/METADATA` & `mtbp3-0.2.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtbp3
-Version: 0.2.3
+Version: 0.2.4
 Summary: my tool box
 License: GNU General Public License v3.0
 Author: Y. Hsu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `mtbp3-0.2.3.dist-info/RECORD` & `mtbp3-0.2.4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,14 @@
 mtbp3/data/test_lsr/testfolder2/testfile20,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mtbp3/data/test_lsr/testfolder2/testfile3,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mtbp3/health/__init__.py,sha256=BqJVi0OMHyBp0zcg0IYDcPK1c9q8Fdil-Kcb2AHwNGY,19
 mtbp3/health/clinical.py,sha256=EiDRv70YPkc7sWtAs20a2X6c23uE3SWE9vucZQI1wYs,9095
 mtbp3/health/ectd.py,sha256=r-cifGeHTXbxwgFdkZX7nGfjR2fvEyXjifTAoovguic,2113
 mtbp3/health/emt.py,sha256=FwQUI70DL-O1Y_pGKjDiLziNcgWAYxlYXG6L-Egn0sk,34117
 mtbp3/util/__init__.py,sha256=dbXCXornfglTSgUXCslcrqXyt1lMaUjf5TCn0RdHApc,58
-mtbp3/util/cdt.py,sha256=H7Zsvr39VgIwktVl8kuifHdku2Pc2sPKCTOKAi0r0kw,12727
+mtbp3/util/cdt.py,sha256=XhIKL5vt11fIbMMj5qVBi1_GHsdJNvFLAYszOd0V6zc,13604
 mtbp3/util/cdtg.py,sha256=GC71CPeUhQIpsezfGlZsqASLm-kTQCBM7hl0hbda3Eo,17343
 mtbp3/util/lsr.py,sha256=zwoEKj2slqYa17joB1Zit55G9QEd52MVuW3teV4bUJk,11887
-mtbp3-0.2.3.dist-info/LICENSE,sha256=W6tWaP6lQAHSSUjl4SjXv1Ge3HPPc0CsPwJzih6lkWU,35107
-mtbp3-0.2.3.dist-info/METADATA,sha256=l5Y7Ydq_VAhCZw6SbRxDkC27rkNjxAk5K_jSRHUq2zA,2672
-mtbp3-0.2.3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-mtbp3-0.2.3.dist-info/RECORD,,
+mtbp3-0.2.4.dist-info/LICENSE,sha256=W6tWaP6lQAHSSUjl4SjXv1Ge3HPPc0CsPwJzih6lkWU,35107
+mtbp3-0.2.4.dist-info/METADATA,sha256=2sBcpiWFc1kvgJjn9hKv3kM-2uDUxq8A96IR-Pys4Ho,2672
+mtbp3-0.2.4.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+mtbp3-0.2.4.dist-info/RECORD,,
```

