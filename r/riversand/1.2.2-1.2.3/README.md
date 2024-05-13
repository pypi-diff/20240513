# Comparing `tmp/riversand-1.2.2.tar.gz` & `tmp/riversand-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riversand-1.2.2.tar", last modified: Wed Feb 28 13:14:45 2024, max compression
+gzip compressed data, was "riversand-1.2.3.tar", last modified: Mon May 13 14:35:53 2024, max compression
```

## Comparing `riversand-1.2.2.tar` & `riversand-1.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-02-28 13:14:45.708496 riversand-1.2.2/
--rw-rw-r--   0 user      (1001) user      (1001)    35150 2023-02-25 18:17:07.000000 riversand-1.2.2/LICENSE
--rw-r--r--   0 user      (1001) user      (1001)     3933 2024-02-28 13:14:45.708496 riversand-1.2.2/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)     3009 2024-02-28 12:48:41.000000 riversand-1.2.2/README.md
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-02-28 13:14:45.708496 riversand-1.2.2/riversand/
--rw-rw-r--   0 user      (1001) user      (1001)      580 2024-02-28 08:51:27.000000 riversand-1.2.2/riversand/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)      813 2024-02-28 12:44:42.000000 riversand-1.2.2/riversand/_version.py
--rw-rw-r--   0 user      (1001) user      (1001)    27701 2024-02-28 11:40:02.000000 riversand-1.2.2/riversand/calc.py
--rw-rw-r--   0 user      (1001) user      (1001)    66371 2024-02-28 12:31:09.000000 riversand-1.2.2/riversand/geospatial.py
--rw-rw-r--   0 user      (1001) user      (1001)     3312 2024-02-28 11:34:22.000000 riversand-1.2.2/riversand/params.py
--rw-rw-r--   0 user      (1001) user      (1001)    11378 2024-02-28 08:29:04.000000 riversand-1.2.2/riversand/plot.py
--rw-rw-r--   0 user      (1001) user      (1001)    23435 2024-02-28 11:38:25.000000 riversand-1.2.2/riversand/utils.py
--rw-rw-r--   0 user      (1001) user      (1001)     9269 2023-02-25 20:02:22.000000 riversand-1.2.2/riversand/xml.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-02-28 13:14:45.708496 riversand-1.2.2/riversand.egg-info/
--rw-r--r--   0 user      (1001) user      (1001)     3933 2024-02-28 13:14:45.000000 riversand-1.2.2/riversand.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      350 2024-02-28 13:14:45.000000 riversand-1.2.2/riversand.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2024-02-28 13:14:45.000000 riversand-1.2.2/riversand.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       59 2024-02-28 13:14:45.000000 riversand-1.2.2/riversand.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       10 2024-02-28 13:14:45.000000 riversand-1.2.2/riversand.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2024-02-28 13:14:45.708496 riversand-1.2.2/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     1269 2024-02-28 12:50:11.000000 riversand-1.2.2/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-13 14:35:53.782469 riversand-1.2.3/
+-rw-rw-r--   0 user      (1001) user      (1001)    35150 2023-02-25 18:17:07.000000 riversand-1.2.3/LICENSE
+-rw-r--r--   0 user      (1001) user      (1001)     3927 2024-05-13 14:35:53.782469 riversand-1.2.3/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)     3003 2024-05-13 14:21:49.000000 riversand-1.2.3/README.md
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-13 14:35:53.782469 riversand-1.2.3/riversand/
+-rw-rw-r--   0 user      (1001) user      (1001)      739 2024-05-10 17:59:33.000000 riversand-1.2.3/riversand/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)      220 2024-05-13 14:19:48.000000 riversand-1.2.3/riversand/_version.py
+-rw-rw-r--   0 user      (1001) user      (1001)    35160 2024-05-12 15:25:43.000000 riversand-1.2.3/riversand/calc.py
+-rw-rw-r--   0 user      (1001) user      (1001)    69209 2024-05-12 15:20:42.000000 riversand-1.2.3/riversand/geospatial.py
+-rw-rw-r--   0 user      (1001) user      (1001)     4150 2024-05-10 16:12:46.000000 riversand-1.2.3/riversand/params.py
+-rw-rw-r--   0 user      (1001) user      (1001)    11378 2024-02-28 08:29:04.000000 riversand-1.2.3/riversand/plot.py
+-rw-rw-r--   0 user      (1001) user      (1001)    51868 2024-05-12 15:15:49.000000 riversand-1.2.3/riversand/utils.py
+-rw-rw-r--   0 user      (1001) user      (1001)    16086 2024-05-10 20:13:34.000000 riversand-1.2.3/riversand/xml.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-13 14:35:53.782469 riversand-1.2.3/riversand.egg-info/
+-rw-r--r--   0 user      (1001) user      (1001)     3927 2024-05-13 14:35:53.000000 riversand-1.2.3/riversand.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      350 2024-05-13 14:35:53.000000 riversand-1.2.3/riversand.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2024-05-13 14:35:53.000000 riversand-1.2.3/riversand.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       59 2024-05-13 14:35:53.000000 riversand-1.2.3/riversand.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       10 2024-05-13 14:35:53.000000 riversand-1.2.3/riversand.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2024-05-13 14:35:53.782469 riversand-1.2.3/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     1269 2024-05-13 14:20:13.000000 riversand-1.2.3/setup.py
```

### Comparing `riversand-1.2.2/LICENSE` & `riversand-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `riversand-1.2.2/PKG-INFO` & `riversand-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riversand
-Version: 1.2.2
+Version: 1.2.3
 Summary: Catchmentwide erosion rate calculator
 Home-page: https://github.com/kstueb/riversand
 Author: Konstanze Stuebner
 Author-email: kstueb@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -56,16 +56,16 @@
 Definitely check out the documentation of the online calculator (e.g. [here](http://stoneage.ice-d.org/math/docs/v3/v3_input_explained.html)
 or [here](https://sites.google.com/a/bgc.org/v3docs/)) and the publication
 [Balco et al. (2008)](http://hess.ess.washington.edu/math/docs/al_be_v2/al_be_calc_2007.pdf)
 before using this calculator.
 
 Documentation
 -------------
-- [`quickstart.ipynb`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/quickstart_v20240228.ipynb)
-- [`step_by_step.ipynb`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/step_by_step_v20240228.ipynb)
+- [`quickstart.ipynb`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/quickstart_v1.2.3.ipynb)
+- [`step_by_step.ipynb`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/step_by_step_v1.2.3.ipynb)
 - [`test_data/`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/test_data) : geotiffs of a 35m-resolution digital elevation model, a topographic shielding raster generated with [TopoToolbox](https://topotoolbox.wordpress.com/) and a binary raster indicating quartz-bearing and quartz-free lithologies; shapefiles with catchment outlines; a spreadsheet with sample data. 
 
 Installation
 ------------
 Install riversand by running:
 ```
 $ pip install riversand
```

### Comparing `riversand-1.2.2/README.md` & `riversand-1.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 Definitely check out the documentation of the online calculator (e.g. [here](http://stoneage.ice-d.org/math/docs/v3/v3_input_explained.html)
 or [here](https://sites.google.com/a/bgc.org/v3docs/)) and the publication
 [Balco et al. (2008)](http://hess.ess.washington.edu/math/docs/al_be_v2/al_be_calc_2007.pdf)
 before using this calculator.
 
 Documentation
 -------------
-- [`quickstart.ipynb`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/quickstart_v20240228.ipynb)
-- [`step_by_step.ipynb`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/step_by_step_v20240228.ipynb)
+- [`quickstart.ipynb`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/quickstart_v1.2.3.ipynb)
+- [`step_by_step.ipynb`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/step_by_step_v1.2.3.ipynb)
 - [`test_data/`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/test_data) : geotiffs of a 35m-resolution digital elevation model, a topographic shielding raster generated with [TopoToolbox](https://topotoolbox.wordpress.com/) and a binary raster indicating quartz-bearing and quartz-free lithologies; shapefiles with catchment outlines; a spreadsheet with sample data. 
 
 Installation
 ------------
 Install riversand by running:
 ```
 $ pip install riversand
```

### Comparing `riversand-1.2.2/riversand/calc.py` & `riversand-1.2.3/riversand/calc.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,16 +22,18 @@
 
 *******************************************************************************
 
 General functions:
 - get_textline() : Cast 'sample' and 'topo' data to textstring for the online
     calculator. Input dict ot pd.Series. If possible, missing values are filled
     with default values from params.Params.
-- get_erates_from_server() and get_NofE_from_server : Get pd.DataFrame,
-    diagnosis and version for any string sent to the online calculator.
+    (get_textblock() for point-based ages & erosion rates is part of utils.py)
+- get_ages_from_server(), get_erates_from_server(), get_NofE_from_server() :
+    Get pd.DataFrame, diagnosis and version for any string sent to the
+    online calculator.
 
 Specialized function:
 - get_E() : dict w/ keys 'St', 'Lm', 'LSDn' for a single sample-nuclide pair.
 - get_NofE_FullTable() : Full table of 'NpredXX' for 'topostats' and suite of
     'erates'. Results are weighted by 'wt' ('XX_wt').
 - get_NofE() : Wrapper for _FullTable(): groups data by 'E_cmyr'.
 
@@ -56,45 +58,49 @@
 
 
 def get_textline(sample:pd.Series, topo:pd.Series, shielding) -> str:
     """
     Cast sample and topo data to textstring for the online calculator. Input
     data are validated by utils.validate_*().
 
+    Parameters
+    ----------
     sample : pandas Series or dict
         > sample_data = S.data.iloc[n]
         Missing data are replaced by default values, faulty data raise ValueError.
     topo : pandas Series or dict 
         'lat', 'long', 'elevation' (and 'shielding' if shielding='topo').
         > topo_data = topotable.iloc[n]
         or:
         > summary['elevation'] = summary['elevLo']
         > topo_data = summary
-    shielding : str or numeric
-        'sample', 'topo' or a numeric shielding factor. Defines whether
-        shielding is taken from sample or raster data.
+    shielding : str or float
+        'sample', 'topo' or a numeric shielding factor.
+        Defines whether shielding is taken from sample or raster data.
     
     Returns
     -------
     textline : str
         String corresponding to one location and one set of sample data (Be-10
         or Al-26). Re-standardized nuclide concentrations.
         
     Raises
     ------
-    TypeError : input data format is invalid
-    ValueError : data cannot be validated
+    TypeError
+        Input data format is invalid.
+    ValueError
+        Data cannot be validated.
         
     """
     
     sample = deepcopy(sample)
     topo = deepcopy(topo)
     
     from riversand.utils import validate_topo, validate_nuclide, validate_sample
-    from riversand.utils import restandardize    
+    #from riversand.utils import restandardize_item
         
     if isinstance(sample, pd.DataFrame):
         if len(sample)!=1:
             raise TypeError("get_textline() argument 'sample' must be length 1")
         sample = sample.iloc[0] # recast to pd.Series
             
         if isinstance(sample, pd.Series):
@@ -153,93 +159,240 @@
         except ValueError as e:
             raise e
     else:
         raise ValueError("Invalid shielding: must be 'topo', 'sample' or numeric")
     
     out = {**out1, **out2, **out3}
     
-    out = restandardize(out)
+    #out = restandardize_item(out)
             
     textline = "{} {:.5f} {:.5f} {:.3f} {} {} {} {:.5f} {:.5f} {} ; {} {} {} {} {} {} ;".format(
         out['name'], out['lat'], out['long'], out['elevation'], out['press_flag'],
         out['thickness'], out['density'], out['shielding'], out['erate'], out['year'],
         out['name'], out['nuclide'], out['mineral'], out['N'], out['delN'], out['standardization'])
-    return textline    
+    return textline
+
+
+
+def get_ages_from_server(
+    textblock:str,
+    url:str=None,
+    norm=False
+    ) -> (pd.DataFrame, str, dict):
+    """
+    Get ages in yr from online calculator. Example of usage:
+        
+    > df = pd.read_excel('./folder/file.xlsx')  # read from excel spreadsheet
+    > df = import_data(df)                      # recast for online calculator / validate
+    > textblock = get_textblock(df)
+    > ages, diagnostics, version = get_ages_from_server(textblock)
+    or
+    > ages, diagnostics, version = get_ages_from_server(textblock, norm=True)
+    
+    Parameters
+    ----------
+    textblock : str
+        Any valid string of a single sample or multiple samples.
+    norm : bool
+        If True the results include the normalized values used for plotting. 
+    
+    Returns
+    -------
+    ages : pd.DataFrane
+        Age results; one row per sample and nuclide.
+        Keys are: 'name', 'nuclide',
+            'St_age', 'St_interr', 'St_exterr',
+            'Lm_age', 'Lm_interr', 'Lm_exterr',
+            'LSDn_age', 'LSDn_interr', 'LSDn_exterr',
+    diagnostics : str
+        "No response from {}".format(url)
+        "No diagnostics" as returned by the server
+        "Sample PH-1 -- N10quartz appears to be saturated WRT Stone(2000) SF at this erosion rate."  ...or similar
+        "validate_v2_input.m: Wrong total number of data elements"  ...or similar if the server does not accept the input string
+        "Empty string returned from the server. This may happen if at least one sample has an extremely low nuclide concentration."
+    version :  dict
+        Returned by the server.
+       
+    Raises
+    ------
+    TypeError
+        "'textblock' is empty string"
+        
+    """
+    
+    # rename from xml-string to online output
+    out_cols = {'sample': 'name',
+                'nuclide': 'nuclide',
+                't_St': 'St_age',
+                'delt_int_St': 'St_interr',
+                'delt_ext_St': 'St_exterr',
+                't_Lm': 'Lm_age',
+                'delt_int_Lm': 'Lm_interr',
+                'delt_ext_Lm': 'Lm_exterr',
+                't_LSDn': 'LSDn_age',
+                'delt_int_LSDn': 'LSDn_interr',
+                'delt_ext_LSDn': 'LSDn_exterr',
+                #'Ag_age', 'Ag_interr', 'Ag_exterr'
+                }
+           
+       
+    # additional columns for norm=True:
+    norm_cols = ['Nnorm_St', 'delNnorm_int_St', 'delNnorm_ext_St',
+                 'Nnorm_Lm', 'delNnorm_int_Lm', 'delNnorm_ext_Lm',
+                 'Nnorm_LSDn', 'delNnorm_int_LSDn', 'delNnorm_ext_LSDn']
+    version = {}
+    
+    ages = pd.DataFrame(columns=out_cols.values()) # empty DataFrame if no response from server
+    if norm: ages[norm_cols] = None # append norm columns at end
+    
+    from riversand import xml
+    from riversand.utils import get_textblock
+    
+    if url is None: url = Params.url
+
+    if isinstance(textblock, pd.DataFrame):
+        try:
+            textblock = get_textblock(textblock)
+        except ValueError:
+            raise TypeError("cannot convert input to textblock for online calculator. "+
+                            "Try get_textblock() for details.") from None
+            # This should never happen; get_textblock() uses import_data2() to
+            # validate input and returns an empty string if data is faulty
+
+    if len(textblock.replace(' ',''))==0:
+        raise TypeError("'textblock' is empty string")
+    
+    # request ages from server
+    request_vars = {"mlmfile" : "age_input_v3", #erosion_input_v3
+                    "reportType" : "XML",
+                    "resultType" : "long",
+                    "summary" : "no",
+                    "plotFlag" : "no",
+                    "text_block" : textblock }
+
+    form_data = urllib.parse.urlencode(request_vars).encode('ascii')
+    try:
+        result = urllib.request.urlopen(url, form_data)
+    except urllib.error.URLError:
+        diagnostics = "No response from {}".format(url) ## is this actually a valid return string?
+    else:    
+        result_xml = result.read()
+        ages, diagnostics, version = xml.ages_from_xml(result_xml, norm)
+    
+    ages = ages.rename(columns=out_cols)
+    ages = ages[[c for c in ages if c not in norm_cols] + # keep age columns at beginning
+                [c for c in norm_cols if c in ages]] # move norm columns to end
+    
+    return ages, diagnostics, version
 
 
 
 def get_erates_from_server(
-        textline:str,
+        textblock:str,
         url:str=None
         ) -> (pd.DataFrame, str, dict):
     """
-    Get erosion rates in g/cm2/yr from online calculator.
+    Get erosion rates in g/cm2/yr from online calculator. Example of usage:
     
-    textline : str
-        textline returned by get_textline()
-        > textline = get_textline(sample, topo, shielding='sample')
-        or
-        > out_summary['Elevation'] = out_summary['elevLo']
-        > textline = get_textline(sample, out_summary, shielding='topo')
-        May also be any valid textblock of multiple samples / nuclide / erates.
+    > df = pd.read_excel('./folder/file.xlsx')  # read from excel spreadsheet
+    > df = import_data(df)                      # recast for online calculator / validate
+    > textblock = get_textblock(df)
+    > erates, diagnostics, version = get_erates_from_server(textblock)
+    
+    Parameters
+    ----------
+    textblock : str
+        Any valid string of a single sample or multiple samples.
         
     Returns
     -------
-    dfE : pd.DataFrame
-        erosion rate results; one row per sample and nuclide.
-        keys are: 'name', 'nuclide', 'density',
+    erates : pd.DataFrame
+        Erosion rate results; one row per sample and nuclide.
+        Keys are: 'name', 'nuclide', 'density',
                   'E_St', 'delE_int_St', 'delE_ext_St',
                   'E_Lm', 'delE_int_Lm', 'delE_ext_Lm',
                   'E_LSDn', 'delE_int_LSDn', 'delE_ext_LSDn' 
     diagnostics : str
         "No response from {}".format(url)
         "No diagnostics" as returned by the server
+        "Sample PH-1 -- N10quartz appears to be saturated WRT Stone(2000) SF at this erosion rate."  ...or similar
+        "validate_v2_input.m: Wrong total number of data elements"  ...or similar if the server does not accept the input string
+        "Empty string returned from the server. This may happen if at least one sample has an extremely low nuclide concentration."
     version : dict
-        returned by the server.
+        Returned by the server.
+        
+    Raises
+    ------
+    TypeError
+        "'textblock' is empty string"
         
     """
     
-    dfE = pd.DataFrame(columns=['name', 'nuclide', 'density',
-              'E_St', 'delE_int_St', 'delE_ext_St',
-              'E_Lm', 'delE_int_Lm', 'delE_ext_Lm',
-              'E_LSDn', 'delE_int_LSDn', 'delE_ext_LSDn'])
+    # rename from xml-string to online output
+    out_cols = {'sample': 'name',
+                'nuclide': 'nuclide',
+                'density': 'density',
+                'E_gcm2_St': 'E_St',
+                'delE_int_gcm2_St': 'delE_int_St',
+                'delE_ext_gcm2_St': 'delE_ext_St',
+                'E_gcm2_Lm': 'E_Lm',
+                'delE_int_gcm2_Lm': 'delE_int_Lm',
+                'delE_ext_gcm2_Lm': 'delE_ext_Lm',
+                'E_gcm2_LSDn': 'E_LSDn',
+                'delE_int_gcm2_LSDn': 'delE_int_LSDn',
+                'delE_ext_gcm2_LSDn': 'delE_ext_LSDn'}
     version = {}
     
-    from riversand import xml
+    erates = pd.DataFrame(columns=out_cols.values()) # empty DataFrame if no response from server
     
+    from riversand import xml
+    from riversand.utils import get_textblock
+
     if url is None: url = Params.url
         
-    if not isinstance(textline, str):
-        raise TypeError("get_erates_from_server() 'textline' must be string")
-    if len(textline)==0:
-        raise TypeError("'textline' empty string")
-        
+    if isinstance(textblock, pd.DataFrame):
+        try:
+            textblock = get_textblock(textblock)
+        except ValueError:
+            raise TypeError("cannot convert input to textblock for online calculator. "+
+                            "Try get_textblock() for details.") from None
+            # This should never happen; get_textblock() uses import_data2() to
+            # validate input and returns an empty string if data is faulty
+            
+    if len(textblock.replace(' ',''))==0:
+        raise TypeError("'textblock' is empty string")
+    
+    
     # request erosion rate from server
     request_vars = {"mlmfile" : "erosion_input_v3",
                     "reportType" : "XML",
                     "resultType" : "long",
                     "summary" : "no",
                     "plotFlag" : "no",
-                    "text_block" : textline }
+                    "text_block" : textblock }
+    
     form_data = urllib.parse.urlencode(request_vars).encode('ascii')
     try:        
         result = urllib.request.urlopen(url, form_data)
     except urllib.error.URLError:
         diagnostics = "No response from {}".format(url)
     else:    
         result_xml = result.read()
-        dfE, diagnostics, version = xml.read_erates(result_xml)
+        erates, diagnostics, version = xml.erates_from_xml(result_xml)
     
-    return dfE, diagnostics, version
+    erates = erates.rename(columns=out_cols)
+    
+    return erates, diagnostics, version
     
 
 def get_E(textline:str, url:str=None) -> dict:
     """
-    Get erosion rates in cm/yr from online calculator for a 
-    *single* sample and nuclide.
+    Get erosion rates in cm/yr from online calculator for
+    a SINGLE sample and nuclide.
+    
 
     Returns
     -------
     ret_dict : dict
         keys 'St', 'Lm', 'LSDn'; erosion rate in cm/yr
     
     Raises RuntimeError if diagnostics is anything but "No diagnostics". 
@@ -285,28 +438,30 @@
         textline:str,
         url:str=None
         ) -> (pd.DataFrame, str, dict):
     """
     Get predicted nuclide concentrations in at/g from online calculator.
     Note that result is independent of nuclide concentration and standardization.
     
+    Parameters
+    ----------
     textline : str
-        any valid textblock of multiple samples / nuclide / erates.
+        Any valid textblock of multiple samples / nuclide / erates.
         
     Returns
     -------
     dfN : pd.DataFrame
-        nuclide concentration results; one row per sample and nuclide.
-        keys are: 'name', 'nuclide', 'E_cmyr',
+        Nuclide concentration results; one row per sample and nuclide.
+        Keys are: 'name', 'nuclide', 'E_cmyr',
                   'NpredSt', 'NpredLm', 'NpredLSDn' 
     diagnostics : str
         "No response from {}".format(url)
         "No diagnostics" as returned by the server
     version : dict
-        returned by the server.
+        Returned by the server.
         
     """
     
     dfN = pd.DataFrame(columns = ['name', 'nuclide', 'E_cmyr',
                                   'NpredSt', 'NpredLm', 'NpredLSDn'])
     version = {}
     
@@ -325,15 +480,15 @@
     
     try:        
         result = urllib.request.urlopen(url, form_data)
     except urllib.error.URLError:
         diagnostics = "No response from {}".format(url)
     else:    
         result_xml = result.read() # extract result
-        dfN, diagnostics, version = xml.read_NofE(result_xml)
+        dfN, diagnostics, version = xml.NofE_from_xml(result_xml)
     
     return dfN, diagnostics, version
     
     
     
 def get_NofE_FullTable(
         sample_data:pd.Series,
@@ -345,34 +500,45 @@
     """
     Get predicted nuclide concentrations for given topographic statistics
     for a single sample and a suite of erates.
     - lat, long, elevation from topostats
     - N, delN, press_flag, density, etc. from sample_data
     Sample names are auto-generated (one for each topostats entry).
     Sample thickness is 0.
-    Note that result is independent of nuclide concentration and standardization.
+    Note that result is independent of nuclide concentration and standardization
+    specified in 'sample_data'.
 
     Parameters
     ----------
-    sample_data : pd.Series or dict; single sample.
-    topostats : pd.DataFrame; elevation-binned topo data.
-    shielding : 'topo', 'sample' or numeric.
-    erates : iterable or numeric.
+    sample_data : pd.Series or dict
+        Single sample.
+    topostats : pd.DataFrame
+        Elevation-binned topo data.
+    shielding : str or float
+        'topo', 'sample' or numeric.
+    erates : iterable or float.
+        (Suite of) erosion rates in cm/yr.
     
     Returns
     ----------
     dfA : pd.DataFrame
-        full table of nuclide predictions for each elevation bin and each erate
-        keys are: 'name', 'nuclide', 'E_cmyr',
+        Full table of nuclide predictions for each elevation bin and each erate
+        Keys are: 'name', 'nuclide', 'E_cmyr',
                   'NpredSt', 'NpredLm', 'NpredLSDn', # at/g as returned by the server
                   'St_wt', 'Lm_wt', 'LSDn_wt'        # at/g weighted by topostats['wt']
     diagnostics : str
     version : dict
-        returned from the server.
+        Returned from the server.
         
+    Raises
+    -----
+    ValueError
+        "Cannot get valid input for the online calculator:..."
+        "Missing column 'wt' in topostats"
+    
     """
     
     if url is None: url = Params.url
     
     if isinstance(erates, Number):
         erates = [erates]
     
@@ -393,31 +559,35 @@
         topostats = temp
         
     if isinstance(topostats, pd.Series): # e.g. if a single row of topostats is passed 
         temp = pd.DataFrame(data=[topostats])
         if 'wt' not in temp.keys():
             temp['wt'] = 1.
         topostats = temp
-        
+    
+    if 'wt' not in topostats.columns:
+        raise ValueError("Missing column 'wt' in topostats")
+                         
     # create text_block from all erates and all topotable entries
     tempS = deepcopy(sample_data)
     newline = '.'
     text_block = ''
     for e, erate in enumerate(erates):
         for i, tempT in topostats.iterrows():
             name_str = ("B_{}_{}".format(i,e))
             tempS['name'] = name_str
             tempS['erate'] = erate
             try:
                 newline = get_textline(tempS,
                                        tempT, #topostats.iloc[i],
                                        shielding=shielding)
-            except ValueError as e:
+            except (ValueError, TypeError) as e:
                 raise ValueError("Cannot get valid input for the online calculator:\n   "+
-                                 str(e))
+                                 str(e)) from None
+                
             text_block = text_block + newline + ' '
 
     dfA, diagnostics, version = get_NofE_from_server(text_block, url=url)
     
     # apply weighting factor 'wt' to calculate 'St', 'Lm', 'LSDn'
     if len(dfA)>0:
         # generate a column 'topo' in order to map the weights from dfT.wt to the samples
@@ -442,32 +612,44 @@
         erates:np.ndarray,
         url:str=None
     ) -> pd.DataFrame:
     """
     Wrapper for get_NofE_FullTable:
     Predicted nuclide concentrations for a given catchment topography
     for a single sample and a suite of erosion rates.
-    Note that result is independent of nuclide concentration and standardization.
+    Note that predicted nuclide conc. are valid for standardization with CF=1
+    and can be converted to other standardizations if necessary (the output of
+    this function is independent of nuclide concentration and standardization
+    specified in 'sample_data').
     
     Parameters
     ----------
-    sample_data : pd.Series or dict; single sample.
-    topostats : pd.DataFrame; elevation-binned topo data.
-    shielding : 'topo', 'sample' or numeric.
-    erates : iterable or scalar; (suite of) erosion rates in cm/yr.
+    sample_data : pd.Series or dict
+        Single sample.
+    topostats : pd.DataFrame
+        Elevation-binned topo data.
+    shielding : str or float
+        'topo', 'sample' or numeric.
+    erates : iterable or float
+        (Suite of) erosion rates in cm/yr.
     
     Returns
     ----------
     NofE : pd.DataFrame
         Predicted nuclide concentrations for each erosion rate in erates
         and each scaling method
-        keys are : 'St', 'Lm', 'LSDn'
-        index name is 'E_cmyr'.
+        Keys are : 'St', 'Lm', 'LSDn'
+        Index name is 'E_cmyr'.
     
-    Raises RuntimeError if diagnostics is anything but "No diagnostics".
+    Raises
+    ------
+    ValueError
+        Missing or faulty input data
+    RuntimeError
+        Diagnostics is anything but "No diagnostics".
         
     """
         
     from riversand.utils import validate_topo, validate_nuclide, validate_sample
 
     if not isinstance(topostats, pd.DataFrame):
         raise TypeError("get_NofE() argument 'topostats' must be pandas DataFrame")
@@ -480,33 +662,35 @@
         raise TypeError("get_NofE() argument 'sample_data' must be dict, "+
                         "pandas Series or single-row pandas Dataframe")
     
     # validate sample_data and a line of topodata to avoid Exceptions raised by
     # get_NofE_FullTable() (ValueError "Cannot get valid input...")
     try:
         _ = validate_topo(topostats.iloc[0])
-    except:
-        raise ValueError("Invalid values in 'topostats' or empty table")
+    except ValueError:
+        raise ValueError("Invalid values in 'topostats'") from None
+    except IndexError:
+        raise ValueError("Empty table 'topostats'") from None
     try:
         _ = validate_sample(sample_data)
-    except:
-        raise ValueError("Invalid values in 'sample_data'")
+    except ValueError:
+        raise ValueError("Invalid values in 'sample_data'") from None
     try:
         _ = validate_nuclide(sample_data)
-    except:
-        raise ValueError("Invalid values in 'sample_data'")
+    except ValueError:
+        raise ValueError("Invalid values in 'sample_data'") from None
     
     if (shielding=='topo') and ('shielding' not in topostats.keys()):
         raise ValueError("shielding='topo' but no shielding factor defined in 'topostats'")
             
     if (shielding=='sample'):
         try:
             _ = validate_sample(sample_data, shielding=True)
-        except:
-            raise ValueError("shielding='sample' but no shielding factor defined in 'sample_data'")
+        except ValueError:
+            raise ValueError("shielding='sample' but no shielding factor defined in 'sample_data'") from None
          
     dfA, diagnostics, version = get_NofE_FullTable(
         sample_data, topostats, shielding, erates, url=url)
     
     # saturated samples or low nuclide concentration are never an issue with NofE:
     if "No response from" in diagnostics:
         raise RuntimeError("get_NofE() : {}".format(diagnostics))
@@ -529,64 +713,74 @@
         NofE = temp.set_index('E_cmyr')
     return NofE
 
 
 def guess_erates(*args, **kwargs) -> np.ndarray:
     """
     Generate a suite of initial erosion rates in cm/yr.
-
-    One positional argument : erates = 0.5*E ... 2*E
-    Two positional arguments : erates = E1 ... E2
-    Positional arguments can be dict of erosion rates with keys 'St', 'Lm',
-        'LSDn' if 'scaling' is specified as keyword argument.        
+    
+    One positional argument yields erosion rates ranging from 0.5*E to 2*E
+    > guess_erates(0.001, N=10)
+    
+    Two positional arguments yields erosion rates ranging from E1 to E2
+    > guess_erates(0.001, 0.003, N=5)
+    
+    Positional arguments can also be a dict of erosion rates with keys
+        'St', 'Lm', 'LSDn' if 'scaling' is specified as keyword argument.        
+    
     'N' defines the number of output erosion rates; defaults to N=6
 
+    Raises
+    ------
+    KeyError
+    
     """
     
     if 'N' in kwargs.keys(): N = kwargs['N']
     else: N = 6
 
     if 'scaling' in kwargs.keys(): scaling = kwargs['scaling']
-    else: scaling = None
+    else: scaling = 'St'
             
     if len(args)==2:
         E1 = args[0]
         E2 = args[1]
         
         if isinstance(E1, Number) and isinstance(E2, Number):
             pass
         elif isinstance(E1, dict) and isinstance(E2, dict):
             try:
                 E1 = E1[scaling]
                 E2 = E2[scaling]
-            except:
-                raise ValueError("guess_erates() invalid keyword argument "+
-                                 "scaling '{}'"
-                                 .format(scaling))
+            except KeyError as e:
+                raise e
+                #ValueError("guess_erates() invalid keyword argument "+
+                #"scaling='{}'".format(scaling))
         else:
-            raise ValueError("guess_erates() invalid arguments")
+            raise KeyError("guess_erates() invalid arguments")
        
     elif len(args)==1:
         E = args[0]
         
         if isinstance(E, Number):
             pass
         elif isinstance(E, dict):
             try:
                 E = E[scaling]
-            except:
-                raise ValueError("guess_erates() invalid keyword argument "+
-                                 "scaling '{}'"
-                                 .format(scaling))
+            except KeyError as e:
+                raise e
+                #ValueError("guess_erates() invalid keyword argument "+
+                #                 "scaling '{}'"
+                #                 .format(scaling))
         else:
-            raise ValueError("guess_erates() invalid arguments")
+            raise KeyError("guess_erates() invalid arguments")
         E1 = E/2
         E2 = 2*E
     else:
-        raise ValueError("guess_erates() invalid arguments")
+        raise KeyError("guess_erates() invalid arguments")
         
     minE = min(E1, E2)
     maxE = max(E1, E2)
     
     minE = np.log(max([minE, 0.001*maxE]))
     maxE = np.log(maxE)
     return np.exp(np.linspace(minE, maxE, int(N))) # cm/yr
@@ -602,34 +796,45 @@
         shielding:str,
         erates:np.ndarray,
         scaling:str,
         url:str=None,
         strict=True
     ) -> (Number, tuple, pd.DataFrame, list):
     """
-    Calculate catchmentwide erosion rate E and uncertainty delE for a single
-    sample based on 'topostats' and a suite of initial erosion rates.
+    Calculate catchmentwide erosion rate E and uncertainty delE in cm/yr for a
+    single sample based on 'topostats' and a suite of initial erosion rates.
     
-    sample_data : pd.Series or dict; single sample.
-    topostats : pd.DataFrame; elevation-binned topo data.
-    shielding : 'topo', 'sample' or numeric.
-    erates : iterable or scalar; (suite of) erosion rates in cm/yr.
-    scaling : str; scaling method 'St', 'Lm' or 'LSDn'.
+    Parameters
+    ----------
+    sample_data : pd.Series or dict
+        Single sample. Will be restandardized.
+    topostats : pd.DataFrame
+        Elevation-binned topo data.
+    shielding : str or float
+        'topo', 'sample' or numeric.
+    erates : iterable or scalar
+        (Suite of) erosion rates in cm/yr.
+    scaling : str
+        Scaling method 'St', 'Lm' or 'LSDn'.
     
     Returns
     ----------
-    E : float; erosion rate in cm/yr.
-    delE : tuple of floats, uncertainty (-delE, +delE).
-    NofE : pd.Series with keys defined by 'scaling' and index 'E_cmyr'.
-    error : list or error strings. In case of 'minE too high' or 'maxE too low'
-        the list has only this error!
+    E : float
+        Erosion rate in cm/yr.
+    delE : tuple of floats
+        Uncertainty (-delE, +delE).
+    NofE : pd.Series
+        Keys are defined by 'scaling' and index 'E_cmyr'.
+    error : list of error strings.
+        In case of 'minE too high' or 'maxE too low' the list shows only this error.
     
     """
 
-    from riversand.utils import restandardize
+    #from riversand.utils import restandardize_item
+    from riversand import utils
     if url is None: url = Params.url
     
     if scaling not in Params._scalingmethods:
         raise ValueError("Invalid scaling '{}' (must be 'St', 'Lm' or 'LSDn')")
     # other requirements are validated by get_NofE() and raised as TypeError or ValueError
     
     if isinstance(erates, Number):
@@ -645,19 +850,23 @@
     E_poly = np.nan
     delE = (np.nan, np.nan)
     
     error = []
     
     erates[:] = np.sort(erates)
     
-    if isinstance(sample_data, (pd.DataFrame)) and len(sample_data)>0:
+    if isinstance(sample_data, pd.DataFrame):
         raise TypeError("poly_E_results() : 'sample_data' must be dict or pandas Series")
         
-    sample_data = restandardize(sample_data)
-    
+    #restandardize any dict or pd.Series with columns N, delN, nuclide, standardization
+    try:
+        sample_data = utils.restandardize(pd.DataFrame([sample_data])).iloc[0]
+    except KeyError: # "restandardize() needs columns 'N', ...."
+        raise ValueError("invalid sample data")
+        
     try:
         NofE = get_NofE(sample_data, topostats, shielding, erates, url=url)
     except TypeError as e: # input data format
         raise e
     except ValueError as e: # input data
         raise e
     except RuntimeError as e: # no server response
```

### Comparing `riversand-1.2.2/riversand/geospatial.py` & `riversand-1.2.3/riversand/geospatial.py`

 * *Files 12% similar despite different names*

```diff
@@ -87,14 +87,27 @@
     except:# rasterio.RasterioIOError as error:
         pass
     
     return src
 
 
 class Raster():
+    """
+    Elevation, shielding or lithology raster dataset.
+    
+    Attributes are:
+    - self.fname: file name
+    - self.src: source (closed DatasetReader)
+    - self.crs: coordinate reference system
+    - self.epsg: epsg code
+    - self.res: resolution (tuple)
+    - self.dtype: type ('elevation', 'shielding' or 'quartz')
+    
+    """
+    
     dtypes = ('elevation', 'shielding', 'quartz') # valid Raster types
     
     def __init__(self, fname:str, dtype:str):
         
         dtype = dtype.lower()
         if dtype not in self.dtypes:
             raise TypeError("Invalid Raster dtype '{}' (must be 'elevation', 'shielding' or 'quartz')".format(dtype))
@@ -154,14 +167,26 @@
     except fiona.errors.DriverError as e:
         print(e)
             
     return src
 
 
 class Catchment():
+    """
+    Attributes are:
+    - self.fname: file name
+    - self.src: source (closed Collection)
+    - self.crs: coordinate reference system
+    - self.epsg: epsg code
+    - self.attrs: list of shapefile attribute fields
+    - self.cid: attribute field used to match samples to catchments
+    - self.catchments: list of catchment polygons (fiona.model.Feature)
+    - self.len: number of catchment polygons in shapefile
+    
+    """
     
     def __init__(self, fname:str):
         
         if not isinstance(fname, str):
             raise TypeError("Invalid Catchment fname (must be string)")
         
         src = get_shapefile(fname) # closed fiona.collection
@@ -203,15 +228,23 @@
                      self.crs])
 
         else:
             raise IOError("Cannot read shapefile {}".format(fname))
         
         
     def set_cid(self, cid:str='id'):
-        """ Set Catchment.cid (fyi only, Riversand.cid is relevant) """
+        """
+        Set Catchment.cid (fyi only, Riversand.cid is relevant).
+        
+        Parameters
+        ----------
+        cid : str
+            Shapefile attribute field used for catchment names.
+            
+        """
         
         if cid is None:
             self.cid = None
         else:
             if self.attrs is None:
                 print("ValueError : Invalid cid='{}';\n".format(cid) +
                       "   shapefile has no attribute fields")
@@ -225,14 +258,19 @@
 
 
     def get_names(self, cid:str=None) -> list:
         """
         Get sorted list of all catchment names from attribute field 'cid'.
         Duplicates are included, missing values are shown as 'None'.
         
+        Parameters
+        ----------
+        cid : str
+            Shapefile attribute field used for catchment names.
+            
         """
         
         if cid is None:
             cid = self.cid
         if cid is None:
             print("ValueError : use .set_cid() to set catchment identifier")
             return None
@@ -251,14 +289,19 @@
         return c_names
         
     def get_valid_names(self, cid:str) -> list:
         """
         Get a sorted list of valid catchment names from attribute field 'cid'.
         Duplicates and missing values are excluded.
         
+        Parameters
+        ----------
+        cid : str
+            Shapefile attribute field used for catchment names.
+        
         """
         
         c_names = self.get_names(cid) # returns None for invalid cid
         if c_names is None:
             print("ValueError : use .set_cid() to set catchment identifier")
         else:
             c_invalid = [itm for itm, cnt in collections.Counter(c_names).items() if cnt>1] # non-unique
@@ -291,29 +334,34 @@
 # =============================================================================
 # Riversand object
 # =============================================================================
  
 
 class Riversand():
     """
-    A Riversand object contains all the data needed to calculate catchmentwide
-    erosion rates. Methods:
+    A 'Riversand' object contains all the data needed to calculate
+    catchmentwide erosion rates. Methods are:
     
-    .add_rasters()  # add Raster objects (.elevation, .shielding, .quartz)
-    .add_catchments()  # add Catchment object (.catchments)
-    .add_samples()  # add sample data (.samples)
+    self.set_path_to_data() # define path to input data
+    self.add_raster()  # add Raster objects (elevation, shielding, quartz)
+    self.add_catchments()  # add Catchment object (catchments)
+    self.add_samples()  # add sample data (samples)
  
-    .validate()   # validate projection and resolution of the geospatial data
-        (.res, .crs, .epsg.)
+    self.validate()   # validate projection and resolution of geospatial data
+        (res, crs, epsg.)
+        
+    self.process_single_catchment()  # calculate erosion rate for a single catchment
+    self.process_multi_catchment()  # calculate erosion rates for a shapefile with
+        multiple catchments (use self.set_cid() to set the shapefile attribute
+        to be used as catchment name)
+        
+    self.catchment_stats()  # calculate some catchment statistics
+    self.restandardize()  # convert nuclide concentrations to defaults
+        Be-10: 07KNSTD; Al-26: KNSTD
         
-    .process_single_catchment()  # calculate erosion rate for a single catchment
-    .process_multi_catchment()  # calculate erosion rates for a shapefile with
-        multiple catchments (use .set_cid() to set the shapefile attribute to
-        be used as catchment name)
-    
     """
     
 
     
     def __init__(self, path:str=None):
         self.path_to_data = None
         self.elevation = None # Raster object
@@ -521,15 +569,15 @@
             except IOError as e:
                 if e.errno==2:
                     raise FileNotFoundError("{}: No such file or directory"
                                             .format(e.filename))
                 else:
                     raise e
             else:
-                df = xls.parse(0)
+                df = xls.parse(0) # imports the first sheet no matter the name
     
         for c in df.columns:
             c_new = c.strip(' \n\t')
             df.rename(columns={c: c_new}, inplace=True)
         
         if df.empty:
             raise ValueError("No sample data in file")
@@ -609,15 +657,16 @@
         if errS:
             raise ValueError(errS[0]) # e.g. 'Invalid / missing data in line(s): 6, 7'
     
     
     def add_samples_from_dict(self, data:dict, add:bool=False):
         """
         Write sample data from dict or pd.Series to self.samples.
-        Colunms sorted as in Params.all_keys with topo and other info at the end of the table.
+        Colunms sorted as in Params.all_keys with topo and other info at the
+        end of the table.
         
         """
         
         from riversand.utils import validate_nuclide, validate_sample
                         
         if not isinstance(data, (dict, pd.Series)):
             raise TypeError("add_samples_from_dict() 'data' must be dictionary")
@@ -661,67 +710,48 @@
                                   columns=mandatory_keys+other_keys,
                                   index=[len(self.samples)])
                 self.samples = (pd.concat([df, self.samples])
                                 .sort_index().reset_index(drop=True))        
                 
             self.valid_catchments = None # set by self.validate()
         
-    def restandardize(self):
+    def restandardize(self, verbose=True):
         """
-        Restandardize Riversand.samples to the default standardizations.
+        Convert self.samples to Be-10: 07KNSTD; Al-26: KNSTD.
         Requires columns 'nuclide', 'standardization', 'N', 'delN'.
+        
+        Note that utils.restandardize() is not caught up by samples with
+        invalid standardization and/or N=0; it sets 'N'='delN'='standardization'
+        to NaN). self.validate() will call out these problems.
 
         """
+        from riversand import utils
+        
         if self.samples is None:
             raise ValueError("No samples defined, use .add_samples() before re-standardizing")
-            
-        df = deepcopy(self.samples)
-        try:
-            df['_N'], df['_delN'], df['_standardization'] = df['N'], df['delN'], df['standardization']
-            _ = df['nuclide']
-        except KeyError as e:
-            raise ValueError("restandardize() missing mandarory column '{}'".format(e.args[0]))
-        
-        if not (is_numeric_dtype(df['N']) and is_numeric_dtype(df['delN'])):
-            raise ValueError("Invalid input data; use .validate() before re-standardizing")
-                
-        df['N'], df['delN'], df['standardization'] = np.nan, np.nan, np.nan
-        
-        nucls = ['Be-10', 'Al-26']
-        stdss = [pd.Series(Params.Be_stds), pd.Series(Params.Al_stds)]
-        for nu, st in zip(nucls, stdss): 
-            sel = df['nuclide']==nu
-            
-            df.loc[sel, 'N'] = (
-                df.loc[sel,'_standardization'].map(st)
-                * df.loc[sel,'_N']
-                )
-            df.loc[sel, 'delN'] = (
-                df.loc[sel,'_standardization'].map(st)
-                * df.loc[sel,'_delN']
-                )
-            df.loc[sel*df['N'].notnull(), 'standardization'] = (
-                Params._default_standards[nu]
-                )
-        self.samples = df
-        print("Re-standardized sample data. Original data are stored in columns '_N', '_delN', '_standardization'.")
+        
+        self.samples = utils.restandardize(self.samples)
+        #raises KeyError if N, delN, nuclide, standardization are missing; this should never happen for self.samples
+        if verbose:
+            print("Nuclide data converted to default standardizations Be-10: {}; Al-26: {}."
+                  .format(Params._default_standards['Be-10'],
+                          Params._default_standards['Al-26']))
+        
+        
     
     def get_valid_catchments(self):
         self.validate(verbose=False)
         if self.valid_catchments is None:
             return []
         else:
             return self.valid_catchments
     
         
     def validate(self, multi:bool=None, verbose=True):
-        """
-        Validate Riversand object and print error report.
-                 
-        """
+        """ Validate Riversand object and print error report. """
         
         from riversand.utils import validate_topo, validate_nuclide, validate_sample
         from riversand.utils import feature_in_raster
 
         class ValidationError(Exception):
             pass
         
@@ -922,34 +952,42 @@
         
     
     def process_single_catchment(self,
             bins=500, scaling='LSDn', shielding=1, unit='mm/yr',
             plot=None,
             url=None, verbose=True) -> pd.DataFrame:
         """
-        Calculate catchmentwide erosion rates for a single-catchment shapefile.
+        Calculate catchmentwide erosion rates in cm/yr for a single-catchment
+        shapefile. Nuclide concentrations in self.samples are restandardized.
 
         Parameters
         ----------
-        bins : numeric, optional
-            bin size in meters for elevation binning. The default is 500.
+        bins : float, optional
+            Bin size in metres for elevation binning. The default is 500.
         scaling : str, optional
-            scaling method 'St', 'Lm' or 'LSDn'. The default is 'LSDn'.
-        shielding : str or numeric, optional
-            shielding method, 'sample', 'topo' or numeric (0 to 1).
+            Scaling method 'St', 'Lm' or 'LSDn'. The default is 'LSDn'.
+        shielding : str or float, optional
+            Shielding method, 'sample', 'topo' or numeric (0 to 1).
             The default is 1.
         unit : str, optional
-            unit for plotting. The default is 'mm/yr'.
+            Unit for plotting. The default is 'mm/yr'.
         plot : str, optional
-            flag for saving plots, 'jpg' or 'png'. The default is None.
+            Flag for saving plots, 'jpg' or 'png'. The default is None.
 
         Returns
         -------
         results : pd.DataFrame
             Table of results for each sample.
+            
+        Raises
+        ------
+        ValueError
+            self.elevation, self.catchments or self.samples are not defined.
+            More than one polygon in self.catchments.
+            Invalid argument 'shielding' or 'unit'.
 
         """
         
         if url is None: url = Params.url
             
         #from riversand.utils import validate_topo, validate_nuclide, validate_sample
         from riversand.utils import eliminate_quartzfree, get_topostats
@@ -1042,14 +1080,18 @@
                 _ = get_textline(self.samples.iloc[0],
                                  summary,
                                  shielding=shielding)
             except ValueError as e: # raised by get_textline() for invalid shielding
                 print(type(e).__name__, ":", e.args[0])
                 return results
                 
+            self.restandardize(verbose=False)
+            # modifies self.samples to restandardized values
+            # in either case poly_E_results() uses restandardized values for calculation but does not touch self.samples
+            
             for idx, sample_data in self.samples.iterrows(): # sample_data as pd.Series
                 
                 E = np.nan
                 delE = (np.nan, np.nan)
                 NRMSE = np.nan
             
                 # sample name from input or default value
@@ -1151,35 +1193,42 @@
     
         
     def process_multi_catchment(self,
             bins=500, scaling='LSDn', shielding=1, unit='mm/yr',
             plot=None,
             url=None, verbose=True) -> pd.DataFrame:
         """
-        Calculate catchmentwide erosion rates for a multi-catchment shapefile.
+        Calculate catchmentwide erosion rates in cm/yr for a multi-catchment
+        shapefile. Nuclide concentrations in self.samples are restandardized.
         
         Parameters
         ----------
-        bins : numeric, optional
-            bin size in meters for elevation binning. The default is 500.
+        bins : float, optional
+            Bin size in meters for elevation binning. The default is 500.
         scaling : str, optional
-            scaling method 'St', 'Lm' or 'LSDn'. The default is 'LSDn'.
+            Scaling method 'St', 'Lm' or 'LSDn'. The default is 'LSDn'.
         shielding : str or numeric, optional
-            shielding method, 'sample', 'topo' or numeric (0 to 1).
+            Shielding method, 'sample', 'topo' or numeric (0 to 1).
             The default is 1.
         unit : str, optional
-            unit for plotting. The default is 'mm/yr'.
+            Unit for plotting. The default is 'mm/yr'.
         plot : str, optional
-            flag for saving plots, 'jpg' or 'png'. The default is None.
+            Flag for saving plots, 'jpg' or 'png'. The default is None.
     
         Returns
         -------
         results : pd.DataFrame
             Table of results for each sample.
             
+        Raises
+        ------
+        ValueError
+            self.elevation, self.catchments or self.samples are not defined.
+            Invalid argument 'shielding' or 'unit'.
+            
         """
         
         if url is None: url = Params.url
             
         #from riversand.utils import validate_topo, validate_nuclide, validate_sample
         from riversand.utils import eliminate_quartzfree, get_topostats
         from riversand.calc import get_textline, get_E, guess_erates
@@ -1248,14 +1297,17 @@
         Nf = max([len(l) for l in self.samples['name'].values]) # fill length for sample name
         Ef = 26 # fill length for erosion rate result        
         order_str = "{: >"+str(If)+"} {: <"+str(Nf)+"} : "
         #order_str_E2 = "{: >"+str(If)+"} {: <"+str(Nf)+"} : {: >"+str(Ef)+"}"  # erosion rate result
         order_str_F1 = "{: >"+str(If)+"} {: <"+str(Nf)+"} : "  # erosion rate result
         #order_str_F2 = "{: >"+str(If)+"} {: <"+str(Nf)+"} : {}"  # erosion rate result
 
+        self.restandardize(verbose=False)
+        # modifies self.samples to restandardized values
+        # in either case poly_E_results() uses restandardized values for calculation but does not touch self.samples
         
         for idx, sample_data in self.samples.iterrows(): # iterate over all samples
         
             Qpc = 0 # quartz-free lithology removed; default value
             E = np.nan
             delE = (np.nan, np.nan)
             NRMSE = np.nan
@@ -1310,15 +1362,15 @@
                         textline = get_textline(sample_data, summary, shielding=shielding)
                         E_Hi = get_E(textline) # erosion rates in cm/yr
                     except ValueError as e: # raised by get_textline() for invalid shielding
                         print(type(e).__name__, ":", e.args[0])
                         err = [e.args[0]]
                     
                     except RuntimeError as e: # raised by get_E()
-                        error_code = e.args[0][10:]
+                        error_code = e.args[0][10:] # e.g. "get_E() : sample appears to be saturated"
                     else:
             
                         # generate suitable erates
                         erates = guess_erates(E_Lo, E_Hi, scaling=scaling) # cm/yr
                         E, delE, NofE, err = (
                             poly_E_results(sample_data, topostats, 
                             shielding=shielding, erates=erates, scaling=scaling, url=url))
@@ -1410,15 +1462,27 @@
     def catchment_stats(self, verbose=True) -> pd.DataFrame:
         """
         Calculate topo statistics for all catchments in shapefile.
     
         Returns
         -------
         results : pd.DataFrame
-            Table of results for each catchment.
+            Table of results for each catchment. Keys are:
+            - centr_lat, centr_long : centroid coordinates (in WGS84)
+            - mean_elev, stdev_elev : mean and standard deviation of catchment elevations
+            - relief : difference betweem highesta and lowest elevation
+            - area : catchment area in km2 assuming geotiff resolution in metres!
+            - mean_sf : mean shielding factor
+            - qtz_pc : percent area of catchment that contributes quartz
+            - error : "catchment out of bounds" if not within bounds of geotiff
+            
+        Raises
+        ------
+        ValueError
+            self.elevation, self.catchments or self.samples are not defined.
             
         """
         
         from riversand.utils import eliminate_quartzfree, get_topostats
         from riversand.utils import projected_xy_to_longlat, get_xarray_centroid
         
         if self.elevation is None:
@@ -1453,18 +1517,20 @@
                 end = ", "
                 
             try:
                 clips = self.clip_all_rasters(idx) # function calls rv.validate()
             except ValueError as e:
                 results.loc[idx, 'error'] = 'catchment out of bounds'
             else:
+                results.loc[idx, 'error'] = ''
                 if 'quartz' in clips.keys():
                     clips, Qpc = eliminate_quartzfree(clips, verbose=False, Qpc=True)
                     results.loc[idx, 'qtz_pc'] = np.round(100-Qpc,1)
-                
+                else:
+                    results.loc[idx, 'qtz_pc'] = 100.
                 (cx, cy) = projected_xy_to_longlat(get_xarray_centroid(
                                 clips['elevation']),
                                 clips['epsg']
                                 )
                 
                 area_per_pixel = float(
                     np.abs(clips['elevation'].transform[0] * 
@@ -1519,15 +1585,15 @@
             
         if not self.catchments is None:
             s += ["---------------"]
             s += ["Catchment polygons:\n"]
             s += [str(self.catchments)+"\n"]
             
         if self.epsg or self.res:
-            s += ["---------------"]
+            s += ["==============="]
             s += ["Validated projection:"]
             if self.epsg:
                 s += ["epsg  : {}".format(self.epsg)]
             if self.res:
                 s += ["res   : {}".format(self.res)]
             s += [""]
             
@@ -1547,57 +1613,61 @@
     
 
 
     def clip_all_rasters(self, n:int=None) -> dict:
         """
         Clip all rasters 'elevation', 'shielding', 'quartz' to a single polygon.
         
-        n : number of the catchment
-            polygon = rv.catchment.catchments[n]['geometry']
-            for single-catchment shapefile set n=0 or or n=None (default value)
+        n : int
+            Number of the catchment.
+            > polygon = selg.catchment.catchments[n]['geometry']
+            For single-catchment shapefile set n=0 or or n=None (default value).
         
         """
         
         from riversand.utils import clip_raster
         
         if n is None:
             n=0
         
         #if self.epsg is None:
         #    print("WARNING : dataset does not seem validated, run .validate()")
         errR, errS, errC = self.validate(verbose=False)
         if len(errR+errC)>0:
-            raise ValueError("Cannnot validate 'rv'; use 'rv.validate()' for details")
+            raise ValueError("Cannnot validate data; use .validate() for details")
         
         try:
             polygon = self.catchments.catchments[n]['geometry'] # raises IndexError
             #try:
             #    c_name = self.catchments.catchments[n]['properties'][self.cid]
             #except:
             #    c_name = '' # for Exception message
         except IndexError as e:
-            raise ValueError("clip_all_rasters() : 'catchments' does not have "+
-                             "n={} polygons".format(n))
+            raise ValueError("clip_all_rasters() : .catchments does not have "+
+                             "n={} polygons".format(n)
+                             ) from None
         
         clips = {}
         
         rr = [r for r in [self.elevation, self.shielding, self.quartz]
              if r is not None]
         
         for r in rr:
             label = r.dtype
             try:    
                 Z = clip_raster(polygon, r.src, label)
             except ValueError as e:
-                raise ValueError("clip_all_rasters() : catchment polygon out of bounds")
+                raise ValueError("clip_all_rasters() : catchment polygon out of bounds"
+                                 ) from None
             clips[label] = Z
             
         # out of bounds is caught by validation of the clipped catchment
         if any(x is None for x in clips.values()):
-            raise ValueError("clip_all_rasters() : catchment polygon out of bounds")
+            raise ValueError("clip_all_rasters() : catchment polygon out of bounds"
+                             ) from None
         
         clips['epsg'] = self.epsg # validated at the beginning of the function
         return clips
 
 
 
 def main():
```

### Comparing `riversand-1.2.2/riversand/params.py` & `riversand-1.2.3/riversand/params.py`

 * *Files 24% similar despite different names*

```diff
@@ -46,43 +46,64 @@
                       'mineral'    : 'quartz', # 'quartz'
                       }
     
     _default_standards = {'Be-10': '07KNSTD',
                           'Al-26': 'KNSTD',
                          }
     
-    Be_stds = {"07KNSTD":1.0000,"KNSTD":0.9042,"NIST_Certified":1.0425,
-               "LLNL31000":0.8761,"LLNL10000":0.9042,"LLNL3000":0.8644,
-               "LLNL1000":0.9313,"LLNL300":0.8562,"NIST_30000":0.9313,
-               "NIST_30200":0.9251,"NIST_30300":0.9221,"NIST_30600":0.9130,
+
+
+
+    Be_stds = {"07KNSTD":1.0000,"KNSTD":0.9042,"NIST_Certified": 1.0425,
+               "LLNL31000":0.8761,"LLNL10000":0.9042,"LLNL3000": 0.8644,
+               "LLNL1000":0.9313,"LLNL300":0.8562,"NIST_30000": 0.9313,
+               "NIST_30200":0.9251,"NIST_30300":0.9221,"NIST_30600": 0.9130,
                "NIST_27900":1.0000,"S555":0.9124,"S2007":0.9124,
                "BEST433":0.9124,"BEST433N":1.0000,"S555N":1.0000,
-               "S2007N":1.0000,"STD11":1.0000,"NIST_30500":0.9148,
-               "SMDBe12":1.0000}
-    Al_stds = {"KNSTD":1.0000,"ZAL94":0.9134,"SMAL11":1.0209,"ZAL94N":1.0000,
-               "ASTER":1.0209,"Z92-0222":1.0000, "SMDAl11": 1.018}
+               "S2007N":1.0000,"STD11":1.0000,"0":0,"NIST_30500":0.9124,
+               "SMDBe12": 1.0000}
+    Al_stds = {"KNSTD":1.0000,"ZAL94":0.9134,"SMAL11":1.021,"0":0,
+               "ZAL94N":1.0000,"ASTER":1.021,"Z92-0222":1.0000,
+               "SMDAl11":1.018}
     
     _scalingmethods = ['St', 'Lm', 'LSDn']
     
     _XML_scalingmethods = ['NpredSt', 'NpredLm', 'NpredLSDn'] # returned by the online calculator
     
     # keys for the display of sample data
     all_keys = ['name',
                 'lat', 'latitude', 'long', 'longitude', 'elev', 'elevation',
                 'press_flag', 'thickness', 'density', 'shielding', 'erate', 'year',
                 'nuclide', 'mineral', 'N', 'delN', 'standardization']
     
     @classmethod
     def set_outpath(cls, value):
         cls.out_path = value
-        
 
 
-def set_outpath(value):
+def set_folder(value):
     Params.set_outpath(value)
 
+def get_folder():
+    print("Plots are saved in folder '{}'.".format(Params.out_path))
 
-
-
-
- 
-
+def print_units():
+    print("Valid units of erosion rate are: {}.".format(', '.join(Params.units.keys())))
+    
+def print_defaults():
+    print("\nDefault values:")
+    for k,v in Params.default_values.items():
+        print("  {0: <10} : {1: <10}".format(k, v))
+        
+    print("\nDefault standardizations:")
+    for k,v in Params._default_standards.items():
+        print("  {0: <10} : {1: <10}".format(k, v))
+    print()
+    
+def print_standardizations():
+    print("\nBe-10 standardizations:")
+    for k,v in Params.Be_stds.items():
+        print("  {0: <10} : {1: <10}".format(k, v))
+    print("\nAl-26 standardizations:")
+    for k,v in Params.Al_stds.items():
+        print("  {0: <10} : {1: <10}".format(k, v))
+    print()
```

### Comparing `riversand-1.2.2/riversand/plot.py` & `riversand-1.2.3/riversand/plot.py`

 * *Files identical despite different names*

### Comparing `riversand-1.2.2/riversand.egg-info/PKG-INFO` & `riversand-1.2.3/riversand.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riversand
-Version: 1.2.2
+Version: 1.2.3
 Summary: Catchmentwide erosion rate calculator
 Home-page: https://github.com/kstueb/riversand
 Author: Konstanze Stuebner
 Author-email: kstueb@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -56,16 +56,16 @@
 Definitely check out the documentation of the online calculator (e.g. [here](http://stoneage.ice-d.org/math/docs/v3/v3_input_explained.html)
 or [here](https://sites.google.com/a/bgc.org/v3docs/)) and the publication
 [Balco et al. (2008)](http://hess.ess.washington.edu/math/docs/al_be_v2/al_be_calc_2007.pdf)
 before using this calculator.
 
 Documentation
 -------------
-- [`quickstart.ipynb`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/quickstart_v20240228.ipynb)
-- [`step_by_step.ipynb`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/step_by_step_v20240228.ipynb)
+- [`quickstart.ipynb`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/quickstart_v1.2.3.ipynb)
+- [`step_by_step.ipynb`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/step_by_step_v1.2.3.ipynb)
 - [`test_data/`](https://github.com/kstueb/riversand/blob/main/riversand/example_scripts/test_data) : geotiffs of a 35m-resolution digital elevation model, a topographic shielding raster generated with [TopoToolbox](https://topotoolbox.wordpress.com/) and a binary raster indicating quartz-bearing and quartz-free lithologies; shapefiles with catchment outlines; a spreadsheet with sample data. 
 
 Installation
 ------------
 Install riversand by running:
 ```
 $ pip install riversand
```

### Comparing `riversand-1.2.2/setup.py` & `riversand-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.core import setup   
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()   
 setup(                                
    name = 'riversand',
-   version = '1.2.2',
+   version = '1.2.3',
    packages = ['riversand'],
    author = 'Konstanze Stuebner',
    author_email = 'kstueb@gmail.com',
    url = 'https://github.com/kstueb/riversand',
    description = 'Catchmentwide erosion rate calculator',
    classifiers = ["Programming Language :: Python",
                   "Programming Language :: Python :: 3",
```

