# Comparing `tmp/gpx_analysis-edf1101-1.6.tar.gz` & `tmp/gpx_analysis-edf1101-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx_analysis-edf1101-1.6.tar", last modified: Tue Feb  6 16:44:36 2024, max compression
+gzip compressed data, was "gpx_analysis-edf1101-1.7.tar", last modified: Mon May 13 16:02:09 2024, max compression
```

## Comparing `gpx_analysis-edf1101-1.6.tar` & `gpx_analysis-edf1101-1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 edfillingham   (501) staff       (20)        0 2024-02-06 16:44:36.139448 gpx_analysis-edf1101-1.6/
--rw-r--r--   0 edfillingham   (501) staff       (20)     2371 2024-02-06 16:44:36.139346 gpx_analysis-edf1101-1.6/PKG-INFO
--rw-r--r--   0 edfillingham   (501) staff       (20)     1660 2024-02-05 20:02:17.000000 gpx_analysis-edf1101-1.6/README.md
-drwxr-xr-x   0 edfillingham   (501) staff       (20)        0 2024-02-06 16:44:36.138570 gpx_analysis-edf1101-1.6/gpx_analysis/
--rw-r--r--   0 edfillingham   (501) staff       (20)        0 2024-01-18 22:15:07.000000 gpx_analysis-edf1101-1.6/gpx_analysis/__init__.py
--rw-r--r--   0 edfillingham   (501) staff       (20)      322 2024-02-02 17:08:10.000000 gpx_analysis-edf1101-1.6/gpx_analysis/__main__.py
--rw-r--r--   0 edfillingham   (501) staff       (20)    15365 2024-02-06 16:44:06.000000 gpx_analysis-edf1101-1.6/gpx_analysis/app.py
--rw-r--r--   0 edfillingham   (501) staff       (20)     3652 2024-02-03 13:22:55.000000 gpx_analysis-edf1101-1.6/gpx_analysis/components.py
--rw-r--r--   0 edfillingham   (501) staff       (20)     6163 2024-02-06 12:08:43.000000 gpx_analysis-edf1101-1.6/gpx_analysis/gpx_parser.py
--rw-r--r--   0 edfillingham   (501) staff       (20)    21688 2024-02-06 16:29:12.000000 gpx_analysis-edf1101-1.6/gpx_analysis/graph_handler.py
--rw-r--r--   0 edfillingham   (501) staff       (20)    12224 2024-02-06 16:44:06.000000 gpx_analysis-edf1101-1.6/gpx_analysis/gui.py
--rw-r--r--   0 edfillingham   (501) staff       (20)    14858 2024-02-05 18:13:51.000000 gpx_analysis-edf1101-1.6/gpx_analysis/gui_control_menu.py
--rw-r--r--   0 edfillingham   (501) staff       (20)    13547 2024-02-04 20:57:23.000000 gpx_analysis-edf1101-1.6/gpx_analysis/gui_finishline_menu.py
--rw-r--r--   0 edfillingham   (501) staff       (20)     8789 2024-02-03 19:45:59.000000 gpx_analysis-edf1101-1.6/gpx_analysis/gui_playback_menu.py
--rw-r--r--   0 edfillingham   (501) staff       (20)    16210 2024-02-06 16:44:06.000000 gpx_analysis-edf1101-1.6/gpx_analysis/gui_stats_menu.py
--rw-r--r--   0 edfillingham   (501) staff       (20)     8447 2024-02-04 13:43:53.000000 gpx_analysis-edf1101-1.6/gpx_analysis/sporting.py
--rw-r--r--   0 edfillingham   (501) staff       (20)     8759 2024-02-05 17:49:29.000000 gpx_analysis-edf1101-1.6/gpx_analysis/stats_graph_handler.py
--rw-r--r--   0 edfillingham   (501) staff       (20)    10116 2024-02-05 16:50:21.000000 gpx_analysis-edf1101-1.6/gpx_analysis/tkscrolledframe.py
-drwxr-xr-x   0 edfillingham   (501) staff       (20)        0 2024-02-06 16:44:36.139160 gpx_analysis-edf1101-1.6/gpx_analysis_edf1101.egg-info/
--rw-r--r--   0 edfillingham   (501) staff       (20)     2371 2024-02-06 16:44:36.000000 gpx_analysis-edf1101-1.6/gpx_analysis_edf1101.egg-info/PKG-INFO
--rw-r--r--   0 edfillingham   (501) staff       (20)      638 2024-02-06 16:44:36.000000 gpx_analysis-edf1101-1.6/gpx_analysis_edf1101.egg-info/SOURCES.txt
--rw-r--r--   0 edfillingham   (501) staff       (20)        1 2024-02-06 16:44:36.000000 gpx_analysis-edf1101-1.6/gpx_analysis_edf1101.egg-info/dependency_links.txt
--rw-r--r--   0 edfillingham   (501) staff       (20)       25 2024-02-06 16:44:36.000000 gpx_analysis-edf1101-1.6/gpx_analysis_edf1101.egg-info/requires.txt
--rw-r--r--   0 edfillingham   (501) staff       (20)       13 2024-02-06 16:44:36.000000 gpx_analysis-edf1101-1.6/gpx_analysis_edf1101.egg-info/top_level.txt
--rw-r--r--   0 edfillingham   (501) staff       (20)       38 2024-02-06 16:44:36.139508 gpx_analysis-edf1101-1.6/setup.cfg
--rw-r--r--   0 edfillingham   (501) staff       (20)      712 2024-02-06 16:44:33.000000 gpx_analysis-edf1101-1.6/setup.py
+drwxr-xr-x   0 edfillingham   (501) staff       (20)        0 2024-05-13 16:02:09.071426 gpx_analysis-edf1101-1.7/
+-rw-r--r--   0 edfillingham   (501) staff       (20)     1059 2024-05-06 13:34:23.000000 gpx_analysis-edf1101-1.7/LICENSE
+-rw-r--r--   0 edfillingham   (501) staff       (20)     1889 2024-05-13 16:02:09.071317 gpx_analysis-edf1101-1.7/PKG-INFO
+-rw-r--r--   0 edfillingham   (501) staff       (20)     1460 2024-05-06 13:34:23.000000 gpx_analysis-edf1101-1.7/README.md
+drwxr-xr-x   0 edfillingham   (501) staff       (20)        0 2024-05-13 16:02:09.070541 gpx_analysis-edf1101-1.7/gpx_analysis/
+-rw-r--r--   0 edfillingham   (501) staff       (20)        0 2024-05-06 13:34:23.000000 gpx_analysis-edf1101-1.7/gpx_analysis/__init__.py
+-rw-r--r--   0 edfillingham   (501) staff       (20)      322 2024-05-06 13:34:23.000000 gpx_analysis-edf1101-1.7/gpx_analysis/__main__.py
+-rw-r--r--   0 edfillingham   (501) staff       (20)    17000 2024-05-13 15:47:52.000000 gpx_analysis-edf1101-1.7/gpx_analysis/app.py
+-rw-r--r--   0 edfillingham   (501) staff       (20)     3652 2024-05-06 13:34:23.000000 gpx_analysis-edf1101-1.7/gpx_analysis/components.py
+-rw-r--r--   0 edfillingham   (501) staff       (20)     6163 2024-05-06 13:34:23.000000 gpx_analysis-edf1101-1.7/gpx_analysis/gpx_parser.py
+-rw-r--r--   0 edfillingham   (501) staff       (20)    22816 2024-05-13 15:50:43.000000 gpx_analysis-edf1101-1.7/gpx_analysis/graph_handler.py
+-rw-r--r--   0 edfillingham   (501) staff       (20)    12453 2024-05-13 14:55:16.000000 gpx_analysis-edf1101-1.7/gpx_analysis/gui.py
+-rw-r--r--   0 edfillingham   (501) staff       (20)    17378 2024-05-13 15:40:01.000000 gpx_analysis-edf1101-1.7/gpx_analysis/gui_control_menu.py
+-rw-r--r--   0 edfillingham   (501) staff       (20)    13548 2024-05-10 12:08:27.000000 gpx_analysis-edf1101-1.7/gpx_analysis/gui_finishline_menu.py
+-rw-r--r--   0 edfillingham   (501) staff       (20)     8789 2024-05-06 13:34:23.000000 gpx_analysis-edf1101-1.7/gpx_analysis/gui_playback_menu.py
+-rw-r--r--   0 edfillingham   (501) staff       (20)    16210 2024-05-06 13:34:23.000000 gpx_analysis-edf1101-1.7/gpx_analysis/gui_stats_menu.py
+-rw-r--r--   0 edfillingham   (501) staff       (20)     8851 2024-05-09 20:19:21.000000 gpx_analysis-edf1101-1.7/gpx_analysis/sporting.py
+-rw-r--r--   0 edfillingham   (501) staff       (20)     8759 2024-05-06 13:34:23.000000 gpx_analysis-edf1101-1.7/gpx_analysis/stats_graph_handler.py
+drwxr-xr-x   0 edfillingham   (501) staff       (20)        0 2024-05-13 16:02:09.071145 gpx_analysis-edf1101-1.7/gpx_analysis_edf1101.egg-info/
+-rw-r--r--   0 edfillingham   (501) staff       (20)     1889 2024-05-13 16:02:09.000000 gpx_analysis-edf1101-1.7/gpx_analysis_edf1101.egg-info/PKG-INFO
+-rw-r--r--   0 edfillingham   (501) staff       (20)      614 2024-05-13 16:02:09.000000 gpx_analysis-edf1101-1.7/gpx_analysis_edf1101.egg-info/SOURCES.txt
+-rw-r--r--   0 edfillingham   (501) staff       (20)        1 2024-05-13 16:02:09.000000 gpx_analysis-edf1101-1.7/gpx_analysis_edf1101.egg-info/dependency_links.txt
+-rw-r--r--   0 edfillingham   (501) staff       (20)       43 2024-05-13 16:02:09.000000 gpx_analysis-edf1101-1.7/gpx_analysis_edf1101.egg-info/requires.txt
+-rw-r--r--   0 edfillingham   (501) staff       (20)       13 2024-05-13 16:02:09.000000 gpx_analysis-edf1101-1.7/gpx_analysis_edf1101.egg-info/top_level.txt
+-rw-r--r--   0 edfillingham   (501) staff       (20)       38 2024-05-13 16:02:09.071466 gpx_analysis-edf1101-1.7/setup.cfg
+-rw-r--r--   0 edfillingham   (501) staff       (20)      733 2024-05-13 16:00:25.000000 gpx_analysis-edf1101-1.7/setup.py
```

### Comparing `gpx_analysis-edf1101-1.6/PKG-INFO` & `gpx_analysis-edf1101-1.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 Metadata-Version: 2.1
 Name: gpx_analysis-edf1101
-Version: 1.6
+Version: 1.7
 Summary: GPX Analysis Program
 Home-page: https://github.com/edf1101/Rowing-GPX-Analysis
 Author: edf1101
 Author-email: blank@blank.com
-License: UNKNOWN
-Description: # Rowing-GPX-Analysis
-        ## Introduction
-        _GPX Analysis for rowing written in Python with a tkinter matplotlib interface_
-        #### Why?
-        I couldn't find the code for the old GPX analysis tool I wrote, so I'm taking the
-        opportunity to build a better/ more robust one.
-        
-        ## Prerequisites
-        #### Python Requirements
-        - Python 3.11+
-        - Numpy ```pip install numpy```
-        - Matplotlib ```pip install matplotlib```
-        - tkScrolledFrame ```pip install tkScrolledFrame```
-        - Pillow (should already be installed with mpl) ```pip install pillow```
-        
-        _Given it downloads map images from online it requires an internet connection to run._
-        
-        ## Installation
-        - For Standard users go to the GitHub page and download from releases
-        - For Developers you can clone the repository, install the requirements and run as you wish.
-        - It can also be installed with ```pip install gpx-analysis-edf1101``` and run from command line with ```python -m gpx_analysis``` 
-        ## Getting Started & Notes
-        - For instructions on how to use please view the [Getting started page](Getting_started.md) on the project's GitHub
-        - On python due to tkinter bug workarounds it doesn't exit the application when you close the window, you will have to force quit it.
-        
-        ## Details
-        The project is hosted online at https://github.com/edf1101/Rowing-GPX-Analysis
-        
-        ### License & Policies
-        - This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
-        - The only exception to this is the example data, which should not be used elsewhere.
-        - Code in graph_handler.py to fetch images from tile servers should be used with caution to make sure you comply with the
-        terms of service of the tile server you are using.
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Rowing-GPX-Analysis
+
+<img src="readme_images/total.png" alt="drawing" width="400"/>
+
+[Video Demonstration](https://youtu.be/zElEyXIQTWE)
+
+
+## Introduction
+_GPX Analysis for rowing written in Python with a tkinter matplotlib interface_
+#### Why?
+I couldn't find the code for the old GPX analysis tool I wrote, so I'm taking the
+opportunity to build a better/ more robust one.
+
+## Prerequisites
+#### Python Requirements
+- Python 3.11+
+- Numpy ```pip install numpy```
+- Matplotlib ```pip install matplotlib```
+- appdirs ```pip install appdirs```
+- Pillow (should already be installed with mpl) ```pip install pillow```
+
+_Given it downloads map images from online it requires an internet connection to run._
+
+## Installation
+- It can also be installed with ```pip install gpx-analysis-edf1101``` and run from command line with ```python -m gpx_analysis``` 
+## Getting Started & Notes
+- For instructions on how to use please view the [Getting started page](Getting_started.md) on the project's GitHub
+
+## Details
+The project is hosted online at https://github.com/edf1101/GPX-Analysis
+
+### License & Policies
+- This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
+- The only exception to this is the example data, which should not be used elsewhere.
+- Code in graph_handler.py to fetch images from tile servers should be used with caution to make sure you comply with the
+terms of service of the tile server you are using.
```

### Comparing `gpx_analysis-edf1101-1.6/README.md` & `gpx_analysis-edf1101-1.7/gpx_analysis_edf1101.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,50 @@
+Metadata-Version: 2.1
+Name: gpx-analysis-edf1101
+Version: 1.7
+Summary: GPX Analysis Program
+Home-page: https://github.com/edf1101/Rowing-GPX-Analysis
+Author: edf1101
+Author-email: blank@blank.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Rowing-GPX-Analysis
+
+<img src="readme_images/total.png" alt="drawing" width="400"/>
+
+[Video Demonstration](https://youtu.be/zElEyXIQTWE)
+
+
 ## Introduction
 _GPX Analysis for rowing written in Python with a tkinter matplotlib interface_
 #### Why?
 I couldn't find the code for the old GPX analysis tool I wrote, so I'm taking the
 opportunity to build a better/ more robust one.
 
 ## Prerequisites
 #### Python Requirements
 - Python 3.11+
 - Numpy ```pip install numpy```
 - Matplotlib ```pip install matplotlib```
-- tkScrolledFrame ```pip install tkScrolledFrame```
+- appdirs ```pip install appdirs```
 - Pillow (should already be installed with mpl) ```pip install pillow```
 
 _Given it downloads map images from online it requires an internet connection to run._
 
 ## Installation
-- For Standard users go to the GitHub page and download from releases
-- For Developers you can clone the repository, install the requirements and run as you wish.
 - It can also be installed with ```pip install gpx-analysis-edf1101``` and run from command line with ```python -m gpx_analysis``` 
 ## Getting Started & Notes
 - For instructions on how to use please view the [Getting started page](Getting_started.md) on the project's GitHub
-- On python due to tkinter bug workarounds it doesn't exit the application when you close the window, you will have to force quit it.
 
 ## Details
-The project is hosted online at https://github.com/edf1101/Rowing-GPX-Analysis
+The project is hosted online at https://github.com/edf1101/GPX-Analysis
 
 ### License & Policies
 - This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
 - The only exception to this is the example data, which should not be used elsewhere.
 - Code in graph_handler.py to fetch images from tile servers should be used with caution to make sure you comply with the
-terms of service of the tile server you are using.
+terms of service of the tile server you are using.
```

### Comparing `gpx_analysis-edf1101-1.6/gpx_analysis/app.py` & `gpx_analysis-edf1101-1.7/gpx_analysis/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 # pylint: disable=R0914
 
 import time
 # Import external libs
 import tkinter as tk
 import pathlib
 import random
+import numpy as np
 
 try:
     from gpx_analysis import gpx_parser as gpx
     from gpx_analysis import graph_handler as gh
     from gpx_analysis.gui import AppGUI
     from gpx_analysis import sporting as sport
     from gpx_analysis import components as geo
 except ImportError:
     import gpx_parser as gpx
     import graph_handler as gh
-    from gpx_analysis.gui import AppGUI
+    from gui import AppGUI
     import sporting as sport
     import components as geo
 
 
 class GpxAnalysisApp:
     """
     This app handles all the functionality of the GPX analysis tool
@@ -88,14 +89,15 @@
         self.__gui.set_set_plaback_speed_callback(self.__set_playback_speed)
         self.__gui.set_set_playback_time_callback(self.set_playback_time)
         self.__gui.set_get_playback_time_callback(self.get_playback_time)
         self.__gui.set_zoom_level_callback(self.__set_zoom_level)
         self.__gui.set_set_start_finish_time_callback(self.__set_start_finish_times)
         self.__gui.set_get_start_finish_time_callback(self.__get_start_finish_times)
         self.__gui.set_on_colour_change(self.__on_athlete_colour_change)
+        self.__gui.set_on_colourscheme_change(self.__on_athlete_colourscheme_change)
 
     def __get_playing(self) -> bool:
         """
         A getter for the playing variable
 
         :return: is the simulation playing or not
         """
@@ -258,21 +260,36 @@
             # print("Already been imported")
             return
 
         # Clean up the filename
         path = pathlib.PurePath(filename)
         clean_path = f'/{path.parent.name}/{path.name}'
 
+        # calculate stats for athlete speed throughout the track
+        speed_data = []
+        for track_point in new_track.get_track_points():
+            speed_data.append(sport.get_speed_at_time(new_track, track_point.time))
+        speed_data = np.array(speed_data)
+        speed_mean = np.mean(speed_data)
+        speed_max = np.max(speed_data)
+        speed_std = np.std(speed_data)
+        outlier_std_count = 1.5  # how many standard deviations to consider an outlier
+        # calculate the acceptable range for the speed, outside of this range is considered outlier
+        speed_range = [speed_mean - outlier_std_count * speed_std, speed_mean + outlier_std_count * speed_std]
+        print(speed_range)
+
         # We will put the athlete data into the list as a dict of the important parts
         athlete_data = {'track': new_track,
                         "filename": clean_path,
                         'display_name': clean_path,
                         'colour': self.__assign_colour(),
+                        'colour_scheme': 'normal',
                         'start_time': 0,
-                        'finish_time': new_track.get_total_time()}
+                        'finish_time': new_track.get_total_time(),
+                        'speed_range': speed_range}
 
         self.__athletes[clean_path] = athlete_data
 
         self.__mpl_map.add_athlete(clean_path, athlete_data)  # add it to the map
 
         # update the GUI's list of athletes
         self.__gui.update_athletes(self.__athletes)
@@ -326,42 +343,61 @@
         # update the map's list of athletes and then update the map image on the GUI
         self.__mpl_map.modify_athlete(athlete_key, self.__athletes[athlete_key])
         self.__gui.update_map()
 
         # update the gui's stats display with the new name
         self.__gui.update_stats()
 
+    def __on_athlete_colourscheme_change(self, athlete_key: str, scheme: str):
+        """
+        Called when an athlete's colour scheme is changed
+
+        :param athlete_key: The athlete to change
+        :param scheme: The new scheme to change to. (normal, speed)
+        """
+
+        print(f'{athlete_key} changed their colour scheme to {scheme}')
+
+        # modify athlete data in this class
+        self.__athletes[athlete_key]['colour_scheme'] = scheme
+
+        # update the guis's list of athletes
+        self.__gui.update_athletes(self.__athletes)
+
+        # update the map's list of athletes and then update the map image on the GUI
+        self.__mpl_map.modify_athlete(athlete_key, self.__athletes[athlete_key])
+        self.__gui.update_map(force=True)
+
     def __on_athlete_colour_change(self, athlete_key: str,
                                    colour: tuple[float, float, float]) -> None:
         """
         Gets called when an athlete changes their colour
 
         :param athlete_key: The key of the athlete changing colour
         :param colour: The colour changing to
         :return: None
         """
 
         # update the data in the app class dict
         self.__athletes[athlete_key]['colour'] = colour
 
         # update the guis's list of athletes
-        self.__gui.update_athletes(self.__athletes,remake_widgets=False)
+        self.__gui.update_athletes(self.__athletes, remake_widgets=False)
 
         # update the map
         self.__mpl_map.modify_athlete(athlete_key, self.__athletes[athlete_key])
         self.__gui.update_map()
 
     def __on_athlete_deleted(self, athlete_key: str) -> None:
         """
         Callback function for when an athlete is deleted
 
         :param athlete_key: The dictionary key for the athlete we are deleting
         :return: None
         """
-        # print(f'{athlete_key} got deleted')
 
         if len(self.__athletes) - 1 == 0:  # if its now empty
             self.__mpl_map.reset()
             self.__gui.update_map()
         else:
             # first remove from the map and update it
             self.__mpl_map.remove_athlete(athlete_key)
```

### Comparing `gpx_analysis-edf1101-1.6/gpx_analysis/components.py` & `gpx_analysis-edf1101-1.7/gpx_analysis/components.py`

 * *Files identical despite different names*

### Comparing `gpx_analysis-edf1101-1.6/gpx_analysis/gpx_parser.py` & `gpx_analysis-edf1101-1.7/gpx_analysis/gpx_parser.py`

 * *Files identical despite different names*

### Comparing `gpx_analysis-edf1101-1.6/gpx_analysis/graph_handler.py` & `gpx_analysis-edf1101-1.7/gpx_analysis/graph_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 import matplotlib
 import matplotlib.pyplot as plt
 import matplotlib.patches as mpatches
 
 try:
     from gpx_analysis import components as geo
     from gpx_analysis import gpx_parser as gpx
+    from gpx_analysis import sporting as sport
 except ImportError:
     import components as geo
     import gpx_parser as gpx
+    import sporting as sport
 
 # If we are on macos then run this to fix the issues
 if sys_pf == 'darwin':
     matplotlib.use("TkAgg")
 
 
 def deg2num(lat_deg: float, lon_deg: float, zoom: int) -> tuple[int, int]:
@@ -231,17 +233,19 @@
         :param new_value: The new value
         :return: None
         """
 
         # modify new parts individually so we don't remove references to drawn tracks/ points
         self.__athletes[athlete_key]['colour'] = new_value['colour']
         self.__athletes[athlete_key]['display_name'] = new_value['display_name']
+        self.__athletes[athlete_key]['colour_scheme'] = new_value['colour_scheme']
 
         # redo track / legend which contain old data / colours
-        self.draw_track(athlete_key, new_value['colour'])
+        colour = new_value['colour'] if new_value['colour_scheme'] == 'normal' else 'speed'
+        self.draw_track(athlete_key, colour)
         self.__draw_legend()
 
     def modify_start_finish_times(self, athlete_key: str, start: float, finish: float) -> None:
         """
         Modifies the start and finish times for an athlete
 
         :param athlete_key: The key to modify in the dictionary
@@ -455,23 +459,40 @@
         if ('draw_track' in self.__athletes[athlete_key] and
                 self.__athletes[athlete_key]['draw_track'] is not None):
             self.__remove_drawn_track(athlete_key)
 
         track = self.__athletes[athlete_key]['track']
         line_data = []
 
+        color_scheme = 'speed' if color == 'speed' else 'normal'
+        if color == 'speed':
+            speed_range = self.__athletes[athlete_key]['speed_range']  # get the acceptable speed range
+
         for i in range(len(track.get_track_points()) - 1):
             start_point = track.get_track_points()[i]  # get start and end points of line
             end_point = track.get_track_points()[i + 1]
 
             # dont plot this line if its out of the start finish zone
             if (end_point.get_relative_time() < self.__athletes[athlete_key]['start_time'] or
                     start_point.get_relative_time() > self.__athletes[athlete_key]['finish_time']):
                 continue
 
+            if color_scheme == 'speed':  # if the colour scheme is speed then calculate the new colour
+                speed = sport.get_speed_at_time(track, start_point.get_relative_time())
+                # make it grey if it's an outlier
+                if speed is None or speed < speed_range[0] :
+                    color = 'grey'
+                elif speed > speed_range[1]:
+                    color = (0, 1, 0)
+                else:
+                    # scale the speed to be between 0 and 1
+                    speed = (speed - speed_range[0]) / (speed_range[1] - speed_range[0])
+                    # lerp between red and green
+                    color = (1 - speed, speed, 0)
+
             single_line = self.draw_line(start_point.get_position_degrees(),
                                          end_point.get_position_degrees(),
                                          color=color)
             line_data.append(single_line)
 
         self.__athletes[athlete_key]['draw_track'] = line_data
```

### Comparing `gpx_analysis-edf1101-1.6/gpx_analysis/gui.py` & `gpx_analysis-edf1101-1.7/gpx_analysis/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """
 This script contains the main GUI class
 The AppGUI class is the only one to use outside of this class
 """
-# Pylint ignores
+# Pylint ignores some are just wrongly generated
 # pylint: disable=R0902
 # pylint: disable=R0914
 # pylint: disable=R0904
+# pylint: disable=E0401
 
 import tkinter as tk
 from tkinter import ttk
 import time
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg  # for importing figs to mpl
+from tkscrollableframe import ScrolledFrame
 
 # import the individual separate classes
 try:
     from gpx_analysis import graph_handler as gh
     from gpx_analysis.gui_control_menu import ControlMenuFrame
     from gpx_analysis.gui_finishline_menu import FinishlineMenuFrame
     from gpx_analysis.gui_playback_menu import PlaybackMenuFrame
     from gpx_analysis.gui_stats_menu import StatsMenuFrame
-    from gpx_analysis.tkscrolledframe import ScrolledFrame
 except ImportError:
     from .gui_control_menu import ControlMenuFrame
     from .gui_finishline_menu import FinishlineMenuFrame
     from .gui_playback_menu import PlaybackMenuFrame
     from .gui_stats_menu import StatsMenuFrame
-    from gpx_analysis import graph_handler as gh
-    from gpx_analysis.tkscrolledframe import ScrolledFrame
 
 
 class AppGUI:
     """
     Class containing the entire GUI for the GPX Analysis App, using OOP so encapsulation makes
     it better for modularity, readability etc.
     """
@@ -102,14 +101,15 @@
 
         self.set_zoom_level = None
 
         self.set_start_finish_time = None
         self.get_start_finish_time = None
 
         self.on_colour_change = None
+        self.on_colourscheme_change = None
 
         # Athlete list
         self.__athletes = {}
 
         # Set the submenus here after the other variables have been set
         self.__set_submenus()
 
@@ -184,15 +184,15 @@
 
         :param event:
         :return:
         """
         if not isinstance(event.widget, ttk.Entry):
             self.__window.focus()
 
-    def update_map(self,force:bool = False) -> None:
+    def update_map(self, force: bool = False) -> None:
         """
         This sets/ updates the mpl figure map on the GUI
 
         :param force: whether to force an update regardless of whether it's too soon
         :return: None
         """
 
@@ -359,15 +359,24 @@
         Sets the callback function to be used when a start or finish time is requested
 
         :param func: The function to be called
         :return: None
         """
         self.get_start_finish_time = func
 
-    def set_on_colour_change(self,func) -> None:
+    def set_on_colour_change(self, func) -> None:
         """
         Setter for on colour change callback func
 
         :param func: the function to be called
         :return: None
         """
         self.on_colour_change = func
+
+    def set_on_colourscheme_change(self, func) -> None:
+        """
+        Setter for on colourscheme change callback func
+
+        :param func: the function to be called
+        :return: None
+        """
+        self.on_colourscheme_change = func
```

### Comparing `gpx_analysis-edf1101-1.6/gpx_analysis/gui_control_menu.py` & `gpx_analysis-edf1101-1.7/gpx_analysis/gui_control_menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         # Athlete Data
         self.__athlete_data = {}
 
         # This centers the items (unless we specify a stickiness)
         self.__frm_map_control_menu.grid_columnconfigure(0, weight=1)
 
         # Set up the widgets that won't ever change
+        self.__checkbox_control_colourscheme = None  # For changing colour scheme of a track
         self.__setup_static_widgets()
 
         # Create the name selector / deletion menu and initialise its variables here
         self.__last_selected = None  # Holds the last athlete selected so we know what swapped
         self.__athlete_names = ['None']
         self.__frm_map_control_dropdown = None
         self.__dropdown_map_control = None
@@ -78,14 +79,31 @@
         if len(athlete_data):
             self.__athlete_names = [v['display_name'] for v in athlete_data.values()]
         else:
             self.__athlete_names = ['None']
 
         if remake_widgets:
             self.__create_name_selector()  # recreate name selector with new fields
+
+            # get selected athlete key
+            athlete_key = None
+            # Also need to find the current filename.
+            for key, value in self.__athlete_data.items():
+
+                if value['display_name'] == self.__last_selected:
+                    athlete_key = key
+
+            # if it is found then change it in the callback function
+
+            if athlete_key:
+                print('found')
+                speed_colourscheme_state = athlete_data[athlete_key]['colour_scheme'] == 'speed'
+                flag = 'selected' if speed_colourscheme_state else '!selected'
+                self.__checkbox_control_colourscheme.state(['!disabled', flag])
+
             self.__set_athlete_data()
 
     def __setup_namechange(self) -> None:
         """
         Sets up the name change frame data
 
         :return: None
@@ -228,28 +246,65 @@
         self.__frm_map_control_menu.rowconfigure(4, minsize=30)
 
         # This won't be modified either
         label_control_menu_changename = ttk.Label(master=self.__frm_map_control_menu,
                                                   text="Change display name:")
         label_control_menu_changename.grid(row=7, column=0, sticky='w', )
 
+        self.__setup_colourscheme_checkbox()
+
         # add the button to change colours
         self.__btn_colour_picker = ttk.Button(master=self.__frm_map_control_menu,
                                               text="Change colour",
                                               command=self.__on_change_colour)
-        self.__btn_colour_picker.grid(row=9, column=0, sticky='w')
+        self.__btn_colour_picker.grid(row=10, column=0, sticky='w')
+
+    def __setup_colourscheme_checkbox(self):
+        """
+        Set up the colour scheme checkbox
+
+        :return: None
+        """
+
+        # have a checkbox to decide whether to show tracks as speed gradient
+        self.__checkbox_control_colourscheme = ttk.Checkbutton(master=self.__frm_map_control_menu,
+                                                               text="Speed Colour Scheme",
+                                                               command=self.__on_checkbox_change)
+        self.__checkbox_control_colourscheme.state(['!disabled', '!selected'])
+        self.__checkbox_control_colourscheme.state(['!alternate'])
+        self.__checkbox_control_colourscheme.grid(row=9, column=0, sticky='w')
+
+    def __on_checkbox_change(self):
+        """
+        Called when the checkbox is changed
+        """
+
+        state = self.__checkbox_control_colourscheme.instate(['selected'])
+
+        # Get the athlete's key
+        athlete_key = None
+
+        # Also need to find the current filename.
+        for key, value in self.__athlete_data.items():
+
+            if value['display_name'] == self.__last_selected:
+                athlete_key = key
+
+        # if it is found then change it in the callback function
+        if athlete_key:
+            self.__parent_class.on_colourscheme_change(athlete_key, "speed" if state else "normal")
 
     def __on_open_press(self) -> None:
         """
         When the open file button is pressed this is called
 
         :return: None
         """
 
-        file_path = filedialog.askopenfilename()  # get the file path
+        file_path = filedialog.askopenfilename(filetypes=[('GPX Files', '*.gpx')])  # get gpx path
         if file_path != '':  # check it's not blank
             self.__open_file_callback(file_path)
 
     def __on_change_colour(self) -> None:
         """
         Gets called when the change colour button is pressed
 
@@ -318,14 +373,20 @@
 
         # Also need to find the current athlete key
         for key, value in self.__athlete_data.items():
 
             if value['display_name'] == self.__last_selected:
                 athlete_key = key
 
+        # modify colourscheme checkbox
+        if athlete_key:
+            speed_colourscheme_state = self.__athlete_data[athlete_key]['colour_scheme'] == 'speed'
+            flag = 'selected' if speed_colourscheme_state else '!selected'
+            self.__checkbox_control_colourscheme.state(['!disabled', flag])
+
         self.__parent_class.set_finishline_athlete_selected(athlete_key)
         self.__parent_class.stop_finish_start_editing()
 
     def __on_name_change(self) -> None:
         """
         This gets triggered when the name change confirm button is pressed
```

### Comparing `gpx_analysis-edf1101-1.6/gpx_analysis/gui_finishline_menu.py` & `gpx_analysis-edf1101-1.7/gpx_analysis/gui_finishline_menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This script contains the finishline sub frame class related to the tk GUI
 The AppGUI class is the only one to use outside of this class
 """
 # Pylint ignores
 # pylint: disable=R0902
 # pylint: disable=R0914
+
 import tkinter as tk
 from tkinter import ttk
 import tkinter.messagebox as msgbox  # for popups
 
 
 class FinishlineMenuFrame:
     """
```

### Comparing `gpx_analysis-edf1101-1.6/gpx_analysis/gui_playback_menu.py` & `gpx_analysis-edf1101-1.7/gpx_analysis/gui_playback_menu.py`

 * *Files identical despite different names*

### Comparing `gpx_analysis-edf1101-1.6/gpx_analysis/gui_stats_menu.py` & `gpx_analysis-edf1101-1.7/gpx_analysis/gui_stats_menu.py`

 * *Files identical despite different names*

### Comparing `gpx_analysis-edf1101-1.6/gpx_analysis/sporting.py` & `gpx_analysis-edf1101-1.7/gpx_analysis/sporting.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     Returns the two points either side of a given time
 
     :param track: The input track
     :param time: The time to get the points at
     :return: Two gpx.Trackpoint points
     """
 
-
     track_points = track.get_track_points()
 
     # Iterate through all points to find the two points either side of the position
     # Also get the time the boat was at these two points
 
     point_id_above, point_id_below = None, None
     for point_id, point in enumerate(track_points):
@@ -98,23 +97,32 @@
     if time > last_point.get_relative_time():
         # WARNING this time is after the end time it is technically invalid
         return 0.1
 
     # Get the points above and below
     point_below, point_above = get_surrounding_points_at_time(track, time)
 
+    # try to widen the range of points
+    if point_below is not None:
+        below_ind = track_points.index(point_below)
+    if point_above is not None:
+        above_ind = track_points.index(point_above)
+
+    can_expand = point_above is not None and point_below is not None and (below_ind - 2 > 0) and (above_ind + 2 < len(track_points))
+    if can_expand:
+        point_below = track_points[below_ind - 2]
+        point_above = track_points[above_ind + 2]
+
     try:
         position_below = point_below.get_position_degrees()
         position_above = point_above.get_position_degrees()
     except AttributeError:  # when out of range this happens
         return 0.1
 
-    time_below = point_below.get_relative_time()
-    time_above = point_above.get_relative_time()
-    time_delta = time_above - time_below
+    time_delta = point_above.get_relative_time() - point_below.get_relative_time()
 
     # Get distance between two points
     distance = geo.geo_distance(position_below[0], position_below[1],
                                 position_above[0], position_above[1])
 
     speed = distance / time_delta  # Speeds are always in m/s
```

### Comparing `gpx_analysis-edf1101-1.6/gpx_analysis/stats_graph_handler.py` & `gpx_analysis-edf1101-1.7/gpx_analysis/stats_graph_handler.py`

 * *Files identical despite different names*

### Comparing `gpx_analysis-edf1101-1.6/gpx_analysis_edf1101.egg-info/SOURCES.txt` & `gpx_analysis-edf1101-1.7/gpx_analysis_edf1101.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 gpx_analysis/__init__.py
 gpx_analysis/__main__.py
 gpx_analysis/app.py
 gpx_analysis/components.py
 gpx_analysis/gpx_parser.py
@@ -9,13 +10,12 @@
 gpx_analysis/gui.py
 gpx_analysis/gui_control_menu.py
 gpx_analysis/gui_finishline_menu.py
 gpx_analysis/gui_playback_menu.py
 gpx_analysis/gui_stats_menu.py
 gpx_analysis/sporting.py
 gpx_analysis/stats_graph_handler.py
-gpx_analysis/tkscrolledframe.py
 gpx_analysis_edf1101.egg-info/PKG-INFO
 gpx_analysis_edf1101.egg-info/SOURCES.txt
 gpx_analysis_edf1101.egg-info/dependency_links.txt
 gpx_analysis_edf1101.egg-info/requires.txt
 gpx_analysis_edf1101.egg-info/top_level.txt
```

### Comparing `gpx_analysis-edf1101-1.6/setup.py` & `gpx_analysis-edf1101-1.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setuptools.setup(
     name="gpx_analysis-edf1101",
-    version="1.6",
+    version="1.7",
     author="edf1101",
     author_email="blank@blank.com",
     description="GPX Analysis Program",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/edf1101/Rowing-GPX-Analysis",
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.11",
-    install_requires=["matplotlib", "numpy", "appdirs"]
+    install_requires=["matplotlib", "numpy", "appdirs", "tkscrollableframe"]
 )
```

