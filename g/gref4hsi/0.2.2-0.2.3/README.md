# Comparing `tmp/gref4hsi-0.2.2.tar.gz` & `tmp/gref4hsi-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gref4hsi-0.2.2.tar", last modified: Mon May 13 06:58:08 2024, max compression
+gzip compressed data, was "gref4hsi-0.2.3.tar", last modified: Mon May 13 08:02:25 2024, max compression
```

## Comparing `gref4hsi-0.2.2.tar` & `gref4hsi-0.2.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 06:58:08.757146 gref4hsi-0.2.2/
--rw-rw-rw-   0        0        0    14098 2024-03-04 11:54:34.000000 gref4hsi-0.2.2/LICENCE.MD
--rw-rw-rw-   0        0        0       82 2024-03-06 12:25:35.000000 gref4hsi-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0    20439 2024-05-13 06:58:08.756146 gref4hsi-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    18380 2024-04-15 13:37:53.000000 gref4hsi-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 06:58:08.728146 gref4hsi-0.2.2/gref4hsi/
--rw-rw-rw-   0        0        0      213 2024-02-16 10:12:17.000000 gref4hsi-0.2.2/gref4hsi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:58:08.738146 gref4hsi-0.2.2/gref4hsi/scripts/
--rw-rw-rw-   0        0        0        0 2023-11-01 06:48:25.000000 gref4hsi-0.2.2/gref4hsi/scripts/__init__.py
--rw-rw-rw-   0        0        0    69548 2024-05-07 16:41:37.000000 gref4hsi-0.2.2/gref4hsi/scripts/coregistration.py
--rw-rw-rw-   0        0        0    11589 2024-05-03 06:39:17.000000 gref4hsi-0.2.2/gref4hsi/scripts/georeference.py
--rw-rw-rw-   0        0        0    11972 2024-04-24 07:00:32.000000 gref4hsi-0.2.2/gref4hsi/scripts/georeference.py.orig
--rw-rw-rw-   0        0        0     9719 2024-05-02 08:38:08.000000 gref4hsi-0.2.2/gref4hsi/scripts/orthorectification.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:58:08.744147 gref4hsi-0.2.2/gref4hsi/tests/
--rw-rw-rw-   0        0        0        0 2023-11-08 14:43:38.000000 gref4hsi-0.2.2/gref4hsi/tests/__init__.py
--rw-rw-rw-   0        0        0    15091 2024-05-04 04:58:01.000000 gref4hsi-0.2.2/gref4hsi/tests/specim_process.py
--rw-rw-rw-   0        0        0    14929 2024-04-23 10:50:45.000000 gref4hsi-0.2.2/gref4hsi/tests/specim_process.py.orig
--rw-rw-rw-   0        0        0     1669 2024-04-15 13:37:53.000000 gref4hsi-0.2.2/gref4hsi/tests/test_main_hi.py
--rw-rw-rw-   0        0        0     8441 2024-04-23 10:50:45.000000 gref4hsi-0.2.2/gref4hsi/tests/test_main_uhi.py
--rw-rw-rw-   0        0        0     3108 2023-11-01 06:48:25.000000 gref4hsi-0.2.2/gref4hsi/tests/test_multi_ray_trace.py
--rw-rw-rw-   0        0        0     3812 2024-03-12 08:07:09.000000 gref4hsi-0.2.2/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:58:08.754146 gref4hsi-0.2.2/gref4hsi/utils/
--rw-rw-rw-   0        0        0        0 2024-02-15 08:51:42.000000 gref4hsi-0.2.2/gref4hsi/utils/__init__.py
--rw-rw-rw-   0        0        0     2147 2024-04-30 18:24:21.000000 gref4hsi-0.2.2/gref4hsi/utils/colours.py
--rw-rw-rw-   0        0        0     3228 2024-03-17 07:44:28.000000 gref4hsi-0.2.2/gref4hsi/utils/config_utils.py
--rw-rw-rw-   0        0        0    55635 2024-05-03 07:59:57.000000 gref4hsi-0.2.2/gref4hsi/utils/geometry_utils.py
--rw-rw-rw-   0        0        0    49663 2024-05-03 08:37:15.000000 gref4hsi-0.2.2/gref4hsi/utils/gis_tools.py
--rw-rw-rw-   0        0        0    23336 2024-04-23 10:50:45.000000 gref4hsi-0.2.2/gref4hsi/utils/parsing_utils.py
--rw-rw-rw-   0        0        0     8963 2024-03-17 07:44:28.000000 gref4hsi-0.2.2/gref4hsi/utils/photogrammetry_utils.py
--rw-rw-rw-   0        0        0    24256 2024-03-17 07:44:28.000000 gref4hsi-0.2.2/gref4hsi/utils/radiometry.py
--rw-rw-rw-   0        0        0    26314 2024-04-25 19:08:38.000000 gref4hsi-0.2.2/gref4hsi/utils/specim_parsing_utils.py
--rw-rw-rw-   0        0        0    33987 2024-04-23 10:50:45.000000 gref4hsi-0.2.2/gref4hsi/utils/uhi_parsing_utils.py
--rw-rw-rw-   0        0        0    10142 2024-04-23 10:50:45.000000 gref4hsi-0.2.2/gref4hsi/utils/visualize.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:58:08.755146 gref4hsi-0.2.2/gref4hsi.egg-info/
--rw-rw-rw-   0        0        0    20439 2024-05-13 06:58:08.000000 gref4hsi-0.2.2/gref4hsi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1009 2024-05-13 06:58:08.000000 gref4hsi-0.2.2/gref4hsi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 06:58:08.000000 gref4hsi-0.2.2/gref4hsi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2024-05-13 06:58:08.000000 gref4hsi-0.2.2/gref4hsi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-13 06:58:08.000000 gref4hsi-0.2.2/gref4hsi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2024-03-05 11:15:42.000000 gref4hsi-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 06:58:08.757146 gref4hsi-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1621 2024-05-13 06:57:32.000000 gref4hsi-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:02:25.423060 gref4hsi-0.2.3/
+-rw-rw-rw-   0        0        0    14098 2024-03-04 11:54:34.000000 gref4hsi-0.2.3/LICENCE.MD
+-rw-rw-rw-   0        0        0       82 2024-03-06 12:25:35.000000 gref4hsi-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    20439 2024-05-13 08:02:25.422086 gref4hsi-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    18380 2024-04-15 13:37:53.000000 gref4hsi-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 08:02:25.394061 gref4hsi-0.2.3/gref4hsi/
+-rw-rw-rw-   0        0        0      213 2024-02-16 10:12:17.000000 gref4hsi-0.2.3/gref4hsi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:02:25.403059 gref4hsi-0.2.3/gref4hsi/scripts/
+-rw-rw-rw-   0        0        0        0 2023-11-01 06:48:25.000000 gref4hsi-0.2.3/gref4hsi/scripts/__init__.py
+-rw-rw-rw-   0        0        0    66838 2024-05-13 08:01:08.000000 gref4hsi-0.2.3/gref4hsi/scripts/coregistration.py
+-rw-rw-rw-   0        0        0    11589 2024-05-13 07:03:06.000000 gref4hsi-0.2.3/gref4hsi/scripts/georeference.py
+-rw-rw-rw-   0        0        0    11977 2024-05-13 07:03:06.000000 gref4hsi-0.2.3/gref4hsi/scripts/georeference.py.orig
+-rw-rw-rw-   0        0        0     9719 2024-05-13 07:03:06.000000 gref4hsi-0.2.3/gref4hsi/scripts/orthorectification.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:02:25.409079 gref4hsi-0.2.3/gref4hsi/tests/
+-rw-rw-rw-   0        0        0        0 2023-11-08 14:43:38.000000 gref4hsi-0.2.3/gref4hsi/tests/__init__.py
+-rw-rw-rw-   0        0        0    15091 2024-05-13 07:03:06.000000 gref4hsi-0.2.3/gref4hsi/tests/specim_process.py
+-rw-rw-rw-   0        0        0    14929 2024-05-13 07:03:06.000000 gref4hsi-0.2.3/gref4hsi/tests/specim_process.py.orig
+-rw-rw-rw-   0        0        0     1669 2024-04-15 13:37:53.000000 gref4hsi-0.2.3/gref4hsi/tests/test_main_hi.py
+-rw-rw-rw-   0        0        0     8441 2024-05-13 07:03:06.000000 gref4hsi-0.2.3/gref4hsi/tests/test_main_uhi.py
+-rw-rw-rw-   0        0        0     3108 2023-11-01 06:48:25.000000 gref4hsi-0.2.3/gref4hsi/tests/test_multi_ray_trace.py
+-rw-rw-rw-   0        0        0     3812 2024-03-12 08:07:09.000000 gref4hsi-0.2.3/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:02:25.420061 gref4hsi-0.2.3/gref4hsi/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-15 08:51:42.000000 gref4hsi-0.2.3/gref4hsi/utils/__init__.py
+-rw-rw-rw-   0        0        0     2147 2024-05-13 07:03:06.000000 gref4hsi-0.2.3/gref4hsi/utils/colours.py
+-rw-rw-rw-   0        0        0     3228 2024-03-17 07:44:28.000000 gref4hsi-0.2.3/gref4hsi/utils/config_utils.py
+-rw-rw-rw-   0        0        0    55635 2024-05-13 07:03:06.000000 gref4hsi-0.2.3/gref4hsi/utils/geometry_utils.py
+-rw-rw-rw-   0        0        0    49663 2024-05-13 07:03:06.000000 gref4hsi-0.2.3/gref4hsi/utils/gis_tools.py
+-rw-rw-rw-   0        0        0    23336 2024-05-13 07:02:55.000000 gref4hsi-0.2.3/gref4hsi/utils/parsing_utils.py
+-rw-rw-rw-   0        0        0     8963 2024-03-17 07:44:28.000000 gref4hsi-0.2.3/gref4hsi/utils/photogrammetry_utils.py
+-rw-rw-rw-   0        0        0    24256 2024-03-17 07:44:28.000000 gref4hsi-0.2.3/gref4hsi/utils/radiometry.py
+-rw-rw-rw-   0        0        0    26314 2024-05-13 07:03:06.000000 gref4hsi-0.2.3/gref4hsi/utils/specim_parsing_utils.py
+-rw-rw-rw-   0        0        0    33987 2024-04-23 10:50:45.000000 gref4hsi-0.2.3/gref4hsi/utils/uhi_parsing_utils.py
+-rw-rw-rw-   0        0        0    10142 2024-04-23 10:50:45.000000 gref4hsi-0.2.3/gref4hsi/utils/visualize.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:02:25.421059 gref4hsi-0.2.3/gref4hsi.egg-info/
+-rw-rw-rw-   0        0        0    20439 2024-05-13 08:02:25.000000 gref4hsi-0.2.3/gref4hsi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1009 2024-05-13 08:02:25.000000 gref4hsi-0.2.3/gref4hsi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 08:02:25.000000 gref4hsi-0.2.3/gref4hsi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2024-05-13 08:02:25.000000 gref4hsi-0.2.3/gref4hsi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 08:02:25.000000 gref4hsi-0.2.3/gref4hsi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2024-03-05 11:15:42.000000 gref4hsi-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 08:02:25.423060 gref4hsi-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1621 2024-05-13 08:01:56.000000 gref4hsi-0.2.3/setup.py
```

### Comparing `gref4hsi-0.2.2/LICENCE.MD` & `gref4hsi-0.2.3/LICENCE.MD`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/PKG-INFO` & `gref4hsi-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gref4hsi
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for for georeferencing and orthorectifying hyperspectral imagery
 Home-page: https://github.com/havardlovas/gref4hsi
 Author: Haavard Snefjellaa Loevaas
 Author-email: havard.s.lovas@ntnu.no
 License: EUPL-1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gref4hsi-0.2.2/README.md` & `gref4hsi-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/scripts/coregistration.py` & `gref4hsi-0.2.3/gref4hsi/scripts/coregistration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1406,31 +1406,14 @@
 
                         x_err = fun_rp[0:n_features]
                         x_MAE = np.median(np.abs(x_err))
 
                         y_err = fun_rp[n_features:2*n_features]
                         y_MAE = np.median(np.abs(y_err))
 
-                        # Plot the residual time series:
-                        t_start = time_scanlines.min()
-                        t_end = time_scanlines.max()
-                        plt.scatter(time_arr_sorted_features-t_start, x_err, label='x-errors')
-                        plt.scatter(time_arr_sorted_features-t_start, y_err, label='y-errors')
-                        plt.ylim([-15, 15])
-                        plt.xlim([0, t_end-t_start])
-                        plt.ylim([-15, 15])
-                        plt.title(f'No nodes, {x_MAE:.2f}/{y_MAE:.2f} pixels MAE x/y')
-                        plt.xlabel('Time [s]')
-                        plt.ylabel('Reprojection error [pixel]')
-                        plt.legend()
-
-                        fname_plot = f'reprojection_error_{transect_nr}_nonodes.png'
-                        plt.savefig(os.path.join('C:/Users/haavasl/OneDrive - NTNU/GeoHab/Figures', fname_plot))  # Adjust filename as needed
-                        plt.close()
-
                         is_first_iter = False
 
                 # Optimize the transect and record time duration
                 time_start  = time.time()
 
                 if val_mode:
                     # Prepare validation data
@@ -1463,33 +1446,14 @@
                 # Compute the median absolute error (more informative in outlier precence)
                 x_err = res.fun[0:n_train]
                 x_MAE = np.median(np.abs(x_err))
 
                 y_err = res.fun[n_train:2*n_train]
                 y_MAE = np.median(np.abs(y_err))
 
-                # Plot the residual time series:
-                t_start = time_scanlines.min()
-                t_end = time_scanlines.max()
-
-                plt.scatter(time_arr_sorted_features[sorted(idx_train)]-t_start, x_err, label='x-errors')
-                plt.scatter(time_arr_sorted_features[sorted(idx_train)]-t_start, y_err, label='y-errors')
-                plt.ylim([-15, 15])
-                plt.xlim([0, t_end-t_start])
-                plt.title(f'{time_node_spacing:.0f} sec node spacing, {number_of_nodes:.0f} nodes, {x_MAE:.2f}/{y_MAE:.2f} pixels MAE x/y')
-                plt.xlabel('Time [s]')
-                plt.ylabel('Reprojection error [pixel]')
-                plt.legend()
-
-                fname_plot = f'reprojection_error_{transect_nr}_{time_node_spacing}_{number_of_nodes}.png'
-                plt.savefig(os.path.join('C:/Users/haavasl/OneDrive - NTNU/GeoHab/Figures', fname_plot))  # Adjust filename as needed
-                plt.close()
-
-                #plt.show()
-
                 ## Run the validation
                 if val_mode:
                     kwargs['features_df'] = df_current.iloc[sorted(idx_val)]
 
 
                 res_pre_optim = objective_fun_reprojection_error(res.x, **kwargs)
 
@@ -1513,35 +1477,28 @@
 
                 if plot_node_spacing:
                     MAE_median_list.append(MAE_median)
                     rmse_list.append(rmse_val)
                     MAE_mean_list.append(MAE_mean)
                     node_number_list.append(number_of_nodes)
                     node_spacing_list.append(time_node_spacing)
-                    """plt.scatter(number_of_nodes, rmse, c='r')
-                    plt.scatter(number_of_nodes, MAE_mean, c='g')
-                    plt.scatter(number_of_nodes, MAE_median, c='b')"""
                 
                 # Now, if all features were used to optimize, use gaussian interpolation (KRIGING actually)
                 if node_partition == 'all_features':
                     kwargs['time_interpolation_method'] = 'gaussian'
                 
                 param_optimized = res.x # Error curves
 
                 camera_model_dict_updated, position_updated, quaternion_updated = calculate_cam_and_pose_from_param(h5_filename, 
                                                                                                                     param_optimized, 
                                                                                                                     **kwargs, 
                                                                                                                     h5_paths=h5_paths, 
                                                                                                                     plot_err_vec=plot_err_vec_time, 
                                                                                                                     sigma_nodes = None)
 
-                fname_plot = f'error_series_{transect_nr}_{time_node_spacing}_{number_of_nodes}.png'
-                plt.savefig(os.path.join('C:/Users/haavasl/OneDrive - NTNU/GeoHab/Figures', fname_plot))  # Adjust filename as needed
-                plt.close()
-
                 # Now the data has been computed and can be written to h5:
                 if not is_calibrated:
                     if position_updated is None:
                         pass
                     else:
                         Hyperspectral.add_dataset(data=position_updated, 
                                                 name = h5_folder_position_ecef_coreg,
@@ -1567,17 +1524,14 @@
                 plt.plot(np.array(node_number_list), np.array(MAE_mean_list), label = 'MAE (mean)')
                 plt.plot(np.array(node_number_list), np.array(MAE_median_list), label = 'MAE (median)')
                 plt.xlabel('Number of nodes')
                 plt.ylabel('Error [pixels]')
                 plt.ylim(bottom=0)
                 plt.legend()
                 plt.title('')
-                fname_plot = f'rmse_node_spacing_{transect_nr}.png'
-                plt.savefig(os.path.join('C:/Users/haavasl/OneDrive - NTNU/GeoHab/Figures', fname_plot))
-                plt.close()
                 #plt.show()
 
         else:
             
             n_features = df_gcp_filtered.shape[0]
 
             res_pre_optim = objective_fun_reprojection_error(param0_variab, df_gcp_filtered, param0, is_variab_param_intr)
```

### Comparing `gref4hsi-0.2.2/gref4hsi/scripts/georeference.py` & `gref4hsi-0.2.3/gref4hsi/scripts/georeference.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/scripts/georeference.py.orig` & `gref4hsi-0.2.3/gref4hsi/scripts/georeference.py.orig`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def cal_file_to_rays(filename_cal):
         # See paper by Sun, Bo, et al. "Calibration of line-scan cameras for precision measurement." Applied optics 55.25 (2016): 6836-6843.
         # Loads line camera parameters for the hyperspectral imager from an xml file.
 
         # Certain imagers deliver geometry "per pixel". This can be resolved by fitting model parameters.
         calHSI = CalibHSI(file_name_cal_xml=filename_cal)
         f = calHSI.f
-        cx = calHSI.cx
+        u_c = calHSI.cx
 
         # Radial distortion parameters
         k1 = calHSI.k1
         k2 = calHSI.k2
 
         # Tangential distortion parameters
         k3 = calHSI.k3
@@ -45,19 +45,19 @@
         # Number of pixels
         n_pix = calHSI.w
 
         # Define camera model array.
         u = np.arange(1, n_pix + 1)
 
         # Express uhi ray directions in uhi frame using line-camera model
-        x_norm_lin = (u - cx) / f
+        x_norm_lin = (u - u_c) / f
 
-        x_norm_nonlin = -(k1 * ((u - cx) / 1000) ** 5 + \
-                          k2 * ((u - cx) / 1000) ** 3 + \
-                          k3 * ((u - cx) / 1000) ** 2) / f
+        x_norm_nonlin = -(k1 * ((u - u_c) / 1000) ** 5 + \
+                          k2 * ((u - u_c) / 1000) ** 3 + \
+                          k3 * ((u - u_c) / 1000) ** 2) / f
 
         x_norm = x_norm_lin + x_norm_nonlin
 
         p_dir = np.zeros((len(x_norm), 3))
 
         # Rays are defined in the HI frame with positive z down
         p_dir[:, 0] = x_norm
```

### Comparing `gref4hsi-0.2.2/gref4hsi/scripts/orthorectification.py` & `gref4hsi-0.2.3/gref4hsi/scripts/orthorectification.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/tests/specim_process.py` & `gref4hsi-0.2.3/gref4hsi/tests/specim_process.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/tests/specim_process.py.orig` & `gref4hsi-0.2.3/gref4hsi/tests/specim_process.py.orig`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/tests/test_main_hi.py` & `gref4hsi-0.2.3/gref4hsi/tests/test_main_hi.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/tests/test_main_uhi.py` & `gref4hsi-0.2.3/gref4hsi/tests/test_main_uhi.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/tests/test_multi_ray_trace.py` & `gref4hsi-0.2.3/gref4hsi/tests/test_multi_ray_trace.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py` & `gref4hsi-0.2.3/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/utils/colours.py` & `gref4hsi-0.2.3/gref4hsi/utils/colours.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/utils/config_utils.py` & `gref4hsi-0.2.3/gref4hsi/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/utils/geometry_utils.py` & `gref4hsi-0.2.3/gref4hsi/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/utils/gis_tools.py` & `gref4hsi-0.2.3/gref4hsi/utils/gis_tools.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/utils/parsing_utils.py` & `gref4hsi-0.2.3/gref4hsi/utils/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/utils/photogrammetry_utils.py` & `gref4hsi-0.2.3/gref4hsi/utils/photogrammetry_utils.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/utils/radiometry.py` & `gref4hsi-0.2.3/gref4hsi/utils/radiometry.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/utils/specim_parsing_utils.py` & `gref4hsi-0.2.3/gref4hsi/utils/specim_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/utils/uhi_parsing_utils.py` & `gref4hsi-0.2.3/gref4hsi/utils/uhi_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi/utils/visualize.py` & `gref4hsi-0.2.3/gref4hsi/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/gref4hsi.egg-info/PKG-INFO` & `gref4hsi-0.2.3/gref4hsi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gref4hsi
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for for georeferencing and orthorectifying hyperspectral imagery
 Home-page: https://github.com/havardlovas/gref4hsi
 Author: Haavard Snefjellaa Loevaas
 Author-email: havard.s.lovas@ntnu.no
 License: EUPL-1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gref4hsi-0.2.2/gref4hsi.egg-info/SOURCES.txt` & `gref4hsi-0.2.3/gref4hsi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.2.2/setup.py` & `gref4hsi-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 import setuptools
 
 setuptools.setup(
     name='gref4hsi',
-    version='0.2.2',    
+    version='0.2.3',    
     description='A Python package for for georeferencing and orthorectifying hyperspectral imagery',
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type = "text/markdown",
     url='https://github.com/havardlovas/gref4hsi',
     author='Haavard Snefjellaa Loevaas',
     author_email='havard.s.lovas@ntnu.no',
     license='EUPL-1.2',
```

