# Comparing `tmp/nrdp-daemon-1.0.8.tar.gz` & `tmp/nrdp-daemon-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nrdp-daemon-1.0.8.tar", last modified: Wed Nov 25 00:59:32 2020, max compression
+gzip compressed data, was "dist/nrdp-daemon-1.0.9.tar", last modified: Wed Nov 25 16:18:28 2020, max compression
```

## Comparing `nrdp-daemon-1.0.8.tar` & `nrdp-daemon-1.0.9.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     1480 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/PKG-INFO
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      197 2020-11-23 21:44:31.000000 nrdp-daemon-1.0.8/MANIFEST.in
-drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    16142 2020-11-25 00:59:31.000000 nrdp-daemon-1.0.8/docs/configuration.file.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      932 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/objects.inv
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     2881 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/search.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     5772 2020-11-25 00:59:31.000000 nrdp-daemon-1.0.8/docs/libnrdpd.nrdp.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     5088 2020-11-25 00:59:31.000000 nrdp-daemon-1.0.8/docs/index.html
-drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_static/
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       42 2020-04-27 14:42:53.000000 nrdp-daemon-1.0.8/docs/_static/custom.css
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       90 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.8/docs/_static/plus.png
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    10847 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_static/language_data.js
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      353 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_static/documentation_options.js
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)   280364 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.8/docs/_static/jquery-3.4.1.js
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      286 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.8/docs/_static/file.png
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     4798 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_static/pygments.css
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    11185 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_static/alabaster.css
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    12261 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_static/basic.css
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    16323 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.8/docs/_static/searchtools.js
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     9354 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.8/docs/_static/doctools.js
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    88145 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.8/docs/_static/jquery.js
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    12140 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.8/docs/_static/underscore.js
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       90 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.8/docs/_static/minus.png
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    35168 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.8/docs/_static/underscore-1.3.1.js
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      230 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/.buildinfo
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    10675 2020-11-25 00:59:31.000000 nrdp-daemon-1.0.8/docs/configuration.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     4795 2020-11-25 00:59:31.000000 nrdp-daemon-1.0.8/docs/libnrdpd.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    12898 2020-11-25 00:59:31.000000 nrdp-daemon-1.0.8/docs/libnrdpd.error.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/.nojekyll
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     4643 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/py-modindex.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     3399 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/nrdpd.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    10659 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/libnrdpd.util.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    15979 2020-11-25 00:59:31.000000 nrdp-daemon-1.0.8/docs/libnrdpd.config.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    12430 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/libnrdpd.task.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     9203 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/searchindex.js
-drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_sources/
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      227 2020-11-19 21:32:14.000000 nrdp-daemon-1.0.8/docs/_sources/libnrdpd.main.rst.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      145 2020-11-19 17:30:05.000000 nrdp-daemon-1.0.8/docs/_sources/libnrdpd.util.rst.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      182 2020-11-18 23:47:26.000000 nrdp-daemon-1.0.8/docs/_sources/libnrdpd.config.rst.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      331 2020-11-20 20:50:12.000000 nrdp-daemon-1.0.8/docs/_sources/libnrdpd.rst.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     6455 2020-11-24 19:34:15.000000 nrdp-daemon-1.0.8/docs/_sources/configuration.file.rst.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      179 2020-11-18 23:42:17.000000 nrdp-daemon-1.0.8/docs/_sources/libnrdpd.error.rst.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      145 2020-11-20 20:50:41.000000 nrdp-daemon-1.0.8/docs/_sources/libnrdpd.task.rst.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      185 2020-11-24 19:52:04.000000 nrdp-daemon-1.0.8/docs/_sources/nrdpd.rst.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      157 2020-11-20 21:17:52.000000 nrdp-daemon-1.0.8/docs/_sources/libnrdpd.schedule.rst.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     2471 2020-11-24 23:18:47.000000 nrdp-daemon-1.0.8/docs/_sources/configuration.rst.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      145 2020-11-20 17:15:36.000000 nrdp-daemon-1.0.8/docs/_sources/libnrdpd.nrdp.rst.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      477 2020-11-24 19:54:01.000000 nrdp-daemon-1.0.8/docs/_sources/index.rst.txt
-drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_modules/
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     3091 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_modules/index.html
-drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_modules/libnrdpd/
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    18968 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_modules/libnrdpd/schedule.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    31331 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_modules/libnrdpd/util.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    35386 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_modules/libnrdpd/task.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    49940 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_modules/libnrdpd/config.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    16745 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_modules/libnrdpd/nrdp.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    29983 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_modules/libnrdpd/main.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    12769 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/_modules/libnrdpd/error.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     5754 2020-11-25 00:59:31.000000 nrdp-daemon-1.0.8/docs/libnrdpd.main.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    15302 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/docs/genindex.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     6422 2020-11-25 00:59:31.000000 nrdp-daemon-1.0.8/docs/libnrdpd.schedule.html
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      240 2020-11-16 22:03:21.000000 nrdp-daemon-1.0.8/setup.py
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       31 2020-11-18 20:36:31.000000 nrdp-daemon-1.0.8/pyproject.toml
-drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/nrdp_daemon.egg-info/
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     1480 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/nrdp_daemon.egg-info/PKG-INFO
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     2565 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/nrdp_daemon.egg-info/SOURCES.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)        9 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/nrdp_daemon.egg-info/top_level.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       47 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/nrdp_daemon.egg-info/entry_points.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       40 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/nrdp_daemon.egg-info/requires.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)        1 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/nrdp_daemon.egg-info/dependency_links.txt
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)        1 2020-11-18 22:06:59.000000 nrdp-daemon-1.0.8/nrdp_daemon.egg-info/zip-safe
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     1193 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/setup.cfg
-drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/libnrdpd/
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     8687 2020-11-24 22:51:17.000000 nrdp-daemon-1.0.8/libnrdpd/task.py
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      835 2020-11-20 20:48:31.000000 nrdp-daemon-1.0.8/libnrdpd/__init__.py
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     7676 2020-11-20 21:37:19.000000 nrdp-daemon-1.0.8/libnrdpd/util.py
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     5981 2020-11-23 23:21:24.000000 nrdp-daemon-1.0.8/libnrdpd/main.py
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    13325 2020-11-24 22:23:56.000000 nrdp-daemon-1.0.8/libnrdpd/config.py
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     2809 2020-11-20 21:04:11.000000 nrdp-daemon-1.0.8/libnrdpd/error.py
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     3969 2020-11-20 21:52:45.000000 nrdp-daemon-1.0.8/libnrdpd/nrdp.py
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     4101 2020-11-24 22:54:09.000000 nrdp-daemon-1.0.8/libnrdpd/schedule.py
-drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/tests/
-drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/tests/config/
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      250 2020-11-24 18:39:05.000000 nrdp-daemon-1.0.8/tests/config/config-valid.ini
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      132 2020-11-19 18:33:16.000000 nrdp-daemon-1.0.8/tests/config/config-mvp.ini
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       56 2020-11-13 18:21:14.000000 nrdp-daemon-1.0.8/tests/config/config-bad-url.ini
-drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/tests/config/conf.d/
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       91 2020-11-24 18:39:31.000000 nrdp-daemon-1.0.8/tests/config/conf.d/004-config.ini
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       17 2020-11-18 22:41:12.000000 nrdp-daemon-1.0.8/tests/config/conf.d/003-config-token.ini
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       37 2020-11-19 20:46:44.000000 nrdp-daemon-1.0.8/tests/config/conf.d/000-defaults.ini
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      106 2020-11-19 20:46:51.000000 nrdp-daemon-1.0.8/tests/config/conf.d/001-test.ini
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     1905 2020-11-20 20:52:35.000000 nrdp-daemon-1.0.8/tests/test_util.py
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      475 2020-11-20 20:42:45.000000 nrdp-daemon-1.0.8/tests/test_task.py
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     1986 2020-11-24 18:34:17.000000 nrdp-daemon-1.0.8/tests/test_config.py
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      879 2020-11-23 21:43:32.000000 nrdp-daemon-1.0.8/Makefile
-drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 00:59:32.000000 nrdp-daemon-1.0.8/doc-src/
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      331 2020-11-20 20:50:12.000000 nrdp-daemon-1.0.8/doc-src/libnrdpd.rst
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      145 2020-11-20 17:15:36.000000 nrdp-daemon-1.0.8/doc-src/libnrdpd.nrdp.rst
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      477 2020-11-24 19:54:01.000000 nrdp-daemon-1.0.8/doc-src/index.rst
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     2093 2020-11-23 18:08:44.000000 nrdp-daemon-1.0.8/doc-src/conf.py
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      185 2020-11-24 19:52:04.000000 nrdp-daemon-1.0.8/doc-src/nrdpd.rst
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     2471 2020-11-24 23:18:47.000000 nrdp-daemon-1.0.8/doc-src/configuration.rst
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      227 2020-11-19 21:32:14.000000 nrdp-daemon-1.0.8/doc-src/libnrdpd.main.rst
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      179 2020-11-18 23:42:17.000000 nrdp-daemon-1.0.8/doc-src/libnrdpd.error.rst
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      145 2020-11-20 20:50:41.000000 nrdp-daemon-1.0.8/doc-src/libnrdpd.task.rst
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      157 2020-11-20 21:17:52.000000 nrdp-daemon-1.0.8/doc-src/libnrdpd.schedule.rst
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      182 2020-11-18 23:47:26.000000 nrdp-daemon-1.0.8/doc-src/libnrdpd.config.rst
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      145 2020-11-19 17:30:05.000000 nrdp-daemon-1.0.8/doc-src/libnrdpd.util.rst
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    11358 2020-07-30 19:40:08.000000 nrdp-daemon-1.0.8/LICENSE
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      499 2020-11-23 21:47:11.000000 nrdp-daemon-1.0.8/tox.ini
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      521 2020-11-23 21:27:06.000000 nrdp-daemon-1.0.8/README.rst
--rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       32 2020-11-20 22:52:36.000000 nrdp-daemon-1.0.8/requirements-doc.txt
+drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     1480 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/PKG-INFO
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      197 2020-11-23 21:44:31.000000 nrdp-daemon-1.0.9/MANIFEST.in
+drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/docs/
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    16142 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/configuration.file.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      932 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/objects.inv
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     2881 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/search.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     5772 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/libnrdpd.nrdp.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     5088 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/index.html
+drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/docs/_static/
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       42 2020-04-27 14:42:53.000000 nrdp-daemon-1.0.9/docs/_static/custom.css
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       90 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.9/docs/_static/plus.png
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    10847 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/_static/language_data.js
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      353 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/_static/documentation_options.js
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)   280364 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.9/docs/_static/jquery-3.4.1.js
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      286 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.9/docs/_static/file.png
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     4798 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/_static/pygments.css
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    11185 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/_static/alabaster.css
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    12261 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/_static/basic.css
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    16323 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.9/docs/_static/searchtools.js
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     9354 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.9/docs/_static/doctools.js
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    88145 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.9/docs/_static/jquery.js
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    12140 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.9/docs/_static/underscore.js
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       90 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.9/docs/_static/minus.png
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    35168 2020-04-27 14:42:54.000000 nrdp-daemon-1.0.9/docs/_static/underscore-1.3.1.js
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      230 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/.buildinfo
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    10675 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/configuration.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     4795 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/libnrdpd.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    12898 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/libnrdpd.error.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/.nojekyll
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     4643 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/py-modindex.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     3399 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/nrdpd.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    10659 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/libnrdpd.util.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    15979 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/libnrdpd.config.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    12430 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/libnrdpd.task.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     9203 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/searchindex.js
+drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/docs/_sources/
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      227 2020-11-19 21:32:14.000000 nrdp-daemon-1.0.9/docs/_sources/libnrdpd.main.rst.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      145 2020-11-19 17:30:05.000000 nrdp-daemon-1.0.9/docs/_sources/libnrdpd.util.rst.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      182 2020-11-18 23:47:26.000000 nrdp-daemon-1.0.9/docs/_sources/libnrdpd.config.rst.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      331 2020-11-20 20:50:12.000000 nrdp-daemon-1.0.9/docs/_sources/libnrdpd.rst.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     6455 2020-11-24 19:34:15.000000 nrdp-daemon-1.0.9/docs/_sources/configuration.file.rst.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      179 2020-11-18 23:42:17.000000 nrdp-daemon-1.0.9/docs/_sources/libnrdpd.error.rst.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      145 2020-11-20 20:50:41.000000 nrdp-daemon-1.0.9/docs/_sources/libnrdpd.task.rst.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      185 2020-11-24 19:52:04.000000 nrdp-daemon-1.0.9/docs/_sources/nrdpd.rst.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      157 2020-11-20 21:17:52.000000 nrdp-daemon-1.0.9/docs/_sources/libnrdpd.schedule.rst.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     2471 2020-11-24 23:18:47.000000 nrdp-daemon-1.0.9/docs/_sources/configuration.rst.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      145 2020-11-20 17:15:36.000000 nrdp-daemon-1.0.9/docs/_sources/libnrdpd.nrdp.rst.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      477 2020-11-24 19:54:01.000000 nrdp-daemon-1.0.9/docs/_sources/index.rst.txt
+drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/docs/_modules/
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     3091 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/_modules/index.html
+drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/docs/_modules/libnrdpd/
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    18968 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/_modules/libnrdpd/schedule.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    31331 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/_modules/libnrdpd/util.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    35272 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/_modules/libnrdpd/task.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    50051 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/_modules/libnrdpd/config.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    16745 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/_modules/libnrdpd/nrdp.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    29983 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/_modules/libnrdpd/main.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    12769 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/_modules/libnrdpd/error.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     5754 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/libnrdpd.main.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    15302 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/genindex.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     6422 2020-11-25 16:18:27.000000 nrdp-daemon-1.0.9/docs/libnrdpd.schedule.html
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      240 2020-11-16 22:03:21.000000 nrdp-daemon-1.0.9/setup.py
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       31 2020-11-18 20:36:31.000000 nrdp-daemon-1.0.9/pyproject.toml
+drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/nrdp_daemon.egg-info/
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     1480 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/nrdp_daemon.egg-info/PKG-INFO
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     2596 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/nrdp_daemon.egg-info/SOURCES.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)        9 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/nrdp_daemon.egg-info/top_level.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       47 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/nrdp_daemon.egg-info/entry_points.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       40 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/nrdp_daemon.egg-info/requires.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)        1 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/nrdp_daemon.egg-info/dependency_links.txt
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)        1 2020-11-18 22:06:59.000000 nrdp-daemon-1.0.9/nrdp_daemon.egg-info/zip-safe
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     1193 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/setup.cfg
+drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/libnrdpd/
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     8667 2020-11-25 16:16:10.000000 nrdp-daemon-1.0.9/libnrdpd/task.py
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      835 2020-11-20 20:48:31.000000 nrdp-daemon-1.0.9/libnrdpd/__init__.py
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     7676 2020-11-20 21:37:19.000000 nrdp-daemon-1.0.9/libnrdpd/util.py
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     5981 2020-11-23 23:21:24.000000 nrdp-daemon-1.0.9/libnrdpd/main.py
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    13343 2020-11-25 16:11:43.000000 nrdp-daemon-1.0.9/libnrdpd/config.py
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     2809 2020-11-20 21:04:11.000000 nrdp-daemon-1.0.9/libnrdpd/error.py
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     3969 2020-11-20 21:52:45.000000 nrdp-daemon-1.0.9/libnrdpd/nrdp.py
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     4101 2020-11-24 22:54:09.000000 nrdp-daemon-1.0.9/libnrdpd/schedule.py
+drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/tests/
+drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/tests/config/
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      250 2020-11-24 18:39:05.000000 nrdp-daemon-1.0.9/tests/config/config-valid.ini
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      132 2020-11-19 18:33:16.000000 nrdp-daemon-1.0.9/tests/config/config-mvp.ini
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       56 2020-11-13 18:21:14.000000 nrdp-daemon-1.0.9/tests/config/config-bad-url.ini
+drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/tests/config/conf.d/
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       91 2020-11-24 18:39:31.000000 nrdp-daemon-1.0.9/tests/config/conf.d/004-config.ini
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       17 2020-11-18 22:41:12.000000 nrdp-daemon-1.0.9/tests/config/conf.d/003-config-token.ini
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       37 2020-11-19 20:46:44.000000 nrdp-daemon-1.0.9/tests/config/conf.d/000-defaults.ini
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      106 2020-11-19 20:46:51.000000 nrdp-daemon-1.0.9/tests/config/conf.d/001-test.ini
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     1905 2020-11-20 20:52:35.000000 nrdp-daemon-1.0.9/tests/test_util.py
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      475 2020-11-20 20:42:45.000000 nrdp-daemon-1.0.9/tests/test_task.py
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     1986 2020-11-24 18:34:17.000000 nrdp-daemon-1.0.9/tests/test_config.py
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      879 2020-11-23 21:43:32.000000 nrdp-daemon-1.0.9/Makefile
+drwxr-xr-x   0 blkmajik  (1000) blkmajik  (1000)        0 2020-11-25 16:18:28.000000 nrdp-daemon-1.0.9/doc-src/
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      331 2020-11-20 20:50:12.000000 nrdp-daemon-1.0.9/doc-src/libnrdpd.rst
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      145 2020-11-20 17:15:36.000000 nrdp-daemon-1.0.9/doc-src/libnrdpd.nrdp.rst
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      477 2020-11-24 19:54:01.000000 nrdp-daemon-1.0.9/doc-src/index.rst
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     2093 2020-11-23 18:08:44.000000 nrdp-daemon-1.0.9/doc-src/conf.py
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     6455 2020-11-24 19:34:15.000000 nrdp-daemon-1.0.9/doc-src/configuration.file.rst
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      185 2020-11-24 19:52:04.000000 nrdp-daemon-1.0.9/doc-src/nrdpd.rst
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)     2471 2020-11-24 23:18:47.000000 nrdp-daemon-1.0.9/doc-src/configuration.rst
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      227 2020-11-19 21:32:14.000000 nrdp-daemon-1.0.9/doc-src/libnrdpd.main.rst
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      179 2020-11-18 23:42:17.000000 nrdp-daemon-1.0.9/doc-src/libnrdpd.error.rst
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      145 2020-11-20 20:50:41.000000 nrdp-daemon-1.0.9/doc-src/libnrdpd.task.rst
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      157 2020-11-20 21:17:52.000000 nrdp-daemon-1.0.9/doc-src/libnrdpd.schedule.rst
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      182 2020-11-18 23:47:26.000000 nrdp-daemon-1.0.9/doc-src/libnrdpd.config.rst
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      145 2020-11-19 17:30:05.000000 nrdp-daemon-1.0.9/doc-src/libnrdpd.util.rst
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)    11358 2020-07-30 19:40:08.000000 nrdp-daemon-1.0.9/LICENSE
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      499 2020-11-23 21:47:11.000000 nrdp-daemon-1.0.9/tox.ini
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)      521 2020-11-23 21:27:06.000000 nrdp-daemon-1.0.9/README.rst
+-rw-r--r--   0 blkmajik  (1000) blkmajik  (1000)       32 2020-11-20 22:52:36.000000 nrdp-daemon-1.0.9/requirements-doc.txt
```

### Comparing `nrdp-daemon-1.0.8/PKG-INFO` & `nrdp-daemon-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: nrdp-daemon
-Version: 1.0.8
+Version: 1.0.9
 Summary: Nagios Remote Data Processing Daemon
 Home-page: https://github.com/HopliteInd/nrdpd-daemon
 Author: Hoplite Industries, Inc.
 Maintainer: Shawn Michael
 Maintainer-email: smichael@hopliteindustries.com
 License: Apache 2.0
 Description: Nagios Remote Data Protocol Daemon
```

### Comparing `nrdp-daemon-1.0.8/docs/configuration.file.html` & `nrdp-daemon-1.0.9/docs/configuration.file.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/objects.inv` & `nrdp-daemon-1.0.9/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/search.html` & `nrdp-daemon-1.0.9/docs/search.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/libnrdpd.nrdp.html` & `nrdp-daemon-1.0.9/docs/libnrdpd.nrdp.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/index.html` & `nrdp-daemon-1.0.9/docs/index.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_static/language_data.js` & `nrdp-daemon-1.0.9/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_static/jquery-3.4.1.js` & `nrdp-daemon-1.0.9/docs/_static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_static/pygments.css` & `nrdp-daemon-1.0.9/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_static/alabaster.css` & `nrdp-daemon-1.0.9/docs/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_static/basic.css` & `nrdp-daemon-1.0.9/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_static/searchtools.js` & `nrdp-daemon-1.0.9/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_static/doctools.js` & `nrdp-daemon-1.0.9/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_static/jquery.js` & `nrdp-daemon-1.0.9/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_static/underscore.js` & `nrdp-daemon-1.0.9/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_static/underscore-1.3.1.js` & `nrdp-daemon-1.0.9/docs/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/configuration.html` & `nrdp-daemon-1.0.9/docs/configuration.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/libnrdpd.html` & `nrdp-daemon-1.0.9/docs/libnrdpd.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/libnrdpd.error.html` & `nrdp-daemon-1.0.9/docs/libnrdpd.error.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/py-modindex.html` & `nrdp-daemon-1.0.9/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/nrdpd.html` & `nrdp-daemon-1.0.9/docs/nrdpd.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/libnrdpd.util.html` & `nrdp-daemon-1.0.9/docs/libnrdpd.util.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/libnrdpd.config.html` & `nrdp-daemon-1.0.9/docs/libnrdpd.config.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/libnrdpd.task.html` & `nrdp-daemon-1.0.9/docs/libnrdpd.task.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/searchindex.js` & `nrdp-daemon-1.0.9/docs/searchindex.js`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_sources/configuration.file.rst.txt` & `nrdp-daemon-1.0.9/docs/_sources/configuration.file.rst.txt`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_sources/configuration.rst.txt` & `nrdp-daemon-1.0.9/docs/_sources/configuration.rst.txt`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_modules/index.html` & `nrdp-daemon-1.0.9/docs/_modules/index.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_modules/libnrdpd/schedule.html` & `nrdp-daemon-1.0.9/docs/_modules/libnrdpd/schedule.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_modules/libnrdpd/util.html` & `nrdp-daemon-1.0.9/docs/_modules/libnrdpd/util.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_modules/libnrdpd/task.html` & `nrdp-daemon-1.0.9/docs/_modules/libnrdpd/task.html`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 <span class="kn">import</span> <span class="nn">shlex</span>
 <span class="kn">import</span> <span class="nn">string</span>
 <span class="kn">import</span> <span class="nn">subprocess</span>
 <span class="kn">import</span> <span class="nn">time</span>
 
 <span class="c1"># Local imports</span>
 <span class="kn">from</span> <span class="nn">.</span> <span class="k">import</span> <span class="n">config</span>
-<span class="kn">from</span> <span class="nn">.</span> <span class="k">import</span> <span class="n">error</span>
 
 
 <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="vm">__name__</span><span class="p">)</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">NullHandler</span><span class="p">())</span>
 
 
 <div class="viewcode-block" id="Task"><a class="viewcode-back" href="../../libnrdpd.task.html#libnrdpd.task.Task">[docs]</a><span class="k">class</span> <span class="nc">Task</span><span class="p">:</span>  <span class="c1"># pylint: disable=R0902</span>
     <span class="sd">&quot;&quot;&quot;Definition of a task to run in the scheduler.&quot;&quot;&quot;</span>
```

#### html2text {}

```diff
@@ -21,15 +21,14 @@
 import shlex
 import string
 import subprocess
 import time
 
 # Local imports
 from . import config
-from . import error
 
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 
 _[_d_o_c_s_]class Task:  # pylint: disable=R0902
     """Definition of a task to run in the scheduler."""
```

### Comparing `nrdp-daemon-1.0.8/docs/_modules/libnrdpd/config.html` & `nrdp-daemon-1.0.9/docs/_modules/libnrdpd/config.html`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         <span class="bp">self</span><span class="o">.</span><span class="n">_servers</span> <span class="o">=</span> <span class="p">[]</span>  <span class="c1"># List of servers to publish to</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_token</span> <span class="o">=</span> <span class="kc">None</span>  <span class="c1"># Server authentication token</span>
         <span class="c1"># Default hostname comes from socket</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_hostname</span> <span class="o">=</span> <span class="n">socket</span><span class="o">.</span><span class="n">gethostname</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_cacert</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_ip</span> <span class="o">=</span> <span class="n">util</span><span class="o">.</span><span class="n">getip</span><span class="p">()</span>
 
-        <span class="bp">self</span><span class="o">.</span><span class="n">_cp</span> <span class="o">=</span> <span class="n">configparser</span><span class="o">.</span><span class="n">ConfigParser</span><span class="p">()</span>
+        <span class="bp">self</span><span class="o">.</span><span class="n">_cp</span> <span class="o">=</span> <span class="n">configparser</span><span class="o">.</span><span class="n">ConfigParser</span><span class="p">(</span><span class="n">interpolation</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_check_re</span> <span class="o">=</span> <span class="n">re</span><span class="o">.</span><span class="n">compile</span><span class="p">(</span><span class="s2">&quot;^[-: a-zA-Z0-9]+&quot;</span><span class="p">)</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_checks</span> <span class="o">=</span> <span class="p">{}</span>  <span class="c1"># Dictionry of checks.  key = name, value = Check</span>
 
         <span class="k">try</span><span class="p">:</span>
             <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">cfgfile</span><span class="p">,</span> <span class="nb">str</span><span class="p">):</span>
                 <span class="k">with</span> <span class="nb">open</span><span class="p">(</span><span class="n">cfgfile</span><span class="p">,</span> <span class="s2">&quot;r&quot;</span><span class="p">)</span> <span class="k">as</span> <span class="n">fobj</span><span class="p">:</span>
```

#### html2text {}

```diff
@@ -182,15 +182,15 @@
         self._servers = []  # List of servers to publish to
         self._token = None  # Server authentication token
         # Default hostname comes from socket
         self._hostname = socket.gethostname().split(".")[0]
         self._cacert = None
         self._ip = util.getip()
 
-        self._cp = configparser.ConfigParser()
+        self._cp = configparser.ConfigParser(interpolation=None)
         self._check_re = re.compile("^[-: a-zA-Z0-9]+")
 
         self._checks = {}  # Dictionry of checks.  key = name, value = Check
 
         try:
             if isinstance(cfgfile, str):
                 with open(cfgfile, "r") as fobj:
```

### Comparing `nrdp-daemon-1.0.8/docs/_modules/libnrdpd/nrdp.html` & `nrdp-daemon-1.0.9/docs/_modules/libnrdpd/nrdp.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_modules/libnrdpd/main.html` & `nrdp-daemon-1.0.9/docs/_modules/libnrdpd/main.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/_modules/libnrdpd/error.html` & `nrdp-daemon-1.0.9/docs/_modules/libnrdpd/error.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/libnrdpd.main.html` & `nrdp-daemon-1.0.9/docs/libnrdpd.main.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/genindex.html` & `nrdp-daemon-1.0.9/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/docs/libnrdpd.schedule.html` & `nrdp-daemon-1.0.9/docs/libnrdpd.schedule.html`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/nrdp_daemon.egg-info/PKG-INFO` & `nrdp-daemon-1.0.9/nrdp_daemon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: nrdp-daemon
-Version: 1.0.8
+Version: 1.0.9
 Summary: Nagios Remote Data Processing Daemon
 Home-page: https://github.com/HopliteInd/nrdpd-daemon
 Author: Hoplite Industries, Inc.
 Maintainer: Shawn Michael
 Maintainer-email: smichael@hopliteindustries.com
 License: Apache 2.0
 Description: Nagios Remote Data Protocol Daemon
```

### Comparing `nrdp-daemon-1.0.8/nrdp_daemon.egg-info/SOURCES.txt` & `nrdp-daemon-1.0.9/nrdp_daemon.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.rst
 pyproject.toml
 requirements-doc.txt
 setup.cfg
 setup.py
 tox.ini
 doc-src/conf.py
+doc-src/configuration.file.rst
 doc-src/configuration.rst
 doc-src/index.rst
 doc-src/libnrdpd.config.rst
 doc-src/libnrdpd.error.rst
 doc-src/libnrdpd.main.rst
 doc-src/libnrdpd.nrdp.rst
 doc-src/libnrdpd.rst
```

### Comparing `nrdp-daemon-1.0.8/setup.cfg` & `nrdp-daemon-1.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nrdp-daemon
-version = 1.0.8
+version = 1.0.9
 description = Nagios Remote Data Processing Daemon
 long_description = file: README.rst
 keywords = nrdp, nagios, passive
 license = Apache 2.0
 license_file = LICENSE
 author = Hoplite Industries, Inc.
 maintainer = Shawn Michael
```

### Comparing `nrdp-daemon-1.0.8/libnrdpd/task.py` & `nrdp-daemon-1.0.9/libnrdpd/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 import shlex
 import string
 import subprocess
 import time
 
 # Local imports
 from . import config
-from . import error
 
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 
 class Task:  # pylint: disable=R0902
     """Definition of a task to run in the scheduler."""
```

### Comparing `nrdp-daemon-1.0.8/libnrdpd/__init__.py` & `nrdp-daemon-1.0.9/libnrdpd/__init__.py`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/libnrdpd/util.py` & `nrdp-daemon-1.0.9/libnrdpd/util.py`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/libnrdpd/main.py` & `nrdp-daemon-1.0.9/libnrdpd/main.py`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/libnrdpd/config.py` & `nrdp-daemon-1.0.9/libnrdpd/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         self._servers = []  # List of servers to publish to
         self._token = None  # Server authentication token
         # Default hostname comes from socket
         self._hostname = socket.gethostname().split(".")[0]
         self._cacert = None
         self._ip = util.getip()
 
-        self._cp = configparser.ConfigParser()
+        self._cp = configparser.ConfigParser(interpolation=None)
         self._check_re = re.compile("^[-: a-zA-Z0-9]+")
 
         self._checks = {}  # Dictionry of checks.  key = name, value = Check
 
         try:
             if isinstance(cfgfile, str):
                 with open(cfgfile, "r") as fobj:
```

### Comparing `nrdp-daemon-1.0.8/libnrdpd/error.py` & `nrdp-daemon-1.0.9/libnrdpd/error.py`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/libnrdpd/nrdp.py` & `nrdp-daemon-1.0.9/libnrdpd/nrdp.py`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/libnrdpd/schedule.py` & `nrdp-daemon-1.0.9/libnrdpd/schedule.py`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/tests/test_util.py` & `nrdp-daemon-1.0.9/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/tests/test_config.py` & `nrdp-daemon-1.0.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/Makefile` & `nrdp-daemon-1.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/doc-src/conf.py` & `nrdp-daemon-1.0.9/doc-src/conf.py`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/doc-src/configuration.rst` & `nrdp-daemon-1.0.9/doc-src/configuration.rst`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/LICENSE` & `nrdp-daemon-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nrdp-daemon-1.0.8/README.rst` & `nrdp-daemon-1.0.9/README.rst`

 * *Files identical despite different names*

