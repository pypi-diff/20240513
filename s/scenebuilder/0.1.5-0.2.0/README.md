# Comparing `tmp/scenebuilder-0.1.5.tar.gz` & `tmp/scenebuilder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenebuilder-0.1.5.tar", max compression
+gzip compressed data, was "scenebuilder-0.2.0.tar", max compression
```

## Comparing `scenebuilder-0.1.5.tar` & `scenebuilder-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-10-19 10:53:34.751175 scenebuilder-0.1.5/LICENSE
--rw-r--r--   0        0        0     3771 2024-05-07 15:17:47.657485 scenebuilder-0.1.5/README.md
--rw-r--r--   0        0        0      486 2024-05-07 15:18:28.059816 scenebuilder-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       39 2024-05-06 09:11:58.678352 scenebuilder-0.1.5/scenebuilder/__init__.py
--rw-r--r--   0        0        0     1020 2024-05-07 09:01:36.601969 scenebuilder-0.1.5/scenebuilder/actions_stack.py
--rw-r--r--   0        0        0     4951 2024-05-07 08:15:28.842583 scenebuilder-0.1.5/scenebuilder/entities.py
--rw-r--r--   0        0        0      604 2024-05-07 05:46:06.554704 scenebuilder-0.1.5/scenebuilder/main.py
--rw-r--r--   0        0        0      454 2024-05-05 23:20:17.691922 scenebuilder-0.1.5/scenebuilder/mixins.py
--rw-r--r--   0        0        0     2196 2024-05-07 10:52:47.060418 scenebuilder-0.1.5/scenebuilder/observer_utils.py
--rw-r--r--   0        0        0     4211 2024-05-07 06:08:47.691838 scenebuilder-0.1.5/scenebuilder/patch_manager.py
--rw-r--r--   0        0        0     4334 2024-05-07 05:25:24.471252 scenebuilder-0.1.5/scenebuilder/patches.py
--rw-r--r--   0        0        0    23610 2024-05-07 13:49:30.666638 scenebuilder-0.1.5/scenebuilder/scenebuilder.py
--rw-r--r--   0        0        0     4060 2024-05-07 14:23:30.282485 scenebuilder-0.1.5/scenebuilder/ui_components.py
--rw-r--r--   0        0        0     4254 2024-05-07 08:21:02.590859 scenebuilder-0.1.5/scenebuilder/utils.py
--rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 scenebuilder-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-19 10:53:34.751175 scenebuilder-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3865 2024-05-13 08:06:35.188088 scenebuilder-0.2.0/README.md
+-rw-r--r--   0        0        0      486 2024-05-13 08:23:52.492933 scenebuilder-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-05-06 09:11:58.678352 scenebuilder-0.2.0/scenebuilder/__init__.py
+-rw-r--r--   0        0        0     1019 2024-05-13 07:57:11.213416 scenebuilder-0.2.0/scenebuilder/actions_stack.py
+-rw-r--r--   0        0        0     5175 2024-05-13 06:52:11.593985 scenebuilder-0.2.0/scenebuilder/entities.py
+-rw-r--r--   0        0        0      691 2024-05-13 06:48:30.899585 scenebuilder-0.2.0/scenebuilder/main.py
+-rw-r--r--   0        0        0      454 2024-05-13 06:48:29.276267 scenebuilder-0.2.0/scenebuilder/mixins.py
+-rw-r--r--   0        0        0     2196 2024-05-13 06:48:28.415383 scenebuilder-0.2.0/scenebuilder/observer_utils.py
+-rw-r--r--   0        0        0     4207 2024-05-13 06:48:27.525252 scenebuilder-0.2.0/scenebuilder/patch_manager.py
+-rw-r--r--   0        0        0     4333 2024-05-13 06:48:26.526321 scenebuilder-0.2.0/scenebuilder/patches.py
+-rw-r--r--   0        0        0    24786 2024-05-13 07:56:47.555041 scenebuilder-0.2.0/scenebuilder/scenebuilder.py
+-rw-r--r--   0        0        0     6966 2024-05-13 08:22:13.364886 scenebuilder-0.2.0/scenebuilder/ui_components.py
+-rw-r--r--   0        0        0     7738 2024-05-13 07:56:01.623626 scenebuilder-0.2.0/scenebuilder/utils.py
+-rw-r--r--   0        0        0     4394 1970-01-01 00:00:00.000000 scenebuilder-0.2.0/PKG-INFO
```

### Comparing `scenebuilder-0.1.5/LICENSE` & `scenebuilder-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.5/README.md` & `scenebuilder-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,17 +16,14 @@
 
 ```bash
 pip install scenebuilder
 ```
 
 This command installs SceneBuilder along with numpy and matplotlib, ensuring that everything needed to run the GUI is properly set up.
 
-
-
-
 ## Prerequisites
 
 SceneBuilder's prerequisites are defined in the pyproject.toml file and include Matplotlib and numpy.
 
 ## Quick Start Guide
 
 ### Using Command-Line Options
@@ -39,14 +36,15 @@
 Example usage:
 
 ```bash
 scenebuilder --load path/to/scene.json --output path/to/output.json
 ```
 
 ### In Code
+
 To use SceneBuilder in code, you need to create an instance of the `SceneBuilder` class and invoke the `draw_scene()` method. Below is a simple example to get you started:
 
 ```python
 from scenebuilder import SceneBuilder
 
 # Create an instance of the SceneBuilder
 scene = SceneBuilder()
@@ -65,30 +63,28 @@
 Specify the path to save your output json to:
 
 ```python
 scene.set_output_path("path/to/output.json")
 scene.draw_scene()
 ```
 
-
-
 ## Features
 
 - **Draw Obstacles**: Click within the GUI to place vertices of polygons that represent obstacles. Press Tab to complete an obstacle.
 - **Add new obstacle vertices**: To add new vertices, click somewhere on the polygon's perimeter and drag to move the vertex to its desired location.
 - **Set Drone Paths**: Click once to place the starting point, and again to place the goal of an agent/drone. An arrow will automatically be drawn from start to goal.
 - **Move or adjust existing obstacles/drones**: Obstacles and drones can be moved by clicking and dragging. Drone start and goal points, as well as existing obstacle vertices can be moved in the same way.
 - **Switch between Obstacle and Drone Modes**: Press b to switch to building/obstacle mode. Press d to switch to drone/agent mode. Alternatively click the Switch button on the bottom left of the gui.
 - **Delete obstacles**: Select the obstacle and press delete or backspace. NOTE this is not yet available for drones.
 - **Remove unwanted points**: To remove unwanted points (either obstacle vertices or a drone start point), press escape.
 - **Undo drone/obstacle placement**: To remove the last obstacle or drone, press ctrl+z.
 - **Reset Scene**: To reset the scene to a blank canvas, click the Reset button in the gui.
 
 ## Saving Scenes
 
-Once you have created a scene, you can save it to a JSON file by clicking the 'Create JSON' button in the GUI. This file can then be used as input for path planning algorithms that require predefined scenes with obstacles and paths.
+Once you have created a scene, you can save it to a JSON or GeoJSON file by clicking the 'Save' button in the GUI. You will then be prompted to select whether you want to use our basic JSON format or GeoGSON. This file can then be used as input for path planning algorithms that require predefined scenes with obstacles and paths.
 
 **_Unless otherwise specified, the file is saved as "scenebuilder.json" in the current working directory._**
 
 ## Contributing
 
 Contributions to SceneBuilder are welcome! If you have suggestions for improvements or new features, feel free to create an issue or pull request on our GitHub repository.
```

### Comparing `scenebuilder-0.1.5/scenebuilder/actions_stack.py` & `scenebuilder-0.2.0/scenebuilder/actions_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             pass
         self.actions.append((action_type, action))
 
     def remove_action(self, action_type: str, action):
         try:
             self.actions.remove((action_type, action))
         except ValueError:
-            # this is in case a json was loaded and therefore the 
+            # this is in case a json was loaded and therefore the
             # object is not in the stack
             pass
 
     def retrieve_last_action(self):
         if self.actions:
             return self.actions.pop()
```

### Comparing `scenebuilder-0.1.5/scenebuilder/entities.py` & `scenebuilder-0.2.0/scenebuilder/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,17 @@
 
 class Obstacle(Entity):
     """Class containing all necessary information about a Building Entity, not including its graphics"""
 
     def __init__(self, vertices: ArrayLike):
         super().__init__(ID="building", position=None)
         # self.vertices = self.sort_vertices(vertices[:, :2])
+        # Ensure the first and last vertices are not the same
+        if np.array_equal(vertices[0, :2], vertices[-1, :2]):
+            vertices = vertices[:-1, :2]  # Remove the last vertex if it's the same as the first one
         self.vertices = vertices[:, :2]
 
     def sort_vertices(self, vertices):
         """Sorts the vertices by angle around the centre of mass of the polygon"""
         Xavg = np.mean(vertices[:, 0:1])
         Yavg = np.mean(vertices[:, 1:2])
         angles = np.arctan2(
@@ -112,15 +115,14 @@
         return False
 
     def _point_near_edge(self, point, start, end, tolerance):
         """Check if the point is near the edge defined by start and end points"""
         # Compute the distance of the point from the line segment
         line_vector = np.array(end) - np.array(start)
         point_vector = np.array(point) - np.array(start)
-
         # Compute the projection of point_vector onto line_vector
         proj_length = np.dot(point_vector, line_vector) / np.linalg.norm(line_vector)
 
         if 0 <= proj_length <= np.linalg.norm(line_vector):
             # The projection is on the line segment
             proj_vector = proj_length * line_vector / np.linalg.norm(line_vector)
             distance = np.linalg.norm(point_vector - proj_vector)
```

### Comparing `scenebuilder-0.1.5/scenebuilder/observer_utils.py` & `scenebuilder-0.2.0/scenebuilder/observer_utils.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.5/scenebuilder/patch_manager.py` & `scenebuilder-0.2.0/scenebuilder/patch_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from matplotlib.lines import Line2D
 from typing import List
 import numpy as np
 from .entities import Obstacle, Drone
 from .patches import ObstaclePatch, DronePatch, Marker
 
+
 class PatchManager:
     def __init__(self, ax: plt.Axes):
         self.ax = ax
         self.building_patches: dict[Obstacle, ObstaclePatch] = {}
         self.drone_patches: dict[Drone, DronePatch] = {}
         # self.temp_drone_starts:list[Line2D] = []
         self.current_building_vertices: list[Line2D] = []
@@ -104,9 +105,7 @@
         for patch in self.building_patches.values():
             patch.remove()
         for patch in self.drone_patches.values():
             patch.remove()
         self.remove_temp_drone_start()
         self.building_patches.clear()
         self.drone_patches.clear()
-
-
```

### Comparing `scenebuilder-0.1.5/scenebuilder/patches.py` & `scenebuilder-0.2.0/scenebuilder/patches.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,8 +128,7 @@
         """Revert appearance to the original state."""
         self.set_facecolor(self.original_facecolor)
         self.set_edgecolor(self.original_edgecolor)
 
     def update_visual(self):
         """Update the visual representation based on the building state."""
         self.set_xy(self.building.vertices)
-
```

### Comparing `scenebuilder-0.1.5/scenebuilder/scenebuilder.py` & `scenebuilder-0.2.0/scenebuilder/scenebuilder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 
 import matplotlib.pyplot as plt
 
 import numpy as np
 
 from .entities import Drone, Obstacle
-from .utils import distance_between_points, create_json, get_from_json
+from .utils import distance_between_points, create_json, get_case_from_dict, convert_from_geojson
 from .utils import load_from_json, validate_json_path
 from .patch_manager import PatchManager
 from .actions_stack import ActionsStack
 from .ui_components import UIComponents
 from .observer_utils import Observer, Observable
 from threading import Timer
 from pathlib import Path
 import traceback
 import os
 
+
 class SceneBuilder(Observer, Observable):
 
     CLICK_THRESHOLD = 0.14
     FIG_SIZE = (8, 8.5)
     AXIS_LIMITS = (-5, 5)
 
     def __init__(self):
@@ -27,40 +28,43 @@
         super().__init__()
         self._selected_building: Obstacle = None
         self.original_colors: dict = {}
         # Setup the default plot
         self._plot_setup()
         # Define variables
         self._setup_data()
-        
+
         # Connect event handlers
         self._connect_event_handlers()
 
-    def set_output_path(self, path: str, exit = False, skip_check = False) -> None:
-        '''Set output path to validated path. call sys.exit() if exit is True and path is invalid'''
+    def set_output_path(self, path: str, exit=False, skip_check=False) -> None:
+        """Set output path to validated path. call sys.exit() if exit is True and path is invalid"""
         try:
             if not skip_check:
                 # Validate the path if not skipping
                 response = validate_json_path(path, exit)
-                result = response['result']
-                #if path invalid, don't set
+                result = response["result"]
+                # if path invalid, don't set
                 if result == 0:
                     return
         finally:
             # This block runs whether validation was skipped, passed, or failed.
             self.output_path = path
             self.ui_components.modify_current_file_text(self.output_path)
-            self._show_warning(f'Set new output path\n{path}', 3, color='g')
+            self._show_warning(f"Set new output path\n{path}", 3, color="g")
 
     def load_scene(self, path: str) -> None:
         """Populates the scene with the obstacles and drones in the specified json
         path: path to compatible json file"""
         self._reset()
-        case_info = load_from_json(path)
-        drones, buildings = get_from_json(case_info)
+        if path.endswith('.geojson'):
+            case_info = convert_from_geojson(path)
+        else:
+            case_info = load_from_json(path)
+        drones, buildings = get_case_from_dict(case_info)
         self.drones = drones
         self.buildings = buildings
         for building in self.buildings:
             self.patch_manager.add_building_patch(building)
         for drone in self.drones:
             self.patch_manager.add_drone_patch(drone)
         self._update()
@@ -69,15 +73,15 @@
         """Draw the scene."""
         plt.show()
 
     def _plot_setup(self):
         fig = plt.figure(figsize=self.FIG_SIZE)
         ax = fig.add_subplot(111)
 
-        fig.subplots_adjust(bottom=0.05, top=0.9)
+        fig.subplots_adjust(bottom=0.1, top=0.85, left=0)
 
         ax.set_xlim(self.AXIS_LIMITS)
         ax.set_ylim(self.AXIS_LIMITS)
         ax.set_box_aspect(1)
         ax.grid(color="k", linestyle="-", linewidth=0.5, which="major")
         ax.grid(color="k", linestyle=":", linewidth=0.5, which="minor")
         # ax.grid(True)
@@ -95,54 +99,52 @@
         fig.text(
             0.2,
             0.91,
             instructions,
             fontsize=10,
             bbox=dict(boxstyle="round", facecolor="wheat", alpha=0.5),
         )
-        #modifiable/interactive ui elements are in ui_components.py
+        # modifiable/interactive ui elements are in ui_components.py
 
-        
-        
         self.fig, self.ax = fig, ax
 
         return None
-    
+
     def _setup_data(self) -> None:
-        '''define additional attributes'''
+        """define additional attributes"""
         self.ui_components = UIComponents(self.ax)
         self.ui_components.add_observer(self)
 
         # this line makes sure the current axes are the main ones
         plt.sca(self.ax)
 
         self.patch_manager = PatchManager(self.ax)
         self.output_path = "scenebuilder.json"
-        
-        self.timer:Timer|None = None
+
+        self.timer: Timer | None = None
 
         self.drones: list[Drone] = []
         self.buildings: list[Obstacle] = []
         self.current_drone = None
         self.mode = "building"  # 'building', 'drone', or None
         self.actions_stack = ActionsStack()  # New line to track the actions
 
-        self.selected_drone: Drone|None = None
+        self.selected_drone: Drone | None = None
         self.initial_click_position = None
         self.selected_vertex = None
         self.warning = self.ax.annotate(
             "WARNING, No Drones!",
             xy=(0.5, 0.5),
             xycoords="axes fraction",
             fontsize=12,
             fontweight="bold",
             color="red",
             ha="center",
             bbox=dict(boxstyle="round", fc="w", ec="0.5", alpha=1),
-            wrap=True
+            wrap=True,
         )
 
         self.warning.set_visible(False)  # Start with warning hidden
 
         return None
 
     @property
@@ -168,20 +170,29 @@
         self._update()
 
     def _hide_warning(self):
         self.warning.set_visible(False)
         self._update()
 
     def _connect_event_handlers(self) -> None:
-
-        self.fig.canvas.mpl_connect("pick_event", self._on_pick)
-        self.fig.canvas.mpl_connect("button_press_event", self._on_click)
-        self.fig.canvas.mpl_connect("key_press_event", self._on_key_press)
+        # supported values are 'resize_event', 'draw_event', 'key_press_event', 'key_release_event', 'button_press_event', 'button_release_event', 'scroll_event', 'motion_notify_event', 'pick_event', 'figure_enter_event', 'figure_leave_event', 'axes_enter_event', 'axes_leave_event', 'close_event'
+        self.on_pick = self.fig.canvas.mpl_connect("pick_event", self._on_pick)
+        self.on_click = self.fig.canvas.mpl_connect(
+            "button_press_event", self._on_click
+        )
+        self.on_key = self.fig.canvas.mpl_connect("key_press_event", self._on_key_press)
         self.fig.canvas.mpl_connect("button_release_event", self._on_button_release)
         self.fig.canvas.mpl_connect("motion_notify_event", self._on_mouse_move)
+        # self.resize=self.fig.canvas.mpl_connect('resize_event', lambda x:print("tool triggered"))
+        return None
+
+    def _disconnect_event_handlers(self) -> None:
+        self.fig.canvas.mpl_disconnect(self.on_click)
+        self.fig.canvas.mpl_disconnect(self.on_key)
+        self.fig.canvas.mpl_disconnect(self.on_pick)
 
         return None
 
     def _handle_vertex_movement(self, event):
         """Returns True if a click is near a vertex of an obstacle"""
         if not self.buildings:
             return False
@@ -358,15 +369,14 @@
         # polygon = event.artist
         building = self.patch_manager.get_building_from_patch(event.artist)
         self.selected_building = building
 
         self.initial_click_position = [event.mouseevent.xdata, event.mouseevent.ydata]
 
     def _on_mouse_move(self, event):
-
         # check to make sure the mouse is still in the main axes
         # and not over a button or other axes object
         # or outside the axes altogether
         if event.inaxes != self.ax:
             return
 
         point = [event.xdata, event.ydata]
@@ -409,14 +419,15 @@
             self.patch_manager.redraw_building(self.selected_building)
             # Update the initial click position for next movement calculation
             self.initial_click_position = point
 
             # Redraw to show the moved building
             self._update()
 
+
     def _on_button_release(self, event):
         self.initial_click_position = None
         self.selected_drone = None
         self.dragging_drone_point = None
         self.selected_vertex = None
 
     def _delete_selected_building(self):
@@ -444,26 +455,26 @@
 
         elif event.key in ["backspace", "delete"]:
             self._delete_selected_building()
 
         elif event.key == "escape":
             self._clear_temp_elements()
 
-    def _show_warning(self, text:str, duration:float = 3, **kwargs)->None:
-        '''Display the central warning temporarily, set kwargs as per ax.annotate'''
+    def _show_warning(self, text: str, duration: float = 3, **kwargs) -> None:
+        """Display the central warning temporarily, set kwargs as per ax.annotate"""
         self.warning.set_text(text)
         self.warning.set(**kwargs)
         self.warning.set_visible(True)  # Start with warning hidden
         self._update()
         # Set a timer to hide the warning after {duration} seconds
         if self.timer and self.timer.is_alive():
             self.timer.cancel()
         self.timer = Timer(duration, self._hide_warning)
         self.timer.start()
-        
+
     def _update(self):
         # draw the canvas again
         self.fig.canvas.draw()
 
     def _clear_temp_elements(self):
 
         self.patch_manager.remove_temp_drone_start()
@@ -524,81 +535,92 @@
         if building:
             # this if statement checks to see if a building was created
             # ie if the vertex number was >=3
             self.buildings.append(building)
             self.actions_stack.add_action("building", building)
             self._update()
 
-    def _verify_path(self, path:str)->bool:
-        '''Verify if path is a json file (existing or not) in a valid directory
-        and show relevant warnings'''
+    def _verify_path(self, path: str) -> bool:
+        """Verify if path is a json file (existing or not) in a valid directory
+        and show relevant warnings"""
         response = validate_json_path(path)
-        result, info = response['result'], response['info']
-        if result!=0:
-            self._show_warning(info, 3, color='g')
+        result, info = response["result"], response["info"]
+        if result != 0:
+            self._show_warning(info, 3, color="g")
             return True
         else:
-            self._show_warning(info,duration=3,color='r')
-            return False        
+            self._show_warning(info, duration=3, color="r")
+            return False
 
-    def _text_box_submit(self, path:str):
+    def _text_box_submit(self, path: str):
         if self._verify_path(path):
-            #set the new path and overwrite any previous warnings
+            # set the new path and overwrite any previous warnings
             self.set_output_path(path, skip_check=True)
 
-    def _load_json(self, path:str):
-        '''Checks validity of input json, shows relevant warnings and calls load_scene'''
-        #first save the existing plot to temporary file
-        create_json('TEMP.json', self.buildings, self.drones)
+    def _load_json(self, path: str):
+        """Checks validity of input json, shows relevant warnings and calls load_scene"""
         if not self._verify_path(path):
             return
+        # first save the existing plot to temporary file
+        create_json("TEMP.json", self.buildings, self.drones)
         try:
             self.load_scene(path)
-            self._show_warning(f'Loaded {Path(path).resolve().name}', duration=3, color='g')
+            self._show_warning(
+                f"Loaded {Path(path).resolve().name}", duration=3, color="g"
+            )
         except FileNotFoundError as e:
-            self._show_warning(f'Error: {path} does not exist.', 3, color='r')
-            #TODO print full exception
+            self._show_warning(f"Error: {path} does not exist.", 3, color="r")
+            # TODO print full exception
             traceback.print_exc()
-            #load back the temporary file
-            self.load_scene('TEMP.json')
+            # load back the temporary file
+            self.load_scene("TEMP.json")
         except Exception as e:
-            #not ideal but catch and json formatting errors for now
-            self._show_warning(f'JSON Decode Error: {Path(path).resolve().name} format incompatible', 3, color='r')
-            #TODO print full exception
+            # not ideal but catch and json formatting errors for now
+            self._show_warning(
+                f"JSON Decode Error: {Path(path).resolve().name} format incompatible",
+                3,
+                color="r",
+            )
+            # TODO print full exception
             traceback.print_exc()
-            #load back the temporary file
-            self.load_scene('TEMP.json')
-        
-        os.remove('TEMP.json')
-        
-    def _create_json(self, path:str):
+            # load back the temporary file
+            self.load_scene("TEMP.json")
+
+        os.remove("TEMP.json")
+
+    def _create_json(self, path: str):
         if not self.drones:
-            #amber warning for no drones
-            self._show_warning(f"Saving scene to file: {path}\nWARNING, No Drones!", duration=3, color = (1,0.75,0,1))
+            # amber warning for no drones
+            self._show_warning(
+                f"Saving scene to file: {path}\nWARNING, No Drones!",
+                duration=3,
+                color=(1, 0.75, 0, 1),
+            )
         else:
-            #green warning if at least one drone
-            self._show_warning(f'Saving to file: \n{path}', duration=3, color = 'g')
+            # green warning if at least one drone
+            self._show_warning(f"Saving to file: \n{path}", duration=3, color="g")
         create_json(path, self.buildings, self.drones)
 
     def _call(self, event: str, *args, **kwargs):
-        '''class called by observers triggered by button or text_box, see ui_components.py and observer_utils.py'''
+        """class called by observers triggered by button or text_box, see ui_components.py and observer_utils.py"""
         if event == "switch_mode":
             self._switch_mode()
         elif event == "reset":
             self._reset()
         elif event == "create_json":
-            self._create_json(path=self.output_path)
+            path = kwargs.get("input", self.output_path)
+            self.set_output_path(path)
+            self._create_json(path=path)
         elif event == "load_json":
-            path = kwargs["input"]
+            path = kwargs.get("input")
             self._load_json(path)
-        elif event=="text_box_submit":
+        elif event == "text_box_submit":
             path = kwargs["input"]
             self._text_box_submit(path)
 
-
     def _reset(self):
         self.selected_building = None
         self._clear_temp_elements()
         # Remove all building and drone patches
         self.patch_manager.clear_all()
 
         # Empty the buildings and drones lists
@@ -629,7 +651,10 @@
 # Save arena, just buildings, just drones etc
 # better instructions
 # vectors showing output of panel flow for each drone
 # dragging buildings
 # changing drone with click and drag
 # change drone parameters such as source strength, imaginary source strength, goal strength, goal safety etc
 # cooperating or not (can turn on and off for each drone)
+
+
+# for status here:https://stackoverflow.com/questions/70842267/in-matplotlib-how-do-i-catch-that-event-zoom-tool-has-been-selected
```

### Comparing `scenebuilder-0.1.5/PKG-INFO` & `scenebuilder-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenebuilder
-Version: 0.1.5
+Version: 0.2.0
 Summary: A simple GUI to create 2D scenes with obstacles and drone paths for multi-agent path planning algorithms
 Author: Adrian del Ser
 Author-email: adrian.delser@gmail.com
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -30,17 +30,14 @@
 
 ```bash
 pip install scenebuilder
 ```
 
 This command installs SceneBuilder along with numpy and matplotlib, ensuring that everything needed to run the GUI is properly set up.
 
-
-
-
 ## Prerequisites
 
 SceneBuilder's prerequisites are defined in the pyproject.toml file and include Matplotlib and numpy.
 
 ## Quick Start Guide
 
 ### Using Command-Line Options
@@ -53,14 +50,15 @@
 Example usage:
 
 ```bash
 scenebuilder --load path/to/scene.json --output path/to/output.json
 ```
 
 ### In Code
+
 To use SceneBuilder in code, you need to create an instance of the `SceneBuilder` class and invoke the `draw_scene()` method. Below is a simple example to get you started:
 
 ```python
 from scenebuilder import SceneBuilder
 
 # Create an instance of the SceneBuilder
 scene = SceneBuilder()
@@ -79,31 +77,29 @@
 Specify the path to save your output json to:
 
 ```python
 scene.set_output_path("path/to/output.json")
 scene.draw_scene()
 ```
 
-
-
 ## Features
 
 - **Draw Obstacles**: Click within the GUI to place vertices of polygons that represent obstacles. Press Tab to complete an obstacle.
 - **Add new obstacle vertices**: To add new vertices, click somewhere on the polygon's perimeter and drag to move the vertex to its desired location.
 - **Set Drone Paths**: Click once to place the starting point, and again to place the goal of an agent/drone. An arrow will automatically be drawn from start to goal.
 - **Move or adjust existing obstacles/drones**: Obstacles and drones can be moved by clicking and dragging. Drone start and goal points, as well as existing obstacle vertices can be moved in the same way.
 - **Switch between Obstacle and Drone Modes**: Press b to switch to building/obstacle mode. Press d to switch to drone/agent mode. Alternatively click the Switch button on the bottom left of the gui.
 - **Delete obstacles**: Select the obstacle and press delete or backspace. NOTE this is not yet available for drones.
 - **Remove unwanted points**: To remove unwanted points (either obstacle vertices or a drone start point), press escape.
 - **Undo drone/obstacle placement**: To remove the last obstacle or drone, press ctrl+z.
 - **Reset Scene**: To reset the scene to a blank canvas, click the Reset button in the gui.
 
 ## Saving Scenes
 
-Once you have created a scene, you can save it to a JSON file by clicking the 'Create JSON' button in the GUI. This file can then be used as input for path planning algorithms that require predefined scenes with obstacles and paths.
+Once you have created a scene, you can save it to a JSON or GeoJSON file by clicking the 'Save' button in the GUI. You will then be prompted to select whether you want to use our basic JSON format or GeoGSON. This file can then be used as input for path planning algorithms that require predefined scenes with obstacles and paths.
 
 **_Unless otherwise specified, the file is saved as "scenebuilder.json" in the current working directory._**
 
 ## Contributing
 
 Contributions to SceneBuilder are welcome! If you have suggestions for improvements or new features, feel free to create an issue or pull request on our GitHub repository.
```

