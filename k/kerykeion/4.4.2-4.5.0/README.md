# Comparing `tmp/kerykeion-4.4.2.tar.gz` & `tmp/kerykeion-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerykeion-4.4.2.tar", max compression
+gzip compressed data, was "kerykeion-4.5.0.tar", max compression
```

## Comparing `kerykeion-4.4.2.tar` & `kerykeion-4.5.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    34273 2024-03-05 19:55:06.854597 kerykeion-4.4.2/LICENSE
--rw-r--r--   0        0        0     8634 2024-03-05 19:55:06.855014 kerykeion-4.4.2/README.md
--rw-r--r--   0        0        0     3874 2024-03-05 19:18:31.414622 kerykeion-4.4.2/kerykeion/__init__.py
--rw-r--r--   0        0        0      293 2024-03-05 19:18:31.414757 kerykeion-4.4.2/kerykeion/aspects/__init__.py
--rw-r--r--   0        0        0     5832 2024-03-05 19:18:31.414940 kerykeion-4.4.2/kerykeion/aspects/aspects_utils.py
--rw-r--r--   0        0        0     4507 2024-03-05 19:18:31.415083 kerykeion-4.4.2/kerykeion/aspects/natal_aspects.py
--rw-r--r--   0        0        0     3993 2024-03-05 19:18:31.415179 kerykeion-4.4.2/kerykeion/aspects/synastry_aspects.py
--rw-r--r--   0        0        0    24706 2024-03-25 11:28:19.058468 kerykeion-4.4.2/kerykeion/astrological_subject.py
--rw-r--r--   0        0        0      127 2024-03-05 19:18:31.415447 kerykeion-4.4.2/kerykeion/charts/__init__.py
--rw-r--r--   0        0        0     3197 2024-03-05 19:18:31.415523 kerykeion-4.4.2/kerykeion/charts/charts_utils.py
--rwxr-xr-x   0        0        0    65295 2024-03-19 11:01:58.830365 kerykeion-4.4.2/kerykeion/charts/kerykeion_chart_svg.py
--rwxr-xr-x   0        0        0    69874 2024-03-05 19:18:31.416341 kerykeion-4.4.2/kerykeion/charts/templates/chart.xml
--rw-r--r--   0        0        0     4444 2024-03-05 19:18:31.416503 kerykeion-4.4.2/kerykeion/fetch_geonames.py
--rw-r--r--   0        0        0      205 2024-03-05 19:18:31.416620 kerykeion-4.4.2/kerykeion/kr_types/__init__.py
--rw-r--r--   0        0        0     1945 2024-03-05 19:18:31.416709 kerykeion-4.4.2/kerykeion/kr_types/chart_types.py
--rw-r--r--   0        0        0      314 2024-03-05 19:18:31.416783 kerykeion-4.4.2/kerykeion/kr_types/kerykeion_exception.py
--rw-r--r--   0        0        0     1034 2024-03-05 19:18:31.416860 kerykeion-4.4.2/kerykeion/kr_types/kr_literals.py
--rw-r--r--   0        0        0     4093 2024-03-05 19:18:31.416939 kerykeion-4.4.2/kerykeion/kr_types/kr_models.py
--rw-r--r--   0        0        0    12737 2024-03-05 19:18:31.417044 kerykeion-4.4.2/kerykeion/kr_types/settings_models.py
--rw-r--r--   0        0        0     6794 2024-03-05 19:18:31.417198 kerykeion-4.4.2/kerykeion/relationship_score.py
--rw-r--r--   0        0        0     2565 2024-03-05 19:18:31.417278 kerykeion-4.4.2/kerykeion/report.py
--rw-r--r--   0        0        0       69 2024-03-05 19:18:31.417375 kerykeion-4.4.2/kerykeion/settings/__init__.py
--rw-r--r--   0        0        0     2341 2024-03-05 19:18:31.417455 kerykeion-4.4.2/kerykeion/settings/kerykeion_settings.py
--rw-r--r--   0        0        0    12282 2024-03-05 19:18:31.417645 kerykeion-4.4.2/kerykeion/settings/kr.config.json
--rw-r--r--   0        0        0       73 2024-03-05 19:18:31.417768 kerykeion-4.4.2/kerykeion/sweph/README.md
--rw-r--r--   0        0        0   223002 2024-03-05 19:18:31.418653 kerykeion-4.4.2/kerykeion/sweph/seas_18.se1
--rw-r--r--   0        0        0     6280 2024-03-05 19:18:31.418814 kerykeion-4.4.2/kerykeion/utilities.py
--rw-r--r--   0        0        0     2354 2024-03-25 11:28:19.058642 kerykeion-4.4.2/pyproject.toml
--rw-r--r--   0        0        0    10260 1970-01-01 00:00:00.000000 kerykeion-4.4.2/PKG-INFO
+-rw-r--r--   0        0        0    34273 2024-03-05 19:55:06.854597 kerykeion-4.5.0/LICENSE
+-rw-r--r--   0        0        0     8634 2024-03-05 19:55:06.855014 kerykeion-4.5.0/README.md
+-rw-r--r--   0        0        0     3917 2024-05-13 20:03:16.435516 kerykeion-4.5.0/kerykeion/__init__.py
+-rw-r--r--   0        0        0      293 2024-03-05 19:18:31.414757 kerykeion-4.5.0/kerykeion/aspects/__init__.py
+-rw-r--r--   0        0        0     5832 2024-03-05 19:18:31.414940 kerykeion-4.5.0/kerykeion/aspects/aspects_utils.py
+-rw-r--r--   0        0        0     4507 2024-03-05 19:18:31.415083 kerykeion-4.5.0/kerykeion/aspects/natal_aspects.py
+-rw-r--r--   0        0        0     3993 2024-03-05 19:18:31.415179 kerykeion-4.5.0/kerykeion/aspects/synastry_aspects.py
+-rw-r--r--   0        0        0    25672 2024-05-13 20:03:16.435931 kerykeion-4.5.0/kerykeion/astrological_subject.py
+-rw-r--r--   0        0        0      127 2024-03-05 19:18:31.415447 kerykeion-4.5.0/kerykeion/charts/__init__.py
+-rw-r--r--   0        0        0     3197 2024-03-05 19:18:31.415523 kerykeion-4.5.0/kerykeion/charts/charts_utils.py
+-rwxr-xr-x   0        0        0    65295 2024-03-19 11:01:58.830365 kerykeion-4.5.0/kerykeion/charts/kerykeion_chart_svg.py
+-rwxr-xr-x   0        0        0    69874 2024-03-05 19:18:31.416341 kerykeion-4.5.0/kerykeion/charts/templates/chart.xml
+-rw-r--r--   0        0        0      965 2024-05-13 20:03:16.436187 kerykeion-4.5.0/kerykeion/enums.py
+-rw-r--r--   0        0        0     4444 2024-03-05 19:18:31.416503 kerykeion-4.5.0/kerykeion/fetch_geonames.py
+-rw-r--r--   0        0        0      205 2024-03-05 19:18:31.416620 kerykeion-4.5.0/kerykeion/kr_types/__init__.py
+-rw-r--r--   0        0        0     1945 2024-03-05 19:18:31.416709 kerykeion-4.5.0/kerykeion/kr_types/chart_types.py
+-rw-r--r--   0        0        0      314 2024-03-05 19:18:31.416783 kerykeion-4.5.0/kerykeion/kr_types/kerykeion_exception.py
+-rw-r--r--   0        0        0     1034 2024-03-05 19:18:31.416860 kerykeion-4.5.0/kerykeion/kr_types/kr_literals.py
+-rw-r--r--   0        0        0     4100 2024-05-13 20:03:16.436568 kerykeion-4.5.0/kerykeion/kr_types/kr_models.py
+-rw-r--r--   0        0        0    12737 2024-03-05 19:18:31.417044 kerykeion-4.5.0/kerykeion/kr_types/settings_models.py
+-rw-r--r--   0        0        0     6794 2024-03-05 19:18:31.417198 kerykeion-4.5.0/kerykeion/relationship_score.py
+-rw-r--r--   0        0        0     2565 2024-03-05 19:18:31.417278 kerykeion-4.5.0/kerykeion/report.py
+-rw-r--r--   0        0        0       69 2024-03-05 19:18:31.417375 kerykeion-4.5.0/kerykeion/settings/__init__.py
+-rw-r--r--   0        0        0     2341 2024-03-05 19:18:31.417455 kerykeion-4.5.0/kerykeion/settings/kerykeion_settings.py
+-rw-r--r--   0        0        0    12282 2024-03-05 19:18:31.417645 kerykeion-4.5.0/kerykeion/settings/kr.config.json
+-rw-r--r--   0        0        0       73 2024-03-05 19:18:31.417768 kerykeion-4.5.0/kerykeion/sweph/README.md
+-rw-r--r--   0        0        0   223002 2024-03-05 19:18:31.418653 kerykeion-4.5.0/kerykeion/sweph/seas_18.se1
+-rw-r--r--   0        0        0     6207 2024-05-13 20:03:16.436971 kerykeion-4.5.0/kerykeion/utilities.py
+-rw-r--r--   0        0        0     2354 2024-05-13 20:03:16.437302 kerykeion-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0    10311 1970-01-01 00:00:00.000000 kerykeion-4.5.0/PKG-INFO
```

### Comparing `kerykeion-4.4.2/LICENSE` & `kerykeion-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/README.md` & `kerykeion-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/__init__.py` & `kerykeion-4.5.0/kerykeion/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,7 +102,8 @@
 from .astrological_subject import AstrologicalSubject
 from .charts.kerykeion_chart_svg import KerykeionChartSVG
 from .kr_types import *
 from .relationship_score import RelationshipScore
 from .aspects import SynastryAspects, NatalAspects
 from .report import Report
 from .settings import KerykeionSettingsModel, get_settings
+from .enums import Planets, Aspects, Signs
```

### Comparing `kerykeion-4.4.2/kerykeion/aspects/aspects_utils.py` & `kerykeion-4.5.0/kerykeion/aspects/aspects_utils.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/aspects/natal_aspects.py` & `kerykeion-4.5.0/kerykeion/aspects/natal_aspects.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/aspects/synastry_aspects.py` & `kerykeion-4.5.0/kerykeion/aspects/synastry_aspects.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/astrological_subject.py` & `kerykeion-4.5.0/kerykeion/astrological_subject.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,16 @@
     - tz_str (Union[str, bool], optional): _ Defaults to False.
     - geonames_username (str, optional): _ Defaults to 'century.boy'.
     - online (bool, optional): Sets if you want to use the online mode (using
         geonames) or not. Defaults to True.
     - utc_datetime (datetime, optional): An alternative way of constructing the object, 
         if you know the UTC datetime but do not have easy access to e.g. timezone identifier
         _ Defaults to None.
+    - disable_chiron (bool, optional): Disables the calculation of Chiron. Defaults to False.
+        Chiron calculation can create some issues with the Swiss Ephemeris when the date is too far in the past.
     """
 
     # Defined by the user
     name: str
     utc_datetime: Union[datetime, None]
     year: int
     month: int
@@ -87,15 +89,15 @@
     jupiter: KerykeionPointModel
     saturn: KerykeionPointModel
     uranus: KerykeionPointModel
     neptune: KerykeionPointModel
     pluto: KerykeionPointModel
     true_node: KerykeionPointModel
     mean_node: KerykeionPointModel
-    chiron: KerykeionPointModel
+    chiron: KerykeionPointModel | None
 
     # Houses
     first_house: KerykeionPointModel
     second_house: KerykeionPointModel
     third_house: KerykeionPointModel
     fourth_house: KerykeionPointModel
     fifth_house: KerykeionPointModel
@@ -128,14 +130,15 @@
         lng: Union[int, float, None] = None,
         lat: Union[int, float, None] = None,
         tz_str: Union[str, None] = None,
         geonames_username: Union[str, None] = None,
         zodiac_type: ZodiacType = "Tropic",
         online: bool = True,
         utc_datetime: Union[datetime, None] = None,
+        disable_chiron: bool = False
     ) -> None:
         logging.debug("Starting Kerykeion")
 
         # We set the swisseph path to the current directory
         swe.set_ephe_path(
             str(
                 Path(__file__).parent.absolute() / "sweph"
@@ -154,14 +157,15 @@
         self.lat = lat
         self.tz_str = tz_str
         self.zodiac_type = zodiac_type
         self.online = online
         self.json_dir = Path.home()
         self.geonames_username = geonames_username
         self.utc_datetime = utc_datetime
+        self.disable_chiron = disable_chiron
 
         # This message is set to encourage the user to set a custom geonames username
         if geonames_username is None and online:
             logging.info(
                 "\n"
                 "********" +
                 "\n" +
@@ -371,31 +375,37 @@
         jupiter_deg = swe.calc(self.julian_day, 5, self._iflag)[0][0]
         saturn_deg = swe.calc(self.julian_day, 6, self._iflag)[0][0]
         uranus_deg = swe.calc(self.julian_day, 7, self._iflag)[0][0]
         neptune_deg = swe.calc(self.julian_day, 8, self._iflag)[0][0]
         pluto_deg = swe.calc(self.julian_day, 9, self._iflag)[0][0]
         mean_node_deg = swe.calc(self.julian_day, 10, self._iflag)[0][0]
         true_node_deg = swe.calc(self.julian_day, 11, self._iflag)[0][0]
-        chiron_deg = swe.calc(self.julian_day, 15, self._iflag)[0][0]
+        
+        if not self.disable_chiron:
+            chiron_deg = swe.calc(self.julian_day, 15, self._iflag)[0][0]
+        else:
+            chiron_deg = 0
 
         self.planets_degrees_ut = [
             sun_deg,
             moon_deg,
             mercury_deg,
             venus_deg,
             mars_deg,
             jupiter_deg,
             saturn_deg,
             uranus_deg,
             neptune_deg,
             pluto_deg,
             mean_node_deg,
             true_node_deg,
-            chiron_deg,
         ]
+        
+        if not self.disable_chiron:
+            self.planets_degrees_ut.append(chiron_deg)
 
     def _planets(self) -> None:
         """Defines body positon in signs and information and
         stores them in dictionaries"""
 
         point_type: Literal["Planet", "House"] = "Planet"
         # stores the planets in singular dictionaries.
@@ -407,15 +417,19 @@
         self.jupiter = calculate_position(self.planets_degrees_ut[5], "Jupiter", point_type=point_type)
         self.saturn = calculate_position(self.planets_degrees_ut[6], "Saturn", point_type=point_type)
         self.uranus = calculate_position(self.planets_degrees_ut[7], "Uranus", point_type=point_type)
         self.neptune = calculate_position(self.planets_degrees_ut[8], "Neptune", point_type=point_type)
         self.pluto = calculate_position(self.planets_degrees_ut[9], "Pluto", point_type=point_type)
         self.mean_node = calculate_position(self.planets_degrees_ut[10], "Mean_Node", point_type=point_type)
         self.true_node = calculate_position(self.planets_degrees_ut[11], "True_Node", point_type=point_type)
-        self.chiron = calculate_position(self.planets_degrees_ut[12], "Chiron", point_type=point_type)
+        
+        if not self.disable_chiron:
+            self.chiron = calculate_position(self.planets_degrees_ut[12], "Chiron", point_type=point_type)
+        else:
+            self.chiron = None
 
     def _planets_in_houses(self) -> None:
         """Calculates the house of the planet and updates
         the planets dictionary."""
 
         def for_every_planet(planet, planet_deg):
             """Function to do the calculation.
@@ -468,31 +482,37 @@
         self.jupiter = for_every_planet(self.jupiter, self.planets_degrees_ut[5])
         self.saturn = for_every_planet(self.saturn, self.planets_degrees_ut[6])
         self.uranus = for_every_planet(self.uranus, self.planets_degrees_ut[7])
         self.neptune = for_every_planet(self.neptune, self.planets_degrees_ut[8])
         self.pluto = for_every_planet(self.pluto, self.planets_degrees_ut[9])
         self.mean_node = for_every_planet(self.mean_node, self.planets_degrees_ut[10])
         self.true_node = for_every_planet(self.true_node, self.planets_degrees_ut[11])
-        self.chiron = for_every_planet(self.chiron, self.planets_degrees_ut[12])
+
+        if not self.disable_chiron:
+            self.chiron = for_every_planet(self.chiron, self.planets_degrees_ut[12])
+        else:
+            self.chiron = None
 
         self.planets_list = [
             self.sun,
             self.moon,
             self.mercury,
             self.venus,
             self.mars,
             self.jupiter,
             self.saturn,
             self.uranus,
             self.neptune,
             self.pluto,
             self.mean_node,
             self.true_node,
-            self.chiron
         ]
+        
+        if not self.disable_chiron:
+            self.planets_list.append(self.chiron)
 
         # Check in retrograde or not:
         planets_ret = []
         for p in self.planets_list:
             planet_number = get_number_from_name(p["name"])
             if swe.calc(self.julian_day, planet_number, self._iflag)[0][3] < 0:
                 p["retrograde"] = True
@@ -639,14 +659,23 @@
 
         return AstrologicalSubjectModel(**self.__dict__)
 
 
 if __name__ == "__main__":
     import json
     from kerykeion.utilities import setup_logging
-    setup_logging(level="debug")
 
+    setup_logging(level="debug")
+    
+    # With Chiron enabled
     johnny = AstrologicalSubject("Johnny Depp", 1963, 6, 9, 0, 0, "Owensboro", "US")
     print(json.loads(johnny.json(dump=True)))
 
     print('\n')
     print(johnny.chiron)
+
+    # With Chiron disabled
+    johnny = AstrologicalSubject("Johnny Depp", 1963, 6, 9, 0, 0, "Owensboro", "US", disable_chiron=True)
+    print(json.loads(johnny.json(dump=True)))
+
+    print('\n')
+    print(johnny.chiron)
```

### Comparing `kerykeion-4.4.2/kerykeion/charts/charts_utils.py` & `kerykeion-4.5.0/kerykeion/charts/charts_utils.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/charts/kerykeion_chart_svg.py` & `kerykeion-4.5.0/kerykeion/charts/kerykeion_chart_svg.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/charts/templates/chart.xml` & `kerykeion-4.5.0/kerykeion/charts/templates/chart.xml`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/fetch_geonames.py` & `kerykeion-4.5.0/kerykeion/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/kr_types/chart_types.py` & `kerykeion-4.5.0/kerykeion/kr_types/chart_types.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/kr_types/kr_literals.py` & `kerykeion-4.5.0/kerykeion/kr_types/kr_literals.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/kr_types/kr_models.py` & `kerykeion-4.5.0/kerykeion/kr_types/kr_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     venus: KerykeionPointModel
     mars: KerykeionPointModel
     jupiter: KerykeionPointModel
     saturn: KerykeionPointModel
     uranus: KerykeionPointModel
     neptune: KerykeionPointModel
     pluto: KerykeionPointModel
-    chiron: KerykeionPointModel
+    chiron: KerykeionPointModel | None
 
     # Houses
     first_house: KerykeionPointModel
     second_house: KerykeionPointModel
     third_house: KerykeionPointModel
     fourth_house: KerykeionPointModel
     fifth_house: KerykeionPointModel
```

### Comparing `kerykeion-4.4.2/kerykeion/kr_types/settings_models.py` & `kerykeion-4.5.0/kerykeion/kr_types/settings_models.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/relationship_score.py` & `kerykeion-4.5.0/kerykeion/relationship_score.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/report.py` & `kerykeion-4.5.0/kerykeion/report.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/settings/kerykeion_settings.py` & `kerykeion-4.5.0/kerykeion/settings/kerykeion_settings.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/settings/kr.config.json` & `kerykeion-4.5.0/kerykeion/settings/kr.config.json`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/sweph/seas_18.se1` & `kerykeion-4.5.0/kerykeion/sweph/seas_18.se1`

 * *Files identical despite different names*

### Comparing `kerykeion-4.4.2/kerykeion/utilities.py` & `kerykeion-4.5.0/kerykeion/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -199,19 +199,24 @@
             "point_type": point_type,
         }
     else:
         raise KerykeionException(f"Error in calculating positions! Degrees: {degree}")
 
     return KerykeionPointModel(**dictionary)
 
+
 def setup_logging(level: str) -> None:
-    """Setup logging for testing.
-    
+    """
+    Setup logging for testing.
+
     Args:
-        level: Log level as a string, options: debug, info, warning, error"""
-    logopt: dict[str, int]  = {"debug": logging.DEBUG, 
-                               "info": logging.INFO, 
-                               "warning": logging.WARNING , 
-                               "error": logging.ERROR}
-    format: str             = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    loglevel: int           = logopt.get(level, logging.INFO)
-    logging.basicConfig(format=format, level=loglevel)
+        level: Log level as a string, options: debug, info, warning, error
+    """
+    logopt: dict[str, int] = {
+        "debug": logging.DEBUG,
+        "info": logging.INFO,
+        "warning": logging.WARNING,
+        "error": logging.ERROR,
+    }
+    format: str = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+    loglevel: int = logopt.get(level, logging.INFO)
+    logging.basicConfig(format=format, level=loglevel)
```

### Comparing `kerykeion-4.4.2/pyproject.toml` & `kerykeion-4.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kerykeion"
-version = "4.4.2"
+version = "4.5.0"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>"]
 description = "A python library for astrology."
 license = "AGPL-3.0"
 homepage = "https://github.com/g-battaglia/kerykeion"
 repository = "https://github.com/g-battaglia/kerykeion"
 keywords = [
     "astrology",
```

### Comparing `kerykeion-4.4.2/PKG-INFO` & `kerykeion-4.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerykeion
-Version: 4.4.2
+Version: 4.5.0
 Summary: A python library for astrology.
 Home-page: https://github.com/g-battaglia/kerykeion
 License: AGPL-3.0
 Keywords: astrology,ephemeris,astrology library,birtchart,svg,zodiac,zodiac-sing,astronomical-algorithms,synastry,astrology-calculator
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<4.0
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: pydantic (>=2.5,<3.0)
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
-Metadata-Version: 2.1 Name: kerykeion Version: 4.4.2 Summary: A python library
+Metadata-Version: 2.1 Name: kerykeion Version: 4.5.0 Summary: A python library
 for astrology. Home-page: https://github.com/g-battaglia/kerykeion License:
 AGPL-3.0 Keywords: astrology,ephemeris,astrology
 library,birtchart,svg,zodiac,zodiac-sing,astronomical-
 algorithms,synastry,astrology-calculator Author: Giacomo Battaglia Author-
 email: battaglia.giacomo@yahoo.it Requires-Python: >=3.9,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 License :: OSI Approved :: GNU General Public License (GPL) Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
-Scientific/Engineering :: Astronomy Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Typing :: Typed
-Requires-Dist: pydantic (>=2.5,<3.0) Requires-Dist: pyswisseph
-(>=2.10.3.1,<3.0.0.0) Requires-Dist: pytz (>=2022.7,<2023.0) Requires-Dist:
-requests (>=2.28.1,<3.0.0) Requires-Dist: requests-cache (>=0.9.7,<0.10.0)
-Requires-Dist: terminaltables (>=3.1.10,<4.0.0) Project-URL: Repository, https:
-//github.com/g-battaglia/kerykeion Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Topic :: Scientific/Engineering ::
+Astronomy Classifier: Topic :: Software Development Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Typing :: Typed Requires-Dist: pydantic
+(>=2.5,<3.0) Requires-Dist: pyswisseph (>=2.10.3.1,<3.0.0.0) Requires-Dist:
+pytz (>=2022.7,<2023.0) Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-
+Dist: requests-cache (>=0.9.7,<0.10.0) Requires-Dist: terminaltables
+(>=3.1.10,<4.0.0) Project-URL: Repository, https://github.com/g-battaglia/
+kerykeion Description-Content-Type: text/markdown
                             ************ KKeerryykkeeiioonn ************
    _[_c_o_n_t_r_i_b_u_t_o_r_s_]_[_s_t_a_r_s_]_[_f_o_r_k_s_]_[_v_i_s_i_t_o_r_s_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n
                                    _v_e_r_s_i_o_n_s_]
   Kerykeion is a python library for Astrology. It can calculate all the planet
 and house position, also it can calculate the aspects of a single persone or
 between two, you can set how many planets you need in the settings in the
 utility module. It also can generate an SVG of a birthchart, a synastry chart
```

