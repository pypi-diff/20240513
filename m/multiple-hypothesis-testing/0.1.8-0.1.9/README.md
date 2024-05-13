# Comparing `tmp/multiple-hypothesis-testing-0.1.8.tar.gz` & `tmp/multiple-hypothesis-testing-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiple-hypothesis-testing-0.1.8.tar", last modified: Wed Dec 13 10:21:29 2023, max compression
+gzip compressed data, was "multiple-hypothesis-testing-0.1.9.tar", last modified: Tue Feb 20 15:54:41 2024, max compression
```

## Comparing `multiple-hypothesis-testing-0.1.8.tar` & `multiple-hypothesis-testing-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-12-13 10:21:29.143808 multiple-hypothesis-testing-0.1.8/
--rw-r--r--   0 kipnisal   (503) staff       (20)     1073 2022-02-20 07:18:17.000000 multiple-hypothesis-testing-0.1.8/LICENSE
--rw-r--r--   0 kipnisal   (503) staff       (20)     1619 2023-12-13 10:21:29.143753 multiple-hypothesis-testing-0.1.8/PKG-INFO
--rw-r--r--   0 kipnisal   (503) staff       (20)     1028 2023-09-06 06:53:46.000000 multiple-hypothesis-testing-0.1.8/README.md
--rw-r--r--   0 kipnisal   (503) staff       (20)      103 2023-03-02 23:02:15.000000 multiple-hypothesis-testing-0.1.8/pyproject.toml
--rw-r--r--   0 kipnisal   (503) staff       (20)      727 2023-12-13 10:21:29.144056 multiple-hypothesis-testing-0.1.8/setup.cfg
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-12-13 10:21:29.141308 multiple-hypothesis-testing-0.1.8/src/
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-12-13 10:21:29.143447 multiple-hypothesis-testing-0.1.8/src/multiple_hypothesis_testing.egg-info/
--rw-r--r--   0 kipnisal   (503) staff       (20)     1619 2023-12-13 10:21:29.000000 multiple-hypothesis-testing-0.1.8/src/multiple_hypothesis_testing.egg-info/PKG-INFO
--rw-r--r--   0 kipnisal   (503) staff       (20)      369 2023-12-13 10:21:29.000000 multiple-hypothesis-testing-0.1.8/src/multiple_hypothesis_testing.egg-info/SOURCES.txt
--rw-r--r--   0 kipnisal   (503) staff       (20)        1 2023-12-13 10:21:29.000000 multiple-hypothesis-testing-0.1.8/src/multiple_hypothesis_testing.egg-info/dependency_links.txt
--rw-r--r--   0 kipnisal   (503) staff       (20)       27 2023-12-13 10:21:29.000000 multiple-hypothesis-testing-0.1.8/src/multiple_hypothesis_testing.egg-info/requires.txt
--rw-r--r--   0 kipnisal   (503) staff       (20)       10 2023-12-13 10:21:29.000000 multiple-hypothesis-testing-0.1.8/src/multiple_hypothesis_testing.egg-info/top_level.txt
-drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2023-12-13 10:21:29.143152 multiple-hypothesis-testing-0.1.8/src/multitest/
--rw-r--r--   0 kipnisal   (503) staff       (20)     8470 2023-12-13 10:20:46.000000 multiple-hypothesis-testing-0.1.8/src/multitest/MultiTest.py
--rw-r--r--   0 kipnisal   (503) staff       (20)       33 2022-02-20 09:43:43.000000 multiple-hypothesis-testing-0.1.8/src/multitest/__init__.py
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-02-20 15:54:41.338027 multiple-hypothesis-testing-0.1.9/
+-rw-r--r--   0 kipnisal   (503) staff       (20)     1073 2022-02-20 07:18:17.000000 multiple-hypothesis-testing-0.1.9/LICENSE
+-rw-r--r--   0 kipnisal   (503) staff       (20)     1619 2024-02-20 15:54:41.337973 multiple-hypothesis-testing-0.1.9/PKG-INFO
+-rw-r--r--   0 kipnisal   (503) staff       (20)     1028 2023-09-06 06:53:46.000000 multiple-hypothesis-testing-0.1.9/README.md
+-rw-r--r--   0 kipnisal   (503) staff       (20)      103 2023-03-02 23:02:15.000000 multiple-hypothesis-testing-0.1.9/pyproject.toml
+-rw-r--r--   0 kipnisal   (503) staff       (20)      727 2024-02-20 15:54:41.338268 multiple-hypothesis-testing-0.1.9/setup.cfg
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-02-20 15:54:41.335875 multiple-hypothesis-testing-0.1.9/src/
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-02-20 15:54:41.337786 multiple-hypothesis-testing-0.1.9/src/multiple_hypothesis_testing.egg-info/
+-rw-r--r--   0 kipnisal   (503) staff       (20)     1619 2024-02-20 15:54:41.000000 multiple-hypothesis-testing-0.1.9/src/multiple_hypothesis_testing.egg-info/PKG-INFO
+-rw-r--r--   0 kipnisal   (503) staff       (20)      369 2024-02-20 15:54:41.000000 multiple-hypothesis-testing-0.1.9/src/multiple_hypothesis_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 kipnisal   (503) staff       (20)        1 2024-02-20 15:54:41.000000 multiple-hypothesis-testing-0.1.9/src/multiple_hypothesis_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 kipnisal   (503) staff       (20)       27 2024-02-20 15:54:41.000000 multiple-hypothesis-testing-0.1.9/src/multiple_hypothesis_testing.egg-info/requires.txt
+-rw-r--r--   0 kipnisal   (503) staff       (20)       10 2024-02-20 15:54:41.000000 multiple-hypothesis-testing-0.1.9/src/multiple_hypothesis_testing.egg-info/top_level.txt
+drwxr-xr-x   0 kipnisal   (503) staff       (20)        0 2024-02-20 15:54:41.337477 multiple-hypothesis-testing-0.1.9/src/multitest/
+-rw-r--r--   0 kipnisal   (503) staff       (20)    11685 2024-02-20 15:53:29.000000 multiple-hypothesis-testing-0.1.9/src/multitest/MultiTest.py
+-rw-r--r--   0 kipnisal   (503) staff       (20)       33 2022-02-20 09:43:43.000000 multiple-hypothesis-testing-0.1.9/src/multitest/__init__.py
```

### Comparing `multiple-hypothesis-testing-0.1.8/LICENSE` & `multiple-hypothesis-testing-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `multiple-hypothesis-testing-0.1.8/PKG-INFO` & `multiple-hypothesis-testing-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiple-hypothesis-testing
-Version: 0.1.8
+Version: 0.1.9
 Summary: Several methods of combining P-values
 Home-page: https://github.com/alonkipnis/higher-criticism-test
 Download-URL: https://github.com/alonkipnis/higher-criticism-test
 Author: Alon Kipnis
 Author-email: alonkipnis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multiple-hypothesis-testing-0.1.8/README.md` & `multiple-hypothesis-testing-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `multiple-hypothesis-testing-0.1.8/setup.cfg` & `multiple-hypothesis-testing-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multiple-hypothesis-testing
-version = 0.1.08
+version = 0.1.09
 author = Alon Kipnis
 author_email = alonkipnis@gmail.com
 description = Several methods of combining P-values
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/alonkipnis/higher-criticism-test
 download_url = https://github.com/alonkipnis/higher-criticism-test
```

### Comparing `multiple-hypothesis-testing-0.1.8/src/multiple_hypothesis_testing.egg-info/PKG-INFO` & `multiple-hypothesis-testing-0.1.9/src/multiple_hypothesis_testing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiple-hypothesis-testing
-Version: 0.1.8
+Version: 0.1.9
 Summary: Several methods of combining P-values
 Home-page: https://github.com/alonkipnis/higher-criticism-test
 Download-URL: https://github.com/alonkipnis/higher-criticism-test
 Author: Alon Kipnis
 Author-email: alonkipnis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multiple-hypothesis-testing-0.1.8/src/multitest/MultiTest.py` & `multiple-hypothesis-testing-0.1.9/src/multitest/MultiTest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,124 +1,169 @@
 import numpy as np
 from scipy.stats import beta, chi2
 from matplotlib import pyplot as plt
 
-MIN_PVAL = 1e-20
-
 
 class MultiTest(object):
     """
-    Higher Criticism test 
+    Mulitple testing class for P-values with a focus on tests for rare and weak effects.
+    The package implemnents the following tests:
+    - Higher criticism [1] and varaints from [2] and [3], including HC threshold from [2]
+    - Berk-Jones [4]
+    - Fisher's method
+    - Bonferroni type inference
+    - Family-wise significant testing using FDR control
+    - P-value selection using Benjamini-Hochberg's FDR control
 
     References:
     [1] Donoho, D. L. and Jin, J.,
      "Higher criticism for detecting sparse hetrogenous mixtures", 
      Annals of Stat. 2004
     [2] Donoho, D. L. and Jin, J. "Higher critcism thresholding: Optimal 
     feature selection when useful features are rare and weak", proceedings
     of the national academy of sciences, 2008.
+    [3] Jiashun Jin and Wanjie Wang, "Influential features PCA for
+                 high dimensional clustering"
+    [4] Amit Moscovich, Boaz Nadler, and Clifford Spiegelman. "On the exact Berk-Jones statistics
+      and their p-value calculation." Electronic Journal of Statistics. 10 (2016): 2329-2354.
+
     ========================================================================
 
     Args:
     -----
         pvals    list of p-values. P-values that are np.nan are exluded.
         stbl     normalize by expected P-values (stbl=True) or observed
-                 P-values (stbl=False). stbl=True was suggested in [2].
-                 stbl=False in [1].
-        gamma    lower fruction of p-values to use.
+                 P-values (stbl=False). stbl=True was suggested in [2] while 
+                 [1] studied the case stbl=False. 
         
     Methods :
     -------
-        hc       HC and P-value attaining it
-        hc_star  more stable version of HC (HCdagger in [1])
-        hc_jin   a version of HC from 
-                [2] Jiashun Jin and Wanjie Wang, "Influential features PCA for
-                 high dimensional clustering"
-
-    Todo:
-      Implement Feature selection procedures: HC-thresholding, FDR, BJ, Sims
-      The idea is to return a mask based on the P-values
-      Perhaps implement it in a different module dedicated to feature selection?
-
+        hc       HC and P-value attaining it 
+        hc_star  Only consider P-values larger than 1/n. (HCdagger in [1]) 
+        hc_jin   Only consider P-values larger than log(n)/n. This variant was introduced in [3]
+        berkjones  Exact Berk-Jones statistic (see [4])
     """
 
     def __init__(self, pvals, stbl=True):
 
         self._N = len(pvals)
         assert (self._N > 0)
 
-        self._EPS = 1 / (1e2 + self._N ** 2)
+        self._EPS = 1 / (1e4 + self._N ** 2)
         self._istar = 1
 
-        self._pvals = np.sort(np.asarray(pvals.copy()))
+        self._sorted_pvals = np.sort(np.asarray(pvals.copy()))  # sorted P-values
         self._uu = np.linspace(1 / self._N, 1, self._N)
         self._uu[-1] -= self._EPS # we assume that the largest P-value
                                   # has no effect on the results
         if stbl:
             denom = np.sqrt(self._uu * (1 - self._uu))
         else:
-            denom = np.sqrt(self._pvals * (1 - self._pvals))
+            denom = np.sqrt(self._sorted_pvals * (1 - self._sorted_pvals))
 
-        self._zz = np.sqrt(self._N) * (self._uu - self._pvals) / denom
+        self._zz = np.sqrt(self._N) * (self._uu - self._sorted_pvals) / denom
 
-        self._imin_star = np.argmax(self._pvals > (1 - self._EPS) / self._N)
-        self._imin_jin = np.argmax(self._pvals > np.log(self._N) / self._N)
+        self._imin_star = np.argmax(self._sorted_pvals > (1 - self._EPS) / self._N)
+        self._imin_jin = np.argmax(self._sorted_pvals > np.log(self._N) / self._N)
 
         self._gamma = np.log(self._N) / np.sqrt(self._N)  # for 'auto' setting
-                            # this gamma may be too small when N is large
+                            # this gamma was suggested in [3]
+                            # The rationalle is that HC is not useful for signal denser than 1/sqrt(n)
 
-    def _calculate_hc(self, imin, imax):
+    def _evaluate_hc(self, imin, imax):
         if imin > imax:
             return np.nan
         if imin == imax:
             self._istar = imin
         else:
             self._istar = np.argmax(self._zz[imin:imax]) + imin
         zMaxStar = self._zz[self._istar]
-        return zMaxStar, self._pvals[self._istar]
+        return zMaxStar, self._sorted_pvals[self._istar]
 
     def hc(self, gamma='auto'):
         """
-        Higher Criticism test statistic
+        Higher Criticism test of [1]
 
         Args:
         -----
         gamma   lower fraction of P-values to consider
 
         Return:
         -------
         HC test score, P-value attaining it
 
         """
         imin = 0
         if gamma == 'auto': 
             gamma = self._gamma
         imax = np.maximum(imin, int(gamma * self._N + 0.5))
-        return self._calculate_hc(imin, imax)
+        return self._evaluate_hc(imin, imax)
 
     def hc_jin(self, gamma='auto'):
-        """sample-adjusted higher criticism score from [2]
+        """
+        but only consider P-values larger than log(n)/n. 
+        This variant was introduced in [3]/ 
 
         Args:
         -----
         gamma   lower fraction of P-values to consider
 
         Return:
         -------
         HC score, P-value attaining it
-
         """
 
         if gamma == 'auto': 
             gamma = self._gamma
         imin = self._imin_jin
         imax = np.maximum(imin + 1, int(np.floor(gamma * self._N + 0.5)))
-        return self._calculate_hc(imin, imax)
+        return self._evaluate_hc(imin, imax)
 
-    def berk_jones(self, gamma=.45):
+    def berkjones(self, gamma='auto', min_only=False):
+        """
+        Exact Berk-Jones statistic
+
+        According to Moscovich, Nadler, Spiegelman. (2013). 
+        On the exact Berk-Jones statistics and their p-value calculation
+
+        Args:
+        -----
+        gamma  lower fraction of P-values to consider. 
+
+        Return:
+        -------
+        -log(BJ) score (large values are significant) 
+        (has a scaled chisquared distribution under the null)
+
+        """
+
+        N = self._N
+        if N == 0:
+            return np.nan, np.nan
+        
+        if gamma == 'auto': 
+            gamma = self._gamma
+
+        max_i = max(1, int(gamma * N))
+
+        spv = self._sorted_pvals[:max_i]
+        ii = np.arange(1, max_i + 1)
+
+        bj = spv[0]
+        if len(spv) >= 1:
+            BJpv = beta.cdf(spv, ii, N - ii + 1)
+            Mplus = np.min(BJpv)
+            Mminus = np.min(1 - BJpv)
+            if min_only: #only use BJ+ for the score
+                bj = Mplus 
+            else:
+                bj = np.minimum(Mplus, Mminus) 
+        return -np.log(bj)
+    
+    def berkjones_plus(self, gamma='auto'):
         """
         Exact Berk-Jones statistic
 
         According to Moscovich, Nadler, Spiegelman. (2013). 
         On the exact Berk-Jones statistics and their p-value calculation
 
         Args:
@@ -133,48 +178,79 @@
 
         """
 
         N = self._N
 
         if N == 0:
             return np.nan, np.nan
+        
+        if gamma == 'auto': 
+            gamma = self._gamma
 
         max_i = max(1, int(gamma * N))
 
-        spv = self._pvals[:max_i]
+        spv = self._sorted_pvals[:max_i]
         ii = np.arange(1, max_i + 1)
 
-        bj = spv[0]
+        Mplus = spv[0]
         if len(spv) >= 1:
             BJpv = beta.cdf(spv, ii, N - ii + 1)
             Mplus = np.min(BJpv)
-            Mminus = np.min(1 - BJpv)
-            bj = np.minimum(Mplus, Mminus)
+            
+        return -np.log(Mplus)
+
+    def berkjones_threshold(self, gamma='auto'):
+        """
+        Use the Berk-Jones statistic to find a threshold for P-values in 
+        a manner analogous to the HC threshold of [2]
+
+        Args:
+        -----
+        gamma  lower fraction of P-values to consider
+
+        Return:
+        -------
+        P-value attaining the minimum in Mplus
+        """
+
+        N = self._N
+        if N == 0:
+            return np.nan, np.nan
+        
+        if gamma == 'auto': 
+            gamma = self._gamma
+
+        max_i = max(1, int(gamma * N))
+        spv = self._sorted_pvals[:max_i]
+        ii = np.arange(1, max_i + 1)
 
-        return -np.log(np.maximum(bj, MIN_PVAL))
+        istar = 0
+        if len(spv) >= 1:
+            BJpv = beta.cdf(spv, ii, N - ii + 1)
+            istar = np.argmin(BJpv)
+        return spv[istar]  # P-value attaining the minimum in Mplus
 
     def hc_star(self, gamma='auto'):
         """sample-adjusted higher criticism score
 
         Args:
         -----
         'gamma' : lower fraction of P-values to consider
 
         Returns:
         -------
-        :HC_score:
-        :P-value attaining it:
+        HC score
+        P-value attaining it
 
         """
         if gamma == 'auto': 
             gamma = self._gamma
         imin = self._imin_star
-        imax = np.maximum(imin + 1,
-                          int(np.floor(gamma * self._N + 0.5)))
-        return self._calculate_hc(imin, imax)
+        imax = np.maximum(imin + 1, int(np.floor(gamma * self._N + 0.5)))
+        return self._evaluate_hc(imin, imax)
 
     def hc_dashboard(self, gamma='auto'):
         """
         Illustrates HC over z-scores and sorted P-values.
 
         Args:
             gamma:  HC parameter
@@ -189,15 +265,15 @@
         hc, hct = self.hc(gamma)
         imin = 0
         N = self._N
         istar = self._istar
 
         imax = np.maximum(imin, int(gamma * N + 0.5))
 
-        yy = np.sort(self._pvals)[imin:imax]
+        yy = np.sort(self._sorted_pvals)[imin:imax]
         zz = self._zz[imin:imax]
         xx = self._uu[imin:imax]
 
         ax = plt.subplot(211)
 
         ax.stem(xx, yy, markerfmt='.')
         ax.plot([(istar + 1) / N, (istar + 1) / N], [0, hct], '--r', alpha=.75)
@@ -237,53 +313,73 @@
         fig = plt.gcf()
         fig.set_size_inches(10, 10, forward=True)
 
         plt.show()
         return fig
 
     def get_state(self):
-        return {'pvals': self._pvals,
+        return {'pvals': self._sorted_pvals,
                 'u': self._uu,
                 'z': self._zz,
                 'imin_star': self._imin_star,
                 'imin_jin': self._imin_jin,
                 }
 
     def minp(self):
         """
         Bonferroni type inference
 
+        Returns:
         -log(minimal P-value)
         """
-        return -np.log(np.maximum(self._pvals[0], MIN_PVAL))
+        return -np.log(self._sorted_pvals[0])
 
     def fdr(self):
         """
         Maximal False-discovery rate functional 
 
         Returns:
-            :corrected critical P-value:
-            :critical P-value:
+            -log(p(i^*)), p(i^*) where i^* is the index of the
+            critical P-value
         """
 
-        vals = self._pvals / self._uu
+        vals = self._sorted_pvals / self._uu
         istar = np.argmin(vals)
-        return -np.log(np.maximum(vals[istar], MIN_PVAL)), self._pvals[istar]
+        return -np.log(vals[istar]), self._sorted_pvals[istar]
+
+    def fdr_control(self, fdr_param=0.1):
+        """
+        Binjimini-Hochberg FDR control
+
+        Args:
+            fdr_param: False discovery rate parameter
+
+        Returns:
+            P-value p(i^*) such that the the proportion of false discoveries in {p(i) <= p(i^*)} is 
+            samller in expectation than fdr_param
+        """
+
+        vals = self._sorted_pvals / self._uu
+        indicator = vals > fdr_param # example 0 0 0 1 1 1 1 1 1
+        istar = np.argmax(indicator)-1           # first 1
+        if istar < 0:
+            return np.nan
+        return self._sorted_pvals[istar]
 
     def fisher(self):
         """
         combine P-values using Fisher's method:
 
         Fs = sum(-2 log(pvals))
 
         (here n is the number of P-values)
 
         When pvals are uniform Fs ~ chi^2 with 2*len(pvals) degrees of freedom
 
         Returns:
-            Fs:       Fisher's method statistics
-            Fs_pval:  P-value of the assocaited chi-squared test
+            fisher_comb_stat       Fisher's method statistics
+            chi2_pval              P-value of the assocaited chi-squared test
         """
 
-        Fs = np.sum(-2 * np.log(np.maximum(self._pvals, MIN_PVAL)))
-        chi2_pval = chi2.sf(Fs, df=2 * len(self._pvals))
-        return Fs, chi2_pval
+        fisher_comb_stat = np.sum(-2 * np.log(self._sorted_pvals))
+        chi2_pval = chi2.sf(fisher_comb_stat, df=2 * len(self._sorted_pvals))
+        return fisher_comb_stat, chi2_pval
```

