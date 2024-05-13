# Comparing `tmp/TwoSampleHC-0.3.0.tar.gz` & `tmp/twosamplehc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TwoSampleHC-0.3.0.tar", last modified: Wed Mar 13 10:18:49 2024, max compression
+gzip compressed data, was "twosamplehc-0.3.1.tar", last modified: Mon May 13 07:22:44 2024, max compression
```

## Comparing `TwoSampleHC-0.3.0.tar` & `twosamplehc-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-03-13 10:18:49.639976 TwoSampleHC-0.3.0/
--rw-r--r--   0 kipnisal   (503) staff       (20)     1073 2020-03-01 22:03:16.000000 TwoSampleHC-0.3.0/LICENSE
--rw-r--r--   0 kipnisal   (503) staff       (20)     2474 2024-03-13 10:18:49.639926 TwoSampleHC-0.3.0/PKG-INFO
--rw-r--r--   0 kipnisal   (503) staff       (20)     1919 2024-03-13 09:50:50.000000 TwoSampleHC-0.3.0/README.md
--rw-r--r--   0 kipnisal   (503) staff       (20)      103 2023-02-27 08:30:42.000000 TwoSampleHC-0.3.0/pyproject.toml
--rw-r--r--   0 kipnisal   (503) staff       (20)      688 2024-03-13 10:18:49.640223 TwoSampleHC-0.3.0/setup.cfg
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-03-13 10:18:49.637583 TwoSampleHC-0.3.0/src/
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-03-13 10:18:49.638673 TwoSampleHC-0.3.0/src/TwoSampleHC/
--rw-r--r--   0 kipnisal   (503) staff       (20)    15034 2024-03-13 10:04:42.000000 TwoSampleHC-0.3.0/src/TwoSampleHC/TwoSampleHC.py
--rw-r--r--   0 kipnisal   (503) staff       (20)      660 2020-07-10 04:38:59.000000 TwoSampleHC-0.3.0/src/TwoSampleHC/__init__.py
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-03-13 10:18:49.639739 TwoSampleHC-0.3.0/src/TwoSampleHC.egg-info/
--rw-r--r--   0 kipnisal   (503) staff       (20)     2474 2024-03-13 10:18:49.000000 TwoSampleHC-0.3.0/src/TwoSampleHC.egg-info/PKG-INFO
--rw-r--r--   0 kipnisal   (503) staff       (20)      324 2024-03-13 10:18:49.000000 TwoSampleHC-0.3.0/src/TwoSampleHC.egg-info/SOURCES.txt
--rw-r--r--   0 kipnisal   (503) staff       (20)        1 2024-03-13 10:18:49.000000 TwoSampleHC-0.3.0/src/TwoSampleHC.egg-info/dependency_links.txt
--rw-r--r--   0 kipnisal   (503) staff       (20)       24 2024-03-13 10:18:49.000000 TwoSampleHC-0.3.0/src/TwoSampleHC.egg-info/requires.txt
--rw-r--r--   0 kipnisal   (503) staff       (20)       12 2024-03-13 10:18:49.000000 TwoSampleHC-0.3.0/src/TwoSampleHC.egg-info/top_level.txt
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-03-13 10:18:49.639461 TwoSampleHC-0.3.0/tests/
--rw-r--r--   0 kipnisal   (503) staff       (20)     3339 2021-12-08 07:51:44.000000 TwoSampleHC-0.3.0/tests/test_sparse_normals.py
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-05-13 07:22:44.936646 twosamplehc-0.3.1/
+-rw-r--r--   0 kipnisal   (503) staff       (20)     1073 2020-03-01 22:03:16.000000 twosamplehc-0.3.1/LICENSE
+-rw-r--r--   0 kipnisal   (503) staff       (20)     2467 2024-05-13 07:22:44.936586 twosamplehc-0.3.1/PKG-INFO
+-rw-r--r--   0 kipnisal   (503) staff       (20)     1919 2024-03-13 09:50:50.000000 twosamplehc-0.3.1/README.md
+-rw-r--r--   0 kipnisal   (503) staff       (20)      103 2023-02-27 08:30:42.000000 twosamplehc-0.3.1/pyproject.toml
+-rw-r--r--   0 kipnisal   (503) staff       (20)      681 2024-05-13 07:22:44.936898 twosamplehc-0.3.1/setup.cfg
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-05-13 07:22:44.933773 twosamplehc-0.3.1/src/
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-05-13 07:22:44.935205 twosamplehc-0.3.1/src/TwoSampleHC/
+-rw-r--r--   0 kipnisal   (503) staff       (20)    13216 2024-05-13 07:18:40.000000 twosamplehc-0.3.1/src/TwoSampleHC/TwoSampleHC.py
+-rw-r--r--   0 kipnisal   (503) staff       (20)      722 2024-05-13 07:20:24.000000 twosamplehc-0.3.1/src/TwoSampleHC/__init__.py
+-rw-r--r--   0 kipnisal   (503) staff       (20)     1816 2024-05-13 07:09:29.000000 twosamplehc-0.3.1/src/TwoSampleHC/hc_vals.py
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-05-13 07:22:44.936388 twosamplehc-0.3.1/src/TwoSampleHC.egg-info/
+-rw-r--r--   0 kipnisal   (503) staff       (20)     2467 2024-05-13 07:22:44.000000 twosamplehc-0.3.1/src/TwoSampleHC.egg-info/PKG-INFO
+-rw-r--r--   0 kipnisal   (503) staff       (20)      351 2024-05-13 07:22:44.000000 twosamplehc-0.3.1/src/TwoSampleHC.egg-info/SOURCES.txt
+-rw-r--r--   0 kipnisal   (503) staff       (20)        1 2024-05-13 07:22:44.000000 twosamplehc-0.3.1/src/TwoSampleHC.egg-info/dependency_links.txt
+-rw-r--r--   0 kipnisal   (503) staff       (20)       17 2024-05-13 07:22:44.000000 twosamplehc-0.3.1/src/TwoSampleHC.egg-info/requires.txt
+-rw-r--r--   0 kipnisal   (503) staff       (20)       12 2024-05-13 07:22:44.000000 twosamplehc-0.3.1/src/TwoSampleHC.egg-info/top_level.txt
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-05-13 07:22:44.936147 twosamplehc-0.3.1/tests/
+-rw-r--r--   0 kipnisal   (503) staff       (20)     2256 2024-05-13 07:22:05.000000 twosamplehc-0.3.1/tests/test_sparse_normals.py
```

### Comparing `TwoSampleHC-0.3.0/LICENSE` & `twosamplehc-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TwoSampleHC-0.3.0/PKG-INFO` & `twosamplehc-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: TwoSampleHC
-Version: 0.3.0
+Version: 0.3.1
 Summary: Several two-samples tests for count data
 Home-page: https://github.com/alonkipnis/TwoSampleHC
 Download-URL: https://github.com/alonkipnis/TwoSampleHC
 Author: Alon Kipnis
 Author-email: alonkipnis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.6
-Requires-Dist: scipy[stats]
+Requires-Dist: scipy
 
 # TwoSampleHC -- Higher Criticism Test between Two Frequency Tables
 
 This package provides an adaptation of the Donoho-Jin-Tukey Higher-
 Critisim (HC) test to frequency tables. This adapatation uses a binomial
 allocation model for the number of occurances of each feature in two-
 samples, each of which is associated with a frequency table. The exact
```

### Comparing `TwoSampleHC-0.3.0/README.md` & `twosamplehc-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `TwoSampleHC-0.3.0/setup.cfg` & `twosamplehc-0.3.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TwoSampleHC
-version = 0.3.0
+version = 0.3.1
 author = Alon Kipnis
 author_email = alonkipnis@gmail.com
 description = Several two-samples tests for count data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/alonkipnis/TwoSampleHC
 download_url = https://github.com/alonkipnis/TwoSampleHC
@@ -16,15 +16,15 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy >= 1.6
-	scipy[stats]
+	scipy
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [egg_info]
```

### Comparing `TwoSampleHC-0.3.0/src/TwoSampleHC/TwoSampleHC.py` & `twosamplehc-0.3.1/src/TwoSampleHC/TwoSampleHC.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pandas as pd
 from scipy.stats import binom, norm, poisson, beta
 
-class HC(object):
+class HigherCriticism(object):
     """
     Higher Criticism test 
 
     References:
     [1] Donoho, D. L. and Jin, J., "Higher criticism for detecting sparse
      hetrogenous mixtures", Annals of Stat. 2004
     [2] Donoho, D. L. and Jin, J. "Higher critcism thresholding: Optimal 
@@ -118,14 +118,20 @@
         return {'pvals' : self._sorted_pvals, 
                 'u' : self._uu,
                 'z' : self._zz,
                 'imin_star' : self._imin_star,
                 'imin_jin' : self._imin_jin,
                 }
 
+
+class HC(HigherCriticism):
+    """
+    For legacy
+    """
+
     
 def two_sample_test(smp1, smp2, data_type = 'counts',
                          alt='two-sided', **kwargs) :
     """
     Returns HC score and HC threshold in a two-sample test. 
     =========================================================
 
@@ -156,79 +162,16 @@
     elif data_type == 'reals' :
         z = (smp1 - smp2) / np.sqrt(2)
         if alt == 'greater' :
             pvals = norm.sf(z)
         else :
             pvals = norm.sf(np.abs(z))
 
-    return HC(pvals[~np.isnan(pvals)], stbl).HCstar(gamma)
-
-def hc_vals(pv, gamma=0.2, minPv='one_over_n', stbl=True):
-    """
-    This is the old version of the HC test that is now doen using 
-    the class HC. 
-
-    Higher Criticism test 
-
-    Args:
-    -----
-        pv : list of p-values. P-values that are np.nan are exluded.
-        gamma : lower fruction of p-values to use.
-        stbl : use expected p-value ordering (stbl=True) or observed 
-                (stbl=False)
-        minPv : integer or string 'one_over_n' (default).
-                 Ignote smallest minPv-1 when computing HC score.
-
-    Return :
-    -------
-        hc_star : sample adapted HC (HC dagger in [1])
-        p_star : HC threshold: upper boundary for collection of
-                 p-value indicating the largest deviation from the
-                 uniform distribution.
-
-    """
-    EPS = 0.001
-    pv = np.asarray(pv).copy()
-    n = len(pv)  #number of features
-    pv[np.isnan(pv)] = 1-EPS
-    #n = len(pv)
-    hc_star = np.nan
-    p_star = np.nan
-
-    if n > 1:
-        ps_idx = np.argsort(pv)
-        ps = pv[ps_idx]  #sorted pvals
-
-        uu = np.linspace(1 / n, 1-EPS, n)  #expectation of p-values under
-        # H0; largest P-value assumed to have not effect. 
-        i_lim_up = np.maximum(int(np.floor(gamma * n + 0.5)), 1)
-
-        ps = ps[:i_lim_up]
-        uu = uu[:i_lim_up]
-        
-        if minPv == 'one_over_n' :
-            i_lim_low = np.argmax(ps > (1-EPS)/n)
-        else :
-            i_lim_low = minPv
-
-        if stbl:
-            z = (uu - ps) / np.sqrt(uu * (1 - uu)) * np.sqrt(n)
-        else:
-            z = (uu - ps) / np.sqrt(ps * (1 - ps)) * np.sqrt(n)
-
-        i_lim_up = max(i_lim_low + 1, i_lim_up)
+    return HigherCriticism(pvals[~np.isnan(pvals)], stbl).HCstar(gamma)
 
-        i_max_star = np.argmax(z[i_lim_low:i_lim_up]) + i_lim_low
-
-        z_max_star = z[i_max_star]
-
-        hc_star = z[i_max_star]
-        p_star = ps[i_max_star]
-
-    return hc_star, p_star
 
 def binom_test(x, n, p, alt='greater') :
     """
     Returns:
     --------
     Prob(Bin(n,p) >= x) ('greater')
     or Prob(Bin(n,p) <= x) ('less')
@@ -408,30 +351,30 @@
     else :
         pvals = binom_test_two_sided(c1, c1 + c2, p)
 
     if ret_p :
         return pvals, p
     return pvals
 
-def two_sample_test_df(X, Y, gamma=0.25, min_cnt=0,
+def two_sample_test_df(c1, c2, gamma=0.2, min_cnt=0,
                 stbl=True, randomize=False, 
                 alt='two-sided', HCtype='HCstar'):
     """
     Same as two_sample_test but returns all information for computing
     HC score of the two samples as a pandas data DataFrame. 
     Requires pandas.
 
     Args: 
     -----
-    X, Y       lists of integers of equal length
+    c1, c2       lists of integers of equal length
     gamma      parameter of HC statistic
     stbl       parameter of HC statistic
     randomize  use randomized or not exact binomial test
     alt        type of test alternatives: 'two-sided' or 'one-sided'
-    HCtype     either 'HCstar' (default) or  'original'. Determine
+    HCtype     either 'HCstar' (default) or 'standard'. Determine
                different variations of HC statistic 
 
     Returns:
     -------
     counts : DataFrame with fields: 
             n1, n2, p, T1, T2, pval, sign, HC, thresh
             Here: 
@@ -445,40 +388,41 @@
             'sign' :    indicates whether a feature is more frequent 
                     in sample X (+1) or sample Y (-1)
             'HC' :      is the higher criticism statistic applies to the
                     column 'pval'
             'thresh' :  indicates whether a feature is below the HC 
                         threshold (True) or not (False)
     """
-    import pandas as pd
+    assert len(c1) == len(c2)
 
     counts = pd.DataFrame()
-    counts['n1'] = X
-    counts['n2'] = Y
+    counts['n1'] = c1
+    counts['n2'] = c2
     T1 = counts['n1'].sum()
     T2 = counts['n2'].sum()
     
     counts['T1'] = T1
     counts['T2'] = T2
 
     counts['pval'], counts['p'] = two_sample_pvals(
         counts['n1'], counts['n2'],
         randomize=randomize, alt=alt, ret_p=True)
 
     counts['sign'] = np.sign(counts.n1 - (counts.n1 + counts.n2) * counts.p)
 
     counts.loc[counts.n1 + counts.n2 < min_cnt, 'pval'] = np.nan
     pvals = counts.pval.values
-    hc = HC(pvals[~np.isnan(pvals)], stbl=stbl)
-    #hc_star, p_val_thresh = hc_vals(pvals, gamma=gamma, stbl=stbl)
-    if HCtype == 'original' :
+    hc = HigherCriticism(pvals[~np.isnan(pvals)], stbl=stbl)
+
+    if HCtype == 'standard' :
         hc, p_val_thresh = hc.HC(gamma=gamma)
-    else :
+    else:
         hc, p_val_thresh = hc.HCstar(gamma=gamma)
 
     counts['HC'] = hc
 
     counts['thresh'] = True
     counts.loc[counts['pval'] >= p_val_thresh, ('thresh')] = False
     counts.loc[np.isnan(counts['pval']), ('thresh')] = False
     
     return counts
+
```

### Comparing `TwoSampleHC-0.3.0/src/TwoSampleHC.egg-info/PKG-INFO` & `twosamplehc-0.3.1/src/TwoSampleHC.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: TwoSampleHC
-Version: 0.3.0
+Version: 0.3.1
 Summary: Several two-samples tests for count data
 Home-page: https://github.com/alonkipnis/TwoSampleHC
 Download-URL: https://github.com/alonkipnis/TwoSampleHC
 Author: Alon Kipnis
 Author-email: alonkipnis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.6
-Requires-Dist: scipy[stats]
+Requires-Dist: scipy
 
 # TwoSampleHC -- Higher Criticism Test between Two Frequency Tables
 
 This package provides an adaptation of the Donoho-Jin-Tukey Higher-
 Critisim (HC) test to frequency tables. This adapatation uses a binomial
 allocation model for the number of occurances of each feature in two-
 samples, each of which is associated with a frequency table. The exact
```

