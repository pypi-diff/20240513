# Comparing `tmp/trajan-0.6.0.tar.gz` & `tmp/trajan-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajan-0.6.0.tar", max compression
+gzip compressed data, was "trajan-0.6.1.tar", max compression
```

## Comparing `trajan-0.6.0.tar` & `trajan-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    18092 2024-02-13 11:57:28.969118 trajan-0.6.0/LICENSE
--rw-r--r--   0        0        0     1781 2024-02-13 11:57:28.973118 trajan-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8433 2024-02-13 11:57:28.985118 trajan-0.6.0/trajan/__init__.py
--rw-r--r--   0        0        0     1385 2024-02-13 11:57:28.985118 trajan-0.6.0/trajan/animation/__init__.py
--rw-r--r--   0        0        0     6391 2024-02-13 11:57:28.985118 trajan-0.6.0/trajan/plot/__init__.py
--rw-r--r--   0        0        0     2204 2024-02-13 11:57:28.985118 trajan-0.6.0/trajan/plot/land.py
--rw-r--r--   0        0        0       30 2024-02-13 11:57:28.985118 trajan-0.6.0/trajan/readers/__init__.py
--rw-r--r--   0        0        0    18107 2024-02-13 11:57:28.985118 trajan-0.6.0/trajan/readers/omb.py
--rwxr-xr-x   0        0        0    27653 2024-02-13 11:57:28.985118 trajan-0.6.0/trajan/readers/omb_decoder.py
--rw-r--r--   0        0        0     2016 2024-02-13 11:57:28.985118 trajan-0.6.0/trajan/scripts/trajanshow.py
--rw-r--r--   0        0        0     1317 2024-02-13 11:57:28.985118 trajan-0.6.0/trajan/skill/__init__.py
--rw-r--r--   0        0        0    14042 2024-02-13 11:57:28.985118 trajan-0.6.0/trajan/traj.py
--rw-r--r--   0        0        0     8037 2024-02-13 11:57:28.985118 trajan-0.6.0/trajan/traj1d.py
--rw-r--r--   0        0        0     8677 2024-02-13 11:57:28.985118 trajan-0.6.0/trajan/traj2d.py
--rw-r--r--   0        0        0     3435 2024-02-13 11:57:28.985118 trajan-0.6.0/trajan/trajectory_accessor.py
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 trajan-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-05-13 08:31:29.467515 trajan-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1781 2024-05-13 08:31:29.471515 trajan-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     8434 2024-05-13 08:31:29.483515 trajan-0.6.1/trajan/__init__.py
+-rw-r--r--   0        0        0     1385 2024-05-13 08:31:29.483515 trajan-0.6.1/trajan/animation/__init__.py
+-rw-r--r--   0        0        0     8463 2024-05-13 08:31:29.483515 trajan-0.6.1/trajan/plot/__init__.py
+-rw-r--r--   0        0        0     2204 2024-05-13 08:31:29.483515 trajan-0.6.1/trajan/plot/land.py
+-rw-r--r--   0        0        0       30 2024-05-13 08:31:29.483515 trajan-0.6.1/trajan/readers/__init__.py
+-rw-r--r--   0        0        0    18107 2024-05-13 08:31:29.483515 trajan-0.6.1/trajan/readers/omb.py
+-rwxr-xr-x   0        0        0    27653 2024-05-13 08:31:29.483515 trajan-0.6.1/trajan/readers/omb_decoder.py
+-rw-r--r--   0        0        0     2016 2024-05-13 08:31:29.483515 trajan-0.6.1/trajan/scripts/trajanshow.py
+-rw-r--r--   0        0        0     1317 2024-05-13 08:31:29.483515 trajan-0.6.1/trajan/skill/__init__.py
+-rw-r--r--   0        0        0    14764 2024-05-13 08:31:29.483515 trajan-0.6.1/trajan/traj.py
+-rw-r--r--   0        0        0     8196 2024-05-13 08:31:29.483515 trajan-0.6.1/trajan/traj1d.py
+-rw-r--r--   0        0        0     8848 2024-05-13 08:31:29.483515 trajan-0.6.1/trajan/traj2d.py
+-rw-r--r--   0        0        0     3435 2024-05-13 08:31:29.483515 trajan-0.6.1/trajan/trajectory_accessor.py
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 trajan-0.6.1/PKG-INFO
```

### Comparing `trajan-0.6.0/LICENSE` & `trajan-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trajan-0.6.0/pyproject.toml` & `trajan-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trajan"
-version = "0.6.0"
+version = "0.6.1"
 description = "Trajectory analysis package for simulated and observed trajectories"
 authors = ["Gaute Hope <gauteh@met.no>", "Knut-Frode Dagestad <knutfd@met.no>"]
 license = "GPLv2"
 
 [tool.poetry.scripts]
 trajanshow = "trajan.scripts.trajanshow:main"
```

### Comparing `trajan-0.6.0/trajan/__init__.py` & `trajan-0.6.1/trajan/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,7 +233,8 @@
                         str(np.nanmin(datavars['time'][1])),
                         'time_coverage_end':
                         str(np.nanmax(datavars['time'][1])),
                         **global_attributes
                     })
 
     return ds
+
```

### Comparing `trajan-0.6.0/trajan/animation/__init__.py` & `trajan-0.6.1/trajan/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `trajan-0.6.0/trajan/plot/__init__.py` & `trajan-0.6.1/trajan/plot/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -193,7 +193,82 @@
         else:
             if self.__cartesian__:
                 paths = ax.plot(x, y, *args, **kwargs)
             else:
                 paths = ax.plot(x, y, transform=self.gcrs, *args, **kwargs)
 
         return paths
+
+    def scatter(self, *args, **kwargs):
+        """
+        Plot the particles as points.
+
+        Args:
+
+            ax: Use existing axes, otherwise a new one is set up.
+
+            crs: Specify crs for new axis.
+
+        Returns:
+
+            Matplotlib lines, and axes.
+        """
+
+        logger.debug(f'Plotting points')
+        ax = self.set_up_map(kwargs)
+
+        if 'marker' not in kwargs:
+            kwargs['marker'] = '.'
+
+        if 'color' not in kwargs:
+            kwargs['color'] = self.DEFAULT_LINE_COLOR
+
+        if 'alpha' not in kwargs and 'trajectory' in self.ds.dims:
+            num = self.ds.sizes['trajectory']
+            if num>100:  # If many particles, make more transparent
+                kwargs['alpha'] = np.maximum(.1, 100/np.float64(num))
+
+        if self.__cartesian__:
+            x = self.ds.traj.tx.values.T
+            y = self.ds.traj.ty.values.T
+        else:
+            x = self.ds.traj.tlon.values.T
+            y = self.ds.traj.tlat.values.T
+
+        if self.__cartesian__:
+            paths = ax.scatter(x, y, *args, **kwargs)
+        else:
+            paths = ax.scatter(x, y, transform=self.gcrs, *args, **kwargs)
+
+        return paths
+
+    def convex_hull(self, *args, **kwargs):
+        """
+        Plot the convex hull around all particles
+
+        Args:
+
+            ax: Use existing axes, otherwise a new one is set up.
+
+            crs: Specify crs for new axis.
+
+        Returns:
+
+            Matplotlib lines, and axes.
+        """
+
+        logger.debug(f'Plotting convex hull')
+        hull = self.ds.traj.convex_hull()
+
+        ax = self.set_up_map(kwargs)
+
+        if 'color' not in kwargs:
+            kwargs['color'] = self.DEFAULT_LINE_COLOR
+
+        # TODO: might not work for cartesian plots
+        line_segments = [hull.points[simplex] for simplex in hull.simplices]
+        from matplotlib.collections import LineCollection
+        paths = ax.add_collection(LineCollection(line_segments, transform=self.gcrs,
+                                                 *args, **kwargs))
+
+        return paths
+
```

### Comparing `trajan-0.6.0/trajan/plot/land.py` & `trajan-0.6.1/trajan/plot/land.py`

 * *Files identical despite different names*

### Comparing `trajan-0.6.0/trajan/readers/omb.py` & `trajan-0.6.1/trajan/readers/omb.py`

 * *Files identical despite different names*

### Comparing `trajan-0.6.0/trajan/readers/omb_decoder.py` & `trajan-0.6.1/trajan/readers/omb_decoder.py`

 * *Files identical despite different names*

### Comparing `trajan-0.6.0/trajan/scripts/trajanshow.py` & `trajan-0.6.1/trajan/scripts/trajanshow.py`

 * *Files identical despite different names*

### Comparing `trajan-0.6.0/trajan/skill/__init__.py` & `trajan-0.6.1/trajan/skill/__init__.py`

 * *Files identical despite different names*

### Comparing `trajan-0.6.0/trajan/traj.py` & `trajan-0.6.1/trajan/traj.py`

 * *Files 8% similar despite different names*

```diff
@@ -382,46 +382,66 @@
         azimuth = self.azimuth_to_next()
 
         u = speed * np.cos(azimuth)
         v = speed * np.sin(azimuth)
 
         return u, v
 
-    def get_area_convex_hull(self):
-        """Returns the area of the convex hull spanned by all particles, per timestep"""
+    def convex_hull(self):
+        """Returns the scipy convex hull for all particles, in geographical coordinates"""
 
         from scipy.spatial import ConvexHull
-        from pyproj import Geod
 
-        area = []
-        lons = self.ds.lon.where(self.ds.status == 0)
-        lats = self.ds.lat.where(self.ds.status == 0)
-        for i in range(self.ds.dims['time']):
-            lat = lats.isel(time=i)
-            lon = lons.isel(time=i)
-            fin = np.isfinite(lat + lon)
-            if np.sum(fin) <= 3:
-                area.append(0)
-                continue
-            if len(np.unique(lat)) == 1 and len(np.unique(lon)) == 1:
-                area.append(0)
-                continue
-            lat = lat[fin]
-            lon = lon[fin]
-            aea = pyproj.Proj(
-                f'+proj=aea +lat_0={lat.mean().values} +lat_1={lat.min().values} +lat_2={lat.max().values} +lon_0={lon.mean().values} +x_0=0 +y_0=0 +datum=NAD83 +units=m +no_defs'
-            )
-
-            x, y = aea(lat, lon, inverse=False)
-            fin = np.isfinite(x + y)
-            points = np.vstack((y.T, x.T)).T
-            hull = ConvexHull(points)
-            area.append(hull.volume)  # volume=area for 2D as here
+        lon = self.ds.lon.where(self.ds.status == 0)
+        lat = self.ds.lat.where(self.ds.status == 0)
+        fin = np.isfinite(lat + lon)
+        if np.sum(fin) <= 3:
+            return None
+        if len(np.unique(lat)) == 1 and len(np.unique(lon)) == 1:
+            return None
+        lat = lat[fin]
+        lon = lon[fin]
+        points = np.vstack((lon.T, lat.T)).T
+        return ConvexHull(points)
+
+    def convex_hull_contains_point(self, lon, lat):
+        """Returns True if given point is within the scipy convex hull for all particles"""
+        from matplotlib.patches import Polygon
+
+        hull = self.ds.traj.convex_hull()
+        if hull is None:
+            return False
+        p = Polygon(hull.points[hull.vertices])
+        point = np.c_[lon, lat]
+        return p.contains_points(point)[0]
+
+    def get_area_convex_hull(self):
+        """Returns the area [m2] of the convex hull spanned by all particles"""
+
+        from scipy.spatial import ConvexHull
 
-        return np.array(area)
+        lon = self.ds.lon.where(self.ds.status == 0)
+        lat = self.ds.lat.where(self.ds.status == 0)
+        fin = np.isfinite(lat + lon)
+        if np.sum(fin) <= 3:
+            return 0
+        if len(np.unique(lat)) == 1 and len(np.unique(lon)) == 1:
+            return 0
+        lat = lat[fin]
+        lon = lon[fin]
+        # An equal area projection centered around the particles
+        aea = pyproj.Proj(
+            f'+proj=aea +lat_0={lat.mean().values} +lat_1={lat.min().values} +lat_2={lat.max().values} +lon_0={lon.mean().values} +x_0=0 +y_0=0 +datum=NAD83 +units=m +no_defs'
+        )
+
+        x, y = aea(lat, lon, inverse=False)
+        fin = np.isfinite(x + y)
+        points = np.vstack((y.T, x.T)).T
+        hull = ConvexHull(points)
+        return np.array(hull.volume)  # volume=area for 2D as here
 
     @abstractmethod
     def gridtime(self, times, timedim = None):
         """Interpolate dataset to a regular time interval or a different grid.
 
         Args:
```

### Comparing `trajan-0.6.0/trajan/traj1d.py` & `trajan-0.6.1/trajan/traj1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         return xr.DataArray(s,
                             name='Skill-score',
                             coords={'trajectory': self.ds.trajectory},
                             attrs={'method': method})
 
     @__require_obsdim__
     def gridtime(self, times, timedim=None, round=True):
-        if isinstance(times, str):  # Make time series with given interval
+        if isinstance(times, str) or isinstance(times, pd.Timedelta):  # Make time series with given interval
             if round is True:
                 start_time = np.nanmin(np.asarray(self.ds.time.dt.floor(times)))
                 end_time = np.nanmax(np.asarray(self.ds.time.dt.ceil(times)))
             else:
                 start_time = np.nanmin(np.asarray(self.ds.time))
                 end_time = np.nanmax(np.asarray(self.ds.time))
             times = pd.date_range(start_time,
@@ -235,13 +235,17 @@
         _, ui = np.unique(ds[timedim], return_index=True)
 
         if len(ui) != len(self.ds[timedim]):
             logger.warning('non-unique time points, dropping time-duplicates')
 
         ds = ds.isel({timedim : ui})
         ds = ds.isel({timedim : np.where(~pd.isna(ds[timedim].values))[0]})
-        ds = ds.interp({timedim: times})
+
+        if ds.sizes[timedim] > 0:
+            ds = ds.interp({timedim: times})
+        else:
+            logger.warning(f"time dimension ({timedim}) is zero size")
 
         if not 'trajectory' in ds.dims:
             ds = ds.expand_dims('trajectory')
 
         return ds
```

### Comparing `trajan-0.6.0/trajan/traj2d.py` & `trajan-0.6.1/trajan/traj2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         obs = np.arange(0, maxN)
         ds = ds.assign_coords({self.obsdim: obs})
 
         return ds
 
     @__require_obsdim__
     def gridtime(self, times, timedim=None, round=True):
-        if isinstance(times, str):  # Make time series with given interval
+        if isinstance(times, str) or isinstance(times, pd.Timedelta):  # Make time series with given interval
             if round is True:
                 start_time = np.nanmin(np.asarray(self.ds.time.dt.floor(times)))
                 end_time = np.nanmax(np.asarray(self.ds.time.dt.ceil(times)))
             else:
                 start_time = np.nanmin(np.asarray(self.ds.time))
                 end_time = np.nanmax(np.asarray(self.ds.time))
             times = pd.date_range(start_time,
@@ -226,15 +226,19 @@
                    .drop_vars(self.timedim) \
                    .rename({self.obsdim : timedim}) \
                    .set_index({timedim: timedim})
 
             _, ui = np.unique(dt[timedim], return_index=True)
             dt = dt.isel({timedim: ui})
             dt = dt.isel({timedim : np.where(~pd.isna(dt[timedim].values))[0]})
-            dt = dt.interp({timedim: times})
+
+            if dt.sizes[timedim] > 0:
+                dt = dt.interp({timedim: times})
+            else:
+                logger.warning(f"time dimension ({timedim}) is zero size")
 
             if d is None:
                 d = dt.expand_dims('trajectory')
             else:
                 d = xr.concat((d, dt), "trajectory")
 
         d = d.assign_coords({'trajectory': self.ds['trajectory']})
```

### Comparing `trajan-0.6.0/trajan/trajectory_accessor.py` & `trajan-0.6.1/trajan/trajectory_accessor.py`

 * *Files identical despite different names*

### Comparing `trajan-0.6.0/PKG-INFO` & `trajan-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajan
-Version: 0.6.0
+Version: 0.6.1
 Summary: Trajectory analysis package for simulated and observed trajectories
 License: GPLv2
 Author: Gaute Hope
 Author-email: gauteh@met.no
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

