# Comparing `tmp/schubertpy-0.3.21.tar.gz` & `tmp/schubertpy-0.3.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubertpy-0.3.21.tar", last modified: Wed May  8 14:02:21 2024, max compression
+gzip compressed data, was "schubertpy-0.3.22.tar", last modified: Mon May 13 10:25:50 2024, max compression
```

## Comparing `schubertpy-0.3.21.tar` & `schubertpy-0.3.22.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-08 14:02:21.976234 schubertpy-0.3.21/
--rw-r--r--   0 tranduythanh   (501) staff       (20)    35147 2024-04-29 08:09:23.000000 schubertpy-0.3.21/LICENSE
--rw-r--r--   0 tranduythanh   (501) staff       (20)     7432 2024-05-08 14:02:21.976127 schubertpy-0.3.21/PKG-INFO
--rw-r--r--   0 tranduythanh   (501) staff       (20)     6891 2024-05-08 13:57:52.000000 schubertpy-0.3.21/README.md
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-08 14:02:21.973930 schubertpy-0.3.21/schubertpy/
--rw-r--r--   0 tranduythanh   (501) staff       (20)      377 2024-02-13 13:37:36.000000 schubertpy-0.3.21/schubertpy/__init__.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     6220 2024-04-26 02:35:10.000000 schubertpy-0.3.21/schubertpy/abstract_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      175 2024-05-06 06:28:22.000000 schubertpy-0.3.21/schubertpy/const.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      942 2024-02-13 13:40:38.000000 schubertpy-0.3.21/schubertpy/csv_bijection.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     4806 2024-02-13 13:40:53.000000 schubertpy-0.3.21/schubertpy/grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     4714 2024-02-13 13:40:49.000000 schubertpy-0.3.21/schubertpy/isotropic_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     9213 2024-05-06 06:50:44.000000 schubertpy-0.3.21/schubertpy/lc.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)    12445 2024-02-13 13:41:11.000000 schubertpy-0.3.21/schubertpy/orthogonal_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     3059 2024-02-13 13:42:18.000000 schubertpy-0.3.21/schubertpy/partition.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)    40455 2024-04-27 02:11:49.000000 schubertpy-0.3.21/schubertpy/qcalc.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     3239 2024-05-06 06:20:18.000000 schubertpy-0.3.21/schubertpy/schur.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      203 2024-02-13 13:41:38.000000 schubertpy-0.3.21/schubertpy/util.py
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-08 14:02:21.975734 schubertpy-0.3.21/schubertpy.egg-info/
--rw-r--r--   0 tranduythanh   (501) staff       (20)     7432 2024-05-08 14:02:21.000000 schubertpy-0.3.21/schubertpy.egg-info/PKG-INFO
--rw-r--r--   0 tranduythanh   (501) staff       (20)      566 2024-05-08 14:02:21.000000 schubertpy-0.3.21/schubertpy.egg-info/SOURCES.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)        1 2024-05-08 14:02:21.000000 schubertpy-0.3.21/schubertpy.egg-info/dependency_links.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)       28 2024-05-08 14:02:21.000000 schubertpy-0.3.21/schubertpy.egg-info/requires.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)       24 2024-05-08 14:02:21.000000 schubertpy-0.3.21/schubertpy.egg-info/top_level.txt
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-08 14:02:21.975394 schubertpy-0.3.21/schubertsage/
--rw-r--r--   0 tranduythanh   (501) staff       (20)      304 2024-02-14 06:03:50.000000 schubertpy-0.3.21/schubertsage/__init__.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      793 2024-02-14 06:36:52.000000 schubertpy-0.3.21/schubertsage/conversion.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      132 2024-05-08 14:02:21.976608 schubertpy-0.3.21/setup.cfg
--rw-r--r--   0 tranduythanh   (501) staff       (20)     2038 2024-05-08 14:02:21.000000 schubertpy-0.3.21/setup.py
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-13 10:25:50.100387 schubertpy-0.3.22/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    35147 2024-04-29 08:09:23.000000 schubertpy-0.3.22/LICENSE
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     7549 2024-05-13 10:25:50.100306 schubertpy-0.3.22/PKG-INFO
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     7008 2024-05-09 12:02:43.000000 schubertpy-0.3.22/README.md
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-13 10:25:50.098635 schubertpy-0.3.22/schubertpy/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      458 2024-05-13 09:56:13.000000 schubertpy-0.3.22/schubertpy/__init__.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     6589 2024-05-13 10:18:04.000000 schubertpy-0.3.22/schubertpy/abstract_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      175 2024-05-06 06:28:22.000000 schubertpy-0.3.22/schubertpy/const.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      942 2024-02-13 13:40:38.000000 schubertpy-0.3.22/schubertpy/csv_bijection.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     4806 2024-02-13 13:40:53.000000 schubertpy-0.3.22/schubertpy/grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     4714 2024-02-13 13:40:49.000000 schubertpy-0.3.22/schubertpy/isotropic_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    11806 2024-05-13 10:14:25.000000 schubertpy-0.3.22/schubertpy/lc.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     2911 2024-05-13 10:14:42.000000 schubertpy-0.3.22/schubertpy/mult_table.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    12445 2024-02-13 13:41:11.000000 schubertpy-0.3.22/schubertpy/orthogonal_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     3656 2024-05-13 09:11:53.000000 schubertpy-0.3.22/schubertpy/partition.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    40154 2024-05-13 08:20:38.000000 schubertpy-0.3.22/schubertpy/qcalc.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     3443 2024-05-13 09:11:03.000000 schubertpy-0.3.22/schubertpy/schur.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      203 2024-05-13 08:49:00.000000 schubertpy-0.3.22/schubertpy/util.py
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-13 10:25:50.099914 schubertpy-0.3.22/schubertpy.egg-info/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     7549 2024-05-13 10:25:50.000000 schubertpy-0.3.22/schubertpy.egg-info/PKG-INFO
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      591 2024-05-13 10:25:50.000000 schubertpy-0.3.22/schubertpy.egg-info/SOURCES.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)        1 2024-05-13 10:25:50.000000 schubertpy-0.3.22/schubertpy.egg-info/dependency_links.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)       28 2024-05-13 10:25:50.000000 schubertpy-0.3.22/schubertpy.egg-info/requires.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)       24 2024-05-13 10:25:50.000000 schubertpy-0.3.22/schubertpy.egg-info/top_level.txt
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-13 10:25:50.099736 schubertpy-0.3.22/schubertsage/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      304 2024-02-14 06:03:50.000000 schubertpy-0.3.22/schubertsage/__init__.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      793 2024-02-14 06:36:52.000000 schubertpy-0.3.22/schubertsage/conversion.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      132 2024-05-13 10:25:50.100738 schubertpy-0.3.22/setup.cfg
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     2038 2024-05-13 10:25:49.000000 schubertpy-0.3.22/setup.py
```

### Comparing `schubertpy-0.3.21/LICENSE` & `schubertpy-0.3.22/LICENSE`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.21/PKG-INFO` & `schubertpy-0.3.22/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubertpy
-Version: 0.3.21
+Version: 0.3.22
 Summary: This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes
 Home-page: https://github.com/tranduythanh/schubertpy
 Author: Trần Duy Thanh
 Author-email: fbtranduythanh@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -166,7 +166,11 @@
 - **Submit Pull Requests**: Feel free to fork the repository and submit pull requests. Whether it's adding new features, optimizing existing code, or correcting bugs, your contributions are welcome.
 
 Please ensure your pull requests are well-documented and include any necessary tests. For more details on contributing, refer to our contribution guidelines on GitHub.
 
 ## License
 
 `schubertpy` is open source software (under the GNU General Public License).
+
+## Citing
+
+We encourage you to cite our work if you have used our package. See "Cite this repository" on this page.
```

### Comparing `schubertpy-0.3.21/README.md` & `schubertpy-0.3.22/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -153,7 +153,11 @@
 - **Submit Pull Requests**: Feel free to fork the repository and submit pull requests. Whether it's adding new features, optimizing existing code, or correcting bugs, your contributions are welcome.
 
 Please ensure your pull requests are well-documented and include any necessary tests. For more details on contributing, refer to our contribution guidelines on GitHub.
 
 ## License
 
 `schubertpy` is open source software (under the GNU General Public License).
+
+## Citing
+
+We encourage you to cite our work if you have used our package. See "Cite this repository" on this page.
```

### Comparing `schubertpy-0.3.21/schubertpy/abstract_grassmannian.py` & `schubertpy-0.3.22/schubertpy/abstract_grassmannian.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+from typing import *
 from .qcalc import *
 
 class AbstractGrassmannian(ABC):
     def __init__(self, m: int, n:int):
         self._type = None
         self._k = None
         self._n = None
@@ -110,17 +111,26 @@
     def qgiambelli(self, lc: Union[sp.Expr, LinearCombination, str]) -> LinearCombination:
         # print("qgiambelli")
         lc = LinearCombination(lc)
         # print("lc: ", lc)
         return giambelli_rec(lc, lambda i, p: self._qpieri(i, p, self._k, self._n), self._k)
 
 
-    def qmult(self, lc1: Union[sp.Expr, LinearCombination, str], lc2: Union[sp.Expr, LinearCombination, str]) -> LinearCombination:
+    def qmult(
+        self, 
+        lc1: Union[sp.Expr, LinearCombination, str, Schur, List[int]], 
+        lc2: Union[sp.Expr, LinearCombination, str, Schur, List[int]],
+    ) -> LinearCombination:
+        
         lc1 = LinearCombination(lc1)
         lc2 = LinearCombination(lc2)
+        # if lc1.has_part_zero_padding():
+        #     raise ValueError("The 1st input param contains a partition with zero padding")
+        # if lc2.has_part_zero_padding():
+        #     raise ValueError("The 2nd input param contains a partition with zero padding")
         # print("qmult")
         # print("lc1: ", lc1)
         # print("lc2: ", lc2)
         return self.qact(self.qgiambelli(lc1), lc2)
 
 
     def qtoS(self, lc: Union[sp.Expr, LinearCombination, str]) -> LinearCombination:
```

### Comparing `schubertpy-0.3.21/schubertpy/csv_bijection.py` & `schubertpy-0.3.22/schubertpy/csv_bijection.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.21/schubertpy/grassmannian.py` & `schubertpy-0.3.22/schubertpy/grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.21/schubertpy/isotropic_grassmannian.py` & `schubertpy-0.3.22/schubertpy/isotropic_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.21/schubertpy/lc.py` & `schubertpy-0.3.22/schubertpy/lc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,39 @@
-from functools import total_ordering
 from typing import *
-from .schur import *
-from .const import *
 import sympy as sp
-import ast
+import pandas as pd
+
+from .partition import *
+from .schur import Schur, isSchur, toSchur, translate_schur
+from .const import *
 
 
 class LinearCombination(object):
-    def __init__(self, expr: Union[str, sp.Expr, int, 'LinearCombination']):
+    def __init__(self, expr: Union[str, sp.Expr, int, 'LinearCombination', 'Schur', List[int]]):
+        if isinstance(expr, list) and is_valid_part(expr):
+            self.expr = Schur(expr).symbol()
+            return
+        if isinstance(expr, Schur):
+            self.expr = Schur(expr).symbol()
+            return
         if isinstance(expr, str):
             expr = expr.replace('^', '**')
             expr = expr.translate(ftable)
             self.expr = sp.parse_expr(expr)
-        elif isinstance(expr, (sp.Expr, sp.Number, sp.Symbol)):
+            return
+        if isinstance(expr, (sp.Expr, sp.Number, sp.Symbol)):
             self.expr = expr
-        elif isinstance(expr, (int, float)):
+            return
+        if isinstance(expr, (int, float)):
             self.expr = sp.sympify(expr)
-        elif isinstance(expr, LinearCombination):
+            return
+        if isinstance(expr, LinearCombination):
             self.expr = expr.expr
-        else:
-            raise ValueError(f"Invalid type for LinearCombination: {type(expr)}")
+            return
+        raise ValueError(f"Invalid type for LinearCombination: {type(expr)}")
 
     def __str__(self):
         return translate_schur(self.expr).replace('**', '^')
 
     def __repr__(self):
         return self.__str__()
     
@@ -95,16 +105,16 @@
             return isinstance(self.expr, sp.Mul)
         elif op == '^':
             return isinstance(self.expr, sp.Pow)
         
         raise ValueError(f"Invalid operator: {op}")
     
 
-    def list_schur_oprands(self) -> List[Schur]:
-        def recursive_list(expr: sp.Expr) -> List[Schur]:
+    def list_schur_oprands(self) -> List['Schur']:
+        def recursive_list(expr: sp.Expr) -> List['Schur']:
             if expr.is_Add or expr.is_Mul or expr.is_Pow:
                 return [recursive_list(arg) for arg in expr.args]
             if isSchur(expr):
                 return toSchur(str(expr))
             return None
         
         return recursive_list(self.expr)
@@ -138,14 +148,27 @@
             
             # print("case3: ", _expr)
             return _expr
         
         new_expr = recursive_apply(self.expr)
         return LinearCombination(str(new_expr))
     
+    def has_part_zero_padding(self) -> bool:
+        """
+        Check if the expression has zero padding in the partition.
+        """
+        def recursive_has_part_zero_padding(_expr: sp.Expr) -> bool:
+            if _expr.is_Add or _expr.is_Mul or _expr.is_Pow:
+                return any(recursive_has_part_zero_padding(arg) for arg in _expr.args)
+            if isSchur(_expr):
+                return Schur(_expr).has_part_zero_padding()
+            return False
+        
+        return recursive_has_part_zero_padding(self.expr)
+
     def is_valid(self) -> bool:
         """
         Check if the expression is a linear combination.
         This version considers an expression linear if it involves only:
         - Scalar multiplication (a number multiplied by an expression).
         - Addition or subtraction of linear terms.
         """
@@ -189,14 +212,40 @@
                 raise ValueError(f"Schur function absent or not in order 1: {expr}")
             s = ss[0]
             return (LinearCombination(new_expr), Schur(s).partition())
         raise ValueError(f"Invalid type for cutoff Schur: {expr}")
     
 
     def _schur_expansion(self, expr, include_q=True) -> 'LinearCombination':
+        """
+        Perform the Schur expansion of an expression.
+
+        This method attempts to expand an expression into its Schur components. It handles
+        numbers, Schur functions, and products of expressions. If the expression is a sum,
+        it expands each term individually. The method can optionally exclude terms containing
+        the variable 'q' from the expansion.
+
+        Parameters:
+        - expr: sp.Expr
+            The sympy expression to be expanded into Schur components.
+        - include_q: bool, optional (default=True)
+            A flag indicating whether terms containing the variable 'q' should be included
+            in the expansion.
+
+        Returns:
+        - A list of tuples, where each tuple contains a coefficient and a list
+        representing the partition of a Schur function, or raises a ValueError if the
+        expression cannot be expanded into Schur components.
+
+        Raises:
+        - ValueError
+            If the expression contains a product with multiple Schur functions (which cannot
+            be directly converted to a Schur expansion without prior expansion), or if the
+            expression type is not supported for Schur expansion.
+        """
         if isinstance(expr, sp.Number):
             return (int(expr),[])
         if isSchur(expr):
             return (1, toSchur(str(expr)).partition())
         if isinstance(expr, sp.Mul):
             if self._count_Schur(expr) > 1:
                 raise ValueError(f"Cannot convert a product with multiple Schur functions to schur_expansion. Please expand the expression first: {self.expr}")
@@ -212,10 +261,22 @@
             sorted_array = sorted(res, key=lambda x: x[1])
             return sorted_array
         raise ValueError(f"Invalid type for schur_expansion: {self.expr}")
 
     def schur_expansion(self, include_q=True) -> 'LinearCombination':
         """
         Expand each term in the expression individually.
-        This method assumes that the expression is a polynomial and expands each term separately.
+        This method assumes that the expression is sum of terms.
+
+        Parameters:
+        - expr: sp.Expr
+            The sympy expression to be expanded into Schur components.
+        - include_q: bool, optional (default=True)
+            A flag indicating whether terms containing the variable 'q' should be included
+            in the expansion.
+
+        Returns:
+        - A list of tuples, where each tuple contains a coefficient and a list
+        representing the partition of a Schur function, or raises a ValueError if the
+        expression cannot be expanded into Schur components.
         """
-        return self._schur_expansion(self.expr, include_q)
+        return self._schur_expansion(self.expr, include_q)
```

### Comparing `schubertpy-0.3.21/schubertpy/orthogonal_grassmannian.py` & `schubertpy-0.3.22/schubertpy/orthogonal_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.21/schubertpy/partition.py` & `schubertpy-0.3.22/schubertpy/partition.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,30 @@
-import numpy as np
-import sympy as sp
 from collections import OrderedDict
 from typing import *
 from .util import *
-from .schur import *
-from .lc import *
+
+def _is_sorted_descending(part: List[int]):
+    # Iterate through the list, comparing each element with the next one
+    for i in range(len(part) - 1):
+        # If the current element is smaller than the next one,
+        # the list is not in descending order
+        if part[i] < part[i + 1]:
+            return False
+    return True
+
+def is_valid_part(part: List[int]) -> bool:
+    if not isinstance(part, list):
+        return False
+    if not all(isinstance(x, int) for x in part):
+        return False
+    if not all(x >= 0 for x in part):
+        return False
+    if not _is_sorted_descending(part):
+        return False
+    return True
 
 def _first_kstrict(k: int, rows: int, cols: int) -> List[int]:
     return [max(k, cols - i) for i in range(rows)]
 
 
 def _itr_kstrict(lambda_: List[int], k: int) -> Optional[List[int]]:
     n = len(lambda_)
@@ -30,14 +46,15 @@
         return lambda_[:i-1] + [li - j for j in range(li - k + 1)] + [k] * (n - i - li + k)
 
 
 def part_clip(lambda_: List[int]) -> List[int]:
     '''
     trims or removes trailing zeros from the list lambda.
     '''
+    lambda_ = lambda_.copy()
     i = len(lambda_) - 1
     while i >= 0 and lambda_[i] == 0:
         i -= 1
     return lambda_[:i+1] if i >= 0 else []
 
 def all_kstrict(k: int, rows: int, cols: int) -> Set[Tuple[int, ...]]:
     res = []
```

### Comparing `schubertpy-0.3.21/schubertpy/qcalc.py` & `schubertpy-0.3.22/schubertpy/qcalc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1316,23 +1316,14 @@
 def qgiambelli(lc: Union[sp.Expr, LinearCombination, str]) -> LinearCombination:
     # print("qgiambelli")
     lc = LinearCombination(lc)
     # print("lc: ", lc)
     return giambelli_rec(lc, lambda i, p: _qpieri(i, p, _k, _n), _k)
 
 
-def qmult(lc1: Union[sp.Expr, LinearCombination, str], lc2: Union[sp.Expr, LinearCombination, str]) -> LinearCombination:
-    lc1 = LinearCombination(lc1)
-    lc2 = LinearCombination(lc2)
-    # print("qmult")
-    # print("lc1: ", lc1)
-    # print("lc2: ", lc2)
-    return qact(qgiambelli(lc1), lc2)
-
-
 def qtoS(lc: Union[sp.Expr, LinearCombination, str]) -> LinearCombination:
     # print("qtoS")
     lc = LinearCombination(lc)
     return qact(qgiambelli(lc).expr, LinearCombination(Schur([]).symbol()))
 
 pieri_fillA = _pieri_fillA
 pieri_itrA = _pieri_itrA
```

### Comparing `schubertpy-0.3.21/schubertpy/schur.py` & `schubertpy-0.3.22/schubertpy/schur.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from functools import total_ordering
 
 from typing import *
 import sympy as sp
 from .const import *
+from .partition import *
 import ast
 
 class Schur(object):
-    def __init__(self, p: Union[List[int], sp.Expr, str]):
+    def __init__(self, p: Union[List[int], sp.Expr, str, 'Schur']):
         # Set self.p to p or [] if p is None
         if isinstance(p, (list, tuple)):
             self.p = p if p is not None else []
             return
+        if isinstance(p, Schur):
+            self.p = p.p
+            return
         p = toSchur(p)
         self.p = p.p
 
     def __str__(self):
         return f"S{self.p}".replace(' ', '')
 
     def __repr__(self):
@@ -68,14 +72,17 @@
         raise ValueError(f"Invalid type for addition: {type(other)}")
 
     def symbol(self) -> sp.Symbol:
         return sp.parse_expr(self.__str__().translate(ftable))
 
     def partition(self) -> List[int]:
         return self.p
+    
+    def has_part_zero_padding(self) -> bool:
+        return part_clip(self.p) != self.p
 
 
 def unique_schur_list(schur_list: List[Schur]):
     return  sorted(list(set(schur_list)))
```

### Comparing `schubertpy-0.3.21/schubertpy.egg-info/PKG-INFO` & `schubertpy-0.3.22/schubertpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubertpy
-Version: 0.3.21
+Version: 0.3.22
 Summary: This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes
 Home-page: https://github.com/tranduythanh/schubertpy
 Author: Trần Duy Thanh
 Author-email: fbtranduythanh@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -166,7 +166,11 @@
 - **Submit Pull Requests**: Feel free to fork the repository and submit pull requests. Whether it's adding new features, optimizing existing code, or correcting bugs, your contributions are welcome.
 
 Please ensure your pull requests are well-documented and include any necessary tests. For more details on contributing, refer to our contribution guidelines on GitHub.
 
 ## License
 
 `schubertpy` is open source software (under the GNU General Public License).
+
+## Citing
+
+We encourage you to cite our work if you have used our package. See "Cite this repository" on this page.
```

### Comparing `schubertpy-0.3.21/schubertpy.egg-info/SOURCES.txt` & `schubertpy-0.3.22/schubertpy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 schubertpy/__init__.py
 schubertpy/abstract_grassmannian.py
 schubertpy/const.py
 schubertpy/csv_bijection.py
 schubertpy/grassmannian.py
 schubertpy/isotropic_grassmannian.py
 schubertpy/lc.py
+schubertpy/mult_table.py
 schubertpy/orthogonal_grassmannian.py
 schubertpy/partition.py
 schubertpy/qcalc.py
 schubertpy/schur.py
 schubertpy/util.py
 schubertpy.egg-info/PKG-INFO
 schubertpy.egg-info/SOURCES.txt
```

### Comparing `schubertpy-0.3.21/schubertsage/conversion.py` & `schubertpy-0.3.22/schubertsage/conversion.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.21/setup.py` & `schubertpy-0.3.22/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 # Define package metadata
 package_name = 'schubertpy'
-package_version = '0.3.21'
+package_version = '0.3.22'
 package_author = 'Trần Duy Thanh'
 package_author_email = 'fbtranduythanh@gmail.com'
 package_url = 'https://github.com/tranduythanh/schubertpy'
 package_description = 'This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes'
 package_license = 'GNU General Public License'
 
 # Generate CITATION.cff content
```

