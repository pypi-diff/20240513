# Comparing `tmp/frformat-0.1.2.tar.gz` & `tmp/frformat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frformat-0.1.2.tar", max compression
+gzip compressed data, was "frformat-0.2.0.tar", max compression
```

## Comparing `frformat-0.1.2.tar` & `frformat-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,32 @@
--rw-r--r--   0        0        0    34523 2024-02-09 11:18:16.551326 frformat-0.1.2/LICENSE
--rw-r--r--   0        0        0      456 2024-02-09 11:18:16.555326 frformat-0.1.2/README.md
--rw-r--r--   0        0        0      618 2024-02-09 11:18:25.191353 frformat-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      282 2024-02-09 11:18:16.555326 frformat-0.1.2/src/frformat/__init__.py
--rw-r--r--   0        0        0     1171 2024-02-09 11:18:16.555326 frformat-0.1.2/src/frformat/custom_format.py
--rw-r--r--   0        0        0     4632 2024-02-09 11:18:16.555326 frformat-0.1.2/src/frformat/french_gps_coordinates.py
--rw-r--r--   0        0        0     2666 2024-02-09 11:18:16.555326 frformat-0.1.2/src/frformat/nomenclature_acte_format.py
--rw-r--r--   0        0        0      516 2024-02-09 11:18:16.555326 frformat-0.1.2/src/frformat/siren_format.py
--rw-r--r--   0        0        0      503 2024-02-09 11:18:16.555326 frformat-0.1.2/src/frformat/siret_format.py
--rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 frformat-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-13 08:31:25.866711 frformat-0.2.0/LICENSE
+-rw-r--r--   0        0        0      456 2024-05-13 08:31:25.866711 frformat-0.2.0/README.md
+-rw-r--r--   0        0        0      690 2024-05-13 08:31:34.046774 frformat-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      950 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/__init__.py
+-rw-r--r--   0        0        0      463 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/common.py
+-rw-r--r--   0        0        0     1200 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/custom_format.py
+-rw-r--r--   0        0        0      983 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/enum_format.py
+-rw-r--r--   0        0        0      263 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/geo/canton.py
+-rw-r--r--   0        0        0    45742 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/geo/canton_set.py
+-rw-r--r--   0        0        0      298 2024-05-13 08:31:25.866711 frformat-0.2.0/src/frformat/geo/code_commune_insee.py
+-rw-r--r--   0        0        0   488829 2024-05-13 08:31:25.870711 frformat-0.2.0/src/frformat/geo/code_commune_insee_set.py
+-rw-r--r--   0        0        0      720 2024-05-13 08:31:25.870711 frformat-0.2.0/src/frformat/geo/code_fantoir.py
+-rw-r--r--   0        0        0   313495 2024-05-13 08:31:25.870711 frformat-0.2.0/src/frformat/geo/code_fantoir_set.py
+-rw-r--r--   0        0        0      403 2024-05-13 08:31:25.870711 frformat-0.2.0/src/frformat/geo/code_pays.py
+-rw-r--r--   0        0        0     4566 2024-05-13 08:31:25.870711 frformat-0.2.0/src/frformat/geo/code_pays_set.py
+-rw-r--r--   0        0        0      256 2024-05-13 08:31:25.870711 frformat-0.2.0/src/frformat/geo/code_postal.py
+-rw-r--r--   0        0        0   478708 2024-05-13 08:31:25.874711 frformat-0.2.0/src/frformat/geo/code_postal_set.py
+-rw-r--r--   0        0        0      431 2024-05-13 08:31:25.874711 frformat-0.2.0/src/frformat/geo/code_region.py
+-rw-r--r--   0        0        0      319 2024-05-13 08:31:25.874711 frformat-0.2.0/src/frformat/geo/commune.py
+-rw-r--r--   0        0        0   761291 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/commune_set.py
+-rw-r--r--   0        0        0     4556 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/coordonnees_gps_francaises.py
+-rw-r--r--   0        0        0      291 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/departement.py
+-rw-r--r--   0        0        0     1766 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/departement_set.py
+-rw-r--r--   0        0        0      453 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/numero_departement.py
+-rw-r--r--   0        0        0      238 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/pays.py
+-rw-r--r--   0        0        0     4390 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/pays_set.py
+-rw-r--r--   0        0        0      304 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/region.py
+-rw-r--r--   0        0        0     1315 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/geo/region_set.py
+-rw-r--r--   0        0        0     2593 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/nomenclature_acte_format.py
+-rw-r--r--   0        0        0      516 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/siren.py
+-rw-r--r--   0        0        0      503 2024-05-13 08:31:25.878711 frformat-0.2.0/src/frformat/siret.py
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 frformat-0.2.0/PKG-INFO
```

### Comparing `frformat-0.1.2/LICENSE` & `frformat-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frformat-0.1.2/pyproject.toml` & `frformat-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frformat"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
 authors = [
   "Pierre Camilleri <22995923+pierrecamilleri@users.noreply.github.com>",
   "Amélie Rondot"
 ]
 license = "AGPL-3.0"
 readme = "README.md"
@@ -27,7 +27,12 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+addopts = [
+    "--import-mode=importlib",
+]
```

### Comparing `frformat-0.1.2/src/frformat/custom_format.py` & `frformat-0.2.0/src/frformat/custom_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     @classmethod
     def format(cls, value: str) -> str:
         if not cls.is_valid(value):
             raise ValueError(f"{cls.name()} is not valid")
         return cls._format(value)
 
     @classmethod
-    @abstractmethod
     def _format(cls, value: str) -> str:
-        ...
+        # Specify the default behaviour
+        return value
```

### Comparing `frformat-0.1.2/src/frformat/french_gps_coordinates.py` & `frformat-0.2.0/src/frformat/geo/coordonnees_gps_francaises.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from shapely.geometry import Point, shape
 
 
-class FrenchGPSCoordinates:
+class CoordonneesGPSFrancaises:
     @classmethod
     def name(cls) -> str:
         return "Coordonnées GPS françaises"
 
     @classmethod
     def description(cls) -> str:
         return """Check that GPS coordinates are in a bounding box approximating
     France (including DOM)"""
 
     @classmethod
     def is_valid(cls, lon: float, lat: float) -> bool:
         return is_point_in_france((lon, lat))
 
-    @classmethod
-    def _format(cls, value: str) -> str:
-        return value
-
 
 def is_point_in_france(coordonnees_xy: tuple[float, float]) -> bool:
     """Returns True if the point is in metropolitan France, Guadeloupe, Martinique,
     Guyane, la Réunion or Mayotte. As we are using bounding boxes (with a small margin),
     locations outside of France but quite close by may return True.
     """
     p = Point(*coordonnees_xy)
```

### Comparing `frformat-0.1.2/src/frformat/nomenclature_acte_format.py` & `frformat-0.2.0/src/frformat/nomenclature_acte_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Literal, Tuple, Union
 
-from . import CustomFormat
+from frformat import CustomFormat
 
 AUTHORIZED_VALUES = {
     "Commande publique",
     "Urbanisme",
     "Domaine et patrimoine",
     "Fonction publique",
     "Institutions et vie politique",
@@ -81,14 +81,10 @@
                 details.append(EXTRA_SPACE)
 
             if nomenc.strip() not in AUTHORIZED_VALUES:
                 details.append(INVALID_PREFIX(nomenc.strip()))
 
         return (False, details)
 
-    @classmethod
-    def _format(cls, value: str) -> str:
-        return value
-
     @staticmethod
     def _nomenclature(value: str) -> str:
         return value[: value.find("/")]
```

### Comparing `frformat-0.1.2/src/frformat/siren_format.py` & `frformat-0.2.0/src/frformat/siren.py`

 * *Files identical despite different names*

### Comparing `frformat-0.1.2/PKG-INFO` & `frformat-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frformat
-Version: 0.1.2
+Version: 0.2.0
 Summary: 
 License: AGPL-3.0
 Author: Pierre Camilleri
 Author-email: 22995923+pierrecamilleri@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

