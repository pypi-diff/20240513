# Comparing `tmp/wwdtm-2.9.0.tar.gz` & `tmp/wwdtm-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwdtm-2.9.0.tar", last modified: Sun Apr 21 03:50:55 2024, max compression
+gzip compressed data, was "wwdtm-2.9.1.tar", last modified: Sun Apr 21 23:12:50 2024, max compression
```

## Comparing `wwdtm-2.9.0.tar` & `wwdtm-2.9.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.591853 wwdtm-2.9.0/
--rw-r--r--   0 lpham      (501) staff       (20)    10142 2021-10-14 22:42:34.000000 wwdtm-2.9.0/LICENSE
--rw-r--r--   0 lpham      (501) staff       (20)      267 2022-01-03 00:36:38.000000 wwdtm-2.9.0/MANIFEST.in
--rw-r--r--   0 lpham      (501) staff       (20)     4484 2024-04-21 03:50:55.591563 wwdtm-2.9.0/PKG-INFO
--rw-r--r--   0 lpham      (501) staff       (20)     3497 2024-01-01 01:43:35.000000 wwdtm-2.9.0/README.rst
--rw-r--r--   0 lpham      (501) staff       (20)      344 2022-03-17 03:36:18.000000 wwdtm-2.9.0/config.json.dist
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.574139 wwdtm-2.9.0/docs/
--rw-r--r--   0 lpham      (501) staff       (20)      686 2021-10-14 22:42:34.000000 wwdtm-2.9.0/docs/Makefile
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.564229 wwdtm-2.9.0/docs/_static/
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.574317 wwdtm-2.9.0/docs/_static/css/
--rw-r--r--   0 lpham      (501) staff       (20)     1575 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/_static/css/custom.css
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.574552 wwdtm-2.9.0/docs/_templates/
--rw-r--r--   0 lpham      (501) staff       (20)      193 2021-10-14 22:42:34.000000 wwdtm-2.9.0/docs/_templates/layout.html
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.574949 wwdtm-2.9.0/docs/changes/
--rw-r--r--   0 lpham      (501) staff       (20)    10676 2024-04-21 03:50:14.000000 wwdtm-2.9.0/docs/changes/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)     1752 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/conf.py
--rw-r--r--   0 lpham      (501) staff       (20)      223 2024-01-01 01:43:35.000000 wwdtm-2.9.0/docs/environment.yaml
--rw-r--r--   0 lpham      (501) staff       (20)     1243 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2927 2022-11-13 00:18:03.000000 wwdtm-2.9.0/docs/known_issues.rst
--rw-r--r--   0 lpham      (501) staff       (20)      795 2021-10-14 22:42:34.000000 wwdtm-2.9.0/docs/make.bat
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.576699 wwdtm-2.9.0/docs/migrating/
--rw-r--r--   0 lpham      (501) staff       (20)     1886 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/migrating/guest.rst
--rw-r--r--   0 lpham      (501) staff       (20)     1854 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/migrating/host.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2821 2024-01-01 01:43:35.000000 wwdtm-2.9.0/docs/migrating/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2320 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/migrating/location.rst
--rw-r--r--   0 lpham      (501) staff       (20)     3802 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/migrating/panelist.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2050 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/migrating/scorekeeper.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2572 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/migrating/show.rst
--rw-r--r--   0 lpham      (501) staff       (20)      260 2024-04-21 03:50:14.000000 wwdtm-2.9.0/docs/requirements.txt
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.578363 wwdtm-2.9.0/docs/tests/
--rw-r--r--   0 lpham      (501) staff       (20)      631 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/tests/guest.rst
--rw-r--r--   0 lpham      (501) staff       (20)      608 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/tests/host.rst
--rw-r--r--   0 lpham      (501) staff       (20)      312 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/tests/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)      704 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/tests/location.rst
--rw-r--r--   0 lpham      (501) staff       (20)     1064 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/tests/panelist.rst
--rw-r--r--   0 lpham      (501) staff       (20)      783 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/tests/scorekeeper.rst
--rw-r--r--   0 lpham      (501) staff       (20)      757 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/tests/show.rst
--rw-r--r--   0 lpham      (501) staff       (20)      287 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/tests/validation.rst
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.579959 wwdtm-2.9.0/docs/wwdtm/
--rw-r--r--   0 lpham      (501) staff       (20)      562 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/guest.rst
--rw-r--r--   0 lpham      (501) staff       (20)      579 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/host.rst
--rw-r--r--   0 lpham      (501) staff       (20)      435 2022-03-17 03:36:18.000000 wwdtm-2.9.0/docs/wwdtm/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)      664 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/location.rst
--rw-r--r--   0 lpham      (501) staff       (20)     1034 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/panelist.rst
--rw-r--r--   0 lpham      (501) staff       (20)      712 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/scorekeeper.rst
--rw-r--r--   0 lpham      (501) staff       (20)      676 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/show.rst
--rw-r--r--   0 lpham      (501) staff       (20)      219 2024-01-12 18:49:15.000000 wwdtm-2.9.0/docs/wwdtm/validation.rst
--rw-r--r--   0 lpham      (501) staff       (20)     3004 2024-04-21 03:50:14.000000 wwdtm-2.9.0/pyproject.toml
--rw-r--r--   0 lpham      (501) staff       (20)       38 2024-04-21 03:50:55.591908 wwdtm-2.9.0/setup.cfg
--rw-r--r--   0 lpham      (501) staff       (20)      255 2024-01-12 18:49:15.000000 wwdtm-2.9.0/setup.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.580167 wwdtm-2.9.0/tests/
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.581012 wwdtm-2.9.0/tests/guest/
--rw-r--r--   0 lpham      (501) staff       (20)     2008 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/guest/test_guest_appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     4192 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/guest/test_guest_guest.py
--rw-r--r--   0 lpham      (501) staff       (20)     4536 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/guest/test_guest_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.581507 wwdtm-2.9.0/tests/host/
--rw-r--r--   0 lpham      (501) staff       (20)     1999 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/host/test_host_appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     5174 2024-04-21 03:50:14.000000 wwdtm-2.9.0/tests/host/test_host_host.py
--rw-r--r--   0 lpham      (501) staff       (20)     4346 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/host/test_host_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.581993 wwdtm-2.9.0/tests/location/
--rw-r--r--   0 lpham      (501) staff       (20)     5395 2024-04-21 03:50:14.000000 wwdtm-2.9.0/tests/location/test_location_location.py
--rw-r--r--   0 lpham      (501) staff       (20)     2112 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/location/test_location_recordings.py
--rw-r--r--   0 lpham      (501) staff       (20)     8722 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/location/test_location_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.582987 wwdtm-2.9.0/tests/panelist/
--rw-r--r--   0 lpham      (501) staff       (20)     4016 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/panelist/test_panelist_appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     6795 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/panelist/test_panelist_decimal_scores.py
--rw-r--r--   0 lpham      (501) staff       (20)     6377 2024-04-21 03:50:14.000000 wwdtm-2.9.0/tests/panelist/test_panelist_panelist.py
--rw-r--r--   0 lpham      (501) staff       (20)     6641 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/panelist/test_panelist_scores.py
--rw-r--r--   0 lpham      (501) staff       (20)     5183 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/panelist/test_panelist_statistics.py
--rw-r--r--   0 lpham      (501) staff       (20)     4688 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/panelist/test_panelist_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.583490 wwdtm-2.9.0/tests/scorekeeper/
--rw-r--r--   0 lpham      (501) staff       (20)     2236 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/scorekeeper/test_scorekeeper_appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     6074 2024-04-21 03:50:14.000000 wwdtm-2.9.0/tests/scorekeeper/test_scorekeeper_scorekeeper.py
--rw-r--r--   0 lpham      (501) staff       (20)     5122 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/scorekeeper/test_scorekeeper_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.584133 wwdtm-2.9.0/tests/show/
--rw-r--r--   0 lpham      (501) staff       (20)     4204 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/show/test_show_info.py
--rw-r--r--   0 lpham      (501) staff       (20)     9501 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/show/test_show_info_multiple.py
--rw-r--r--   0 lpham      (501) staff       (20)    15332 2024-02-12 01:12:44.000000 wwdtm-2.9.0/tests/show/test_show_show.py
--rw-r--r--   0 lpham      (501) staff       (20)     5144 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/show/test_show_utility.py
--rw-r--r--   0 lpham      (501) staff       (20)      848 2024-01-12 18:49:15.000000 wwdtm-2.9.0/tests/test_validation.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.584559 wwdtm-2.9.0/wwdtm/
--rw-r--r--   0 lpham      (501) staff       (20)      792 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/__init__.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.585996 wwdtm-2.9.0/wwdtm/guest/
--rw-r--r--   0 lpham      (501) staff       (20)      317 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/guest/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)     4814 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/guest/appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     7500 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/guest/guest.py
--rw-r--r--   0 lpham      (501) staff       (20)     4162 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/guest/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.586823 wwdtm-2.9.0/wwdtm/host/
--rw-r--r--   0 lpham      (501) staff       (20)      312 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/host/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)     4488 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/host/appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     7745 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/host/host.py
--rw-r--r--   0 lpham      (501) staff       (20)     4133 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/host/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.587648 wwdtm-2.9.0/wwdtm/location/
--rw-r--r--   0 lpham      (501) staff       (20)      330 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/location/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)    10282 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/location/location.py
--rw-r--r--   0 lpham      (501) staff       (20)     4460 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/location/recordings.py
--rw-r--r--   0 lpham      (501) staff       (20)     5472 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/location/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.589105 wwdtm-2.9.0/wwdtm/panelist/
--rw-r--r--   0 lpham      (501) staff       (20)      460 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/panelist/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)    10466 2024-03-21 02:45:32.000000 wwdtm-2.9.0/wwdtm/panelist/appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)    11473 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/panelist/decimal_scores.py
--rw-r--r--   0 lpham      (501) staff       (20)     9765 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/panelist/panelist.py
--rw-r--r--   0 lpham      (501) staff       (20)    10553 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/panelist/scores.py
--rw-r--r--   0 lpham      (501) staff       (20)    10132 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/panelist/statistics.py
--rw-r--r--   0 lpham      (501) staff       (20)     4315 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/panelist/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.589939 wwdtm-2.9.0/wwdtm/scorekeeper/
--rw-r--r--   0 lpham      (501) staff       (20)      347 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/scorekeeper/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)     4782 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/scorekeeper/appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     8468 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/scorekeeper/scorekeeper.py
--rw-r--r--   0 lpham      (501) staff       (20)     4530 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/scorekeeper/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.591026 wwdtm-2.9.0/wwdtm/show/
--rw-r--r--   0 lpham      (501) staff       (20)      342 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/show/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)    15317 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/show/info.py
--rw-r--r--   0 lpham      (501) staff       (20)    30759 2024-04-21 03:50:14.000000 wwdtm-2.9.0/wwdtm/show/info_multiple.py
--rw-r--r--   0 lpham      (501) staff       (20)    29362 2024-01-17 00:39:30.000000 wwdtm-2.9.0/wwdtm/show/show.py
--rw-r--r--   0 lpham      (501) staff       (20)     4313 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/show/utility.py
--rw-r--r--   0 lpham      (501) staff       (20)      824 2024-01-12 18:49:15.000000 wwdtm-2.9.0/wwdtm/validation.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 03:50:55.591229 wwdtm-2.9.0/wwdtm.egg-info/
--rw-r--r--   0 lpham      (501) staff       (20)     4484 2024-04-21 03:50:55.000000 wwdtm-2.9.0/wwdtm.egg-info/PKG-INFO
--rw-r--r--   0 lpham      (501) staff       (20)     3400 2024-04-21 03:50:55.000000 wwdtm-2.9.0/wwdtm.egg-info/SOURCES.txt
--rw-r--r--   0 lpham      (501) staff       (20)        1 2024-04-21 03:50:55.000000 wwdtm-2.9.0/wwdtm.egg-info/dependency_links.txt
--rw-r--r--   0 lpham      (501) staff       (20)       79 2024-04-21 03:50:55.000000 wwdtm-2.9.0/wwdtm.egg-info/requires.txt
--rw-r--r--   0 lpham      (501) staff       (20)        6 2024-04-21 03:50:55.000000 wwdtm-2.9.0/wwdtm.egg-info/top_level.txt
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.492581 wwdtm-2.9.1/
+-rw-r--r--   0 lpham      (501) staff       (20)    10142 2021-10-14 22:42:34.000000 wwdtm-2.9.1/LICENSE
+-rw-r--r--   0 lpham      (501) staff       (20)      267 2022-01-03 00:36:38.000000 wwdtm-2.9.1/MANIFEST.in
+-rw-r--r--   0 lpham      (501) staff       (20)     4484 2024-04-21 23:12:50.492274 wwdtm-2.9.1/PKG-INFO
+-rw-r--r--   0 lpham      (501) staff       (20)     3497 2024-01-01 01:43:35.000000 wwdtm-2.9.1/README.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      344 2022-03-17 03:36:18.000000 wwdtm-2.9.1/config.json.dist
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.469512 wwdtm-2.9.1/docs/
+-rw-r--r--   0 lpham      (501) staff       (20)      686 2021-10-14 22:42:34.000000 wwdtm-2.9.1/docs/Makefile
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.455176 wwdtm-2.9.1/docs/_static/
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.469800 wwdtm-2.9.1/docs/_static/css/
+-rw-r--r--   0 lpham      (501) staff       (20)     1575 2024-01-12 18:49:15.000000 wwdtm-2.9.1/docs/_static/css/custom.css
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.470038 wwdtm-2.9.1/docs/_templates/
+-rw-r--r--   0 lpham      (501) staff       (20)      193 2021-10-14 22:42:34.000000 wwdtm-2.9.1/docs/_templates/layout.html
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.470306 wwdtm-2.9.1/docs/changes/
+-rw-r--r--   0 lpham      (501) staff       (20)    10831 2024-04-21 23:12:29.000000 wwdtm-2.9.1/docs/changes/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     1752 2024-01-12 18:49:15.000000 wwdtm-2.9.1/docs/conf.py
+-rw-r--r--   0 lpham      (501) staff       (20)      223 2024-01-01 01:43:35.000000 wwdtm-2.9.1/docs/environment.yaml
+-rw-r--r--   0 lpham      (501) staff       (20)     1243 2024-01-12 18:49:15.000000 wwdtm-2.9.1/docs/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2927 2022-11-13 00:18:03.000000 wwdtm-2.9.1/docs/known_issues.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      795 2021-10-14 22:42:34.000000 wwdtm-2.9.1/docs/make.bat
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.472326 wwdtm-2.9.1/docs/migrating/
+-rw-r--r--   0 lpham      (501) staff       (20)     1886 2022-03-17 03:36:18.000000 wwdtm-2.9.1/docs/migrating/guest.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     1854 2022-03-17 03:36:18.000000 wwdtm-2.9.1/docs/migrating/host.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2821 2024-01-01 01:43:35.000000 wwdtm-2.9.1/docs/migrating/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2320 2022-03-17 03:36:18.000000 wwdtm-2.9.1/docs/migrating/location.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     3802 2022-03-17 03:36:18.000000 wwdtm-2.9.1/docs/migrating/panelist.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2050 2022-03-17 03:36:18.000000 wwdtm-2.9.1/docs/migrating/scorekeeper.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2572 2022-03-17 03:36:18.000000 wwdtm-2.9.1/docs/migrating/show.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      260 2024-04-21 03:50:14.000000 wwdtm-2.9.1/docs/requirements.txt
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.474147 wwdtm-2.9.1/docs/tests/
+-rw-r--r--   0 lpham      (501) staff       (20)      631 2024-01-12 18:49:15.000000 wwdtm-2.9.1/docs/tests/guest.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      608 2022-03-17 03:36:18.000000 wwdtm-2.9.1/docs/tests/host.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      312 2024-01-12 18:49:15.000000 wwdtm-2.9.1/docs/tests/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      704 2022-03-17 03:36:18.000000 wwdtm-2.9.1/docs/tests/location.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     1064 2022-03-17 03:36:18.000000 wwdtm-2.9.1/docs/tests/panelist.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      783 2022-03-17 03:36:18.000000 wwdtm-2.9.1/docs/tests/scorekeeper.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      757 2022-03-17 03:36:18.000000 wwdtm-2.9.1/docs/tests/show.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      287 2022-03-17 03:36:18.000000 wwdtm-2.9.1/docs/tests/validation.rst
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.475786 wwdtm-2.9.1/docs/wwdtm/
+-rw-r--r--   0 lpham      (501) staff       (20)      562 2024-01-12 18:49:15.000000 wwdtm-2.9.1/docs/wwdtm/guest.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      579 2024-01-12 18:49:15.000000 wwdtm-2.9.1/docs/wwdtm/host.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      435 2022-03-17 03:36:18.000000 wwdtm-2.9.1/docs/wwdtm/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      664 2024-01-12 18:49:15.000000 wwdtm-2.9.1/docs/wwdtm/location.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     1034 2024-01-12 18:49:15.000000 wwdtm-2.9.1/docs/wwdtm/panelist.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      712 2024-01-12 18:49:15.000000 wwdtm-2.9.1/docs/wwdtm/scorekeeper.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      676 2024-01-12 18:49:15.000000 wwdtm-2.9.1/docs/wwdtm/show.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      219 2024-01-12 18:49:15.000000 wwdtm-2.9.1/docs/wwdtm/validation.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     3004 2024-04-21 03:50:14.000000 wwdtm-2.9.1/pyproject.toml
+-rw-r--r--   0 lpham      (501) staff       (20)       38 2024-04-21 23:12:50.492639 wwdtm-2.9.1/setup.cfg
+-rw-r--r--   0 lpham      (501) staff       (20)      255 2024-01-12 18:49:15.000000 wwdtm-2.9.1/setup.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.476002 wwdtm-2.9.1/tests/
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.476912 wwdtm-2.9.1/tests/guest/
+-rw-r--r--   0 lpham      (501) staff       (20)     2008 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/guest/test_guest_appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4192 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/guest/test_guest_guest.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4536 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/guest/test_guest_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.477688 wwdtm-2.9.1/tests/host/
+-rw-r--r--   0 lpham      (501) staff       (20)     1999 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/host/test_host_appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     5174 2024-04-21 03:50:14.000000 wwdtm-2.9.1/tests/host/test_host_host.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4346 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/host/test_host_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.478283 wwdtm-2.9.1/tests/location/
+-rw-r--r--   0 lpham      (501) staff       (20)     7105 2024-04-21 23:12:29.000000 wwdtm-2.9.1/tests/location/test_location_location.py
+-rw-r--r--   0 lpham      (501) staff       (20)     2112 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/location/test_location_recordings.py
+-rw-r--r--   0 lpham      (501) staff       (20)     8722 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/location/test_location_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.479877 wwdtm-2.9.1/tests/panelist/
+-rw-r--r--   0 lpham      (501) staff       (20)     4016 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/panelist/test_panelist_appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     6795 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/panelist/test_panelist_decimal_scores.py
+-rw-r--r--   0 lpham      (501) staff       (20)     6377 2024-04-21 03:50:14.000000 wwdtm-2.9.1/tests/panelist/test_panelist_panelist.py
+-rw-r--r--   0 lpham      (501) staff       (20)     6641 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/panelist/test_panelist_scores.py
+-rw-r--r--   0 lpham      (501) staff       (20)     5183 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/panelist/test_panelist_statistics.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4688 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/panelist/test_panelist_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.480609 wwdtm-2.9.1/tests/scorekeeper/
+-rw-r--r--   0 lpham      (501) staff       (20)     2236 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/scorekeeper/test_scorekeeper_appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     6074 2024-04-21 03:50:14.000000 wwdtm-2.9.1/tests/scorekeeper/test_scorekeeper_scorekeeper.py
+-rw-r--r--   0 lpham      (501) staff       (20)     5122 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/scorekeeper/test_scorekeeper_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.481826 wwdtm-2.9.1/tests/show/
+-rw-r--r--   0 lpham      (501) staff       (20)     4204 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/show/test_show_info.py
+-rw-r--r--   0 lpham      (501) staff       (20)     9501 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/show/test_show_info_multiple.py
+-rw-r--r--   0 lpham      (501) staff       (20)    15332 2024-02-12 01:12:44.000000 wwdtm-2.9.1/tests/show/test_show_show.py
+-rw-r--r--   0 lpham      (501) staff       (20)     5144 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/show/test_show_utility.py
+-rw-r--r--   0 lpham      (501) staff       (20)      848 2024-01-12 18:49:15.000000 wwdtm-2.9.1/tests/test_validation.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.482281 wwdtm-2.9.1/wwdtm/
+-rw-r--r--   0 lpham      (501) staff       (20)      792 2024-04-21 23:12:29.000000 wwdtm-2.9.1/wwdtm/__init__.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.483637 wwdtm-2.9.1/wwdtm/guest/
+-rw-r--r--   0 lpham      (501) staff       (20)      317 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/guest/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4814 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/guest/appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     7500 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/guest/guest.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4162 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/guest/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.485609 wwdtm-2.9.1/wwdtm/host/
+-rw-r--r--   0 lpham      (501) staff       (20)      312 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/host/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4488 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/host/appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     7745 2024-04-21 03:50:14.000000 wwdtm-2.9.1/wwdtm/host/host.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4133 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/host/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.486366 wwdtm-2.9.1/wwdtm/location/
+-rw-r--r--   0 lpham      (501) staff       (20)      330 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/location/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)    10889 2024-04-21 23:12:29.000000 wwdtm-2.9.1/wwdtm/location/location.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4460 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/location/recordings.py
+-rw-r--r--   0 lpham      (501) staff       (20)     5472 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/location/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.489087 wwdtm-2.9.1/wwdtm/panelist/
+-rw-r--r--   0 lpham      (501) staff       (20)      460 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/panelist/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)    10466 2024-03-21 02:45:32.000000 wwdtm-2.9.1/wwdtm/panelist/appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)    11473 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/panelist/decimal_scores.py
+-rw-r--r--   0 lpham      (501) staff       (20)     9765 2024-04-21 03:50:14.000000 wwdtm-2.9.1/wwdtm/panelist/panelist.py
+-rw-r--r--   0 lpham      (501) staff       (20)    10553 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/panelist/scores.py
+-rw-r--r--   0 lpham      (501) staff       (20)    10132 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/panelist/statistics.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4315 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/panelist/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.490079 wwdtm-2.9.1/wwdtm/scorekeeper/
+-rw-r--r--   0 lpham      (501) staff       (20)      347 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/scorekeeper/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4782 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/scorekeeper/appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     8468 2024-04-21 03:50:14.000000 wwdtm-2.9.1/wwdtm/scorekeeper/scorekeeper.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4530 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/scorekeeper/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.491708 wwdtm-2.9.1/wwdtm/show/
+-rw-r--r--   0 lpham      (501) staff       (20)      342 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/show/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)    15535 2024-04-21 23:12:29.000000 wwdtm-2.9.1/wwdtm/show/info.py
+-rw-r--r--   0 lpham      (501) staff       (20)    31185 2024-04-21 23:12:29.000000 wwdtm-2.9.1/wwdtm/show/info_multiple.py
+-rw-r--r--   0 lpham      (501) staff       (20)    29362 2024-01-17 00:39:30.000000 wwdtm-2.9.1/wwdtm/show/show.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4313 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/show/utility.py
+-rw-r--r--   0 lpham      (501) staff       (20)      824 2024-01-12 18:49:15.000000 wwdtm-2.9.1/wwdtm/validation.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2024-04-21 23:12:50.491915 wwdtm-2.9.1/wwdtm.egg-info/
+-rw-r--r--   0 lpham      (501) staff       (20)     4484 2024-04-21 23:12:50.000000 wwdtm-2.9.1/wwdtm.egg-info/PKG-INFO
+-rw-r--r--   0 lpham      (501) staff       (20)     3400 2024-04-21 23:12:50.000000 wwdtm-2.9.1/wwdtm.egg-info/SOURCES.txt
+-rw-r--r--   0 lpham      (501) staff       (20)        1 2024-04-21 23:12:50.000000 wwdtm-2.9.1/wwdtm.egg-info/dependency_links.txt
+-rw-r--r--   0 lpham      (501) staff       (20)       79 2024-04-21 23:12:50.000000 wwdtm-2.9.1/wwdtm.egg-info/requires.txt
+-rw-r--r--   0 lpham      (501) staff       (20)        6 2024-04-21 23:12:50.000000 wwdtm-2.9.1/wwdtm.egg-info/top_level.txt
```

### Comparing `wwdtm-2.9.0/LICENSE` & `wwdtm-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/PKG-INFO` & `wwdtm-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwdtm
-Version: 2.9.0
+Version: 2.9.1
 Summary: Library used to query data from copy of Wait Wait Stats Database.
 Author-email: Linh Pham <dev@wwdt.me>
 License: Apache-2.0
 Project-URL: Documentation, https://docs.wwdt.me
 Project-URL: Source Code, https://github.com/questionlp/wwdtm
 Project-URL: Changes, https://docs.wwdt.me/latest/changes/
 Project-URL: Stats Page, https://stats.wwdt.me
```

### Comparing `wwdtm-2.9.0/README.rst` & `wwdtm-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/Makefile` & `wwdtm-2.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/_static/css/custom.css` & `wwdtm-2.9.1/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/changes/index.rst` & `wwdtm-2.9.1/docs/changes/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 *******
 Changes
 *******
 
+2.9.1
+=====
+
+Application Changes
+-------------------
+
+* Encapsulate ``latitude`` and ``longitude`` under the ``coordinates`` property for Locations
+
 2.9.0
 =====
 
 Application Changes
 -------------------
 
-* Add `latitude` and `longitude` properties to Locations
-* Add `pronouns` property to Hosts, Panelists and Scorekeepers
+* Add ``latitude`` and ``longitude`` properties to Locations
+* Add ``pronouns`` property to Hosts, Panelists and Scorekeepers
 
 Component Changes
 -----------------
 
 * Upgrade numpy from 1.26.3 to 1.26.4
 * Upgrade pytz from 2023.3.post1 to 2024.1
```

### Comparing `wwdtm-2.9.0/docs/conf.py` & `wwdtm-2.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/index.rst` & `wwdtm-2.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/known_issues.rst` & `wwdtm-2.9.1/docs/known_issues.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/make.bat` & `wwdtm-2.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/migrating/guest.rst` & `wwdtm-2.9.1/docs/migrating/guest.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/migrating/host.rst` & `wwdtm-2.9.1/docs/migrating/host.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/migrating/index.rst` & `wwdtm-2.9.1/docs/migrating/index.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/migrating/location.rst` & `wwdtm-2.9.1/docs/migrating/location.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/migrating/panelist.rst` & `wwdtm-2.9.1/docs/migrating/panelist.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/migrating/scorekeeper.rst` & `wwdtm-2.9.1/docs/migrating/scorekeeper.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/migrating/show.rst` & `wwdtm-2.9.1/docs/migrating/show.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/tests/guest.rst` & `wwdtm-2.9.1/docs/tests/guest.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/tests/host.rst` & `wwdtm-2.9.1/docs/tests/host.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/tests/location.rst` & `wwdtm-2.9.1/docs/tests/location.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/tests/panelist.rst` & `wwdtm-2.9.1/docs/tests/panelist.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/tests/scorekeeper.rst` & `wwdtm-2.9.1/docs/tests/scorekeeper.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/tests/show.rst` & `wwdtm-2.9.1/docs/tests/show.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/wwdtm/guest.rst` & `wwdtm-2.9.1/docs/wwdtm/guest.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/wwdtm/host.rst` & `wwdtm-2.9.1/docs/wwdtm/host.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/wwdtm/location.rst` & `wwdtm-2.9.1/docs/wwdtm/location.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/wwdtm/panelist.rst` & `wwdtm-2.9.1/docs/wwdtm/panelist.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/wwdtm/scorekeeper.rst` & `wwdtm-2.9.1/docs/wwdtm/scorekeeper.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/docs/wwdtm/show.rst` & `wwdtm-2.9.1/docs/wwdtm/show.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/pyproject.toml` & `wwdtm-2.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/guest/test_guest_appearances.py` & `wwdtm-2.9.1/tests/guest/test_guest_appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/guest/test_guest_guest.py` & `wwdtm-2.9.1/tests/guest/test_guest_guest.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/guest/test_guest_utility.py` & `wwdtm-2.9.1/tests/guest/test_guest_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/host/test_host_appearances.py` & `wwdtm-2.9.1/tests/host/test_host_appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/host/test_host_host.py` & `wwdtm-2.9.1/tests/host/test_host_host.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/host/test_host_utility.py` & `wwdtm-2.9.1/tests/host/test_host_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/location/test_location_location.py` & `wwdtm-2.9.1/tests/location/test_location_location.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,25 +31,45 @@
     """Testing for :py:meth:`wwdtm.location.Location.retrieve_all`."""
     location = Location(connect_dict=get_connect_dict())
     locations = location.retrieve_all()
 
     assert locations, "No locations could be retrieved"
     assert "id" in locations[0], "'id' was not returned for the first list item"
     assert "venue" in locations[0], "'venue' was not returned for the first list item"
+    assert (
+        "coordinates" in locations[0]
+    ), "'coordinates' was not returned for the first list item"
+    if locations[0]["coordinates"]:
+        assert (
+            "latitude" in locations[0]["coordinates"]
+        ), "'latitude' was not returned for the first list item"
+        assert (
+            "longitude" in locations[0]["coordinates"]
+        ), "'longitude' was not returned for the first list item"
 
 
 def test_location_retrieve_all_details():
     """Testing for :py:meth:`wwdtm.location.Location.retrieve_all_details`."""
     location = Location(connect_dict=get_connect_dict())
     locations = location.retrieve_all_details()
 
     assert locations, "No locations could be retrieved"
     assert "id" in locations[0], "'id' was not returned for first list item"
     assert "venue" in locations[0], "'venue' was not returned for the first list item"
     assert (
+        "coordinates" in locations[0]
+    ), "'coordinates' was not returned for the first list item"
+    if locations[0]["coordinates"]:
+        assert (
+            "latitude" in locations[0]["coordinates"]
+        ), "'latitude' was not returned for the first list item"
+        assert (
+            "longitude" in locations[0]["coordinates"]
+        ), "'longitude' was not returned for the first list item"
+    assert (
         "recordings" in locations[0]
     ), "'recordings' was not returned for the first list item"
 
 
 def test_location_retrieve_all_ids():
     """Testing for :py:meth:`wwdtm.location.Location.retrieve_all_ids`."""
     location = Location(connect_dict=get_connect_dict())
@@ -74,31 +94,43 @@
         information
     """
     location = Location(connect_dict=get_connect_dict())
     info = location.retrieve_by_id(location_id)
 
     assert info, f"Location ID {location_id} not found"
     assert "venue" in info, f"'venue' was not returned for ID {location_id}"
-    assert "latitude" in info, f"'latitude' was not returned for ID {location_id}"
-    assert "longitude" in info, f"'longitude' was not returned for ID {location_id}"
+    assert "coordinates" in info, f"'coordinates' was not returned for ID {location_id}"
+    if info["coordinates"]:
+        assert (
+            "latitude" in info["coordinates"]
+        ), f"'latitude' was not returned for ID {location_id}"
+        assert (
+            "longitude" in info["coordinates"]
+        ), f"'longitude' was not returned for ID {location_id}"
 
 
 @pytest.mark.parametrize("location_id", [95])
 def test_location_retrieve_details_by_id(location_id: int):
     """Testing for :py:meth:`wwdtm.location.location.retrieve_details_by_id`.
 
     :param location_id: Location ID to test retrieving location details
     """
     location = Location(connect_dict=get_connect_dict())
     info = location.retrieve_details_by_id(location_id)
 
     assert info, f"Location ID {location_id} not found"
     assert "venue" in info, f"'venue' was not returned for ID {location_id}"
-    assert "latitude" in info, f"'latitude' was not returned for ID {location_id}"
-    assert "longitude" in info, f"'longitude' was not returned for ID {location_id}"
+    assert "coordinates" in info, f"'coordinates' was not returned for ID {location_id}"
+    if info["coordinates"]:
+        assert (
+            "latitude" in info["coordinates"]
+        ), f"'latitude' was not returned for ID {location_id}"
+        assert (
+            "longitude" in info["coordinates"]
+        ), f"'longitude' was not returned for ID {location_id}"
     assert "recordings" in info, f"'recordings' was not returned for ID {location_id}"
 
 
 @pytest.mark.parametrize("location_slug", ["the-chicago-theatre-chicago-il"])
 def test_location_retrieve_by_slug(location_slug: str):
     """Testing for :py:meth:`wwdtm.location.Location.retrieve_by_slug`.
 
@@ -106,28 +138,44 @@
         location information
     """
     location = Location(connect_dict=get_connect_dict())
     info = location.retrieve_by_slug(location_slug)
 
     assert info, f"Location slug {location_slug} not found"
     assert "venue" in info, f"'venue' was not returned for slug {location_slug}"
-    assert "latitude" in info, f"'latitude' was not returned for ID {location_slug}"
-    assert "longitude" in info, f"'longitude' was not returned for ID {location_slug}"
+    assert (
+        "coordinates" in info
+    ), f"'coordinates' was not returned for slug {location_slug}"
+    if info["coordinates"]:
+        assert (
+            "latitude" in info["coordinates"]
+        ), f"'latitude' was not returned for slug {location_slug}"
+        assert (
+            "longitude" in info["coordinates"]
+        ), f"'longitude' was not returned for slug {location_slug}"
 
 
 @pytest.mark.parametrize("location_slug", ["the-chicago-theatre-chicago-il"])
 def test_location_retrieve_details_by_slug(location_slug: str):
     """Testing for :py:meth:`wwdtm.location.Location.retrieve_details_by_slug`.
 
     :param location_slug: Location slug string to test retrieving
         location details
     """
     location = Location(connect_dict=get_connect_dict())
     info = location.retrieve_details_by_slug(location_slug)
 
     assert info, f"Location slug {location_slug} not found"
     assert "venue" in info, f"'venue' was not returned for slug {location_slug}"
-    assert "latitude" in info, f"'latitude' was not returned for ID {location_slug}"
-    assert "longitude" in info, f"'longitude' was not returned for ID {location_slug}"
+    assert (
+        "coordinates" in info
+    ), f"'coordinates' was not returned for slug {location_slug}"
+    if info["coordinates"]:
+        assert (
+            "latitude" in info["coordinates"]
+        ), f"'latitude' was not returned for slug {location_slug}"
+        assert (
+            "longitude" in info["coordinates"]
+        ), f"'longitude' was not returned for slug {location_slug}"
     assert (
         "recordings" in info
     ), f"'recordings' was not returned for slug {location_slug}"
```

### Comparing `wwdtm-2.9.0/tests/location/test_location_recordings.py` & `wwdtm-2.9.1/tests/location/test_location_recordings.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/location/test_location_utility.py` & `wwdtm-2.9.1/tests/location/test_location_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/panelist/test_panelist_appearances.py` & `wwdtm-2.9.1/tests/panelist/test_panelist_appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/panelist/test_panelist_decimal_scores.py` & `wwdtm-2.9.1/tests/panelist/test_panelist_decimal_scores.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/panelist/test_panelist_panelist.py` & `wwdtm-2.9.1/tests/panelist/test_panelist_panelist.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/panelist/test_panelist_scores.py` & `wwdtm-2.9.1/tests/panelist/test_panelist_scores.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/panelist/test_panelist_statistics.py` & `wwdtm-2.9.1/tests/panelist/test_panelist_statistics.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/panelist/test_panelist_utility.py` & `wwdtm-2.9.1/tests/panelist/test_panelist_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/scorekeeper/test_scorekeeper_appearances.py` & `wwdtm-2.9.1/tests/scorekeeper/test_scorekeeper_appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/scorekeeper/test_scorekeeper_scorekeeper.py` & `wwdtm-2.9.1/tests/scorekeeper/test_scorekeeper_scorekeeper.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/scorekeeper/test_scorekeeper_utility.py` & `wwdtm-2.9.1/tests/scorekeeper/test_scorekeeper_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/show/test_show_info.py` & `wwdtm-2.9.1/tests/show/test_show_info.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/show/test_show_info_multiple.py` & `wwdtm-2.9.1/tests/show/test_show_info_multiple.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/show/test_show_show.py` & `wwdtm-2.9.1/tests/show/test_show_show.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/show/test_show_utility.py` & `wwdtm-2.9.1/tests/show/test_show_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/tests/test_validation.py` & `wwdtm-2.9.1/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/__init__.py` & `wwdtm-2.9.1/wwdtm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     PanelistScores,
     PanelistStatistics,
     PanelistUtility,
 )
 from wwdtm.scorekeeper import Scorekeeper, ScorekeeperAppearances, ScorekeeperUtility
 from wwdtm.show import Show, ShowInfo, ShowInfoMultiple, ShowUtility
 
-VERSION = "2.9.0"
+VERSION = "2.9.1"
```

### Comparing `wwdtm-2.9.0/wwdtm/guest/appearances.py` & `wwdtm-2.9.1/wwdtm/guest/appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/guest/guest.py` & `wwdtm-2.9.1/wwdtm/guest/guest.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/guest/utility.py` & `wwdtm-2.9.1/wwdtm/guest/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/host/appearances.py` & `wwdtm-2.9.1/wwdtm/host/appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/host/host.py` & `wwdtm-2.9.1/wwdtm/host/host.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/host/utility.py` & `wwdtm-2.9.1/wwdtm/host/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/location/location.py` & `wwdtm-2.9.1/wwdtm/location/location.py`

 * *Files 9% similar despite different names*

```diff
@@ -71,22 +71,29 @@
         cursor.close()
 
         if not results:
             return []
 
         locations = []
         for row in results:
+            if not row.latitude and not row.longitude:
+                coordinates = None
+            else:
+                coordinates = {
+                    "latitude": row.latitude if row.latitude else None,
+                    "longitude": row.longitude if row.longitude else None,
+                }
+
             locations.append(
                 {
                     "id": row.id,
                     "city": row.city,
                     "state": row.state,
                     "venue": row.venue,
-                    "latitude": row.latitude if row.latitude else None,
-                    "longitude": row.longitude if row.longitude else None,
+                    "coordinates": coordinates,
                     "slug": (
                         row.slug
                         if row.slug
                         else self.utility.slugify_location(
                             location_id=row.id,
                             venue=row.venue,
                             city=row.city,
@@ -122,22 +129,29 @@
         cursor.close()
 
         if not results:
             return []
 
         locations = []
         for row in results:
+            if not row.latitude and not row.longitude:
+                coordinates = None
+            else:
+                coordinates = {
+                    "latitude": row.latitude if row.latitude else None,
+                    "longitude": row.longitude if row.longitude else None,
+                }
+
             locations.append(
                 {
                     "id": row.id,
                     "city": row.city,
                     "state": row.state,
                     "venue": row.venue,
-                    "latitude": row.latitude if row.latitude else None,
-                    "longitude": row.longitude if row.longitude else None,
+                    "coordinates": coordinates,
                     "slug": (
                         row.slug
                         if row.slug
                         else self.utility.slugify_location(
                             location_id=row.id,
                             venue=row.venue,
                             city=row.city,
@@ -217,21 +231,28 @@
         cursor.execute(query, (location_id,))
         result = cursor.fetchone()
         cursor.close()
 
         if not result:
             return {}
 
+        if not result.latitude and not result.longitude:
+            coordinates = None
+        else:
+            coordinates = {
+                "latitude": result.latitude if result.latitude else None,
+                "longitude": result.longitude if result.longitude else None,
+            }
+
         return {
             "id": result.id,
             "city": result.city,
             "state": result.state,
             "venue": result.venue,
-            "latitude": result.latitude if result.latitude else None,
-            "longitude": result.longitude if result.longitude else None,
+            "coordinates": coordinates,
             "slug": (
                 result.slug
                 if result.slug
                 else self.utility.slugify_location(
                     location_id=result.id,
                     venue=result.venue,
                     city=result.city,
```

### Comparing `wwdtm-2.9.0/wwdtm/location/recordings.py` & `wwdtm-2.9.1/wwdtm/location/recordings.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/location/utility.py` & `wwdtm-2.9.1/wwdtm/location/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/panelist/appearances.py` & `wwdtm-2.9.1/wwdtm/panelist/appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/panelist/decimal_scores.py` & `wwdtm-2.9.1/wwdtm/panelist/decimal_scores.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/panelist/panelist.py` & `wwdtm-2.9.1/wwdtm/panelist/panelist.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/panelist/scores.py` & `wwdtm-2.9.1/wwdtm/panelist/scores.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/panelist/statistics.py` & `wwdtm-2.9.1/wwdtm/panelist/statistics.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/panelist/utility.py` & `wwdtm-2.9.1/wwdtm/panelist/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/scorekeeper/appearances.py` & `wwdtm-2.9.1/wwdtm/scorekeeper/appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/scorekeeper/scorekeeper.py` & `wwdtm-2.9.1/wwdtm/scorekeeper/scorekeeper.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/scorekeeper/utility.py` & `wwdtm-2.9.1/wwdtm/scorekeeper/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/show/info.py` & `wwdtm-2.9.1/wwdtm/show/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,22 +207,29 @@
         cursor.execute(query, (show_id,))
         result = cursor.fetchone()
         cursor.close()
 
         if not result:
             return {}
 
+        if not result.latitude and not result.longitude:
+            coordinates = None
+        else:
+            coordinates = {
+                "latitude": result.latitude if result.latitude else None,
+                "longitude": result.longitude if result.longitude else None,
+            }
+
         location_info = {
             "id": result.location_id,
             "slug": result.location_slug,
             "city": result.city,
             "state": result.state,
             "venue": result.venue,
-            "latitude": result.latitude if result.latitude else None,
-            "longitude": result.longitude if result.longitude else None,
+            "coordinates": coordinates if coordinates else None,
         }
 
         if not result.location_slug:
             location_info["slug"] = self.loc_util.slugify_location(
                 location_id=result.location_id,
                 venue=result.venue,
                 city=result.city,
```

### Comparing `wwdtm-2.9.0/wwdtm/show/info_multiple.py` & `wwdtm-2.9.1/wwdtm/show/info_multiple.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,22 +307,29 @@
         cursor.close()
 
         if not results:
             return {}
 
         shows = {}
         for show in results:
+            if not show.latitude and not show.longitude:
+                coordinates = None
+            else:
+                coordinates = {
+                    "latitude": show.latitude if show.latitude else None,
+                    "longitude": show.longitude if show.longitude else None,
+                }
+
             location_info = {
                 "id": show.location_id,
                 "slug": show.location_slug,
                 "city": show.city,
                 "state": show.state,
                 "venue": show.venue,
-                "latitude": show.latitude if show.latitude else None,
-                "longitude": show.longitude if show.longitude else None,
+                "coordinates": coordinates,
             }
 
             if not show.location_slug:
                 location_info["slug"] = self.loc_util.slugify_location(
                     location_id=show.location_id,
                     venue=show.venue,
                     city=show.city,
@@ -433,22 +440,29 @@
         cursor.close()
 
         if not results:
             return {}
 
         shows = {}
         for show in results:
+            if not show.latitude and not show.longitude:
+                coordinates = None
+            else:
+                coordinates = {
+                    "latitude": show.latitude if show.latitude else None,
+                    "longitude": show.longitude if show.longitude else None,
+                }
+
             location_info = {
                 "id": show.location_id,
                 "slug": show.location_slug,
                 "city": show.city,
                 "state": show.state,
                 "venue": show.venue,
-                "latitude": show.latitude if show.latitude else None,
-                "longitude": show.longitude if show.longitude else None,
+                "coordinates": coordinates,
             }
 
             if not show.location_slug:
                 location_info["slug"] = self.loc_util.slugify_location(
                     location_id=show.location_id,
                     venue=show.venue,
                     city=show.city,
```

### Comparing `wwdtm-2.9.0/wwdtm/show/show.py` & `wwdtm-2.9.1/wwdtm/show/show.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/show/utility.py` & `wwdtm-2.9.1/wwdtm/show/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm/validation.py` & `wwdtm-2.9.1/wwdtm/validation.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.9.0/wwdtm.egg-info/PKG-INFO` & `wwdtm-2.9.1/wwdtm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwdtm
-Version: 2.9.0
+Version: 2.9.1
 Summary: Library used to query data from copy of Wait Wait Stats Database.
 Author-email: Linh Pham <dev@wwdt.me>
 License: Apache-2.0
 Project-URL: Documentation, https://docs.wwdt.me
 Project-URL: Source Code, https://github.com/questionlp/wwdtm
 Project-URL: Changes, https://docs.wwdt.me/latest/changes/
 Project-URL: Stats Page, https://stats.wwdt.me
```

### Comparing `wwdtm-2.9.0/wwdtm.egg-info/SOURCES.txt` & `wwdtm-2.9.1/wwdtm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

