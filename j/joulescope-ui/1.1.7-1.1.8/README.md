# Comparing `tmp/joulescope_ui-1.1.7.tar.gz` & `tmp/joulescope_ui-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joulescope_ui-1.1.7.tar", last modified: Sat May 11 14:14:23 2024, max compression
+gzip compressed data, was "joulescope_ui-1.1.8.tar", last modified: Mon May 13 15:39:21 2024, max compression
```

## Comparing `joulescope_ui-1.1.7.tar` & `joulescope_ui-1.1.8.tar`

### file list

```diff
@@ -1,475 +1,475 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.450034 joulescope_ui-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    53673 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/CREDITS.html
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-11 14:14:23.450034 joulescope_ui-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-11 14:14:21.000000 joulescope_ui-1.1.7/joulescope.iss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.390035 joulescope_ui-1.1.7/joulescope_ui/
--rw-r--r--   0 runner    (1001) docker     (127)    53673 2024-05-11 14:14:11.000000 joulescope_ui-1.1.7/joulescope_ui/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-11 14:14:11.000000 joulescope_ui-1.1.7/joulescope_ui/CREDITS.html
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/dev_signal_buffer_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/device_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    24052 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js110.py
--rw-r--r--   0 runner    (1001) docker     (127)    31966 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js220.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js220_fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js220_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)    17812 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/devices/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/test/test_device_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/disk_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/entry_points/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/entry_points/zip_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/error_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    14307 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/error_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/expanding_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/file_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/filename_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/fonts/DSEG14-Modern/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/fonts/Hack/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/fonts/Hack/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/fonts/Lato/
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/fonts/Lato/OFL.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/fonts/SourceCodePro/
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/fonts/SourceCodePro/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/fonts/SourceSerifPro/
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/fonts/SourceSerifPro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)  3102116 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui/fonts.rcc
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/getting_started.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/help_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/intel_graphics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/jls_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/jls_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/jls_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/jls_v2_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/json_plus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/locale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    81702 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   112244 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    71550 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   102499 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    99351 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   130324 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    71667 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   102570 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    73100 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   104062 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    72339 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   103281 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    75547 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   105590 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po
--rw-r--r--   0 runner    (1001) docker     (127)    68383 2024-05-11 14:14:12.000000 joulescope_ui-1.1.7/joulescope_ui/locale/joulescope_ui.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    70320 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   100452 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    61353 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)    91276 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    42189 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/mem_leak_debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/plugins/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p1/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p1/index.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p2/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p2/index.json
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/process_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    66497 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/pubsub_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/pubsub_callable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/pubsub_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.406035 joulescope_ui-1.1.7/joulescope_ui/range_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/cdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/max_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/plugin_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/usb_inrush.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.406035 joulescope_ui-1.1.7/joulescope_ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/dmg_background.png
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/dmg_background.svg
--rw-r--r--   0 runner    (1001) docker     (127)    48138 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/dmg_background@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)   100365 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.406035 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/
--rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_128x128.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_128x128@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_16x16.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_16x16@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_256x256.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_256x256@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_32x32.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_32x32@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_512x512.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     7537 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_512x512@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_64x64.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_64x64@2.png
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/logo-large.png
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/zoom.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-05-11 14:14:21.000000 joulescope_ui-1.1.7/joulescope_ui/resources.rcc
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/safe_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/shift_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/software_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/source_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.410035 joulescope_ui-1.1.7/joulescope_ui/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/color_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/color_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/color_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/font_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.414034 joulescope_ui-1.1.7/joulescope_ui/styles/js1/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/arrow_down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/arrow_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/arrow_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/arrow_up.svg
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/branch_closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/branch_end.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/branch_end_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/branch_more.svg
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/branch_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/branch_vline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/checkbox_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/checkbox_indeterminate.svg
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/checkbox_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/detach.svg
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/hmovetoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/hsepartoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/radio_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/radio_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/sizegrip.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/style.html
--rw-r--r--   0 runner    (1001) docker     (127)    19555 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/tabs_menu.svg
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/transparent.svg
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/vmovetoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/vsepartoolbars.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/parameter_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.414034 joulescope_ui-1.1.7/joulescope_ui/styles/system/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/system/index.json
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/system/style.html
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/system/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/system/zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/system/zoom_in.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/system/zoom_out.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.418035 joulescope_ui-1.1.7/joulescope_ui/styles/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/test/test_color_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/test/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/test/test_parameter_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.418035 joulescope_ui-1.1.7/joulescope_ui/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/anno1.anno.jls
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_annotation_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_disk_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_pubsub_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_pubsub_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_range_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_software_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_source_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_versioned_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/ui_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/versioned_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    14173 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widget_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.418035 joulescope_ui-1.1.7/joulescope_ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.422035 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/accumulator_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.422035 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.422035 joulescope_ui-1.1.7/joulescope_ui/widgets/clock/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/clock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/clock/clock_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.422035 joulescope_ui-1.1.7/joulescope_ui/widgets/developer/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/developer/log_view_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/developer/profile_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/developer/publish_spy_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/developer/pubsub_explorer_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.422035 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/current_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/device_control_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/device_info_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/device_update_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.426035 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/active_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/device_close.svg
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/device_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/doc.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/fuse_normal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/info.svg
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/open.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/target_power.svg
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/target_power_off.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/double_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/draggable_list_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.426035 joulescope_ui-1.1.7/joulescope_ui/widgets/example/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/example_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.426035 joulescope_ui-1.1.7/joulescope_ui/widgets/example/styles/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.426035 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/flyout_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/hamburger/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/hamburger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/hamburger/hamburger_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/help/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/help/help_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/jls_info/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/jls_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/jls_info/jls_info_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/current_offset.png
--rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/js220_cal_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/voltage_offset.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/memory_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/notes/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/notes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/notes/notes_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/progress_bar/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/progress_bar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/record_status_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/record.svg
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.434034 joulescope_ui-1.1.7/joulescope_ui/widgets/report_issue/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/report_issue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/report_issue/report_issue_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.434034 joulescope_ui-1.1.7/joulescope_ui/widgets/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24143 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/settings/settings_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/settings/unique_strings_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.434034 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/sidebar_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.434034 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/device.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/help.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/memory.svg
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/misc.svg
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/pause.svg
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/play.svg
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/record.svg
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/settings.svg
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/stop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/target_power.svg
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/target_power_off.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.434034 joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/disk_full_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/signal_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.434034 joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/statistics_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.438034 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/condition_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.438034 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/active.svg
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/continuous.svg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/inactive.svg
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/searching.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/single.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.438034 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/test_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/test_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)    48890 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/trigger_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.438034 joulescope_ui-1.1.7/joulescope_ui/widgets/value/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.438034 joulescope_ui-1.1.7/joulescope_ui/widgets/value/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)    27149 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/value_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.438034 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.442034 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/add.svg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/delete.svg
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/move.svg
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/reset.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/view_manager_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.442034 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/annotations.md
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/axis_ticks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/interval_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/line_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/quantities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.446034 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/marker_add1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/marker_add2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/marker_clear.svg
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/pin_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/pin_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/style_defines.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/trace.svg
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/zoom_in.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/zoom_out.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.446034 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/test/test_axis_ticks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/test/test_quantities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/text_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/waveform_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/waveform_source_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)   173533 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/waveform_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/y_range_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/zip_inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.446034 joulescope_ui-1.1.7/joulescope_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-11 14:14:23.450034 joulescope_ui-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.748786 joulescope_ui-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    53673 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/CREDITS.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-13 15:39:21.748786 joulescope_ui-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-13 15:39:20.000000 joulescope_ui-1.1.8/joulescope.iss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.684787 joulescope_ui-1.1.8/joulescope_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    53673 2024-05-13 15:39:10.000000 joulescope_ui-1.1.8/joulescope_ui/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-13 15:39:10.000000 joulescope_ui-1.1.8/joulescope_ui/CREDITS.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/dev_signal_buffer_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/device_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24052 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31966 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js220.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js220_fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js220_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17812 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/devices/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/test/test_device_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/disk_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/entry_points/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/entry_points/zip_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/error_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14307 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/error_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/expanding_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/file_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/filename_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/fonts/DSEG14-Modern/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/fonts/Hack/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/fonts/Hack/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/fonts/Lato/
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/fonts/Lato/OFL.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/fonts/SourceCodePro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/fonts/SourceCodePro/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/fonts/SourceSerifPro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/fonts/SourceSerifPro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  3102116 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui/fonts.rcc
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/getting_started.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/help_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/intel_graphics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/jls_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/jls_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/jls_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/jls_v2_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/json_plus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/locale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    81702 2024-05-13 15:39:12.000000 joulescope_ui-1.1.8/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   112244 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    71550 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   102499 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    99351 2024-05-13 15:39:12.000000 joulescope_ui-1.1.8/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   130324 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    71667 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   102570 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    73100 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   104062 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    72339 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   103281 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    75547 2024-05-13 15:39:12.000000 joulescope_ui-1.1.8/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   105590 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po
+-rw-r--r--   0 runner    (1001) docker     (127)    68383 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/joulescope_ui.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    70320 2024-05-13 15:39:12.000000 joulescope_ui-1.1.8/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   100452 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    61353 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    91276 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42189 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/mem_leak_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p1/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p1/index.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p2/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p2/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/process_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66497 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/pubsub_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/pubsub_callable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/pubsub_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.700787 joulescope_ui-1.1.8/joulescope_ui/range_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/cdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/max_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/plugin_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/usb_inrush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.700787 joulescope_ui-1.1.8/joulescope_ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/dmg_background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/dmg_background.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    48138 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/dmg_background@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)   100365 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.704787 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_128x128.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_128x128@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_16x16.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_16x16@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_256x256.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_256x256@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_32x32.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_32x32@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_512x512.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7537 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_512x512@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_64x64.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_64x64@2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/logo-large.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/zoom.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-05-13 15:39:20.000000 joulescope_ui-1.1.8/joulescope_ui/resources.rcc
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/safe_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/shift_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/software_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/source_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.704787 joulescope_ui-1.1.8/joulescope_ui/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/color_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/color_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/color_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/font_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.708787 joulescope_ui-1.1.8/joulescope_ui/styles/js1/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/arrow_down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/arrow_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/arrow_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/arrow_up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/branch_closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/branch_end.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/branch_end_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/branch_more.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/branch_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/branch_vline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/checkbox_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/checkbox_indeterminate.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/checkbox_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/detach.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/hmovetoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/hsepartoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/radio_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/radio_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/sizegrip.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/style.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19555 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/tabs_menu.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/transparent.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/vmovetoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/vsepartoolbars.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/parameter_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.712787 joulescope_ui-1.1.8/joulescope_ui/styles/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/system/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/system/style.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/system/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/system/zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/system/zoom_in.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/system/zoom_out.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.712787 joulescope_ui-1.1.8/joulescope_ui/styles/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/test/test_color_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/test/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/test/test_parameter_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.716787 joulescope_ui-1.1.8/joulescope_ui/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/anno1.anno.jls
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_annotation_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_disk_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_pubsub_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_pubsub_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_range_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_software_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_source_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_versioned_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 15:39:12.000000 joulescope_ui-1.1.8/joulescope_ui/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/ui_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/versioned_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14173 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widget_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.716787 joulescope_ui-1.1.8/joulescope_ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.716787 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/accumulator_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.716787 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.716787 joulescope_ui-1.1.8/joulescope_ui/widgets/clock/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/clock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/clock/clock_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.720787 joulescope_ui-1.1.8/joulescope_ui/widgets/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/developer/log_view_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/developer/profile_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/developer/publish_spy_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/developer/pubsub_explorer_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.720787 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/current_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/device_control_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/device_info_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/device_update_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/active_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/device_close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/device_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/doc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/fuse_normal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/target_power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/target_power_off.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/double_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/draggable_list_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/example_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/example/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/flyout_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/hamburger/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/hamburger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/hamburger/hamburger_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/help/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/help/help_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/jls_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/jls_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/jls_info/jls_info_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/current_offset.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/js220_cal_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/voltage_offset.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/memory_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/notes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/notes/notes_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/progress_bar/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/progress_bar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/record_status_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.732787 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/record.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.732787 joulescope_ui-1.1.8/joulescope_ui/widgets/report_issue/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/report_issue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/report_issue/report_issue_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.732787 joulescope_ui-1.1.8/joulescope_ui/widgets/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24143 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/settings/settings_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/settings/unique_strings_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.732787 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/sidebar_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.736787 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/device.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/memory.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/misc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/pause.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/play.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/record.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/target_power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/target_power_off.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.736787 joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/disk_full_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/signal_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.736787 joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/statistics_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.736787 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/condition_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.736787 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/active.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/continuous.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/inactive.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/searching.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/single.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.736787 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/test_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48890 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/trigger_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.740787 joulescope_ui-1.1.8/joulescope_ui/widgets/value/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.740787 joulescope_ui-1.1.8/joulescope_ui/widgets/value/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)    27149 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/value_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.740787 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.740787 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/add.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/move.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/reset.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/view_manager_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.744787 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/annotations.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/axis_ticks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/interval_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/line_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/quantities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.744787 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/marker_add1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/marker_add2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/marker_clear.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/pin_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/pin_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/style_defines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/trace.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/zoom_in.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/zoom_out.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.744787 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/test/test_axis_ticks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/test/test_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/text_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/waveform_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/waveform_source_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)   174585 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/waveform_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/y_range_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/zip_inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.744787 joulescope_ui-1.1.8/joulescope_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 15:39:21.748786 joulescope_ui-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/setup.py
```

### Comparing `joulescope_ui-1.1.7/CHANGELOG.md` & `joulescope_ui-1.1.8/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope_ui.
 
 ---
 
-## 1.1.7
+## 1.1.8
 
-2024 May 11
+2024 May 13
 
 * Added arbitrary divisor with optional units to Value widget  #265
 * Added Flyout widget click & drag right to resize   #267
 * Deferred data directory creation  #266
 * Updated pyjls from 0.9.2 to 0.9.4 to fix unicode path handling.
 * Fixed crash on JLS file not found  #264
 * Changed to async publish for stream buffer to prevent timeouts  #269
```

### Comparing `joulescope_ui-1.1.7/CREDITS.html` & `joulescope_ui-1.1.8/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/LICENSE.txt` & `joulescope_ui-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/PKG-INFO` & `joulescope_ui-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope_ui
-Version: 1.1.7
+Version: 1.1.8
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope_ui-1.1.7/README.md` & `joulescope_ui-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope.iss` & `joulescope_ui-1.1.8/joulescope.iss`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ; Script generated by the Inno Setup Script Wizard.
 ; SEE THE DOCUMENTATION FOR DETAILS ON CREATING INNO SETUP SCRIPT FILES!
 
 #define MyAppName "Joulescope"
-#define MyAppVersion "1.1.7"
-#define MyAppVersionUnderscores "1_1_7"
+#define MyAppVersion "1.1.8"
+#define MyAppVersionUnderscores "1_1_8"
 #define MyAppPublisher "Jetperch LLC"
 #define MyAppURL "https://www.joulescope.com"
 #define MyAppExeName "joulescope.exe"
 
 [Setup]
 ; NOTE: The value of AppId uniquely identifies this application.
 ; Do not use the same AppId value in installers for other applications.
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/CHANGELOG.md` & `joulescope_ui-1.1.8/joulescope_ui/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope_ui.
 
 ---
 
-## 1.1.7
+## 1.1.8
 
-2024 May 11
+2024 May 13
 
 * Added arbitrary divisor with optional units to Value widget  #265
 * Added Flyout widget click & drag right to resize   #267
 * Deferred data directory creation  #266
 * Updated pyjls from 0.9.2 to 0.9.4 to fix unicode path handling.
 * Fixed crash on JLS file not found  #264
 * Changed to async publish for stream buffer to prevent timeouts  #269
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/CREDITS.html` & `joulescope_ui-1.1.8/joulescope_ui/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/__main__.py` & `joulescope_ui-1.1.8/joulescope_ui/__main__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/about.py` & `joulescope_ui-1.1.8/joulescope_ui/about.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/api.py` & `joulescope_ui-1.1.8/joulescope_ui/api.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/app.py` & `joulescope_ui-1.1.8/joulescope_ui/app.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/capabilities.py` & `joulescope_ui-1.1.8/joulescope_ui/capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/dev_signal_buffer_source.py` & `joulescope_ui-1.1.8/joulescope_ui/dev_signal_buffer_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/devices/device_update.py` & `joulescope_ui-1.1.8/joulescope_ui/devices/device_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/device.py` & `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/device.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js110.py` & `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js110.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js220.py` & `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js220.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js220_fuse.py` & `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js220_fuse.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js220_updater.py` & `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js220_updater.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py` & `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py` & `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/devices/test/test_device_update.py` & `joulescope_ui-1.1.8/joulescope_ui/devices/test/test_device_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/disk_monitor.py` & `joulescope_ui-1.1.8/joulescope_ui/disk_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/entry_points/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/entry_points/ui.py` & `joulescope_ui-1.1.8/joulescope_ui/entry_points/ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/entry_points/zip_inspector.py` & `joulescope_ui-1.1.8/joulescope_ui/entry_points/zip_inspector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/error_dialog.py` & `joulescope_ui-1.1.8/joulescope_ui/error_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/error_window.py` & `joulescope_ui-1.1.8/joulescope_ui/error_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/expanding_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/expanding_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/exporter.py` & `joulescope_ui-1.1.8/joulescope_ui/exporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/file_dialog.py` & `joulescope_ui-1.1.8/joulescope_ui/file_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/filename_formatter.py` & `joulescope_ui-1.1.8/joulescope_ui/filename_formatter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt` & `joulescope_ui-1.1.8/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/fonts/Hack/LICENSE.md` & `joulescope_ui-1.1.8/joulescope_ui/fonts/Hack/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/fonts/Lato/OFL.txt` & `joulescope_ui-1.1.8/joulescope_ui/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/fonts/SourceCodePro/LICENSE.md` & `joulescope_ui-1.1.8/joulescope_ui/fonts/SourceCodePro/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/fonts/SourceSerifPro/OFL.txt` & `joulescope_ui-1.1.8/joulescope_ui/fonts/SourceSerifPro/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/fonts.rcc` & `joulescope_ui-1.1.8/joulescope_ui/fonts.rcc`

 * *Files 1% similar despite different names*

```diff
@@ -193814,70 +193814,70 @@
 002f5150: 0000 0000 0000 0000 0000 0080 0002 0000  ................
 002f5160: 000a 0000 0027 0000 0000 0000 0000 0000  .....'..........
 002f5170: 0050 0002 0000 000c 0000 001b 0000 0000  .P..............
 002f5180: 0000 0000 0000 0010 0002 0000 0006 0000  ................
 002f5190: 0015 0000 0000 0000 0000 0000 0030 0002  .............0..
 002f51a0: 0000 000e 0000 0007 0000 0000 0000 0000  ................
 002f51b0: 0000 071a 0004 0000 0001 0025 4f27 0000  ...........%O'..
-002f51c0: 018f 6800 b746 0000 07c4 0004 0000 0001  ..h..F..........
-002f51d0: 0029 2537 0000 018f 6800 b742 0000 058c  .)%7....h..B....
-002f51e0: 0004 0000 0001 001c 6407 0000 018f 6800  ........d.....h.
-002f51f0: b74a 0000 05ba 0004 0000 0001 001d 95a3  .J..............
-002f5200: 0000 018f 6800 b74e 0000 0750 0004 0000  ....h..N...P....
-002f5210: 0001 0026 8517 0000 018f 6800 b752 0000  ...&......h..R..
+002f51c0: 018f 729b 2ff5 0000 07c4 0004 0000 0001  ..r./...........
+002f51d0: 0029 2537 0000 018f 729b 2ff1 0000 058c  .)%7....r./.....
+002f51e0: 0004 0000 0001 001c 6407 0000 018f 729b  ........d.....r.
+002f51f0: 2ff9 0000 05ba 0004 0000 0001 001d 95a3  /...............
+002f5200: 0000 018f 729b 3001 0000 0750 0004 0000  ....r.0....P....
+002f5210: 0001 0026 8517 0000 018f 729b 3001 0000  ...&......r.0...
 002f5220: 07fc 0004 0000 0001 002a 5802 0000 018f  .........*X.....
-002f5230: 6800 b746 0000 082e 0004 0000 0001 002b  h..F...........+
-002f5240: c4d1 0000 018f 6800 b74a 0000 062c 0004  ......h..J...,..
-002f5250: 0000 0001 0020 3160 0000 018f 6800 b74e  ..... 1`....h..N
+002f5230: 729b 2ff5 0000 082e 0004 0000 0001 002b  r./............+
+002f5240: c4d1 0000 018f 729b 2ff9 0000 062c 0004  ......r./....,..
+002f5250: 0000 0001 0020 3160 0000 018f 729b 2ffd  ..... 1`....r./.
 002f5260: 0000 05f4 0004 0000 0001 001f 01ac 0000  ................
-002f5270: 018f 6800 b74a 0000 078e 0004 0000 0001  ..h..J..........
-002f5280: 0027 bab6 0000 018f 6800 b74e 0000 0666  .'......h..N...f
-002f5290: 0004 0000 0001 0021 6449 0000 018f 6800  .......!dI....h.
-002f52a0: b746 0000 06e6 0004 0000 0001 0023 e72d  .F...........#.-
-002f52b0: 0000 018f 6800 b742 0000 0862 0004 0000  ....h..B...b....
-002f52c0: 0001 002d 262d 0000 018f 6800 b74e 0000  ...-&-....h..N..
+002f5270: 018f 729b 2ffd 0000 078e 0004 0000 0001  ..r./...........
+002f5280: 0027 bab6 0000 018f 729b 2ffd 0000 0666  .'......r./....f
+002f5290: 0004 0000 0001 0021 6449 0000 018f 729b  .......!dI....r.
+002f52a0: 2ff9 0000 06e6 0004 0000 0001 0023 e72d  /............#.-
+002f52b0: 0000 018f 729b 2ff1 0000 0862 0004 0000  ....r./....b....
+002f52c0: 0001 002d 262d 0000 018f 729b 3001 0000  ...-&-....r.0...
 002f52d0: 06a8 0004 0000 0001 0022 8ce5 0000 018f  ........."......
-002f52e0: 6800 b746 0000 089a 0004 0000 0001 002e  h..F............
-002f52f0: 90bc 0000 018f 6800 b736 0000 08d0 0004  ......h..6......
-002f5300: 0000 0001 002e af00 0000 018f 6800 b736  ............h..6
+002f52e0: 729b 2ff9 0000 089a 0004 0000 0001 002e  r./.............
+002f52f0: 90bc 0000 018f 729b 2fe5 0000 08d0 0004  ......r./.......
+002f5300: 0000 0001 002e af00 0000 018f 729b 2fe5  ............r./.
 002f5310: 0000 097c 0004 0000 0001 002f 0ab2 0000  ...|......./....
-002f5320: 018f 6800 b736 0000 09b0 0004 0000 0001  ..h..6..........
-002f5330: 002f 293e 0000 018f 6800 b736 0000 090c  ./)>....h..6....
-002f5340: 0004 0000 0001 002e cd3f 0000 018f 6800  .........?....h.
-002f5350: b736 0000 094a 0004 0000 0001 002e ec32  .6...J.........2
-002f5360: 0000 018f 6800 b736 0000 0544 0004 0000  ....h..6...D....
-002f5370: 0001 001b 3ffe 0000 018f 6800 b75e 0000  ....?.....h..^..
+002f5320: 018f 729b 2fe5 0000 09b0 0004 0000 0001  ..r./...........
+002f5330: 002f 293e 0000 018f 729b 2fe5 0000 090c  ./)>....r./.....
+002f5340: 0004 0000 0001 002e cd3f 0000 018f 729b  .........?....r.
+002f5350: 2fe5 0000 094a 0004 0000 0001 002e ec32  /....J.........2
+002f5360: 0000 018f 729b 2fe5 0000 0544 0004 0000  ....r./....D....
+002f5370: 0001 001b 3ffe 0000 018f 729b 300d 0000  ....?.....r.0...
 002f5380: 036a 0004 0000 0001 0010 f545 0000 018f  .j.........E....
-002f5390: 6800 b756 0000 041a 0004 0000 0001 0014  h..V............
-002f53a0: f75f 0000 018f 6800 b75a 0000 048c 0004  ._....h..Z......
-002f53b0: 0000 0001 0017 6f8d 0000 018f 6800 b75a  ......o.....h..Z
+002f5390: 729b 3005 0000 041a 0004 0000 0001 0014  r.0.............
+002f53a0: f75f 0000 018f 729b 3009 0000 048c 0004  ._....r.0.......
+002f53b0: 0000 0001 0017 6f8d 0000 018f 729b 3009  ......o.....r.0.
 002f53c0: 0000 04c2 0004 0000 0001 0018 d613 0000  ................
-002f53d0: 018f 6800 b756 0000 03aa 0004 0000 0001  ..h..V..........
-002f53e0: 0012 1971 0000 018f 6800 b756 0000 03de  ...q....h..V....
-002f53f0: 0004 0000 0001 0013 8810 0000 018f 6800  ..............h.
-002f5400: b75e 0000 02dc 0004 0000 0001 000e c39f  .^..............
-002f5410: 0000 018f 6800 b75a 0000 0452 0004 0000  ....h..Z...R....
-002f5420: 0001 0016 0ed3 0000 018f 6800 b75a 0000  ..........h..Z..
+002f53d0: 018f 729b 3009 0000 03aa 0004 0000 0001  ..r.0...........
+002f53e0: 0012 1971 0000 018f 729b 3005 0000 03de  ...q....r.0.....
+002f53f0: 0004 0000 0001 0013 8810 0000 018f 729b  ..............r.
+002f5400: 300d 0000 02dc 0004 0000 0001 000e c39f  0...............
+002f5410: 0000 018f 729b 3009 0000 0452 0004 0000  ....r.0....R....
+002f5420: 0001 0016 0ed3 0000 018f 729b 300d 0000  ..........r.0...
 002f5430: 0502 0004 0000 0001 001a 2aab 0000 018f  ..........*.....
-002f5440: 6800 b752 0000 031e 0004 0000 0001 000f  h..R............
-002f5450: e47b 0000 018f 6800 b756 0000 02a6 0004  .{....h..V......
-002f5460: 0000 0001 000d 65a3 0000 018f 6800 b752  ......e.....h..R
+002f5440: 729b 3005 0000 031e 0004 0000 0001 000f  r.0.............
+002f5450: e47b 0000 018f 729b 3009 0000 02a6 0004  .{....r.0.......
+002f5460: 0000 0001 000d 65a3 0000 018f 729b 3001  ......e.....r.0.
 002f5470: 0000 01ae 0004 0000 0001 0003 6c6f 0000  ............lo..
-002f5480: 018f 6800 b73e 0000 008e 0004 0000 0001  ..h..>..........
-002f5490: 0000 0000 0000 018f 6800 b73e 0000 018a  ........h..>....
-002f54a0: 0004 0000 0001 0002 e1fa 0000 018f 6800  ..............h.
-002f54b0: b73e 0000 010a 0004 0000 0001 0001 72aa  .>............r.
-002f54c0: 0000 018f 6800 b73e 0000 00e8 0004 0000  ....h..>........
-002f54d0: 0001 0000 f2c6 0000 018f 6800 b73e 0000  ..........h..>..
+002f5480: 018f 729b 2fed 0000 008e 0004 0000 0001  ..r./...........
+002f5490: 0000 0000 0000 018f 729b 2fed 0000 018a  ........r./.....
+002f54a0: 0004 0000 0001 0002 e1fa 0000 018f 729b  ..............r.
+002f54b0: 2fed 0000 010a 0004 0000 0001 0001 72aa  /.............r.
+002f54c0: 0000 018f 729b 2ff1 0000 00e8 0004 0000  ....r./.........
+002f54d0: 0001 0000 f2c6 0000 018f 729b 2fed 0000  ..........r./...
 002f54e0: 015e 0004 0000 0001 0002 7e0b 0000 018f  .^........~.....
-002f54f0: 6800 b742 0000 00ba 0004 0000 0001 0000  h..B............
-002f5500: 8b33 0000 018f 6800 b73e 0000 01f0 0004  .3....h..>......
-002f5510: 0000 0001 0004 74f0 0000 018f 6800 b742  ......t.....h..B
+002f54f0: 729b 2ff1 0000 00ba 0004 0000 0001 0000  r./.............
+002f5500: 8b33 0000 018f 729b 2fed 0000 01f0 0004  .3....r./.......
+002f5510: 0000 0001 0004 74f0 0000 018f 729b 2ff1  ......t.....r./.
 002f5520: 0000 01ce 0004 0000 0001 0003 ee66 0000  .............f..
-002f5530: 018f 6800 b73e 0000 0130 0004 0000 0001  ..h..>...0......
-002f5540: 0001 f768 0000 018f 6800 b73e 0000 0210  ...h....h..>....
-002f5550: 0004 0000 0001 0004 f353 0000 018f 6800  .........S....h.
-002f5560: b73a 0000 027a 0004 0000 0001 000b 366d  .:...z........6m
-002f5570: 0000 018f 6800 b73a 0000 0234 0004 0000  ....h..:...4....
-002f5580: 0001 0007 158f 0000 018f 6800 b736 0000  ..........h..6..
+002f5530: 018f 729b 2fed 0000 0130 0004 0000 0001  ..r./....0......
+002f5540: 0001 f768 0000 018f 729b 2fed 0000 0210  ...h....r./.....
+002f5550: 0004 0000 0001 0004 f353 0000 018f 729b  .........S....r.
+002f5560: 2fe9 0000 027a 0004 0000 0001 000b 366d  /....z........6m
+002f5570: 0000 018f 729b 2fe9 0000 0234 0004 0000  ....r./....4....
+002f5580: 0001 0007 158f 0000 018f 729b 2fe5 0000  ..........r./...
 002f5590: 0254 0004 0000 0001 0009 2ac5 0000 018f  .T........*.....
-002f55a0: 6800 b73e                                h..>
+002f55a0: 729b 2fed                                r./.
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/getting_started.py` & `joulescope_ui-1.1.8/joulescope_ui/getting_started.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/help_ui.py` & `joulescope_ui-1.1.8/joulescope_ui/help_ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/intel_graphics_dialog.py` & `joulescope_ui-1.1.8/joulescope_ui/intel_graphics_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/jls_source.py` & `joulescope_ui-1.1.8/joulescope_ui/jls_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/jls_v1.py` & `joulescope_ui-1.1.8/joulescope_ui/jls_v1.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/jls_v2.py` & `joulescope_ui-1.1.8/joulescope_ui/jls_v2.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/jls_v2_annotations.py` & `joulescope_ui-1.1.8/joulescope_ui/jls_v2_annotations.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/json_plus.py` & `joulescope_ui-1.1.8/joulescope_ui/json_plus.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.8/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.8/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
 msgid "Email"
 msgstr "البريد الإلكتروني"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "الوصف"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
 msgid "Edit"
 msgstr "تحرير"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "عرض كتخفيض"
 
@@ -1454,15 +1454,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3104
+#: widgets/waveform/waveform_widget.py:3110
 msgid "Name"
 msgstr "الاسم"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "مخزن جولسكوب للتيار"
 
@@ -2664,34 +2664,34 @@
 msgstr "المثلث الأيمن"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "المثلث الأيسر"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3056
 msgid "Manual"
 msgstr "دليل"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "المركز"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Text"
 msgstr "النص"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3398
+#: widgets/waveform/waveform_widget.py:3404
 msgid "Show text"
 msgstr "إظهار النص"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3410
+#: widgets/waveform/waveform_widget.py:3416
 msgid "Shape"
 msgstr "الشكل"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "الوضع Y"
 
@@ -3016,20 +3016,20 @@
 msgstr "كمية الإشارة المراد إظهارها في الملخص."
 
 #: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "وضع التعليق التوضيحي للمحور X"
 
 #: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2936
 msgid "Absolute"
 msgstr "المطلق"
 
 #: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2935
+#: widgets/waveform/waveform_widget.py:2941
 msgid "Relative"
 msgstr "نسبي"
 
 #: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "المصادر الفرعية المتاحة."
 
@@ -3037,158 +3037,158 @@
 msgid "The selected subsources for each trace."
 msgstr "المصادر الفرعية المختارة لكل تتبع."
 
 #: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr "أولوية التتبع: أعلى قيمة للتيار في الأعلى، لا شيء متوقف."
 
-#: widgets/waveform/waveform_widget.py:2877
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2883
+#: widgets/waveform/waveform_widget.py:3185
 msgid "Save image to file"
 msgstr "حفظ الصورة في ملف"
 
-#: widgets/waveform/waveform_widget.py:2924
-#: widgets/waveform/waveform_widget.py:2993
+#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2999
 msgid "Single marker"
 msgstr "علامة واحدة"
 
-#: widgets/waveform/waveform_widget.py:2925
-#: widgets/waveform/waveform_widget.py:2994
+#: widgets/waveform/waveform_widget.py:2931
+#: widgets/waveform/waveform_widget.py:3000
 msgid "Dual markers"
 msgstr "علامات مزدوجة"
 
-#: widgets/waveform/waveform_widget.py:2927
+#: widgets/waveform/waveform_widget.py:2933
 msgid "Mode"
 msgstr "الوضع"
 
-#: widgets/waveform/waveform_widget.py:2940
-#: widgets/waveform/waveform_widget.py:2995
-#: widgets/waveform/waveform_widget.py:3155
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:2946
+#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Clear all"
 msgstr "مسح الكل"
 
-#: widgets/waveform/waveform_widget.py:2951
-#: widgets/waveform/waveform_widget.py:3040
-#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:2957
+#: widgets/waveform/waveform_widget.py:3046
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Annotations"
 msgstr "التعليقات التوضيحية"
 
-#: widgets/waveform/waveform_widget.py:3043
+#: widgets/waveform/waveform_widget.py:3049
 msgid "Range"
 msgstr "النطاق"
 
-#: widgets/waveform/waveform_widget.py:3047
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Auto"
 msgstr "تلقائي"
 
-#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3059
 msgid "Exact"
 msgstr "دقيق"
 
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3068
 msgid "Scale"
 msgstr "المقياس"
 
-#: widgets/waveform/waveform_widget.py:3065
+#: widgets/waveform/waveform_widget.py:3071
 msgid "Linear"
 msgstr "الخطي"
 
-#: widgets/waveform/waveform_widget.py:3070
+#: widgets/waveform/waveform_widget.py:3076
 msgid "Logarithmic"
 msgstr "لوغاريتمي"
 
-#: widgets/waveform/waveform_widget.py:3078
+#: widgets/waveform/waveform_widget.py:3084
 msgid "Logarithmic zero"
 msgstr "الصفر اللوغاريتمي"
 
-#: widgets/waveform/waveform_widget.py:3092
+#: widgets/waveform/waveform_widget.py:3098
 msgid "Preferred prefix"
 msgstr "البادئة المفضلة"
 
-#: widgets/waveform/waveform_widget.py:3152
+#: widgets/waveform/waveform_widget.py:3158
 msgid "Add"
 msgstr "إضافة"
 
-#: widgets/waveform/waveform_widget.py:3153
+#: widgets/waveform/waveform_widget.py:3159
 msgid "Hide all text"
 msgstr "إخفاء كل النص"
 
-#: widgets/waveform/waveform_widget.py:3154
+#: widgets/waveform/waveform_widget.py:3160
 msgid "Show all text"
 msgstr "إظهار كل النص"
 
-#: widgets/waveform/waveform_widget.py:3162
+#: widgets/waveform/waveform_widget.py:3168
 msgid "Vertical"
 msgstr "عمودي"
 
-#: widgets/waveform/waveform_widget.py:3165
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Horizontal"
 msgstr "أفقي"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3177
 msgid "Save"
 msgstr "حفظ"
 
-#: widgets/waveform/waveform_widget.py:3176
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Y-axis auto range"
 msgstr "النطاق التلقائي للمحور Y"
 
-#: widgets/waveform/waveform_widget.py:3180
+#: widgets/waveform/waveform_widget.py:3186
 msgid "Copy image to clipboard"
 msgstr "نسخ الصورة إلى الحافظة"
 
-#: widgets/waveform/waveform_widget.py:3181
+#: widgets/waveform/waveform_widget.py:3187
 msgid "Export visible data"
 msgstr "تصدير البيانات المرئية"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3188
 msgid "Export all data"
 msgstr "تصدير جميع البيانات"
 
-#: widgets/waveform/waveform_widget.py:3354
+#: widgets/waveform/waveform_widget.py:3360
 msgid "Export"
 msgstr "التصدير"
 
-#: widgets/waveform/waveform_widget.py:3355
+#: widgets/waveform/waveform_widget.py:3361
 msgid "Analysis"
 msgstr "التحليل"
 
-#: widgets/waveform/waveform_widget.py:3363
+#: widgets/waveform/waveform_widget.py:3369
 msgid "Interval"
 msgstr "الفاصل الزمني"
 
-#: widgets/waveform/waveform_widget.py:3372
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Zoom"
 msgstr "تكبير"
 
-#: widgets/waveform/waveform_widget.py:3376
+#: widgets/waveform/waveform_widget.py:3382
 msgid "Show statistics"
 msgstr "عرض الإحصائيات"
 
-#: widgets/waveform/waveform_widget.py:3381
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Left"
 msgstr "يسار"
 
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3390
 msgid "Right"
 msgstr "صحيح"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3393
 msgid "Off"
 msgstr "إيقاف التشغيل"
 
-#: widgets/waveform/waveform_widget.py:3390
-#: widgets/waveform/waveform_widget.py:3418
-#: widgets/waveform/waveform_widget.py:3448
+#: widgets/waveform/waveform_widget.py:3396
+#: widgets/waveform/waveform_widget.py:3424
+#: widgets/waveform/waveform_widget.py:3454
 msgid "Remove"
 msgstr "إزالة"
 
-#: widgets/waveform/waveform_widget.py:3401
+#: widgets/waveform/waveform_widget.py:3407
 msgid "Y mode"
 msgstr "الوضع Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "الحد الأقصى"
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.8/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.8/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
 msgid "Email"
 msgstr "E-Mail"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Beschreibung"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
 msgid "Edit"
 msgstr "Bearbeiten"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Als Markdown anzeigen"
 
@@ -1522,15 +1522,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3104
+#: widgets/waveform/waveform_widget.py:3110
 msgid "Name"
 msgstr "Name"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Joulescope Strompuffer"
 
@@ -2781,34 +2781,34 @@
 msgstr "Dreieck rechts"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "Dreieck links"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3056
 msgid "Manual"
 msgstr "Handbuch"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Zentriert"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Text"
 msgstr "Text"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3398
+#: widgets/waveform/waveform_widget.py:3404
 msgid "Show text"
 msgstr "Text anzeigen"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3410
+#: widgets/waveform/waveform_widget.py:3416
 msgid "Shape"
 msgstr "Form"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Y Mode"
 
@@ -3152,20 +3152,20 @@
 msgstr "Die Signalgröße, die in der Zusammenfassung angezeigt werden soll."
 
 #: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "X-Achsen-Anmerkungsmodus"
 
 #: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2936
 msgid "Absolute"
 msgstr "Absolut"
 
 #: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2935
+#: widgets/waveform/waveform_widget.py:2941
 msgid "Relative"
 msgstr "Relativ"
 
 #: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "Die verfügbaren Teilquellen."
 
@@ -3174,158 +3174,158 @@
 msgstr "Die ausgewählten Teilquellen für jede Messkurve."
 
 #: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "Die Priorität der Messkurve: Der höchste int-Wert steht oben, None ist aus."
 
-#: widgets/waveform/waveform_widget.py:2877
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2883
+#: widgets/waveform/waveform_widget.py:3185
 msgid "Save image to file"
 msgstr "Bild in Datei speichern"
 
-#: widgets/waveform/waveform_widget.py:2924
-#: widgets/waveform/waveform_widget.py:2993
+#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2999
 msgid "Single marker"
 msgstr "Einzelner Marker"
 
-#: widgets/waveform/waveform_widget.py:2925
-#: widgets/waveform/waveform_widget.py:2994
+#: widgets/waveform/waveform_widget.py:2931
+#: widgets/waveform/waveform_widget.py:3000
 msgid "Dual markers"
 msgstr "Zwei Marker"
 
-#: widgets/waveform/waveform_widget.py:2927
+#: widgets/waveform/waveform_widget.py:2933
 msgid "Mode"
 msgstr "Modus"
 
-#: widgets/waveform/waveform_widget.py:2940
-#: widgets/waveform/waveform_widget.py:2995
-#: widgets/waveform/waveform_widget.py:3155
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:2946
+#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Clear all"
 msgstr "Alles löschen"
 
-#: widgets/waveform/waveform_widget.py:2951
-#: widgets/waveform/waveform_widget.py:3040
-#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:2957
+#: widgets/waveform/waveform_widget.py:3046
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Annotations"
 msgstr "Anmerkungen"
 
-#: widgets/waveform/waveform_widget.py:3043
+#: widgets/waveform/waveform_widget.py:3049
 msgid "Range"
 msgstr "Range"
 
-#: widgets/waveform/waveform_widget.py:3047
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3059
 msgid "Exact"
 msgstr "Genau"
 
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3068
 msgid "Scale"
 msgstr "Skala"
 
-#: widgets/waveform/waveform_widget.py:3065
+#: widgets/waveform/waveform_widget.py:3071
 msgid "Linear"
 msgstr "Linear"
 
-#: widgets/waveform/waveform_widget.py:3070
+#: widgets/waveform/waveform_widget.py:3076
 msgid "Logarithmic"
 msgstr "Logarithmisch"
 
-#: widgets/waveform/waveform_widget.py:3078
+#: widgets/waveform/waveform_widget.py:3084
 msgid "Logarithmic zero"
 msgstr "Logarithmischer Nullpunkt"
 
-#: widgets/waveform/waveform_widget.py:3092
+#: widgets/waveform/waveform_widget.py:3098
 msgid "Preferred prefix"
 msgstr "Bevorzugte Vorsilbe"
 
-#: widgets/waveform/waveform_widget.py:3152
+#: widgets/waveform/waveform_widget.py:3158
 msgid "Add"
 msgstr "hinzufügen"
 
-#: widgets/waveform/waveform_widget.py:3153
+#: widgets/waveform/waveform_widget.py:3159
 msgid "Hide all text"
 msgstr "Alle Texte ausblenden"
 
-#: widgets/waveform/waveform_widget.py:3154
+#: widgets/waveform/waveform_widget.py:3160
 msgid "Show all text"
 msgstr "Alle Texte anzeigen"
 
-#: widgets/waveform/waveform_widget.py:3162
+#: widgets/waveform/waveform_widget.py:3168
 msgid "Vertical"
 msgstr "Vertikal"
 
-#: widgets/waveform/waveform_widget.py:3165
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Horizontal"
 msgstr "Horizontal"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3177
 msgid "Save"
 msgstr "Speichern Sie"
 
-#: widgets/waveform/waveform_widget.py:3176
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Y-axis auto range"
 msgstr "Automatischer Bereich der Y-Achse"
 
-#: widgets/waveform/waveform_widget.py:3180
+#: widgets/waveform/waveform_widget.py:3186
 msgid "Copy image to clipboard"
 msgstr "Bild in die Zwischenablage kopieren"
 
-#: widgets/waveform/waveform_widget.py:3181
+#: widgets/waveform/waveform_widget.py:3187
 msgid "Export visible data"
 msgstr "Sichtbare Daten exportieren"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3188
 msgid "Export all data"
 msgstr "Alle Daten exportieren"
 
-#: widgets/waveform/waveform_widget.py:3354
+#: widgets/waveform/waveform_widget.py:3360
 msgid "Export"
 msgstr "Exportieren"
 
-#: widgets/waveform/waveform_widget.py:3355
+#: widgets/waveform/waveform_widget.py:3361
 msgid "Analysis"
 msgstr "Analyse"
 
-#: widgets/waveform/waveform_widget.py:3363
+#: widgets/waveform/waveform_widget.py:3369
 msgid "Interval"
 msgstr "Interval"
 
-#: widgets/waveform/waveform_widget.py:3372
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Zoom"
 msgstr "Zoom"
 
-#: widgets/waveform/waveform_widget.py:3376
+#: widgets/waveform/waveform_widget.py:3382
 msgid "Show statistics"
 msgstr "Statistik anzeigen"
 
-#: widgets/waveform/waveform_widget.py:3381
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Left"
 msgstr "Links"
 
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3390
 msgid "Right"
 msgstr "Rechts"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3393
 msgid "Off"
 msgstr "Aus"
 
-#: widgets/waveform/waveform_widget.py:3390
-#: widgets/waveform/waveform_widget.py:3418
-#: widgets/waveform/waveform_widget.py:3448
+#: widgets/waveform/waveform_widget.py:3396
+#: widgets/waveform/waveform_widget.py:3424
+#: widgets/waveform/waveform_widget.py:3454
 msgid "Remove"
 msgstr "entfernen"
 
-#: widgets/waveform/waveform_widget.py:3401
+#: widgets/waveform/waveform_widget.py:3407
 msgid "Y mode"
 msgstr "Y-Modus"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "max"
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.8/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.8/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
 msgid "Email"
 msgstr "Email"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Περιγραφή"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
 msgid "Edit"
 msgstr "Επεξεργασία"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Προβολή ως Markdown"
 
@@ -1529,15 +1529,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3104
+#: widgets/waveform/waveform_widget.py:3110
 msgid "Name"
 msgstr "Όνομα"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Απομονωτής ρεύματος Joulescope"
 
@@ -2791,34 +2791,34 @@
 msgstr "τρίγωνο δεξιά"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "τρίγωνο αριστερά"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3056
 msgid "Manual"
 msgstr "Εγχειρίδιο"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Centered"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Text"
 msgstr "Κείμενο"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3398
+#: widgets/waveform/waveform_widget.py:3404
 msgid "Show text"
 msgstr "Εμφάνιση κειμένου"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3410
+#: widgets/waveform/waveform_widget.py:3416
 msgid "Shape"
 msgstr "Σχήμα"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Λειτουργία Y"
 
@@ -3160,20 +3160,20 @@
 msgstr "Η ποσότητα σήματος που θα εμφανίζεται στη σύνοψη."
 
 #: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "Λειτουργία σχολιασμού του άξονα Χ"
 
 #: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2936
 msgid "Absolute"
 msgstr "Απόλυτο"
 
 #: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2935
+#: widgets/waveform/waveform_widget.py:2941
 msgid "Relative"
 msgstr "Σχετική"
 
 #: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "Οι διαθέσιμες υποπηγές."
 
@@ -3183,158 +3183,158 @@
 
 #: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "Η προτεραιότητα του ίχνους: η υψηλότερη τιμή int στην κορυφή, το None είναι "
 "απενεργοποιημένο."
 
-#: widgets/waveform/waveform_widget.py:2877
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2883
+#: widgets/waveform/waveform_widget.py:3185
 msgid "Save image to file"
 msgstr "Αποθήκευση εικόνας σε αρχείο"
 
-#: widgets/waveform/waveform_widget.py:2924
-#: widgets/waveform/waveform_widget.py:2993
+#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2999
 msgid "Single marker"
 msgstr "Ενιαίος δείκτης"
 
-#: widgets/waveform/waveform_widget.py:2925
-#: widgets/waveform/waveform_widget.py:2994
+#: widgets/waveform/waveform_widget.py:2931
+#: widgets/waveform/waveform_widget.py:3000
 msgid "Dual markers"
 msgstr "Διπλοί δείκτες"
 
-#: widgets/waveform/waveform_widget.py:2927
+#: widgets/waveform/waveform_widget.py:2933
 msgid "Mode"
 msgstr "Λειτουργία"
 
-#: widgets/waveform/waveform_widget.py:2940
-#: widgets/waveform/waveform_widget.py:2995
-#: widgets/waveform/waveform_widget.py:3155
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:2946
+#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Clear all"
 msgstr "Εκκαθάριση όλων"
 
-#: widgets/waveform/waveform_widget.py:2951
-#: widgets/waveform/waveform_widget.py:3040
-#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:2957
+#: widgets/waveform/waveform_widget.py:3046
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Annotations"
 msgstr "Σημειώσεις"
 
-#: widgets/waveform/waveform_widget.py:3043
+#: widgets/waveform/waveform_widget.py:3049
 msgid "Range"
 msgstr "Εύρος"
 
-#: widgets/waveform/waveform_widget.py:3047
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3059
 msgid "Exact"
 msgstr "Ακριβές"
 
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3068
 msgid "Scale"
 msgstr "Κλίμακα"
 
-#: widgets/waveform/waveform_widget.py:3065
+#: widgets/waveform/waveform_widget.py:3071
 msgid "Linear"
 msgstr "Γραμμική"
 
-#: widgets/waveform/waveform_widget.py:3070
+#: widgets/waveform/waveform_widget.py:3076
 msgid "Logarithmic"
 msgstr "Λογαριθμική"
 
-#: widgets/waveform/waveform_widget.py:3078
+#: widgets/waveform/waveform_widget.py:3084
 msgid "Logarithmic zero"
 msgstr "Λογαριθμικό μηδέν"
 
-#: widgets/waveform/waveform_widget.py:3092
+#: widgets/waveform/waveform_widget.py:3098
 msgid "Preferred prefix"
 msgstr "Προτιμώμενο πρόθεμα"
 
-#: widgets/waveform/waveform_widget.py:3152
+#: widgets/waveform/waveform_widget.py:3158
 msgid "Add"
 msgstr "Προσθήκη"
 
-#: widgets/waveform/waveform_widget.py:3153
+#: widgets/waveform/waveform_widget.py:3159
 msgid "Hide all text"
 msgstr "Απόκρυψη όλου του κειμένου"
 
-#: widgets/waveform/waveform_widget.py:3154
+#: widgets/waveform/waveform_widget.py:3160
 msgid "Show all text"
 msgstr "Εμφάνιση όλου του κειμένου"
 
-#: widgets/waveform/waveform_widget.py:3162
+#: widgets/waveform/waveform_widget.py:3168
 msgid "Vertical"
 msgstr "Κατακόρυφο"
 
-#: widgets/waveform/waveform_widget.py:3165
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Horizontal"
 msgstr "Οριζόντια"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3177
 msgid "Save"
 msgstr "Αποθήκευση"
 
-#: widgets/waveform/waveform_widget.py:3176
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Y-axis auto range"
 msgstr "Αυτόματο εύρος του άξονα Y"
 
-#: widgets/waveform/waveform_widget.py:3180
+#: widgets/waveform/waveform_widget.py:3186
 msgid "Copy image to clipboard"
 msgstr "Αντιγραφή εικόνας στο πρόχειρο"
 
-#: widgets/waveform/waveform_widget.py:3181
+#: widgets/waveform/waveform_widget.py:3187
 msgid "Export visible data"
 msgstr "Εξαγωγή ορατών δεδομένων"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3188
 msgid "Export all data"
 msgstr "Εξαγωγή όλων των δεδομένων"
 
-#: widgets/waveform/waveform_widget.py:3354
+#: widgets/waveform/waveform_widget.py:3360
 msgid "Export"
 msgstr "Εξαγωγή"
 
-#: widgets/waveform/waveform_widget.py:3355
+#: widgets/waveform/waveform_widget.py:3361
 msgid "Analysis"
 msgstr "Ανάλυση"
 
-#: widgets/waveform/waveform_widget.py:3363
+#: widgets/waveform/waveform_widget.py:3369
 msgid "Interval"
 msgstr "Διάστημα"
 
-#: widgets/waveform/waveform_widget.py:3372
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Zoom"
 msgstr "Ζουμ"
 
-#: widgets/waveform/waveform_widget.py:3376
+#: widgets/waveform/waveform_widget.py:3382
 msgid "Show statistics"
 msgstr "Εμφάνιση στατιστικών στοιχείων"
 
-#: widgets/waveform/waveform_widget.py:3381
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Left"
 msgstr "Αριστερά"
 
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3390
 msgid "Right"
 msgstr "Σωστό"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3393
 msgid "Off"
 msgstr "Off"
 
-#: widgets/waveform/waveform_widget.py:3390
-#: widgets/waveform/waveform_widget.py:3418
-#: widgets/waveform/waveform_widget.py:3448
+#: widgets/waveform/waveform_widget.py:3396
+#: widgets/waveform/waveform_widget.py:3424
+#: widgets/waveform/waveform_widget.py:3454
 msgid "Remove"
 msgstr "Αφαίρεση"
 
-#: widgets/waveform/waveform_widget.py:3401
+#: widgets/waveform/waveform_widget.py:3407
 msgid "Y mode"
 msgstr "Λειτουργία Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "max"
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.8/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.8/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
 msgid "Email"
 msgstr "Correo electrónico"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Descripción"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
 msgid "Edit"
 msgstr "Editar"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Ver como Markdown"
 
@@ -1520,15 +1520,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3104
+#: widgets/waveform/waveform_widget.py:3110
 msgid "Name"
 msgstr "Nombre"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Búfer de corriente de Joulescope"
 
@@ -2769,34 +2769,34 @@
 msgstr "triángulo derecho"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "triángulo izquierdo"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3056
 msgid "Manual"
 msgstr "Manual"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Centrado"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Text"
 msgstr "Texto"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3398
+#: widgets/waveform/waveform_widget.py:3404
 msgid "Show text"
 msgstr "Mostrar texto"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3410
+#: widgets/waveform/waveform_widget.py:3416
 msgid "Shape"
 msgstr "Forma"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Modo Y"
 
@@ -3136,20 +3136,20 @@
 msgstr "La cantidad de señal a mostrar en el resumen."
 
 #: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "Modo de anotación en el eje X"
 
 #: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2936
 msgid "Absolute"
 msgstr "Absoluto"
 
 #: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2935
+#: widgets/waveform/waveform_widget.py:2941
 msgid "Relative"
 msgstr "Relativa"
 
 #: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "Las subfuentes disponibles."
 
@@ -3159,158 +3159,158 @@
 
 #: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "La prioridad de la traza: el valor int más alto en la parte superior, "
 "Ninguno está desactivado."
 
-#: widgets/waveform/waveform_widget.py:2877
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2883
+#: widgets/waveform/waveform_widget.py:3185
 msgid "Save image to file"
 msgstr "Guardar imagen en archivo"
 
-#: widgets/waveform/waveform_widget.py:2924
-#: widgets/waveform/waveform_widget.py:2993
+#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2999
 msgid "Single marker"
 msgstr "Marcador único"
 
-#: widgets/waveform/waveform_widget.py:2925
-#: widgets/waveform/waveform_widget.py:2994
+#: widgets/waveform/waveform_widget.py:2931
+#: widgets/waveform/waveform_widget.py:3000
 msgid "Dual markers"
 msgstr "Marcadores duales"
 
-#: widgets/waveform/waveform_widget.py:2927
+#: widgets/waveform/waveform_widget.py:2933
 msgid "Mode"
 msgstr "Modo"
 
-#: widgets/waveform/waveform_widget.py:2940
-#: widgets/waveform/waveform_widget.py:2995
-#: widgets/waveform/waveform_widget.py:3155
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:2946
+#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Clear all"
 msgstr "Borrar todo"
 
-#: widgets/waveform/waveform_widget.py:2951
-#: widgets/waveform/waveform_widget.py:3040
-#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:2957
+#: widgets/waveform/waveform_widget.py:3046
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Annotations"
 msgstr "Anotaciones"
 
-#: widgets/waveform/waveform_widget.py:3043
+#: widgets/waveform/waveform_widget.py:3049
 msgid "Range"
 msgstr "Gama"
 
-#: widgets/waveform/waveform_widget.py:3047
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3059
 msgid "Exact"
 msgstr "Exacto"
 
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3068
 msgid "Scale"
 msgstr "Escala"
 
-#: widgets/waveform/waveform_widget.py:3065
+#: widgets/waveform/waveform_widget.py:3071
 msgid "Linear"
 msgstr "Lineal"
 
-#: widgets/waveform/waveform_widget.py:3070
+#: widgets/waveform/waveform_widget.py:3076
 msgid "Logarithmic"
 msgstr "Logarítmica"
 
-#: widgets/waveform/waveform_widget.py:3078
+#: widgets/waveform/waveform_widget.py:3084
 msgid "Logarithmic zero"
 msgstr "Cero logarítmico"
 
-#: widgets/waveform/waveform_widget.py:3092
+#: widgets/waveform/waveform_widget.py:3098
 msgid "Preferred prefix"
 msgstr "Prefijo preferido"
 
-#: widgets/waveform/waveform_widget.py:3152
+#: widgets/waveform/waveform_widget.py:3158
 msgid "Add"
 msgstr "Añadir"
 
-#: widgets/waveform/waveform_widget.py:3153
+#: widgets/waveform/waveform_widget.py:3159
 msgid "Hide all text"
 msgstr "Ocultar todo el texto"
 
-#: widgets/waveform/waveform_widget.py:3154
+#: widgets/waveform/waveform_widget.py:3160
 msgid "Show all text"
 msgstr "Mostrar todo el texto"
 
-#: widgets/waveform/waveform_widget.py:3162
+#: widgets/waveform/waveform_widget.py:3168
 msgid "Vertical"
 msgstr "Vertical"
 
-#: widgets/waveform/waveform_widget.py:3165
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Horizontal"
 msgstr "Horizontal"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3177
 msgid "Save"
 msgstr "Guardar"
 
-#: widgets/waveform/waveform_widget.py:3176
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Y-axis auto range"
 msgstr "Rango automático del eje Y"
 
-#: widgets/waveform/waveform_widget.py:3180
+#: widgets/waveform/waveform_widget.py:3186
 msgid "Copy image to clipboard"
 msgstr "Copiar imagen al portapapeles"
 
-#: widgets/waveform/waveform_widget.py:3181
+#: widgets/waveform/waveform_widget.py:3187
 msgid "Export visible data"
 msgstr "Exportación de datos visibles"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3188
 msgid "Export all data"
 msgstr "Exportar todos los datos"
 
-#: widgets/waveform/waveform_widget.py:3354
+#: widgets/waveform/waveform_widget.py:3360
 msgid "Export"
 msgstr "Exportar"
 
-#: widgets/waveform/waveform_widget.py:3355
+#: widgets/waveform/waveform_widget.py:3361
 msgid "Analysis"
 msgstr "Análisis"
 
-#: widgets/waveform/waveform_widget.py:3363
+#: widgets/waveform/waveform_widget.py:3369
 msgid "Interval"
 msgstr "Intervalo"
 
-#: widgets/waveform/waveform_widget.py:3372
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Zoom"
 msgstr "Zoom"
 
-#: widgets/waveform/waveform_widget.py:3376
+#: widgets/waveform/waveform_widget.py:3382
 msgid "Show statistics"
 msgstr "Mostrar estadísticas"
 
-#: widgets/waveform/waveform_widget.py:3381
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Left"
 msgstr "Izquierda"
 
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3390
 msgid "Right"
 msgstr "Derecha"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3393
 msgid "Off"
 msgstr "Apagado"
 
-#: widgets/waveform/waveform_widget.py:3390
-#: widgets/waveform/waveform_widget.py:3418
-#: widgets/waveform/waveform_widget.py:3448
+#: widgets/waveform/waveform_widget.py:3396
+#: widgets/waveform/waveform_widget.py:3424
+#: widgets/waveform/waveform_widget.py:3454
 msgid "Remove"
 msgstr "Eliminar"
 
-#: widgets/waveform/waveform_widget.py:3401
+#: widgets/waveform/waveform_widget.py:3407
 msgid "Y mode"
 msgstr "Modo Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "máx"
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.8/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.8/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,15 @@
 msgid "Email"
 msgstr "Courriel"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Description"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
 msgid "Edit"
 msgstr "Editer"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Voir comme Markdown"
 
@@ -1533,15 +1533,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3104
+#: widgets/waveform/waveform_widget.py:3110
 msgid "Name"
 msgstr "Nom"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Joulescope stream buffer"
 
@@ -2787,34 +2787,34 @@
 msgstr "triangle droit"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "triangle gauche"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3056
 msgid "Manual"
 msgstr "Manuel"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Centré"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Text"
 msgstr "Texte"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3398
+#: widgets/waveform/waveform_widget.py:3404
 msgid "Show text"
 msgstr "Afficher le texte"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3410
+#: widgets/waveform/waveform_widget.py:3416
 msgid "Shape"
 msgstr "Forme"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Mode Y"
 
@@ -3156,20 +3156,20 @@
 msgstr "La quantité de signal à afficher dans le résumé."
 
 #: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "Mode d'annotation de l'axe X"
 
 #: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2936
 msgid "Absolute"
 msgstr "Absolu"
 
 #: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2935
+#: widgets/waveform/waveform_widget.py:2941
 msgid "Relative"
 msgstr "Relatif"
 
 #: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "Les sous-sources disponibles."
 
@@ -3179,158 +3179,158 @@
 
 #: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "La priorité de la trace : la valeur int la plus élevée est en haut, None est"
 " désactivé."
 
-#: widgets/waveform/waveform_widget.py:2877
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2883
+#: widgets/waveform/waveform_widget.py:3185
 msgid "Save image to file"
 msgstr "Enregistrer l'image dans un fichier"
 
-#: widgets/waveform/waveform_widget.py:2924
-#: widgets/waveform/waveform_widget.py:2993
+#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2999
 msgid "Single marker"
 msgstr "Marqueur unique"
 
-#: widgets/waveform/waveform_widget.py:2925
-#: widgets/waveform/waveform_widget.py:2994
+#: widgets/waveform/waveform_widget.py:2931
+#: widgets/waveform/waveform_widget.py:3000
 msgid "Dual markers"
 msgstr "Double marqueur"
 
-#: widgets/waveform/waveform_widget.py:2927
+#: widgets/waveform/waveform_widget.py:2933
 msgid "Mode"
 msgstr "Mode de fonctionnement"
 
-#: widgets/waveform/waveform_widget.py:2940
-#: widgets/waveform/waveform_widget.py:2995
-#: widgets/waveform/waveform_widget.py:3155
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:2946
+#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Clear all"
 msgstr "Tout effacer"
 
-#: widgets/waveform/waveform_widget.py:2951
-#: widgets/waveform/waveform_widget.py:3040
-#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:2957
+#: widgets/waveform/waveform_widget.py:3046
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Annotations"
 msgstr "Annotations"
 
-#: widgets/waveform/waveform_widget.py:3043
+#: widgets/waveform/waveform_widget.py:3049
 msgid "Range"
 msgstr "Gamme"
 
-#: widgets/waveform/waveform_widget.py:3047
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3059
 msgid "Exact"
 msgstr "Exact"
 
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3068
 msgid "Scale"
 msgstr "Échelle"
 
-#: widgets/waveform/waveform_widget.py:3065
+#: widgets/waveform/waveform_widget.py:3071
 msgid "Linear"
 msgstr "Linéaire"
 
-#: widgets/waveform/waveform_widget.py:3070
+#: widgets/waveform/waveform_widget.py:3076
 msgid "Logarithmic"
 msgstr "Logarithmique"
 
-#: widgets/waveform/waveform_widget.py:3078
+#: widgets/waveform/waveform_widget.py:3084
 msgid "Logarithmic zero"
 msgstr "Zéro logarithmique"
 
-#: widgets/waveform/waveform_widget.py:3092
+#: widgets/waveform/waveform_widget.py:3098
 msgid "Preferred prefix"
 msgstr "Préfixe préféré"
 
-#: widgets/waveform/waveform_widget.py:3152
+#: widgets/waveform/waveform_widget.py:3158
 msgid "Add"
 msgstr "Ajouter"
 
-#: widgets/waveform/waveform_widget.py:3153
+#: widgets/waveform/waveform_widget.py:3159
 msgid "Hide all text"
 msgstr "Cacher tout le texte"
 
-#: widgets/waveform/waveform_widget.py:3154
+#: widgets/waveform/waveform_widget.py:3160
 msgid "Show all text"
 msgstr "Afficher tous les textes"
 
-#: widgets/waveform/waveform_widget.py:3162
+#: widgets/waveform/waveform_widget.py:3168
 msgid "Vertical"
 msgstr "Vertical"
 
-#: widgets/waveform/waveform_widget.py:3165
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Horizontal"
 msgstr "Horizontal"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3177
 msgid "Save"
 msgstr "Sauvegarder"
 
-#: widgets/waveform/waveform_widget.py:3176
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Y-axis auto range"
 msgstr "Plage automatique de l'axe Y"
 
-#: widgets/waveform/waveform_widget.py:3180
+#: widgets/waveform/waveform_widget.py:3186
 msgid "Copy image to clipboard"
 msgstr "Copier l'image dans le presse-papiers"
 
-#: widgets/waveform/waveform_widget.py:3181
+#: widgets/waveform/waveform_widget.py:3187
 msgid "Export visible data"
 msgstr "Export visible data"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3188
 msgid "Export all data"
 msgstr "Exporter toutes les données"
 
-#: widgets/waveform/waveform_widget.py:3354
+#: widgets/waveform/waveform_widget.py:3360
 msgid "Export"
 msgstr "Exportation"
 
-#: widgets/waveform/waveform_widget.py:3355
+#: widgets/waveform/waveform_widget.py:3361
 msgid "Analysis"
 msgstr "Analyse"
 
-#: widgets/waveform/waveform_widget.py:3363
+#: widgets/waveform/waveform_widget.py:3369
 msgid "Interval"
 msgstr "Intervalle"
 
-#: widgets/waveform/waveform_widget.py:3372
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Zoom"
 msgstr "Zoom"
 
-#: widgets/waveform/waveform_widget.py:3376
+#: widgets/waveform/waveform_widget.py:3382
 msgid "Show statistics"
 msgstr "Afficher les statistiques"
 
-#: widgets/waveform/waveform_widget.py:3381
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Left"
 msgstr "Gauche"
 
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3390
 msgid "Right"
 msgstr "Droit"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3393
 msgid "Off"
 msgstr "Off"
 
-#: widgets/waveform/waveform_widget.py:3390
-#: widgets/waveform/waveform_widget.py:3418
-#: widgets/waveform/waveform_widget.py:3448
+#: widgets/waveform/waveform_widget.py:3396
+#: widgets/waveform/waveform_widget.py:3424
+#: widgets/waveform/waveform_widget.py:3454
 msgid "Remove"
 msgstr "Enlever"
 
-#: widgets/waveform/waveform_widget.py:3401
+#: widgets/waveform/waveform_widget.py:3407
 msgid "Y mode"
 msgstr "Mode Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "max"
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.8/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.8/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
 msgid "Email"
 msgstr "E-mail"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Descrizione"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
 msgid "Edit"
 msgstr "Modifica"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Visualizza come Markdown"
 
@@ -1529,15 +1529,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3104
+#: widgets/waveform/waveform_widget.py:3110
 msgid "Name"
 msgstr "Nome"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Buffer di flusso Joulescope"
 
@@ -2785,34 +2785,34 @@
 msgstr "triangolo destro"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "triangolo a sinistra"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3056
 msgid "Manual"
 msgstr "Manuale"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Centrato"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Text"
 msgstr "Testo"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3398
+#: widgets/waveform/waveform_widget.py:3404
 msgid "Show text"
 msgstr "Mostra testo"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3410
+#: widgets/waveform/waveform_widget.py:3416
 msgid "Shape"
 msgstr "Forma"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Modalità Y"
 
@@ -3149,20 +3149,20 @@
 msgstr "La quantità di segnale da mostrare nel riepilogo."
 
 #: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "Modalità di annotazione sull'asse X"
 
 #: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2936
 msgid "Absolute"
 msgstr "Assoluta"
 
 #: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2935
+#: widgets/waveform/waveform_widget.py:2941
 msgid "Relative"
 msgstr "Relativo"
 
 #: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "Le sotto-sorgenti disponibili."
 
@@ -3172,158 +3172,158 @@
 
 #: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "La priorità della traccia: il valore int più alto è in cima, nessuno è "
 "spento."
 
-#: widgets/waveform/waveform_widget.py:2877
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2883
+#: widgets/waveform/waveform_widget.py:3185
 msgid "Save image to file"
 msgstr "Salva l'immagine su file"
 
-#: widgets/waveform/waveform_widget.py:2924
-#: widgets/waveform/waveform_widget.py:2993
+#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2999
 msgid "Single marker"
 msgstr "Marcatore singolo"
 
-#: widgets/waveform/waveform_widget.py:2925
-#: widgets/waveform/waveform_widget.py:2994
+#: widgets/waveform/waveform_widget.py:2931
+#: widgets/waveform/waveform_widget.py:3000
 msgid "Dual markers"
 msgstr "Doppio marcatore"
 
-#: widgets/waveform/waveform_widget.py:2927
+#: widgets/waveform/waveform_widget.py:2933
 msgid "Mode"
 msgstr "Modalità"
 
-#: widgets/waveform/waveform_widget.py:2940
-#: widgets/waveform/waveform_widget.py:2995
-#: widgets/waveform/waveform_widget.py:3155
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:2946
+#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Clear all"
 msgstr "Cancella tutto"
 
-#: widgets/waveform/waveform_widget.py:2951
-#: widgets/waveform/waveform_widget.py:3040
-#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:2957
+#: widgets/waveform/waveform_widget.py:3046
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Annotations"
 msgstr "Annotazioni"
 
-#: widgets/waveform/waveform_widget.py:3043
+#: widgets/waveform/waveform_widget.py:3049
 msgid "Range"
 msgstr "Gamma"
 
-#: widgets/waveform/waveform_widget.py:3047
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3059
 msgid "Exact"
 msgstr "Esatta"
 
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3068
 msgid "Scale"
 msgstr "Scale"
 
-#: widgets/waveform/waveform_widget.py:3065
+#: widgets/waveform/waveform_widget.py:3071
 msgid "Linear"
 msgstr "Lineare"
 
-#: widgets/waveform/waveform_widget.py:3070
+#: widgets/waveform/waveform_widget.py:3076
 msgid "Logarithmic"
 msgstr "Logaritmico"
 
-#: widgets/waveform/waveform_widget.py:3078
+#: widgets/waveform/waveform_widget.py:3084
 msgid "Logarithmic zero"
 msgstr "Zero logaritmico"
 
-#: widgets/waveform/waveform_widget.py:3092
+#: widgets/waveform/waveform_widget.py:3098
 msgid "Preferred prefix"
 msgstr "Prefisso preferito"
 
-#: widgets/waveform/waveform_widget.py:3152
+#: widgets/waveform/waveform_widget.py:3158
 msgid "Add"
 msgstr "Aggiungere"
 
-#: widgets/waveform/waveform_widget.py:3153
+#: widgets/waveform/waveform_widget.py:3159
 msgid "Hide all text"
 msgstr "Nascondi tutto il testo"
 
-#: widgets/waveform/waveform_widget.py:3154
+#: widgets/waveform/waveform_widget.py:3160
 msgid "Show all text"
 msgstr "Mostra tutto il testo"
 
-#: widgets/waveform/waveform_widget.py:3162
+#: widgets/waveform/waveform_widget.py:3168
 msgid "Vertical"
 msgstr "Verticale"
 
-#: widgets/waveform/waveform_widget.py:3165
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Horizontal"
 msgstr "Orizzontale"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3177
 msgid "Save"
 msgstr "Risparmiare"
 
-#: widgets/waveform/waveform_widget.py:3176
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Y-axis auto range"
 msgstr "Gamma automatica dell'asse Y"
 
-#: widgets/waveform/waveform_widget.py:3180
+#: widgets/waveform/waveform_widget.py:3186
 msgid "Copy image to clipboard"
 msgstr "Copia l'immagine negli appunti"
 
-#: widgets/waveform/waveform_widget.py:3181
+#: widgets/waveform/waveform_widget.py:3187
 msgid "Export visible data"
 msgstr "Esportazione di dati visibili"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3188
 msgid "Export all data"
 msgstr "Esportazione di tutti i dati"
 
-#: widgets/waveform/waveform_widget.py:3354
+#: widgets/waveform/waveform_widget.py:3360
 msgid "Export"
 msgstr "Esportazione"
 
-#: widgets/waveform/waveform_widget.py:3355
+#: widgets/waveform/waveform_widget.py:3361
 msgid "Analysis"
 msgstr "Analisi"
 
-#: widgets/waveform/waveform_widget.py:3363
+#: widgets/waveform/waveform_widget.py:3369
 msgid "Interval"
 msgstr "Intervallo"
 
-#: widgets/waveform/waveform_widget.py:3372
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Zoom"
 msgstr "Zoom"
 
-#: widgets/waveform/waveform_widget.py:3376
+#: widgets/waveform/waveform_widget.py:3382
 msgid "Show statistics"
 msgstr "Mostra le statistiche"
 
-#: widgets/waveform/waveform_widget.py:3381
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Left"
 msgstr "A sinistra"
 
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3390
 msgid "Right"
 msgstr "A destra"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3393
 msgid "Off"
 msgstr "Spento"
 
-#: widgets/waveform/waveform_widget.py:3390
-#: widgets/waveform/waveform_widget.py:3418
-#: widgets/waveform/waveform_widget.py:3448
+#: widgets/waveform/waveform_widget.py:3396
+#: widgets/waveform/waveform_widget.py:3424
+#: widgets/waveform/waveform_widget.py:3454
 msgid "Remove"
 msgstr "Rimuovere"
 
-#: widgets/waveform/waveform_widget.py:3401
+#: widgets/waveform/waveform_widget.py:3407
 msgid "Y mode"
 msgstr "Modalità Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "max"
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.8/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.8/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
 msgid "Email"
 msgstr "電子メール"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "商品概要"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
 msgid "Edit"
 msgstr "編集"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "マークダウンで表示"
 
@@ -1352,15 +1352,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3104
+#: widgets/waveform/waveform_widget.py:3110
 msgid "Name"
 msgstr "名称"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Joulescope ストリームバッファ"
 
@@ -2523,34 +2523,34 @@
 msgstr "トライアングルライト"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "左三角形"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3056
 msgid "Manual"
 msgstr "マニュアル"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "中心"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Text"
 msgstr "テキスト"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3398
+#: widgets/waveform/waveform_widget.py:3404
 msgid "Show text"
 msgstr "テキストを表示"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3410
+#: widgets/waveform/waveform_widget.py:3416
 msgid "Shape"
 msgstr "形状"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Yモード"
 
@@ -2856,20 +2856,20 @@
 msgstr "サマリーに表示する信号量。"
 
 #: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "X軸注釈モード"
 
 #: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2936
 msgid "Absolute"
 msgstr "絶対値"
 
 #: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2935
+#: widgets/waveform/waveform_widget.py:2941
 msgid "Relative"
 msgstr "相対"
 
 #: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "利用可能なサブソース"
 
@@ -2877,158 +2877,158 @@
 msgid "The selected subsources for each trace."
 msgstr "各トレースで選択されたサブソース。"
 
 #: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr "トレースの優先順位：最高 int 値が一番上、None はオフ。"
 
-#: widgets/waveform/waveform_widget.py:2877
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2883
+#: widgets/waveform/waveform_widget.py:3185
 msgid "Save image to file"
 msgstr "画像をファイルに保存"
 
-#: widgets/waveform/waveform_widget.py:2924
-#: widgets/waveform/waveform_widget.py:2993
+#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2999
 msgid "Single marker"
 msgstr "シングルマーカー"
 
-#: widgets/waveform/waveform_widget.py:2925
-#: widgets/waveform/waveform_widget.py:2994
+#: widgets/waveform/waveform_widget.py:2931
+#: widgets/waveform/waveform_widget.py:3000
 msgid "Dual markers"
 msgstr "デュアルマーカー"
 
-#: widgets/waveform/waveform_widget.py:2927
+#: widgets/waveform/waveform_widget.py:2933
 msgid "Mode"
 msgstr "モード"
 
-#: widgets/waveform/waveform_widget.py:2940
-#: widgets/waveform/waveform_widget.py:2995
-#: widgets/waveform/waveform_widget.py:3155
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:2946
+#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Clear all"
 msgstr "すべてクリア"
 
-#: widgets/waveform/waveform_widget.py:2951
-#: widgets/waveform/waveform_widget.py:3040
-#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:2957
+#: widgets/waveform/waveform_widget.py:3046
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Annotations"
 msgstr "注釈"
 
-#: widgets/waveform/waveform_widget.py:3043
+#: widgets/waveform/waveform_widget.py:3049
 msgid "Range"
 msgstr "測定範囲"
 
-#: widgets/waveform/waveform_widget.py:3047
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Auto"
 msgstr "オート"
 
-#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3059
 msgid "Exact"
 msgstr "正確"
 
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3068
 msgid "Scale"
 msgstr "スケール"
 
-#: widgets/waveform/waveform_widget.py:3065
+#: widgets/waveform/waveform_widget.py:3071
 msgid "Linear"
 msgstr "リニア"
 
-#: widgets/waveform/waveform_widget.py:3070
+#: widgets/waveform/waveform_widget.py:3076
 msgid "Logarithmic"
 msgstr "対数"
 
-#: widgets/waveform/waveform_widget.py:3078
+#: widgets/waveform/waveform_widget.py:3084
 msgid "Logarithmic zero"
 msgstr "対数ゼロ"
 
-#: widgets/waveform/waveform_widget.py:3092
+#: widgets/waveform/waveform_widget.py:3098
 msgid "Preferred prefix"
 msgstr "優先接頭辞"
 
-#: widgets/waveform/waveform_widget.py:3152
+#: widgets/waveform/waveform_widget.py:3158
 msgid "Add"
 msgstr "追加"
 
-#: widgets/waveform/waveform_widget.py:3153
+#: widgets/waveform/waveform_widget.py:3159
 msgid "Hide all text"
 msgstr "すべてのテキストを隠す"
 
-#: widgets/waveform/waveform_widget.py:3154
+#: widgets/waveform/waveform_widget.py:3160
 msgid "Show all text"
 msgstr "すべてのテキストを表示"
 
-#: widgets/waveform/waveform_widget.py:3162
+#: widgets/waveform/waveform_widget.py:3168
 msgid "Vertical"
 msgstr "垂直"
 
-#: widgets/waveform/waveform_widget.py:3165
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Horizontal"
 msgstr "水平"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3177
 msgid "Save"
 msgstr "節約"
 
-#: widgets/waveform/waveform_widget.py:3176
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Y-axis auto range"
 msgstr "Y軸オートレンジ"
 
-#: widgets/waveform/waveform_widget.py:3180
+#: widgets/waveform/waveform_widget.py:3186
 msgid "Copy image to clipboard"
 msgstr "画像をクリップボードにコピー"
 
-#: widgets/waveform/waveform_widget.py:3181
+#: widgets/waveform/waveform_widget.py:3187
 msgid "Export visible data"
 msgstr "可視データをエクスポート"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3188
 msgid "Export all data"
 msgstr "すべてのデータをエクスポート"
 
-#: widgets/waveform/waveform_widget.py:3354
+#: widgets/waveform/waveform_widget.py:3360
 msgid "Export"
 msgstr "輸出"
 
-#: widgets/waveform/waveform_widget.py:3355
+#: widgets/waveform/waveform_widget.py:3361
 msgid "Analysis"
 msgstr "解析"
 
-#: widgets/waveform/waveform_widget.py:3363
+#: widgets/waveform/waveform_widget.py:3369
 msgid "Interval"
 msgstr "インターバル"
 
-#: widgets/waveform/waveform_widget.py:3372
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Zoom"
 msgstr "ズーム"
 
-#: widgets/waveform/waveform_widget.py:3376
+#: widgets/waveform/waveform_widget.py:3382
 msgid "Show statistics"
 msgstr "統計を表示"
 
-#: widgets/waveform/waveform_widget.py:3381
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Left"
 msgstr "左"
 
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3390
 msgid "Right"
 msgstr "右"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3393
 msgid "Off"
 msgstr "オフ"
 
-#: widgets/waveform/waveform_widget.py:3390
-#: widgets/waveform/waveform_widget.py:3418
-#: widgets/waveform/waveform_widget.py:3448
+#: widgets/waveform/waveform_widget.py:3396
+#: widgets/waveform/waveform_widget.py:3424
+#: widgets/waveform/waveform_widget.py:3454
 msgid "Remove"
 msgstr "削除"
 
-#: widgets/waveform/waveform_widget.py:3401
+#: widgets/waveform/waveform_widget.py:3407
 msgid "Y mode"
 msgstr "Yモード"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "最大"
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/joulescope_ui.pot` & `joulescope_ui-1.1.8/joulescope_ui/locale/joulescope_ui.pot`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) 2024 Jetperch LLC
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: PROJECT 1.1.7\n"
+"Project-Id-Version: PROJECT 1.1.8\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -284,15 +284,15 @@
 msgid "Email"
 msgstr ""
 
 #: error_window.py:103
 msgid "Description"
 msgstr ""
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
 msgid "Edit"
 msgstr ""
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr ""
 
@@ -1308,15 +1308,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3104
+#: widgets/waveform/waveform_widget.py:3110
 msgid "Name"
 msgstr ""
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr ""
 
@@ -2460,34 +2460,34 @@
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3056
 msgid "Manual"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Text"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3398
+#: widgets/waveform/waveform_widget.py:3404
 msgid "Show text"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3410
+#: widgets/waveform/waveform_widget.py:3416
 msgid "Shape"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr ""
 
@@ -2792,20 +2792,20 @@
 msgstr ""
 
 #: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr ""
 
 #: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2936
 msgid "Absolute"
 msgstr ""
 
 #: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2935
+#: widgets/waveform/waveform_widget.py:2941
 msgid "Relative"
 msgstr ""
 
 #: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr ""
 
@@ -2813,158 +2813,158 @@
 msgid "The selected subsources for each trace."
 msgstr ""
 
 #: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2877
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2883
+#: widgets/waveform/waveform_widget.py:3185
 msgid "Save image to file"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2924
-#: widgets/waveform/waveform_widget.py:2993
+#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2999
 msgid "Single marker"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2925
-#: widgets/waveform/waveform_widget.py:2994
+#: widgets/waveform/waveform_widget.py:2931
+#: widgets/waveform/waveform_widget.py:3000
 msgid "Dual markers"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2927
+#: widgets/waveform/waveform_widget.py:2933
 msgid "Mode"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2940
-#: widgets/waveform/waveform_widget.py:2995
-#: widgets/waveform/waveform_widget.py:3155
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:2946
+#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Clear all"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2951
-#: widgets/waveform/waveform_widget.py:3040
-#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:2957
+#: widgets/waveform/waveform_widget.py:3046
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Annotations"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3043
+#: widgets/waveform/waveform_widget.py:3049
 msgid "Range"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3047
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Auto"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3059
 msgid "Exact"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3068
 msgid "Scale"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3065
+#: widgets/waveform/waveform_widget.py:3071
 msgid "Linear"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3070
+#: widgets/waveform/waveform_widget.py:3076
 msgid "Logarithmic"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3078
+#: widgets/waveform/waveform_widget.py:3084
 msgid "Logarithmic zero"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3092
+#: widgets/waveform/waveform_widget.py:3098
 msgid "Preferred prefix"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3152
+#: widgets/waveform/waveform_widget.py:3158
 msgid "Add"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3153
+#: widgets/waveform/waveform_widget.py:3159
 msgid "Hide all text"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3154
+#: widgets/waveform/waveform_widget.py:3160
 msgid "Show all text"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3162
+#: widgets/waveform/waveform_widget.py:3168
 msgid "Vertical"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3165
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Horizontal"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3177
 msgid "Save"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3176
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Y-axis auto range"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3180
+#: widgets/waveform/waveform_widget.py:3186
 msgid "Copy image to clipboard"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3181
+#: widgets/waveform/waveform_widget.py:3187
 msgid "Export visible data"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3188
 msgid "Export all data"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3354
+#: widgets/waveform/waveform_widget.py:3360
 msgid "Export"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3355
+#: widgets/waveform/waveform_widget.py:3361
 msgid "Analysis"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3363
+#: widgets/waveform/waveform_widget.py:3369
 msgid "Interval"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3372
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Zoom"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3376
+#: widgets/waveform/waveform_widget.py:3382
 msgid "Show statistics"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3381
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Left"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3390
 msgid "Right"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3393
 msgid "Off"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3390
-#: widgets/waveform/waveform_widget.py:3418
-#: widgets/waveform/waveform_widget.py:3448
+#: widgets/waveform/waveform_widget.py:3396
+#: widgets/waveform/waveform_widget.py:3424
+#: widgets/waveform/waveform_widget.py:3454
 msgid "Remove"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3401
+#: widgets/waveform/waveform_widget.py:3407
 msgid "Y mode"
 msgstr ""
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr ""
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.8/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.8/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 msgid "Email"
 msgstr "이메일"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "설명"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
 msgid "Edit"
 msgstr "Edit"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "마크다운으로 보기"
 
@@ -1373,15 +1373,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3104
+#: widgets/waveform/waveform_widget.py:3110
 msgid "Name"
 msgstr "이름"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "줄스코프 스트림 버퍼"
 
@@ -2548,34 +2548,34 @@
 msgstr "삼각형 오른쪽"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "왼쪽 삼각형"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3056
 msgid "Manual"
 msgstr "매뉴얼"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "중심"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Text"
 msgstr "텍스트"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3398
+#: widgets/waveform/waveform_widget.py:3404
 msgid "Show text"
 msgstr "텍스트 표시"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3410
+#: widgets/waveform/waveform_widget.py:3416
 msgid "Shape"
 msgstr "모양"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Y 모드"
 
@@ -2882,20 +2882,20 @@
 msgstr "요약에 표시할 신호 양입니다."
 
 #: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "X축 주석 모드"
 
 #: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2936
 msgid "Absolute"
 msgstr "절대"
 
 #: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2935
+#: widgets/waveform/waveform_widget.py:2941
 msgid "Relative"
 msgstr "상대"
 
 #: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "사용 가능한 하위 소스."
 
@@ -2903,158 +2903,158 @@
 msgid "The selected subsources for each trace."
 msgstr "각 트레이스에 대해 선택된 하위 소스."
 
 #: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr "트레이스 우선순위: 가장 높은 int 값이 위에 있고 없음은 꺼져 있습니다."
 
-#: widgets/waveform/waveform_widget.py:2877
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2883
+#: widgets/waveform/waveform_widget.py:3185
 msgid "Save image to file"
 msgstr "파일에 이미지 저장"
 
-#: widgets/waveform/waveform_widget.py:2924
-#: widgets/waveform/waveform_widget.py:2993
+#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2999
 msgid "Single marker"
 msgstr "단일 마커"
 
-#: widgets/waveform/waveform_widget.py:2925
-#: widgets/waveform/waveform_widget.py:2994
+#: widgets/waveform/waveform_widget.py:2931
+#: widgets/waveform/waveform_widget.py:3000
 msgid "Dual markers"
 msgstr "듀얼 마커"
 
-#: widgets/waveform/waveform_widget.py:2927
+#: widgets/waveform/waveform_widget.py:2933
 msgid "Mode"
 msgstr "모드"
 
-#: widgets/waveform/waveform_widget.py:2940
-#: widgets/waveform/waveform_widget.py:2995
-#: widgets/waveform/waveform_widget.py:3155
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:2946
+#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Clear all"
 msgstr "모두 지우기"
 
-#: widgets/waveform/waveform_widget.py:2951
-#: widgets/waveform/waveform_widget.py:3040
-#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:2957
+#: widgets/waveform/waveform_widget.py:3046
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Annotations"
 msgstr "주석"
 
-#: widgets/waveform/waveform_widget.py:3043
+#: widgets/waveform/waveform_widget.py:3049
 msgid "Range"
 msgstr "범위"
 
-#: widgets/waveform/waveform_widget.py:3047
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3059
 msgid "Exact"
 msgstr "정확한"
 
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3068
 msgid "Scale"
 msgstr "스케일"
 
-#: widgets/waveform/waveform_widget.py:3065
+#: widgets/waveform/waveform_widget.py:3071
 msgid "Linear"
 msgstr "선형"
 
-#: widgets/waveform/waveform_widget.py:3070
+#: widgets/waveform/waveform_widget.py:3076
 msgid "Logarithmic"
 msgstr "로그"
 
-#: widgets/waveform/waveform_widget.py:3078
+#: widgets/waveform/waveform_widget.py:3084
 msgid "Logarithmic zero"
 msgstr "로그 제로"
 
-#: widgets/waveform/waveform_widget.py:3092
+#: widgets/waveform/waveform_widget.py:3098
 msgid "Preferred prefix"
 msgstr "기본 접두사"
 
-#: widgets/waveform/waveform_widget.py:3152
+#: widgets/waveform/waveform_widget.py:3158
 msgid "Add"
 msgstr "추가"
 
-#: widgets/waveform/waveform_widget.py:3153
+#: widgets/waveform/waveform_widget.py:3159
 msgid "Hide all text"
 msgstr "모든 텍스트 숨기기"
 
-#: widgets/waveform/waveform_widget.py:3154
+#: widgets/waveform/waveform_widget.py:3160
 msgid "Show all text"
 msgstr "모든 텍스트 표시"
 
-#: widgets/waveform/waveform_widget.py:3162
+#: widgets/waveform/waveform_widget.py:3168
 msgid "Vertical"
 msgstr "수직"
 
-#: widgets/waveform/waveform_widget.py:3165
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Horizontal"
 msgstr "수평"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3177
 msgid "Save"
 msgstr "저장"
 
-#: widgets/waveform/waveform_widget.py:3176
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Y-axis auto range"
 msgstr "Y축 자동 범위"
 
-#: widgets/waveform/waveform_widget.py:3180
+#: widgets/waveform/waveform_widget.py:3186
 msgid "Copy image to clipboard"
 msgstr "이미지를 클립보드에 복사"
 
-#: widgets/waveform/waveform_widget.py:3181
+#: widgets/waveform/waveform_widget.py:3187
 msgid "Export visible data"
 msgstr "가시 데이터 내보내기"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3188
 msgid "Export all data"
 msgstr "모든 데이터 내보내기"
 
-#: widgets/waveform/waveform_widget.py:3354
+#: widgets/waveform/waveform_widget.py:3360
 msgid "Export"
 msgstr "Export"
 
-#: widgets/waveform/waveform_widget.py:3355
+#: widgets/waveform/waveform_widget.py:3361
 msgid "Analysis"
 msgstr "분석"
 
-#: widgets/waveform/waveform_widget.py:3363
+#: widgets/waveform/waveform_widget.py:3369
 msgid "Interval"
 msgstr "Interval"
 
-#: widgets/waveform/waveform_widget.py:3372
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Zoom"
 msgstr "줌"
 
-#: widgets/waveform/waveform_widget.py:3376
+#: widgets/waveform/waveform_widget.py:3382
 msgid "Show statistics"
 msgstr "통계 보기"
 
-#: widgets/waveform/waveform_widget.py:3381
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Left"
 msgstr "왼쪽"
 
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3390
 msgid "Right"
 msgstr "Right"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3393
 msgid "Off"
 msgstr "Off"
 
-#: widgets/waveform/waveform_widget.py:3390
-#: widgets/waveform/waveform_widget.py:3418
-#: widgets/waveform/waveform_widget.py:3448
+#: widgets/waveform/waveform_widget.py:3396
+#: widgets/waveform/waveform_widget.py:3424
+#: widgets/waveform/waveform_widget.py:3454
 msgid "Remove"
 msgstr "제거"
 
-#: widgets/waveform/waveform_widget.py:3401
+#: widgets/waveform/waveform_widget.py:3407
 msgid "Y mode"
 msgstr "Y 모드"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "최대"
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.8/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.8/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
 msgid "Email"
 msgstr "电子邮件"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "描述"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
 msgid "Edit"
 msgstr "编辑"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "以 Markdown 格式查看"
 
@@ -1322,15 +1322,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3104
+#: widgets/waveform/waveform_widget.py:3110
 msgid "Name"
 msgstr "名称"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Joulescope 数据流缓冲器"
 
@@ -2477,34 +2477,34 @@
 msgstr "右三角"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "左三角形"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3056
 msgid "Manual"
 msgstr "手册"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "居中"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Text"
 msgstr "文本"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3398
+#: widgets/waveform/waveform_widget.py:3404
 msgid "Show text"
 msgstr "显示文本"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3410
+#: widgets/waveform/waveform_widget.py:3416
 msgid "Shape"
 msgstr "形状"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Y 模式"
 
@@ -2809,20 +2809,20 @@
 msgstr "要在摘要中显示的信号量。"
 
 #: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "X 轴注释模式"
 
 #: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2936
 msgid "Absolute"
 msgstr "绝对值"
 
 #: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2935
+#: widgets/waveform/waveform_widget.py:2941
 msgid "Relative"
 msgstr "相对值"
 
 #: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "可用的子源。"
 
@@ -2830,158 +2830,158 @@
 msgid "The selected subsources for each trace."
 msgstr "每个跟踪所选的子源。"
 
 #: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr "跟踪优先级：最高 int 值在顶部，无则关闭。"
 
-#: widgets/waveform/waveform_widget.py:2877
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2883
+#: widgets/waveform/waveform_widget.py:3185
 msgid "Save image to file"
 msgstr "将图像保存到文件"
 
-#: widgets/waveform/waveform_widget.py:2924
-#: widgets/waveform/waveform_widget.py:2993
+#: widgets/waveform/waveform_widget.py:2930
+#: widgets/waveform/waveform_widget.py:2999
 msgid "Single marker"
 msgstr "单标记"
 
-#: widgets/waveform/waveform_widget.py:2925
-#: widgets/waveform/waveform_widget.py:2994
+#: widgets/waveform/waveform_widget.py:2931
+#: widgets/waveform/waveform_widget.py:3000
 msgid "Dual markers"
 msgstr "双标记"
 
-#: widgets/waveform/waveform_widget.py:2927
+#: widgets/waveform/waveform_widget.py:2933
 msgid "Mode"
 msgstr "模式"
 
-#: widgets/waveform/waveform_widget.py:2940
-#: widgets/waveform/waveform_widget.py:2995
-#: widgets/waveform/waveform_widget.py:3155
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:2946
+#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Clear all"
 msgstr "全部清除"
 
-#: widgets/waveform/waveform_widget.py:2951
-#: widgets/waveform/waveform_widget.py:3040
-#: widgets/waveform/waveform_widget.py:3161
+#: widgets/waveform/waveform_widget.py:2957
+#: widgets/waveform/waveform_widget.py:3046
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Annotations"
 msgstr "注释"
 
-#: widgets/waveform/waveform_widget.py:3043
+#: widgets/waveform/waveform_widget.py:3049
 msgid "Range"
 msgstr "范围"
 
-#: widgets/waveform/waveform_widget.py:3047
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Auto"
 msgstr "自动"
 
-#: widgets/waveform/waveform_widget.py:3053
+#: widgets/waveform/waveform_widget.py:3059
 msgid "Exact"
 msgstr "精确"
 
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3068
 msgid "Scale"
 msgstr "规模"
 
-#: widgets/waveform/waveform_widget.py:3065
+#: widgets/waveform/waveform_widget.py:3071
 msgid "Linear"
 msgstr "线性"
 
-#: widgets/waveform/waveform_widget.py:3070
+#: widgets/waveform/waveform_widget.py:3076
 msgid "Logarithmic"
 msgstr "对数"
 
-#: widgets/waveform/waveform_widget.py:3078
+#: widgets/waveform/waveform_widget.py:3084
 msgid "Logarithmic zero"
 msgstr "对数零"
 
-#: widgets/waveform/waveform_widget.py:3092
+#: widgets/waveform/waveform_widget.py:3098
 msgid "Preferred prefix"
 msgstr "首选前缀"
 
-#: widgets/waveform/waveform_widget.py:3152
+#: widgets/waveform/waveform_widget.py:3158
 msgid "Add"
 msgstr "添加"
 
-#: widgets/waveform/waveform_widget.py:3153
+#: widgets/waveform/waveform_widget.py:3159
 msgid "Hide all text"
 msgstr "隐藏所有文本"
 
-#: widgets/waveform/waveform_widget.py:3154
+#: widgets/waveform/waveform_widget.py:3160
 msgid "Show all text"
 msgstr "显示所有文本"
 
-#: widgets/waveform/waveform_widget.py:3162
+#: widgets/waveform/waveform_widget.py:3168
 msgid "Vertical"
 msgstr "垂直"
 
-#: widgets/waveform/waveform_widget.py:3165
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Horizontal"
 msgstr "水平"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3177
 msgid "Save"
 msgstr "保存"
 
-#: widgets/waveform/waveform_widget.py:3176
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Y-axis auto range"
 msgstr "Y 轴自动量程"
 
-#: widgets/waveform/waveform_widget.py:3180
+#: widgets/waveform/waveform_widget.py:3186
 msgid "Copy image to clipboard"
 msgstr "将图像复制到剪贴板"
 
-#: widgets/waveform/waveform_widget.py:3181
+#: widgets/waveform/waveform_widget.py:3187
 msgid "Export visible data"
 msgstr "导出可见数据"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3188
 msgid "Export all data"
 msgstr "导出所有数据"
 
-#: widgets/waveform/waveform_widget.py:3354
+#: widgets/waveform/waveform_widget.py:3360
 msgid "Export"
 msgstr "出口"
 
-#: widgets/waveform/waveform_widget.py:3355
+#: widgets/waveform/waveform_widget.py:3361
 msgid "Analysis"
 msgstr "分析"
 
-#: widgets/waveform/waveform_widget.py:3363
+#: widgets/waveform/waveform_widget.py:3369
 msgid "Interval"
 msgstr "间隔"
 
-#: widgets/waveform/waveform_widget.py:3372
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Zoom"
 msgstr "放大"
 
-#: widgets/waveform/waveform_widget.py:3376
+#: widgets/waveform/waveform_widget.py:3382
 msgid "Show statistics"
 msgstr "显示统计数据"
 
-#: widgets/waveform/waveform_widget.py:3381
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Left"
 msgstr "左侧"
 
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3390
 msgid "Right"
 msgstr "正确"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3393
 msgid "Off"
 msgstr "关闭"
 
-#: widgets/waveform/waveform_widget.py:3390
-#: widgets/waveform/waveform_widget.py:3418
-#: widgets/waveform/waveform_widget.py:3448
+#: widgets/waveform/waveform_widget.py:3396
+#: widgets/waveform/waveform_widget.py:3424
+#: widgets/waveform/waveform_widget.py:3454
 msgid "Remove"
 msgstr "删除"
 
-#: widgets/waveform/waveform_widget.py:3401
+#: widgets/waveform/waveform_widget.py:3407
 msgid "Y mode"
 msgstr "Y 模式"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "最大值"
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/logging_util.py` & `joulescope_ui-1.1.8/joulescope_ui/logging_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/main.py` & `joulescope_ui-1.1.8/joulescope_ui/main.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/mem_leak_debugger.py` & `joulescope_ui-1.1.8/joulescope_ui/mem_leak_debugger.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/metadata.py` & `joulescope_ui-1.1.8/joulescope_ui/metadata.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/paths.py` & `joulescope_ui-1.1.8/joulescope_ui/paths.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/plugins/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/plugins/manager.py` & `joulescope_ui-1.1.8/joulescope_ui/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/plugins/selector.py` & `joulescope_ui-1.1.8/joulescope_ui/plugins/selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p1/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p1/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/plugins/test/test_manager.py` & `joulescope_ui-1.1.8/joulescope_ui/plugins/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/process_monitor.py` & `joulescope_ui-1.1.8/joulescope_ui/process_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/profile.py` & `joulescope_ui-1.1.8/joulescope_ui/profile.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/pubsub.py` & `joulescope_ui-1.1.8/joulescope_ui/pubsub.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/pubsub_aggregator.py` & `joulescope_ui-1.1.8/joulescope_ui/pubsub_aggregator.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/pubsub_callable.py` & `joulescope_ui-1.1.8/joulescope_ui/pubsub_callable.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/pubsub_proxy.py` & `joulescope_ui-1.1.8/joulescope_ui/pubsub_proxy.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/range_tool.py` & `joulescope_ui-1.1.8/joulescope_ui/range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/range_tools/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/range_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/range_tools/cdf.py` & `joulescope_ui-1.1.8/joulescope_ui/range_tools/cdf.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/range_tools/frequency.py` & `joulescope_ui-1.1.8/joulescope_ui/range_tools/frequency.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/range_tools/histogram.py` & `joulescope_ui-1.1.8/joulescope_ui/range_tools/histogram.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/range_tools/max_window.py` & `joulescope_ui-1.1.8/joulescope_ui/range_tools/max_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/range_tools/plugin_helpers.py` & `joulescope_ui-1.1.8/joulescope_ui/range_tools/plugin_helpers.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/range_tools/usb_inrush.py` & `joulescope_ui-1.1.8/joulescope_ui/range_tools/usb_inrush.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/reporter.py` & `joulescope_ui-1.1.8/joulescope_ui/reporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/dmg_background.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/dmg_background.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/dmg_background.svg` & `joulescope_ui-1.1.8/joulescope_ui/resources/dmg_background.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/dmg_background@2x.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/dmg_background@2x.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/icon.ico` & `joulescope_ui-1.1.8/joulescope_ui/resources/icon.ico`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_128x128.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_128x128@2.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_128x128@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_16x16@2.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_16x16@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_256x256.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_256x256@2.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_256x256@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_32x32.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_32x32@2.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_32x32@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_512x512.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_512x512@2.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_512x512@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_64x64.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_64x64@2.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_64x64@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/icons.svg` & `joulescope_ui-1.1.8/joulescope_ui/resources/icons.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/logo-large.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/logo-large.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/logo-small.png` & `joulescope_ui-1.1.8/joulescope_ui/resources/logo-small.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources/zoom.svg` & `joulescope_ui-1.1.8/joulescope_ui/resources/zoom.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources.py` & `joulescope_ui-1.1.8/joulescope_ui/resources.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/resources.rcc` & `joulescope_ui-1.1.8/joulescope_ui/resources.rcc`

 * *Files 1% similar despite different names*

```diff
@@ -1416,11 +1416,11 @@
 00005870: 5f00 3600 3400 7800 3600 3400 2e00 6900  _.6.4.x.6.4...i.
 00005880: 6300 6f00 0e03 14ce 8700 6c00 6f00 6700  c.o.......l.o.g.
 00005890: 6f00 2d00 6c00 6100 7200 6700 6500 2e00  o.-.l.a.r.g.e...
 000058a0: 7000 6e00 6700 0e0f ebc7 e700 6c00 6f00  p.n.g.......l.o.
 000058b0: 6700 6f00 2d00 7300 6d00 6100 6c00 6c00  g.o.-.s.m.a.l.l.
 000058c0: 2e00 7000 6e00 6700 0000 0000 0200 0000  ..p.n.g.........
 000058d0: 0300 0000 0100 0000 0000 0000 0000 0000  ................
-000058e0: 2200 0000 0000 0100 0001 9900 0001 8f68  "..............h
-000058f0: 00b7 6600 0000 0000 0400 0000 0100 0000  ..f.............
-00005900: 0000 0001 8f68 00b7 6600 0000 4400 0000  .....h..f...D...
-00005910: 0000 0100 0043 f800 0001 8f68 00b7 66    .....C.....h..f
+000058e0: 2200 0000 0000 0100 0001 9900 0001 8f72  "..............r
+000058f0: 9b30 1500 0000 0000 0400 0000 0100 0000  .0..............
+00005900: 0000 0001 8f72 9b30 1500 0000 4400 0000  .....r.0....D...
+00005910: 0000 0100 0043 f800 0001 8f72 9b30 15    .....C.....r.0.
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/safe_mode.py` & `joulescope_ui-1.1.8/joulescope_ui/safe_mode.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/sanitize.py` & `joulescope_ui-1.1.8/joulescope_ui/sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/shift_key.py` & `joulescope_ui-1.1.8/joulescope_ui/shift_key.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/software_update.py` & `joulescope_ui-1.1.8/joulescope_ui/software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/source_selector.py` & `joulescope_ui-1.1.8/joulescope_ui/source_selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/README.md` & `joulescope_ui-1.1.8/joulescope_ui/styles/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/color_editor.py` & `joulescope_ui-1.1.8/joulescope_ui/styles/color_editor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/color_file.py` & `joulescope_ui-1.1.8/joulescope_ui/styles/color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/color_picker.py` & `joulescope_ui-1.1.8/joulescope_ui/styles/color_picker.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/color_scheme.py` & `joulescope_ui-1.1.8/joulescope_ui/styles/color_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.8/joulescope_ui/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/color_scheme_light.txt` & `joulescope_ui-1.1.8/joulescope_ui/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/font_scheme.py` & `joulescope_ui-1.1.8/joulescope_ui/styles/font_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/fonts.py` & `joulescope_ui-1.1.8/joulescope_ui/styles/fonts.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/js1/detach.svg` & `joulescope_ui-1.1.8/joulescope_ui/styles/js1/detach.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/js1/index.json` & `joulescope_ui-1.1.8/joulescope_ui/styles/js1/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/js1/style.qss` & `joulescope_ui-1.1.8/joulescope_ui/styles/js1/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/js1/vmovetoolbar.svg` & `joulescope_ui-1.1.8/joulescope_ui/styles/js1/vmovetoolbar.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/js1/vsepartoolbars.svg` & `joulescope_ui-1.1.8/joulescope_ui/styles/js1/vsepartoolbars.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/manager.py` & `joulescope_ui-1.1.8/joulescope_ui/styles/manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/parameter_file.py` & `joulescope_ui-1.1.8/joulescope_ui/styles/parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/system/style.qss` & `joulescope_ui-1.1.8/joulescope_ui/styles/system/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/system/zoom_all.svg` & `joulescope_ui-1.1.8/joulescope_ui/styles/system/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/test/test_color_file.py` & `joulescope_ui-1.1.8/joulescope_ui/styles/test/test_color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/test/test_manager.py` & `joulescope_ui-1.1.8/joulescope_ui/styles/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/styles/test/test_parameter_file.py` & `joulescope_ui-1.1.8/joulescope_ui/styles/test/test_parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/anno1.anno.jls` & `joulescope_ui-1.1.8/joulescope_ui/test/anno1.anno.jls`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_annotation_load.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_annotation_load.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_capabilities.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_disk_monitor.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_disk_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_metadata.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_pubsub.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_pubsub_aggregator.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_pubsub_aggregator.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_pubsub_registry.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_pubsub_registry.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_range_tool.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_reporter.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_reporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_sanitize.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_software_update.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_source_selector.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_source_selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_time_map.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_tooltip.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_units.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_units.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/test/test_versioned_file.py` & `joulescope_ui-1.1.8/joulescope_ui/test/test_versioned_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/time_map.py` & `joulescope_ui-1.1.8/joulescope_ui/time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/tokens.py` & `joulescope_ui-1.1.8/joulescope_ui/tokens.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/tooltip.py` & `joulescope_ui-1.1.8/joulescope_ui/tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/ui_util.py` & `joulescope_ui-1.1.8/joulescope_ui/ui_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/units.py` & `joulescope_ui-1.1.8/joulescope_ui/units.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/urls.py` & `joulescope_ui-1.1.8/joulescope_ui/urls.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/versioned_file.py` & `joulescope_ui-1.1.8/joulescope_ui/versioned_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/view.py` & `joulescope_ui-1.1.8/joulescope_ui/view.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widget_tools.py` & `joulescope_ui-1.1.8/joulescope_ui/widget_tools.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/accumulator_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/accumulator_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/style.qss` & `joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/clock/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/clock/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/clock/clock_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/clock/clock_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/developer/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/developer/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/developer/log_view_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/developer/log_view_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/developer/profile_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/developer/profile_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/developer/publish_spy_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/developer/publish_spy_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/developer/pubsub_explorer_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/developer/pubsub_explorer_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/current_limits.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/current_limits.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/device_control_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/device_control_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/device_info_dialog.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/device_info_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/device_update_dialog.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/device_update_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/fuse.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/fuse.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/js220_ctrl_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/js220_ctrl_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/device_open.svg` & `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/device_open.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg` & `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/fuse_normal.svg` & `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/fuse_normal.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/index.json` & `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/info.svg` & `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/info.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/style.qss` & `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/double_slider.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/double_slider.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/draggable_list_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/draggable_list_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/example/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/example/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/example/example_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/example/example_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/flyout_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/flyout_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/styles/style.qss` & `joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/hamburger/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/hamburger/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/hamburger/hamburger_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/hamburger/hamburger_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/help/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/help/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/help/help_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/help/help_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/jls_info/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/jls_info/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/jls_info/jls_info_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/jls_info/jls_info_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/current_offset.png` & `joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/current_offset.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/js220_cal_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/js220_cal_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/voltage_offset.png` & `joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/voltage_offset.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/memory/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/memory/memory_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/memory/memory_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/memory/styles/style.qss` & `joulescope_ui-1.1.8/joulescope_ui/widgets/memory/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/notes/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/notes/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/notes/notes_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/notes/notes_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/progress_bar/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/progress_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/progress_bar/progress_bar_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/progress_bar/progress_bar_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/record_status_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/record_status_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/index.json` & `joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/style.qss` & `joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/report_issue/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/report_issue/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/report_issue/report_issue_dialog.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/report_issue/report_issue_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/settings/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/settings/settings_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/settings/settings_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/settings/unique_strings_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/settings/unique_strings_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/sidebar_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/sidebar_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt` & `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg` & `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg` & `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/index.json` & `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/style.qss` & `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/disk_full_dialog.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/disk_full_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/signal_record.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/signal_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/signal_record_config_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/signal_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/statistics_record.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/statistics_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/switch.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/condition_detector.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/condition_detector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/continuous.svg` & `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/continuous.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/index.json` & `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/searching.svg` & `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/searching.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/style.qss` & `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/test_const.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/test_const.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/test_duration.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/test_duration.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/test_edge.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/test_edge.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/trigger_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/trigger_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/value/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/value/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/value/value_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/value/value_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/style.qss` & `joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/view_manager_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/view_manager_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/__init__.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/annotations.md` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/annotations.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/axis_ticks.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/axis_ticks.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/interval_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/interval_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/line_segments.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/line_segments.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/quantities.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/quantities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/index.json` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/style.qss` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/zoom_all.svg` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/test/test_axis_ticks.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/test/test_axis_ticks.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/test/test_quantities.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/test/test_quantities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/text_annotation.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/text_annotation.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/waveform_control.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/waveform_control.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/waveform_source_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/waveform_source_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/waveform_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/waveform_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -806,47 +806,49 @@
         self.pubsub.subscribe('registry_manager/capabilities/signal_buffer.source/list',
                               self._on_source_list, ['pub', 'retain'])
         topic = get_topic_name(self)
         self._control.on_pubsub_register(self.pubsub, topic, source_filter)
         self.pubsub.subscribe('registry/app/settings/units', self._update_on_publish, ['pub'])
         self.pubsub.subscribe('registry/app/settings/defaults/signal_buffer_source',
                               self._on_default_signal_buffer_source, ['pub', 'retain'])
-
-        NoMod = QtCore.Qt.KeyboardModifier.NoModifier
-        self._keymap = {
-            (QtCore.Qt.Key_Asterisk, NoMod): (f'{self.topic}/actions/!x_zoom_all', None),
-            (QtCore.Qt.Key_Left, NoMod): (f'{self.topic}/actions/!x_pan', -1),
-            (QtCore.Qt.Key_Right, NoMod): (f'{self.topic}/actions/!x_pan', 1),
-            (QtCore.Qt.Key_Up, NoMod): (f'{self.topic}/actions/!x_zoom', [1, None]),
-            (QtCore.Qt.Key_Down, NoMod): (f'{self.topic}/actions/!x_zoom', [-1, None]),
-            (QtCore.Qt.Key_Plus, NoMod): (f'{self.topic}/actions/!x_zoom', [1, None]),
-            (QtCore.Qt.Key_Minus, NoMod): (f'{self.topic}/actions/!x_zoom', [-1, None]),
-            (QtCore.Qt.Key_Delete, NoMod): (f'{self.topic}/actions/!annotations', ['clear_all']),
-            (QtCore.Qt.Key_Backspace, NoMod): (f'{self.topic}/actions/!annotations', ['clear_all']),
-            (QtCore.Qt.Key_A, QtCore.Qt.KeyboardModifier.ControlModifier):
-                (f'{self.topic}/actions/!viewport', ['pinned']),
-            (QtCore.Qt.Key_D, NoMod): (f'{self.topic}/actions/!x_markers', 'add_dual'),
-            (QtCore.Qt.Key_S, NoMod): (f'{self.topic}/actions/!x_markers', 'add_single'),
-            (QtCore.Qt.Key_1, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 0]),
-            (QtCore.Qt.Key_2, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 1]),
-            (QtCore.Qt.Key_3, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 2]),
-            (QtCore.Qt.Key_4, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 3]),
-            (QtCore.Qt.Key_5, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 4]),
-            (QtCore.Qt.Key_6, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 5]),
-            (QtCore.Qt.Key_7, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 6]),
-            (QtCore.Qt.Key_8, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 7]),
-            (QtCore.Qt.Key_9, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 8]),
-            (QtCore.Qt.Key_Space, QtCore.Qt.KeyboardModifier.ShiftModifier):
-                (f'{self.topic}/actions/!viewport', ['toggle']),
-        }
-
+        self._keymap_load()
         self._repaint_request = True
         self._paint_state = PaintState.READY
         self._paint_timer.start(1)
 
+    def _keymap_load(self):
+        _any = None
+        _no = QtCore.Qt.KeyboardModifier.NoModifier
+        shift = QtCore.Qt.KeyboardModifier.ShiftModifier
+        ctrl = QtCore.Qt.KeyboardModifier.ControlModifier
+        self._keymap = {
+            (QtCore.Qt.Key_Asterisk, _any): (f'{self.topic}/actions/!x_zoom_all', None),
+            (QtCore.Qt.Key_Left, _any): (f'{self.topic}/actions/!x_pan', -1),
+            (QtCore.Qt.Key_Right, _any): (f'{self.topic}/actions/!x_pan', 1),
+            (QtCore.Qt.Key_Up, _any): (f'{self.topic}/actions/!x_zoom', [1, -1]),
+            (QtCore.Qt.Key_Down, _any): (f'{self.topic}/actions/!x_zoom', [-1, -1]),
+            (QtCore.Qt.Key_Plus, _any): (f'{self.topic}/actions/!x_zoom', [1, -1]),
+            (QtCore.Qt.Key_Minus, _any): (f'{self.topic}/actions/!x_zoom', [-1, -1]),
+            (QtCore.Qt.Key_Delete, _no): (f'{self.topic}/actions/!annotations', ['clear_all']),
+            (QtCore.Qt.Key_Backspace, _no): (f'{self.topic}/actions/!annotations', ['clear_all']),
+            (QtCore.Qt.Key_A, ctrl): (f'{self.topic}/actions/!viewport', ['pinned']),
+            (QtCore.Qt.Key_D, _no): (f'{self.topic}/actions/!x_markers', ['add_dual', -1, None]),
+            (QtCore.Qt.Key_S, _no): (f'{self.topic}/actions/!x_markers', ['add_single', -1]),
+            (QtCore.Qt.Key_1, _no): (f'{self.topic}/actions/!x_markers', ['select', 0]),
+            (QtCore.Qt.Key_2, _no): (f'{self.topic}/actions/!x_markers', ['select', 1]),
+            (QtCore.Qt.Key_3, _no): (f'{self.topic}/actions/!x_markers', ['select', 2]),
+            (QtCore.Qt.Key_4, _no): (f'{self.topic}/actions/!x_markers', ['select', 3]),
+            (QtCore.Qt.Key_5, _no): (f'{self.topic}/actions/!x_markers', ['select', 4]),
+            (QtCore.Qt.Key_6, _no): (f'{self.topic}/actions/!x_markers', ['select', 5]),
+            (QtCore.Qt.Key_7, _no): (f'{self.topic}/actions/!x_markers', ['select', 6]),
+            (QtCore.Qt.Key_8, _no): (f'{self.topic}/actions/!x_markers', ['select', 7]),
+            (QtCore.Qt.Key_9, _no): (f'{self.topic}/actions/!x_markers', ['select', 8]),
+            (QtCore.Qt.Key_Space, shift): (f'{self.topic}/actions/!viewport', ['toggle']),
+        }
+
     def on_action_viewport(self, topic, value):
         cmd = value[0]
         t1 = f'{self.topic}/settings/pin_right'
         t2 = f'{self.topic}/settings/pin_left'
         v1 = self.pubsub.query(t1)
         v2 = self.pubsub.query(t2)
         if cmd == 'toggle':
@@ -866,20 +868,24 @@
         self._repaint_request = True
 
     def _on_default_signal_buffer_source(self, value):
         self._default_source = value
         self._repaint_request = True
 
     def keyPressEvent(self, event: QtGui.QKeyEvent):
-        v = self._keymap.get((event.key(), event.modifiers()))
+        key, modifiers = event.key(), event.modifiers()
+        v = self._keymap.get((key, modifiers))
         if v is None:
-            super().keyPressEvent(event)
-        else:
-            self._log.info(f'key {event.key()} -> publish {v}')
-            self.pubsub.publish(*v)
+            v = self._keymap.get((key, None))
+            if v is None:
+                self._log.info(f'key {(key, modifiers)} unhandled')
+                super().keyPressEvent(event)
+                return
+        self._log.info(f'key {(key, modifiers)} -> publish {v}')
+        self.pubsub.publish(*v)
 
     def on_pubsub_unregister(self):
         self._paint_timer.stop()
         self._paint_state = PaintState.IDLE
 
     def on_pubsub_delete(self):
         for topic, value in self.pubsub.query(f'{self.topic}/settings/close_actions', default=[]):
@@ -3510,17 +3516,23 @@
             marker = self.annotations['x'].pop(marker['id'])
             return marker
         else:
             raise ValueError('unsupported remove')
 
     def _x_marker_add_single(self, pos1=None):
         x0, x1 = self.x_range
+        if pos1 < 0:
+            if self._mouse_pos is not None:
+                pos1 = self._x_map.counter_to_time64(self._mouse_pos[0])
+            else:
+                pos1 = None
         if pos1 is None:
             xc = (x1 + x0) // 2
             pos1 = self._x_marker_position(xc)
+        pos1 = max(x0, min(x1, pos1))
         marker = {
             'id': self._annotation_next_id('x'),
             'dtype': 'single',
             'mode': self.x_axis_annotation_mode,
             'pos1': pos1,
             'changed': True,
             'text_pos1': 'auto',
@@ -3528,25 +3540,37 @@
         }
         if self.x_axis_annotation_mode == 'relative':
             marker['mode'] = 'relative'
             marker['rel1'] = pos1 - self._extents()[1]
         return self._x_marker_add(marker)
 
     def _x_marker_add_dual(self, pos1=None, pos2=None):
+        xc = None
         x0, x1 = self.x_range
         if pos1 is not None and pos2 is None:
-            xc = pos1
+            if pos1 < 0:
+                if self._mouse_pos is not None:
+                    xc = self._x_map.counter_to_time64(self._mouse_pos[0])
+            else:
+                xc = pos1
             pos1 = None
-        else:
+        if xc is None:
             xc = (x1 + x0) // 2
         xd = (x1 - x0) // 10
         if pos1 is None:
             pos1 = self._x_marker_position(xc - xd)
         if pos2 is None:
             pos2 = self._x_marker_position(xc + xd)
+        d0, d1 = pos1 - x0, pos2 - x1
+        if d0 < 0:
+            pos1 -= d0
+            pos2 -= d0
+        elif d1 > 0:
+            pos1 -= d1
+            pos2 -= d1
         marker = {
             'id': self._annotation_next_id('x'),
             'dtype': 'dual',
             'mode': self.x_axis_annotation_mode,
             'pos1': pos1,
             'pos2': pos2,
             'changed': True,
@@ -3969,14 +3993,19 @@
         x0, x1 = self.x_range
         d_e = e1 - e0
         d_x = x1 - x0
         if d_e <= 0:
             return
         elif d_x <= 0:
             d_x = d_e
+        if center is not None and center < 0:
+            if self._mouse_pos is not None:
+                center = self._x_map.counter_to_time64(self._mouse_pos[0])
+            else:
+                center = None
         if center is None:
             center = (x1 + x0) // 2
         elif isinstance(center, float):
             raise ValueError(f'center is not int: {type(center)} {center}')
         center = int(center)
         center = max(x0, min(center, x1))
         f = (center - x0) / d_x
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/y_range_widget.py` & `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/y_range_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui/zip_inspector.py` & `joulescope_ui-1.1.8/joulescope_ui/zip_inspector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/joulescope_ui.egg-info/PKG-INFO` & `joulescope_ui-1.1.8/joulescope_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope_ui
-Version: 1.1.7
+Version: 1.1.8
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope_ui-1.1.7/joulescope_ui.egg-info/SOURCES.txt` & `joulescope_ui-1.1.8/joulescope_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/pyproject.toml` & `joulescope_ui-1.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.7/setup.py` & `joulescope_ui-1.1.8/setup.py`

 * *Files identical despite different names*

