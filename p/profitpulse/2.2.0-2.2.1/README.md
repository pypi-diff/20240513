# Comparing `tmp/profitpulse-2.2.0.tar.gz` & `tmp/profitpulse-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profitpulse-2.2.0.tar", max compression
+gzip compressed data, was "profitpulse-2.2.1.tar", max compression
```

## Comparing `profitpulse-2.2.0.tar` & `profitpulse-2.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-2.2.0/LICENSE
--rw-r--r--   0        0        0     1075 2024-05-04 13:05:41.429315 profitpulse-2.2.0/README.md
--rw-r--r--   0        0        0     1839 2024-05-12 19:40:15.676088 profitpulse-2.2.0/pyproject.toml
--rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-2.2.0/src/profitpulse/__init__.py
--rw-r--r--   0        0        0        0 2024-05-04 13:54:47.669161 profitpulse-2.2.0/src/profitpulse/cli/__init__.py
--rw-r--r--   0        0        0     8195 2024-05-12 19:23:02.361097 profitpulse-2.2.0/src/profitpulse/cli/adapters.py
--rw-r--r--   0        0        0     4941 2024-05-12 19:25:34.206898 profitpulse-2.2.0/src/profitpulse/cli/main.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-2.2.0/src/profitpulse/data/__init__.py
--rw-r--r--   0        0        0     4533 2024-05-12 18:13:22.497175 profitpulse-2.2.0/src/profitpulse/data/assets.py
--rw-r--r--   0        0        0     2409 2024-05-10 06:54:12.883293 profitpulse-2.2.0/src/profitpulse/data/assets_test.py
--rw-r--r--   0        0        0      360 2024-05-10 06:54:12.884114 profitpulse-2.2.0/src/profitpulse/data/data.py
--rw-r--r--   0        0        0     1852 2024-05-12 19:36:31.054109 profitpulse-2.2.0/src/profitpulse/data/expenses_view.py
--rw-r--r--   0        0        0     3191 2024-05-12 19:25:34.189395 profitpulse-2.2.0/src/profitpulse/data/expenses_view_test.py
--rw-r--r--   0        0        0     2149 2024-05-10 06:54:12.885295 profitpulse-2.2.0/src/profitpulse/data/pulse_view.py
--rw-r--r--   0        0        0     3057 2024-05-10 06:54:12.885866 profitpulse-2.2.0/src/profitpulse/data/pulse_view_test.py
--rw-r--r--   0        0        0     1628 2024-05-12 17:04:21.964654 profitpulse-2.2.0/src/profitpulse/data/views.py
--rw-r--r--   0        0        0     1033 2024-05-12 17:04:21.965124 profitpulse-2.2.0/src/profitpulse/data/views_test.py
--rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-2.2.0/src/profitpulse/gateways/__init__.py
--rw-r--r--   0        0        0     3188 2024-05-05 20:11:25.598621 profitpulse-2.2.0/src/profitpulse/gateways/cgdfile.py
--rw-r--r--   0        0        0     2030 2024-05-05 19:43:17.281923 profitpulse-2.2.0/src/profitpulse/gateways/cgdfile_test.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-2.2.0/src/profitpulse/infrastructure/__init__.py
--rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-2.2.0/src/profitpulse/infrastructure/migrations.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-2.2.0/src/profitpulse/lib/__init__.py
--rw-r--r--   0        0        0     1962 2024-05-10 06:54:12.888068 profitpulse-2.2.0/src/profitpulse/lib/asset.py
--rw-r--r--   0        0        0      541 2024-05-07 20:15:15.902011 profitpulse-2.2.0/src/profitpulse/lib/asset_name.py
--rw-r--r--   0        0        0      493 2024-04-27 17:48:38.579236 profitpulse-2.2.0/src/profitpulse/lib/comment.py
--rw-r--r--   0        0        0      964 2024-05-10 06:54:12.889055 profitpulse-2.2.0/src/profitpulse/lib/money.py
--rw-r--r--   0        0        0      232 2024-05-04 22:12:33.559763 profitpulse-2.2.0/src/profitpulse/lib/transaction.py
--rw-r--r--   0        0        0      956 2024-05-12 18:30:01.306766 profitpulse-2.2.0/src/profitpulse/migrations/0001 - Initial.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-2.2.0/src/profitpulse/migrations/0002 - accounts.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-2.2.0/src/profitpulse/migrations/__init__.py
--rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-2.2.0/src/profitpulse/services/__init__.py
--rw-r--r--   0        0        0     1468 2024-05-10 06:54:12.890186 profitpulse-2.2.0/src/profitpulse/services/acquire_asset.py
--rw-r--r--   0        0        0     1636 2024-05-10 06:54:12.891286 profitpulse-2.2.0/src/profitpulse/services/acquire_asset_test.py
--rw-r--r--   0        0        0     1298 2024-05-10 06:54:12.892139 profitpulse-2.2.0/src/profitpulse/services/delete_asset.py
--rw-r--r--   0        0        0     1475 2024-05-10 06:54:12.892714 profitpulse-2.2.0/src/profitpulse/services/delete_asset_test.py
--rw-r--r--   0        0        0     1888 2024-05-10 06:54:12.893192 profitpulse-2.2.0/src/profitpulse/services/deposit_into_asset.py
--rw-r--r--   0        0        0     2680 2024-05-10 06:54:12.893995 profitpulse-2.2.0/src/profitpulse/services/deposit_into_asset_test.py
--rw-r--r--   0        0        0     1428 2024-05-10 06:54:12.894591 profitpulse-2.2.0/src/profitpulse/services/divest_asset.py
--rw-r--r--   0        0        0     1611 2024-05-10 06:54:12.895330 profitpulse-2.2.0/src/profitpulse/services/divest_asset_test.py
--rw-r--r--   0        0        0      285 2024-05-07 20:15:15.913869 profitpulse-2.2.0/src/profitpulse/services/errors.py
--rw-r--r--   0        0        0     1446 2024-05-12 18:43:49.634734 profitpulse-2.2.0/src/profitpulse/services/import_transactions.py
--rw-r--r--   0        0        0     1609 2024-05-10 06:54:12.896794 profitpulse-2.2.0/src/profitpulse/services/revalue_asset.py
--rw-r--r--   0        0        0     1625 2024-05-10 06:54:12.897592 profitpulse-2.2.0/src/profitpulse/services/revalue_test.py
--rw-r--r--   0        0        0     1049 2024-05-10 06:54:12.898087 profitpulse-2.2.0/src/profitpulse/services/services.py
--rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-2.2.0/src/profitpulse/testrig/__init__.py
--rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-2.2.0/src/profitpulse/testrig/factory.py
--rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-2.2.0/src/profitpulse/testrig/fixtures.py
--rw-r--r--   0        0        0     4652 2024-05-12 19:25:34.212907 profitpulse-2.2.0/src/profitpulse/testrig/scenario.py
--rw-r--r--   0        0        0      330 2024-05-04 13:20:47.845916 profitpulse-2.2.0/src/profitpulse/turbofan.py
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 profitpulse-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-2.2.1/LICENSE
+-rw-r--r--   0        0        0     1075 2024-05-04 13:05:41.429315 profitpulse-2.2.1/README.md
+-rw-r--r--   0        0        0     1839 2024-05-12 20:05:56.359038 profitpulse-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-2.2.1/src/profitpulse/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 13:54:47.669161 profitpulse-2.2.1/src/profitpulse/cli/__init__.py
+-rw-r--r--   0        0        0     8195 2024-05-12 19:23:02.361097 profitpulse-2.2.1/src/profitpulse/cli/adapters.py
+-rw-r--r--   0        0        0     4941 2024-05-12 19:25:34.206898 profitpulse-2.2.1/src/profitpulse/cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-2.2.1/src/profitpulse/data/__init__.py
+-rw-r--r--   0        0        0     4533 2024-05-12 18:13:22.497175 profitpulse-2.2.1/src/profitpulse/data/assets.py
+-rw-r--r--   0        0        0     2409 2024-05-10 06:54:12.883293 profitpulse-2.2.1/src/profitpulse/data/assets_test.py
+-rw-r--r--   0        0        0      360 2024-05-10 06:54:12.884114 profitpulse-2.2.1/src/profitpulse/data/data.py
+-rw-r--r--   0        0        0     1852 2024-05-12 19:36:31.054109 profitpulse-2.2.1/src/profitpulse/data/expenses_view.py
+-rw-r--r--   0        0        0     3191 2024-05-12 19:25:34.189395 profitpulse-2.2.1/src/profitpulse/data/expenses_view_test.py
+-rw-r--r--   0        0        0     2149 2024-05-10 06:54:12.885295 profitpulse-2.2.1/src/profitpulse/data/pulse_view.py
+-rw-r--r--   0        0        0     3057 2024-05-10 06:54:12.885866 profitpulse-2.2.1/src/profitpulse/data/pulse_view_test.py
+-rw-r--r--   0        0        0     1628 2024-05-12 17:04:21.964654 profitpulse-2.2.1/src/profitpulse/data/views.py
+-rw-r--r--   0        0        0     1033 2024-05-12 17:04:21.965124 profitpulse-2.2.1/src/profitpulse/data/views_test.py
+-rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-2.2.1/src/profitpulse/gateways/__init__.py
+-rw-r--r--   0        0        0     3181 2024-05-12 20:03:01.452823 profitpulse-2.2.1/src/profitpulse/gateways/cgdfile.py
+-rw-r--r--   0        0        0     2025 2024-05-12 20:00:26.624621 profitpulse-2.2.1/src/profitpulse/gateways/cgdfile_test.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-2.2.1/src/profitpulse/infrastructure/__init__.py
+-rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-2.2.1/src/profitpulse/infrastructure/migrations.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-2.2.1/src/profitpulse/lib/__init__.py
+-rw-r--r--   0        0        0     1962 2024-05-10 06:54:12.888068 profitpulse-2.2.1/src/profitpulse/lib/asset.py
+-rw-r--r--   0        0        0      541 2024-05-07 20:15:15.902011 profitpulse-2.2.1/src/profitpulse/lib/asset_name.py
+-rw-r--r--   0        0        0      493 2024-04-27 17:48:38.579236 profitpulse-2.2.1/src/profitpulse/lib/comment.py
+-rw-r--r--   0        0        0      964 2024-05-10 06:54:12.889055 profitpulse-2.2.1/src/profitpulse/lib/money.py
+-rw-r--r--   0        0        0      230 2024-05-12 19:58:55.502505 profitpulse-2.2.1/src/profitpulse/lib/transaction.py
+-rw-r--r--   0        0        0      956 2024-05-12 18:30:01.306766 profitpulse-2.2.1/src/profitpulse/migrations/0001 - Initial.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-2.2.1/src/profitpulse/migrations/0002 - accounts.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-2.2.1/src/profitpulse/migrations/__init__.py
+-rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-2.2.1/src/profitpulse/services/__init__.py
+-rw-r--r--   0        0        0     1468 2024-05-10 06:54:12.890186 profitpulse-2.2.1/src/profitpulse/services/acquire_asset.py
+-rw-r--r--   0        0        0     1636 2024-05-10 06:54:12.891286 profitpulse-2.2.1/src/profitpulse/services/acquire_asset_test.py
+-rw-r--r--   0        0        0     1298 2024-05-10 06:54:12.892139 profitpulse-2.2.1/src/profitpulse/services/delete_asset.py
+-rw-r--r--   0        0        0     1475 2024-05-10 06:54:12.892714 profitpulse-2.2.1/src/profitpulse/services/delete_asset_test.py
+-rw-r--r--   0        0        0     1888 2024-05-10 06:54:12.893192 profitpulse-2.2.1/src/profitpulse/services/deposit_into_asset.py
+-rw-r--r--   0        0        0     2680 2024-05-10 06:54:12.893995 profitpulse-2.2.1/src/profitpulse/services/deposit_into_asset_test.py
+-rw-r--r--   0        0        0     1428 2024-05-10 06:54:12.894591 profitpulse-2.2.1/src/profitpulse/services/divest_asset.py
+-rw-r--r--   0        0        0     1611 2024-05-10 06:54:12.895330 profitpulse-2.2.1/src/profitpulse/services/divest_asset_test.py
+-rw-r--r--   0        0        0      285 2024-05-07 20:15:15.913869 profitpulse-2.2.1/src/profitpulse/services/errors.py
+-rw-r--r--   0        0        0     1446 2024-05-12 18:43:49.634734 profitpulse-2.2.1/src/profitpulse/services/import_transactions.py
+-rw-r--r--   0        0        0     1609 2024-05-12 20:04:33.857117 profitpulse-2.2.1/src/profitpulse/services/revalue_asset.py
+-rw-r--r--   0        0        0     1625 2024-05-10 06:54:12.897592 profitpulse-2.2.1/src/profitpulse/services/revalue_test.py
+-rw-r--r--   0        0        0     1049 2024-05-10 06:54:12.898087 profitpulse-2.2.1/src/profitpulse/services/services.py
+-rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-2.2.1/src/profitpulse/testrig/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-2.2.1/src/profitpulse/testrig/factory.py
+-rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-2.2.1/src/profitpulse/testrig/fixtures.py
+-rw-r--r--   0        0        0     4652 2024-05-12 19:25:34.212907 profitpulse-2.2.1/src/profitpulse/testrig/scenario.py
+-rw-r--r--   0        0        0      330 2024-05-04 13:20:47.845916 profitpulse-2.2.1/src/profitpulse/turbofan.py
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 profitpulse-2.2.1/PKG-INFO
```

### Comparing `profitpulse-2.2.0/LICENSE` & `profitpulse-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/README.md` & `profitpulse-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/pyproject.toml` & `profitpulse-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["tests", "features"]
 
 [tool.poetry]
 name = "profitpulse"
-version = "2.2.0"
+version = "2.2.1"
 description = "Manage your personal finances"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 maintainers = ["Luís Miranda <luistm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/luistm/profitpulse"
```

### Comparing `profitpulse-2.2.0/src/profitpulse/cli/adapters.py` & `profitpulse-2.2.1/src/profitpulse/cli/adapters.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/cli/main.py` & `profitpulse-2.2.1/src/profitpulse/cli/main.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/data/assets.py` & `profitpulse-2.2.1/src/profitpulse/data/assets.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/data/assets_test.py` & `profitpulse-2.2.1/src/profitpulse/data/assets_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/data/expenses_view.py` & `profitpulse-2.2.1/src/profitpulse/data/expenses_view.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/data/expenses_view_test.py` & `profitpulse-2.2.1/src/profitpulse/data/expenses_view_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/data/pulse_view.py` & `profitpulse-2.2.1/src/profitpulse/data/pulse_view.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/data/pulse_view_test.py` & `profitpulse-2.2.1/src/profitpulse/data/pulse_view_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/data/views.py` & `profitpulse-2.2.1/src/profitpulse/data/views.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/data/views_test.py` & `profitpulse-2.2.1/src/profitpulse/data/views_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/gateways/cgdfile.py` & `profitpulse-2.2.1/src/profitpulse/gateways/cgdfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,32 +17,32 @@
     def __init__(self, row: list):
         if not row:
             raise ValueError("Row cannot be empty")
 
         self.row = row
 
     @property
-    def value(self) -> float:
+    def value(self) -> int:
         """
         Get the value of the transaction.
         """
 
         debit_row_index = 3
         credit_row_index = 4
 
         value_index = debit_row_index
         if not self.row[debit_row_index]:
             value_index = credit_row_index
 
-        parsed_value = self.row[value_index].replace(".", "").replace(",", ".")
+        parsed_value = self.row[value_index].replace(".", "").replace(",", "")
 
         if value_index == credit_row_index:
-            return float(parsed_value)
+            return int(parsed_value)
 
-        return float(parsed_value) * -1
+        return int(parsed_value) * -1
 
     @property
     def description(self) -> str:
         """
         Get the description of the transaction.
         """
```

### Comparing `profitpulse-2.2.0/src/profitpulse/gateways/cgdfile_test.py` & `profitpulse-2.2.1/src/profitpulse/gateways/cgdfile_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,56 +7,56 @@
 class TestRowParser:
     """
     Example of a row list:
         ['01-01-2020', '01-01-2020', 'COMPRAS C DEB FARMACI ', '15,69', '', '2.350,49', '2.350,49', 'COMPRAS ', ''] # noqa
     """
 
     @pytest.mark.parametrize(
-        "row, expectes_error",
+        "row, expects_error",
         [
             ([], True),
             ("", True),
             (None, True),
             (
                 [
                     "MustBeAListANonEmptyList",
                 ],
                 False,
             ),
         ],
     )
-    def test_raise_exception_when_row_is_not_valid(self, row, expectes_error):
-        if not expectes_error:
+    def test_raise_exception_when_row_is_not_valid(self, row, expects_error):
+        if not expects_error:
             RowParser(row)
         else:
             with pytest.raises(ValueError):
                 RowParser(row)
 
     def test_extract_value_when_debit_is_valid(self):
         row = [
             "01-01-2020",
             "",
             "COMPRAS C DEB FARMACI ",
             "2.115,69",
         ]
         row_parser = RowParser(row)
 
-        assert row_parser.value == -2115.69  # nosec
+        assert row_parser.value == -211569  # nosec
 
     def test_extract_value_when_credit_is_valid(self):
         row = [
             "01-01-2020",
             "",
             "COMPRAS C DEB FARMACI ",
             "",
             "2.115,69",
         ]
         row_parser = RowParser(row)
 
-        assert row_parser.value == 2115.69  # nosec
+        assert row_parser.value == 211569  # nosec
 
     def test_extract_description(self):
         row = [
             "01-01-2020",
             "",
             "COMPRAS C DEB FARMACI ",
             "",
```

### Comparing `profitpulse-2.2.0/src/profitpulse/infrastructure/migrations.py` & `profitpulse-2.2.1/src/profitpulse/infrastructure/migrations.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/lib/asset.py` & `profitpulse-2.2.1/src/profitpulse/lib/asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/lib/asset_name.py` & `profitpulse-2.2.1/src/profitpulse/lib/asset_name.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/lib/money.py` & `profitpulse-2.2.1/src/profitpulse/lib/money.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/migrations/0001 - Initial.sql` & `profitpulse-2.2.1/src/profitpulse/migrations/0001 - Initial.sql`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/services/acquire_asset.py` & `profitpulse-2.2.1/src/profitpulse/services/acquire_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/services/acquire_asset_test.py` & `profitpulse-2.2.1/src/profitpulse/services/acquire_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/services/delete_asset.py` & `profitpulse-2.2.1/src/profitpulse/services/delete_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/services/delete_asset_test.py` & `profitpulse-2.2.1/src/profitpulse/services/delete_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/services/deposit_into_asset.py` & `profitpulse-2.2.1/src/profitpulse/services/deposit_into_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/services/deposit_into_asset_test.py` & `profitpulse-2.2.1/src/profitpulse/services/deposit_into_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/services/divest_asset.py` & `profitpulse-2.2.1/src/profitpulse/services/divest_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/services/divest_asset_test.py` & `profitpulse-2.2.1/src/profitpulse/services/divest_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/services/import_transactions.py` & `profitpulse-2.2.1/src/profitpulse/services/import_transactions.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/services/revalue_asset.py` & `profitpulse-2.2.1/src/profitpulse/services/revalue_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/services/revalue_test.py` & `profitpulse-2.2.1/src/profitpulse/services/revalue_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/services/services.py` & `profitpulse-2.2.1/src/profitpulse/services/services.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/testrig/fixtures.py` & `profitpulse-2.2.1/src/profitpulse/testrig/fixtures.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/src/profitpulse/testrig/scenario.py` & `profitpulse-2.2.1/src/profitpulse/testrig/scenario.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.2.0/PKG-INFO` & `profitpulse-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profitpulse
-Version: 2.2.0
+Version: 2.2.1
 Summary: Manage your personal finances
 Home-page: https://github.com/luistm/profitpulse
 License: MIT
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Maintainer: Luís Miranda
 Maintainer-email: luistm@gmail.com
```

