# Comparing `tmp/insilicova-0.1.1.tar.gz` & `tmp/insilicova-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insilicova-0.1.1.tar", last modified: Fri Apr  5 17:05:30 2024, max compression
+gzip compressed data, was "insilicova-0.1.3.tar", last modified: Mon May 13 18:54:41 2024, max compression
```

## Comparing `insilicova-0.1.1.tar` & `insilicova-0.1.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.685387 insilicova-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 17:05:26.000000 insilicova-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 17:05:26.000000 insilicova-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-05 17:05:30.685387 insilicova-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-05 17:05:26.000000 insilicova-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-05 17:05:26.000000 insilicova-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:05:30.685387 insilicova-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-05 17:05:26.000000 insilicova-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.673387 insilicova-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.677387 insilicova-0.1.1/src/insilicova/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.677387 insilicova-0.1.1/src/insilicova/_sampler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47895 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/_sampler/sampler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    76716 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.685387 insilicova-0.1.1/src/insilicova/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/causetext.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/causetextV5.csv
--rw-r--r--   0 runner    (1001) docker     (127)    61954 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/condprob.csv
--rw-r--r--   0 runner    (1001) docker     (127)    74841 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/condprobnum.csv
--rw-r--r--   0 runner    (1001) docker     (127)    96815 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/probbase.csv
--rw-r--r--   0 runner    (1001) docker     (127)    96856 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/probbaseV3.csv
--rw-r--r--   0 runner    (1001) docker     (127)   164661 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/probbaseV5.csv
--rw-r--r--   0 runner    (1001) docker     (127)   944653 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/random_physician.csv
--rw-r--r--   0 runner    (1001) docker     (127)   912053 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/randomva1.csv
--rw-r--r--   0 runner    (1001) docker     (127)   925145 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/randomva2.csv
--rw-r--r--   0 runner    (1001) docker     (127)   286521 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/randomva5.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/sample_category.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/data/sample_physician.csv
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/diag.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24139 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/indiv.py
--rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-05 17:05:26.000000 insilicova-0.1.1/src/insilicova/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.685387 insilicova-0.1.1/src/insilicova.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-05 17:05:30.000000 insilicova-0.1.1/src/insilicova.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-05 17:05:30.000000 insilicova-0.1.1/src/insilicova.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:05:30.000000 insilicova-0.1.1/src/insilicova.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 17:05:30.000000 insilicova-0.1.1/src/insilicova.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 17:05:30.000000 insilicova-0.1.1/src/insilicova.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:05:30.685387 insilicova-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-05 17:05:26.000000 insilicova-0.1.1/tests/test_compare_r.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-05 17:05:26.000000 insilicova-0.1.1/tests/test_diag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-05 17:05:26.000000 insilicova-0.1.1/tests/test_indiv.py
--rw-r--r--   0 runner    (1001) docker     (127)    34028 2024-04-05 17:05:26.000000 insilicova-0.1.1/tests/test_insilicova.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:54:41.783724 insilicova-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 18:54:37.000000 insilicova-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 18:54:37.000000 insilicova-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-13 18:54:41.783724 insilicova-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-13 18:54:37.000000 insilicova-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-13 18:54:37.000000 insilicova-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:54:41.783724 insilicova-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-13 18:54:37.000000 insilicova-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:54:41.771724 insilicova-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:54:41.775724 insilicova-0.1.3/src/insilicova/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:54:41.775724 insilicova-0.1.3/src/insilicova/_sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47895 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/_sampler/sampler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    76980 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:54:41.783724 insilicova-0.1.3/src/insilicova/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/data/causetext.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/data/causetextV5.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    61954 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/data/condprob.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    74841 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/data/condprobnum.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    96815 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/data/probbase.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    96856 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/data/probbaseV3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   164661 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/data/probbaseV5.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   944653 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/data/random_physician.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   912053 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/data/randomva1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   925145 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/data/randomva2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   286521 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/data/randomva5.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/data/sample_category.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/data/sample_physician.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24139 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/indiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-13 18:54:37.000000 insilicova-0.1.3/src/insilicova/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:54:41.783724 insilicova-0.1.3/src/insilicova.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-13 18:54:41.000000 insilicova-0.1.3/src/insilicova.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-13 18:54:41.000000 insilicova-0.1.3/src/insilicova.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:54:41.000000 insilicova-0.1.3/src/insilicova.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 18:54:41.000000 insilicova-0.1.3/src/insilicova.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 18:54:41.000000 insilicova-0.1.3/src/insilicova.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:54:41.783724 insilicova-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-13 18:54:37.000000 insilicova-0.1.3/tests/test_compare_r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-13 18:54:37.000000 insilicova-0.1.3/tests/test_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-13 18:54:37.000000 insilicova-0.1.3/tests/test_indiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34028 2024-05-13 18:54:37.000000 insilicova-0.1.3/tests/test_insilicova.py
```

### Comparing `insilicova-0.1.1/LICENSE` & `insilicova-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/PKG-INFO` & `insilicova-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insilicova
-Version: 0.1.1
+Version: 0.1.3
 Summary: Python implementation of the InSilicoVA Algorithm.
 Author-email: Jason Thomas <jarathomas@gmail.com>, Sherry Zhao <zhao.3248@buckeyemail.osu.edu>
 Maintainer-email: Jason Thomas <jarathomas@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/verbal-autopsy-software/pyinsilicova
 Project-URL: Bug Tracker, https://github.com/verbal-autopsy-software/pyinsilicoVA/issues
 Keywords: verbal autopsy
```

### Comparing `insilicova-0.1.1/README.md` & `insilicova-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/pyproject.toml` & `insilicova-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 build-requires = [
     "virtual:compiler/cpp",
     "pkg:generic/boost",
 ]
 
 [project]
 name = "insilicova"
-version = "0.1.1"
+version = "0.1.3"
 authors = [
     {name = "Jason Thomas", email = "jarathomas@gmail.com"},
     {name = "Sherry Zhao", email =" zhao.3248@buckeyemail.osu.edu"},
 ]
 maintainers = [
     {name = "Jason Thomas", email = "jarathomas@gmail.com"},
 ]
```

### Comparing `insilicova-0.1.1/setup.py` & `insilicova-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/_sampler/sampler.cpp` & `insilicova-0.1.3/src/insilicova/_sampler/sampler.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -392,19 +392,19 @@
             int idx = s*C + c;
             if (s == 0) ptr_count_c[c] = 0;
             ptr_count_m[idx] = 0;
             ptr_count_m_all[idx] = 0;
         }
     }
 
-    // loop over all inidviduals
+    // loop over all individuals
     for (int n = 0; n < N; ++n) {
         // cause of this death
         int c_current = (int) y_new(n);
-        // add to toal counts
+        // add to total counts
         ptr_count_c[c_current] += 1;
         // loop over all symptoms
         for (int s = 0; s < S; ++s) {
             // add to counts of this symptom's appearance
             int idx = s*C + c_current;
             if (ptr_indic[n*S + s] == 1) {
                 ptr_count_m[idx] += 1;
@@ -511,15 +511,15 @@
                     // for (int i : levels_under_s[l_prev]) {
                     py::list levels_under_s_l_prev = levels_under_s[py::cast(l_prev)];
                     for (auto i : levels_under_s_l_prev) {
                         if (proxy_new_pbase(s, i.cast<int>()) < upper) upper = proxy_new_pbase(s, i.cast<int>());
                     }
                     upper = std::min(upper, trunc_max);
                 }
-                // if range is invalide, use higher case
+                // if range is invalid, use higher case
                 if (lower >= upper) {
                     proxy_new_pbase(s, c.cast<int>()) = upper;
                 } else {
                     // find the beta distribution parameters, note level starting from 1
                     a = proxy_prior_a(l_current-1) + count;
                     b = prior_b + count_all - a;
                     proxy_new_pbase(s, c.cast<int>()) = sample_trunc_beta(a, b, lower, upper);
@@ -613,15 +613,15 @@
                     // for (int i : levels_under_c[l_prev]) {
                     py::list levels_under_c_l_prev = levels_under_c[py::cast(l_prev)];
                     for (auto i : levels_under_c_l_prev) {
                         if (proxy_new_pbase(i.cast<int>(), c) < upper) upper = proxy_new_pbase(i.cast<int>(), c);
                     }
                     upper = std::min(upper, trunc_max);
                 }
-                // if range is invalide, use higher case
+                // if range is invalid, use higher case
                 if (lower >= upper) {
                     proxy_new_pbase(s.cast<int>(), c) = upper;
                 } else {
                     // find the beta distribution parameters, note level starting from 1
                     a = proxy_prior_a(l_current-1) + count;
                     b = prior_b + count_all - a;
                     proxy_new_pbase(s.cast<int>(), c) = sample_trunc_beta(a, b, lower, upper);
@@ -889,15 +889,15 @@
         for (int i = 0; i < N_sub; ++i) {
             for (int j = 0; j < C; ++j) {
                 zero_group_matrix(i, j) = 1;
             }
         }       
     }
 
-    // reinitiate after checking impossible
+    // re-initiate after checking impossible
     if (!is_added) {
         for (int sub = 0; sub < N_sub; ++sub) {
             int fix = 0;
             for (int c = 1; c < C; ++c) {
                 if (zero_group_matrix(sub, c) > 0) {
                     fix = c;
                     break;
```

### Comparing `insilicova-0.1.1/src/insilicova/api.py` & `insilicova-0.1.3/src/insilicova/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -910,17 +910,22 @@
         n_iterations = self.data.shape[1] - 1  # ignore ID column
         for i in range(n_iterations):
             # increment index by 1 for data (but not for _probbase!)
             if all(self.data.iloc[:, (i + 1)] == "."):
                 self._missing_all.append(i)
         if len(self._missing_all) > 0:
             missing_all_plus1 = np.array(self._missing_all) + 1
+            pb_no_ext = np.delete(self._probbase,
+                                  self._external_symps,
+                                  axis=0)
             missing_all_names = ", ".join(
-                self._probbase[missing_all_plus1,
-                               int(self.data_type == "WHO2012")])
+                # self._probbase[missing_all_plus1,
+                #                int(self.data_type == "WHO2012")])
+                pb_no_ext[missing_all_plus1,
+                          int(self.data_type == "WHO2012")])
             warnings.warn(f"{len(self._missing_all)} symptoms missing "
                           "completely and added to missing list. \n List of "
                           f"missing symptoms: {missing_all_names}\n",
                           UserWarning)
             drop_col_names = list(self.data.iloc[:, missing_all_plus1])
             self.data.drop(columns=drop_col_names, inplace=True)
             self._prob_orig = np.delete(self._prob_orig,
@@ -1318,15 +1323,14 @@
         C_phy = self._c_phy
         broader = self._va_causes_broader
         assignment = self._assignment
         impossible = self._impossible
         N_thin = int((N_gibbs - burn) / (thin))
         probbase_gibbs = np.zeros((N_thin, S, C))
         levels_gibbs = np.zeros((N_thin, N_level))
-        pnb_mean = np.zeros((N, C))
         p_gibbs = np.zeros((N_thin, N_sub, C))
         pnb_mean = np.zeros((N, C))
         naccept = [0] * N_sub
         mu_now = np.zeros((N_sub, C))
         sigma2_now = [None] * N_sub
         theta_now = np.zeros((N_sub, C))
         p_now = np.zeros((N_sub, C))  # csmf_sub
@@ -1387,18 +1391,19 @@
                 theta_continue = results["theta_last"]
                 # same length as previous chain if added the first time
                 # double the length if the second time
                 # self.n_sim = self.n_sim * 2
                 # self.burnin = self.n_sim / 2
                 N_gibbs = int(np.trunc(N_gibbs * (2 ** (add - 1))))
                 burn = 0
-                N_thin = int((N_gibbs - burn) / (thin))
+                N_thin = int((N_gibbs - burn) / thin)
                 probbase_gibbs = np.zeros((N_thin, S, C))
                 levels_gibbs = np.zeros((N_thin, N_level))
                 p_gibbs = np.zeros((N_thin, N_sub, C))
+                pnb_mean = np.zeros((N, C))
                 warnings.warn(
                     f"Not all causes with CSMF > {self.conv_csmf} are "
                     f"convergent.\n Increase chain length with another "
                     f"{N_gibbs} iterations.\n")
                 N_out = (1 + N_sub * C * N_thin +
                          N * C + N_sub * (C * 2 + 1))
                 if pool == 0:
```

### Comparing `insilicova-0.1.1/src/insilicova/data/causetext.csv` & `insilicova-0.1.3/src/insilicova/data/causetext.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/data/causetextV5.csv` & `insilicova-0.1.3/src/insilicova/data/causetextV5.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/data/condprob.csv` & `insilicova-0.1.3/src/insilicova/data/condprob.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/data/condprobnum.csv` & `insilicova-0.1.3/src/insilicova/data/condprobnum.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/data/probbase.csv` & `insilicova-0.1.3/src/insilicova/data/probbase.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/data/probbaseV3.csv` & `insilicova-0.1.3/src/insilicova/data/probbaseV3.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/data/probbaseV5.csv` & `insilicova-0.1.3/src/insilicova/data/probbaseV5.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/data/random_physician.csv` & `insilicova-0.1.3/src/insilicova/data/random_physician.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/data/randomva1.csv` & `insilicova-0.1.3/src/insilicova/data/randomva1.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/data/randomva2.csv` & `insilicova-0.1.3/src/insilicova/data/randomva2.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/data/randomva5.csv` & `insilicova-0.1.3/src/insilicova/data/randomva5.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/data/sample_category.csv` & `insilicova-0.1.3/src/insilicova/data/sample_category.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/data/sample_physician.csv` & `insilicova-0.1.3/src/insilicova/data/sample_physician.csv`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/diag.py` & `insilicova-0.1.3/src/insilicova/diag.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/exceptions.py` & `insilicova-0.1.3/src/insilicova/exceptions.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/indiv.py` & `insilicova-0.1.3/src/insilicova/indiv.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/structures.py` & `insilicova-0.1.3/src/insilicova/structures.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova/utils.py` & `insilicova-0.1.3/src/insilicova/utils.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/src/insilicova.egg-info/PKG-INFO` & `insilicova-0.1.3/src/insilicova.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insilicova
-Version: 0.1.1
+Version: 0.1.3
 Summary: Python implementation of the InSilicoVA Algorithm.
 Author-email: Jason Thomas <jarathomas@gmail.com>, Sherry Zhao <zhao.3248@buckeyemail.osu.edu>
 Maintainer-email: Jason Thomas <jarathomas@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/verbal-autopsy-software/pyinsilicova
 Project-URL: Bug Tracker, https://github.com/verbal-autopsy-software/pyinsilicoVA/issues
 Keywords: verbal autopsy
```

### Comparing `insilicova-0.1.1/src/insilicova.egg-info/SOURCES.txt` & `insilicova-0.1.3/src/insilicova.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/tests/test_compare_r.py` & `insilicova-0.1.3/tests/test_compare_r.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/tests/test_diag.py` & `insilicova-0.1.3/tests/test_diag.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/tests/test_indiv.py` & `insilicova-0.1.3/tests/test_indiv.py`

 * *Files identical despite different names*

### Comparing `insilicova-0.1.1/tests/test_insilicova.py` & `insilicova-0.1.3/tests/test_insilicova.py`

 * *Files identical despite different names*

