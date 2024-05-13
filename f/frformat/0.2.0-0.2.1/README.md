# Comparing `tmp/frformat-0.2.0.tar.gz` & `tmp/frformat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frformat-0.2.0.tar", max compression
+gzip compressed data, was "frformat-0.2.1.tar", max compression
```

## Comparing `frformat-0.2.0.tar` & `frformat-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    34523 2024-05-13 08:31:25.866711 frformat-0.2.0/LICENSE
--rw-r--r--   0        0        0      456 2024-05-13 08:31:25.866711 frformat-0.2.0/README.md
--rw-r--r--   0        0        0      690 2024-05-13 08:31:34.046774 frformat-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      950 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/__init__.py
--rw-r--r--   0        0        0      463 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/common.py
--rw-r--r--   0        0        0     1200 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/custom_format.py
--rw-r--r--   0        0        0      983 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/enum_format.py
--rw-r--r--   0        0        0      263 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/geo/canton.py
--rw-r--r--   0        0        0    45742 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/geo/canton_set.py
--rw-r--r--   0        0        0      298 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/geo/code_commune_insee.py
--rw-r--r--   0        0        0   488829 2024-05-13 08:31:25.870711 frformat-0.2.0/src/frformat/geo/code_commune_insee_set.py
--rw-r--r--   0        0        0      720 2024-05-13 08:31:25.870711 frformat-0.2.0/src/frformat/geo/code_fantoir.py
--rw-r--r--   0        0        0   313495 2024-05-13 08:31:25.870711 frformat-0.2.0/src/frformat/geo/code_fantoir_set.py
--rw-r--r--   0        0        0      403 2024-05-13 08:31:25.870711 frformat-0.2.0/src/frformat/geo/code_pays.py
--rw-r--r--   0        0        0     4566 2024-05-13 08:31:25.870711 frformat-0.2.0/src/frformat/geo/code_pays_set.py
--rw-r--r--   0        0        0      256 2024-05-13 08:31:25.870711 frformat-0.2.0/src/frformat/geo/code_postal.py
--rw-r--r--   0        0        0   478708 2024-05-13 08:31:25.874711 frformat-0.2.0/src/frformat/geo/code_postal_set.py
--rw-r--r--   0        0        0      431 2024-05-13 08:31:25.874711 frformat-0.2.0/src/frformat/geo/code_region.py
--rw-r--r--   0        0        0      319 2024-05-13 08:31:25.874711 frformat-0.2.0/src/frformat/geo/commune.py
--rw-r--r--   0        0        0   761291 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/commune_set.py
--rw-r--r--   0        0        0     4556 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/coordonnees_gps_francaises.py
--rw-r--r--   0        0        0      291 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/departement.py
--rw-r--r--   0        0        0     1766 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/departement_set.py
--rw-r--r--   0        0        0      453 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/numero_departement.py
--rw-r--r--   0        0        0      238 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/pays.py
--rw-r--r--   0        0        0     4390 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/pays_set.py
--rw-r--r--   0        0        0      304 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/region.py
--rw-r--r--   0        0        0     1315 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/region_set.py
--rw-r--r--   0        0        0     2593 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/nomenclature_acte_format.py
--rw-r--r--   0        0        0      516 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/siren.py
--rw-r--r--   0        0        0      503 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/siret.py
--rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 frformat-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-13 08:43:13.744482 frformat-0.2.1/LICENSE
+-rw-r--r--   0        0        0      456 2024-05-13 08:43:13.744482 frformat-0.2.1/README.md
+-rw-r--r--   0        0        0      690 2024-05-13 08:43:22.416463 frformat-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      950 2024-05-13 08:43:13.744482 frformat-0.2.1/src/frformat/__init__.py
+-rw-r--r--   0        0        0      463 2024-05-13 08:43:13.744482 frformat-0.2.1/src/frformat/common.py
+-rw-r--r--   0        0        0     1200 2024-05-13 08:43:13.744482 frformat-0.2.1/src/frformat/custom_format.py
+-rw-r--r--   0        0        0      983 2024-05-13 08:43:13.744482 frformat-0.2.1/src/frformat/enum_format.py
+-rw-r--r--   0        0        0      263 2024-05-13 08:43:13.744482 frformat-0.2.1/src/frformat/geo/canton.py
+-rw-r--r--   0        0        0    45742 2024-05-13 08:43:13.744482 frformat-0.2.1/src/frformat/geo/canton_set.py
+-rw-r--r--   0        0        0      298 2024-05-13 08:43:13.744482 frformat-0.2.1/src/frformat/geo/code_commune_insee.py
+-rw-r--r--   0        0        0   488829 2024-05-13 08:43:13.748482 frformat-0.2.1/src/frformat/geo/code_commune_insee_set.py
+-rw-r--r--   0        0        0      720 2024-05-13 08:43:13.748482 frformat-0.2.1/src/frformat/geo/code_fantoir.py
+-rw-r--r--   0        0        0   313495 2024-05-13 08:43:13.748482 frformat-0.2.1/src/frformat/geo/code_fantoir_set.py
+-rw-r--r--   0        0        0      403 2024-05-13 08:43:13.748482 frformat-0.2.1/src/frformat/geo/code_pays.py
+-rw-r--r--   0        0        0     4566 2024-05-13 08:43:13.748482 frformat-0.2.1/src/frformat/geo/code_pays_set.py
+-rw-r--r--   0        0        0      256 2024-05-13 08:43:13.748482 frformat-0.2.1/src/frformat/geo/code_postal.py
+-rw-r--r--   0        0        0   478708 2024-05-13 08:43:13.748482 frformat-0.2.1/src/frformat/geo/code_postal_set.py
+-rw-r--r--   0        0        0      431 2024-05-13 08:43:13.748482 frformat-0.2.1/src/frformat/geo/code_region.py
+-rw-r--r--   0        0        0      319 2024-05-13 08:43:13.748482 frformat-0.2.1/src/frformat/geo/commune.py
+-rw-r--r--   0        0        0   761291 2024-05-13 08:43:13.752482 frformat-0.2.1/src/frformat/geo/commune_set.py
+-rw-r--r--   0        0        0     4556 2024-05-13 08:43:13.752482 frformat-0.2.1/src/frformat/geo/coordonnees_gps_francaises.py
+-rw-r--r--   0        0        0      291 2024-05-13 08:43:13.752482 frformat-0.2.1/src/frformat/geo/departement.py
+-rw-r--r--   0        0        0     1766 2024-05-13 08:43:13.752482 frformat-0.2.1/src/frformat/geo/departement_set.py
+-rw-r--r--   0        0        0      453 2024-05-13 08:43:13.752482 frformat-0.2.1/src/frformat/geo/numero_departement.py
+-rw-r--r--   0        0        0      238 2024-05-13 08:43:13.752482 frformat-0.2.1/src/frformat/geo/pays.py
+-rw-r--r--   0        0        0     4390 2024-05-13 08:43:13.752482 frformat-0.2.1/src/frformat/geo/pays_set.py
+-rw-r--r--   0        0        0      304 2024-05-13 08:43:13.752482 frformat-0.2.1/src/frformat/geo/region.py
+-rw-r--r--   0        0        0     1315 2024-05-13 08:43:13.752482 frformat-0.2.1/src/frformat/geo/region_set.py
+-rw-r--r--   0        0        0     2593 2024-05-13 08:43:13.752482 frformat-0.2.1/src/frformat/nomenclature_acte_format.py
+-rw-r--r--   0        0        0      516 2024-05-13 08:43:13.752482 frformat-0.2.1/src/frformat/siren.py
+-rw-r--r--   0        0        0      503 2024-05-13 08:43:13.752482 frformat-0.2.1/src/frformat/siret.py
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 frformat-0.2.1/PKG-INFO
```

### Comparing `frformat-0.2.0/LICENSE` & `frformat-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/pyproject.toml` & `frformat-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frformat"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = [
   "Pierre Camilleri <22995923+pierrecamilleri@users.noreply.github.com>",
   "Amélie Rondot"
 ]
 license = "AGPL-3.0"
 readme = "README.md"
```

### Comparing `frformat-0.2.0/src/frformat/__init__.py` & `frformat-0.2.1/src/frformat/__init__.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/custom_format.py` & `frformat-0.2.1/src/frformat/custom_format.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/enum_format.py` & `frformat-0.2.1/src/frformat/enum_format.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/geo/canton_set.py` & `frformat-0.2.1/src/frformat/geo/canton_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/geo/code_commune_insee_set.py` & `frformat-0.2.1/src/frformat/geo/code_commune_insee_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/geo/code_fantoir.py` & `frformat-0.2.1/src/frformat/geo/code_fantoir.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/geo/code_fantoir_set.py` & `frformat-0.2.1/src/frformat/geo/code_fantoir_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/geo/code_pays_set.py` & `frformat-0.2.1/src/frformat/geo/code_pays_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/geo/code_postal_set.py` & `frformat-0.2.1/src/frformat/geo/code_postal_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/geo/commune_set.py` & `frformat-0.2.1/src/frformat/geo/commune_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/geo/coordonnees_gps_francaises.py` & `frformat-0.2.1/src/frformat/geo/coordonnees_gps_francaises.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/geo/departement_set.py` & `frformat-0.2.1/src/frformat/geo/departement_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/geo/pays_set.py` & `frformat-0.2.1/src/frformat/geo/pays_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/geo/region_set.py` & `frformat-0.2.1/src/frformat/geo/region_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/nomenclature_acte_format.py` & `frformat-0.2.1/src/frformat/nomenclature_acte_format.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/src/frformat/siren.py` & `frformat-0.2.1/src/frformat/siren.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.0/PKG-INFO` & `frformat-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frformat
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: AGPL-3.0
 Author: Pierre Camilleri
 Author-email: 22995923+pierrecamilleri@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

