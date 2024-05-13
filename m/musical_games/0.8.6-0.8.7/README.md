# Comparing `tmp/musical_games-0.8.6.tar.gz` & `tmp/musical_games-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musical_games-0.8.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "musical_games-0.8.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `musical_games-0.8.6.tar` & `musical_games-0.8.7.tar`

### file list

```diff
@@ -1,115 +1,117 @@
--rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.8.6/.coveragerc
--rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.8.6/.editorconfig
--rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.8.6/.gitchangelog.rc
--rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.8.6/.gitchangelog.tpl
--rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.8.6/.gitignore
--rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.8.6/.travis.yml
--rw-r--r--   0        0        0     2472 2024-05-11 19:28:08.211708 musical_games-0.8.6/CHANGELOG.rst
--rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.8.6/LICENSE
--rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.8.6/Makefile
--rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.8.6/README.rst
--rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.8.6/docs/Makefile
--rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.8.6/docs/authors.rst
--rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.8.6/docs/conf.py
--rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.8.6/docs/contributing.rst
--rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.8.6/docs/history.rst
--rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.8.6/docs/index.rst
--rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.8.6/docs/installation.rst
--rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.8.6/docs/make.bat
--rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.8.6/docs/modules.rst
--rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.8.6/docs/musical_games.converters.rst
--rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.8.6/docs/musical_games.dice_games.lilypond.rst
--rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.8.6/docs/musical_games.dice_games.rst
--rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.8.6/docs/musical_games.rst
--rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.8.6/docs/readme.rst
--rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.8.6/docs/usage.rst
--rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.8.6/musical_games/__init__.py
--rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.8.6/musical_games/__version__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.6/musical_games/data/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.8.6/musical_games/data/dice_games/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
--rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
--rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
--rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
--rw-r--r--   0        0        0     1426 2024-05-01 10:00:27.942474 musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     1773 2024-05-01 10:01:07.542475 musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     2987 2024-05-04 11:52:35.602498 musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      524 2024-05-01 10:01:25.466475 musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
--rw-r--r--   0        0        0      623 2024-05-01 10:01:48.778476 musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0      140 2024-04-30 09:20:04.502864 musical_games-0.8.6/musical_games/data/dice_games/gerlach_scottish_dance/__init__.py
--rw-r--r--   0        0        0     2202 2024-05-11 18:10:52.999832 musical_games-0.8.6/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     7480 2024-05-11 18:33:48.383795 musical_games-0.8.6/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     5795 2024-05-11 18:10:52.999832 musical_games-0.8.6/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1208 2024-05-01 12:32:39.650622 musical_games-0.8.6/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly
--rw-r--r--   0        0        0     2193 2024-05-11 18:10:52.999832 musical_games-0.8.6/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    18695 2024-05-11 18:10:52.999832 musical_games-0.8.6/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2515 2024-05-01 10:02:26.562476 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6430 2024-05-01 10:02:36.282477 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4303 2024-05-04 11:52:35.610498 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1115 2024-05-01 10:04:40.982478 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1313 2024-05-01 10:04:40.990478 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
--rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
--rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
--rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
--rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
--rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
--rw-r--r--   0        0        0     2867 2024-05-01 10:06:57.106481 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     4350 2024-05-01 10:06:57.126481 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3773 2024-05-04 11:54:20.298500 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1634 2024-05-01 10:06:57.134481 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
--rw-r--r--   0        0        0     2046 2024-05-01 10:06:57.086481 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.8.6/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
--rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.8.6/musical_games/data/dice_games/mozart_contredanse/__init__.py
--rw-r--r--   0        0        0     8219 2024-05-04 12:42:02.922546 musical_games-0.8.6/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
--rw-r--r--   0        0        0     1439 2024-05-04 12:39:21.850544 musical_games-0.8.6/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2929 2024-05-04 12:41:06.802545 musical_games-0.8.6/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4138 2024-05-04 12:41:06.842545 musical_games-0.8.6/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      892 2024-05-04 12:41:06.822545 musical_games-0.8.6/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.854545 musical_games-0.8.6/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.6/musical_games/data/dice_games/mozart_waltz/__init__.py
--rw-r--r--   0        0        0     1421 2024-05-04 12:21:30.450526 musical_games-0.8.6/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2847 2024-05-04 12:35:43.522540 musical_games-0.8.6/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4087 2024-05-04 12:35:43.510540 musical_games-0.8.6/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      892 2024-05-04 12:22:16.662527 musical_games-0.8.6/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.830545 musical_games-0.8.6/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0     9398 2024-05-04 12:21:02.330526 musical_games-0.8.6/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2534 2024-05-01 10:10:19.634484 musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6430 2024-05-01 10:11:25.454485 musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4406 2024-05-04 11:52:35.630499 musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1115 2024-05-01 10:11:25.482485 musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1313 2024-05-01 10:11:25.494485 musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0     2519 2024-05-11 18:10:52.999832 musical_games-0.8.6/musical_games/data/lilypond_utils/clef_changes.ly
--rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.8.6/musical_games/dice_games/__init__.py
--rw-r--r--   0        0        0    46961 2024-05-04 19:01:22.376069 musical_games-0.8.6/musical_games/dice_games/base.py
--rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.8.6/musical_games/dice_games/data_csv.py
--rw-r--r--   0        0        0    17130 2024-05-04 12:38:10.242543 musical_games-0.8.6/musical_games/dice_games/dice_games.py
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.8.6/musical_games/external/__init__.py
--rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.8.6/musical_games/external/base.py
--rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.8.6/musical_games/external/exceptions.py
--rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.8.6/musical_games/external/images.py
--rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.8.6/musical_games/external/lilypond.py
--rw-r--r--   0        0        0     4729 2024-05-11 19:28:01.583708 musical_games-0.8.6/musical_games/external/midi_converters.py
--rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.8.6/musical_games/external/utils.py
--rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.8.6/musical_games/external/wav_converters.py
--rw-r--r--   0        0        0     4835 2024-04-18 13:39:38.231087 musical_games-0.8.6/musical_games/utils.py
--rw-r--r--   0        0        0     1117 2024-05-11 19:28:08.111708 musical_games-0.8.6/pyproject.toml
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.8.6/scripts/__init__.py
--rw-r--r--   0        0        0     1995 2024-05-04 18:52:13.860087 musical_games-0.8.6/scripts/demo_cpe_bach.py
--rw-r--r--   0        0        0     2364 2024-05-11 18:33:48.383795 musical_games-0.8.6/scripts/demo_gerlach_scottish_dance.py
--rw-r--r--   0        0        0     2228 2024-05-04 18:39:35.968113 musical_games-0.8.6/scripts/demo_kirnberger_meneut_trio.py
--rw-r--r--   0        0        0     1896 2024-05-04 18:37:37.884117 musical_games-0.8.6/scripts/demo_kirnberger_polonaise.py
--rw-r--r--   0        0        0     1898 2024-05-04 18:42:20.816107 musical_games-0.8.6/scripts/demo_mozart_contredanse.py
--rw-r--r--   0        0        0     1852 2024-05-04 12:36:25.506541 musical_games-0.8.6/scripts/demo_mozart_waltz.py
--rw-r--r--   0        0        0     2329 2024-04-18 13:39:38.231087 musical_games-0.8.6/scripts/demo_stadler_meneut_trio.py
--rw-r--r--   0        0        0    26645 2024-04-30 09:20:04.502864 musical_games-0.8.6/scripts/lilypond_copy.py
--rw-r--r--   0        0        0    29517 2024-04-30 09:20:04.502864 musical_games-0.8.6/scripts/lilypond_copy2.py
--rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.8.6/tests/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.8.6/tox.ini
--rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 musical_games-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.8.7/.coveragerc
+-rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.8.7/.editorconfig
+-rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.8.7/.gitchangelog.rc
+-rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.8.7/.gitchangelog.tpl
+-rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.8.7/.gitignore
+-rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.8.7/.travis.yml
+-rw-r--r--   0        0        0     2663 2024-05-13 12:24:39.018715 musical_games-0.8.7/CHANGELOG.rst
+-rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.8.7/LICENSE
+-rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.8.7/Makefile
+-rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.8.7/README.rst
+-rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.8.7/docs/Makefile
+-rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.8.7/docs/authors.rst
+-rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.8.7/docs/conf.py
+-rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.8.7/docs/contributing.rst
+-rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.8.7/docs/history.rst
+-rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.8.7/docs/index.rst
+-rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.8.7/docs/installation.rst
+-rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.8.7/docs/make.bat
+-rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.8.7/docs/modules.rst
+-rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.8.7/docs/musical_games.converters.rst
+-rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.8.7/docs/musical_games.dice_games.lilypond.rst
+-rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.8.7/docs/musical_games.dice_games.rst
+-rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.8.7/docs/musical_games.rst
+-rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.8.7/docs/readme.rst
+-rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.8.7/docs/usage.rst
+-rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.8.7/musical_games/__init__.py
+-rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.8.7/musical_games/__version__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.7/musical_games/data/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.8.7/musical_games/data/dice_games/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
+-rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
+-rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
+-rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
+-rw-r--r--   0        0        0     1426 2024-05-01 10:00:27.942474 musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     1773 2024-05-01 10:01:07.542475 musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     2987 2024-05-04 11:52:35.602498 musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      524 2024-05-01 10:01:25.466475 musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
+-rw-r--r--   0        0        0      623 2024-05-01 10:01:48.778476 musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-30 09:20:04.502864 musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/__init__.py
+-rw-r--r--   0        0        0     2090 2024-05-13 12:13:58.026732 musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6491 2024-05-13 12:17:10.910727 musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     6036 2024-05-13 12:15:29.774729 musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1192 2024-05-13 12:05:01.354746 musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     2177 2024-05-13 12:06:47.754743 musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    18701 2024-05-13 10:45:03.550875 musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv
+-rw-r--r--   0        0        0     2459 2024-05-13 11:45:11.074778 musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars_annotations.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2515 2024-05-01 10:02:26.562476 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6430 2024-05-01 10:02:36.282477 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4303 2024-05-04 11:52:35.610498 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1115 2024-05-01 10:04:40.982478 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1313 2024-05-01 10:04:40.990478 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
+-rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
+-rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
+-rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
+-rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
+-rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
+-rw-r--r--   0        0        0     2867 2024-05-01 10:06:57.106481 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     4350 2024-05-01 10:06:57.126481 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3773 2024-05-04 11:54:20.298500 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1634 2024-05-01 10:06:57.134481 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     2046 2024-05-01 10:06:57.086481 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.8.7/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.8.7/musical_games/data/dice_games/mozart_contredanse/__init__.py
+-rw-r--r--   0        0        0     8219 2024-05-04 12:42:02.922546 musical_games-0.8.7/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
+-rw-r--r--   0        0        0     1439 2024-05-04 12:39:21.850544 musical_games-0.8.7/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2929 2024-05-04 12:41:06.802545 musical_games-0.8.7/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4138 2024-05-04 12:41:06.842545 musical_games-0.8.7/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      892 2024-05-04 12:41:06.822545 musical_games-0.8.7/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.854545 musical_games-0.8.7/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.7/musical_games/data/dice_games/mozart_waltz/__init__.py
+-rw-r--r--   0        0        0     1421 2024-05-04 12:21:30.450526 musical_games-0.8.7/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2847 2024-05-04 12:35:43.522540 musical_games-0.8.7/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4087 2024-05-04 12:35:43.510540 musical_games-0.8.7/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      892 2024-05-04 12:22:16.662527 musical_games-0.8.7/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.830545 musical_games-0.8.7/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     9398 2024-05-04 12:21:02.330526 musical_games-0.8.7/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2534 2024-05-01 10:10:19.634484 musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6430 2024-05-01 10:11:25.454485 musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4406 2024-05-04 11:52:35.630499 musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1115 2024-05-01 10:11:25.482485 musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1313 2024-05-01 10:11:25.494485 musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0     2519 2024-05-11 18:10:52.999832 musical_games-0.8.7/musical_games/data/lilypond_utils/clef_changes.ly
+-rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.8.7/musical_games/dice_games/__init__.py
+-rw-r--r--   0        0        0    47869 2024-05-13 11:49:20.154771 musical_games-0.8.7/musical_games/dice_games/base.py
+-rw-r--r--   0        0        0     5245 2024-05-13 11:51:34.062768 musical_games-0.8.7/musical_games/dice_games/data_csv.py
+-rw-r--r--   0        0        0    18124 2024-05-13 12:22:30.874718 musical_games-0.8.7/musical_games/dice_games/dice_games.py
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.8.7/musical_games/external/__init__.py
+-rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.8.7/musical_games/external/base.py
+-rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.8.7/musical_games/external/exceptions.py
+-rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.8.7/musical_games/external/images.py
+-rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.8.7/musical_games/external/lilypond.py
+-rw-r--r--   0        0        0     4765 2024-05-13 08:28:35.139095 musical_games-0.8.7/musical_games/external/midi_converters.py
+-rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.8.7/musical_games/external/utils.py
+-rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.8.7/musical_games/external/wav_converters.py
+-rw-r--r--   0        0        0     4835 2024-04-18 13:39:38.231087 musical_games-0.8.7/musical_games/utils.py
+-rw-r--r--   0        0        0     1117 2024-05-13 12:24:38.902715 musical_games-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.8.7/scripts/__init__.py
+-rw-r--r--   0        0        0     1995 2024-05-04 18:52:13.860087 musical_games-0.8.7/scripts/demo_cpe_bach.py
+-rw-r--r--   0        0        0     2364 2024-05-13 12:18:24.734725 musical_games-0.8.7/scripts/demo_gerlach_scottish_dance.py
+-rw-r--r--   0        0        0     2228 2024-05-04 18:39:35.968113 musical_games-0.8.7/scripts/demo_kirnberger_meneut_trio.py
+-rw-r--r--   0        0        0     1896 2024-05-04 18:37:37.884117 musical_games-0.8.7/scripts/demo_kirnberger_polonaise.py
+-rw-r--r--   0        0        0     1898 2024-05-04 18:42:20.816107 musical_games-0.8.7/scripts/demo_mozart_contredanse.py
+-rw-r--r--   0        0        0     1852 2024-05-04 12:36:25.506541 musical_games-0.8.7/scripts/demo_mozart_waltz.py
+-rw-r--r--   0        0        0     2329 2024-04-18 13:39:38.231087 musical_games-0.8.7/scripts/demo_stadler_meneut_trio.py
+-rw-r--r--   0        0        0    26645 2024-04-30 09:20:04.502864 musical_games-0.8.7/scripts/lilypond_copy.py
+-rw-r--r--   0        0        0    29517 2024-04-30 09:20:04.502864 musical_games-0.8.7/scripts/lilypond_copy2.py
+-rw-r--r--   0        0        0     1092 2024-05-13 10:54:13.630860 musical_games-0.8.7/scripts/make_annotation.py
+-rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.8.7/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.8.7/tox.ini
+-rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 musical_games-0.8.7/PKG-INFO
```

### Comparing `musical_games-0.8.6/.gitchangelog.rc` & `musical_games-0.8.7/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/.gitignore` & `musical_games-0.8.7/.gitignore`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/CHANGELOG.rst` & `musical_games-0.8.7/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 *********
 Changelog
 *********
 
+v0.8.7 (2024-05-13)
+===================
+
+Added
+-----
+- Adds annotation data to the bars, enabling more information in the renderers.
+
+Other
+-----
+- Increased volume of timidity conversion.
+
+
 v0.8.6 (2024-05-11)
 ===================
 
 Changed
 -------
 - Changed the order of the midi converters to have timidity first. This because in fluidsynth 2.3.1 there is a strange pauze at the end of the tracks.
```

### Comparing `musical_games-0.8.6/LICENSE` & `musical_games-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/Makefile` & `musical_games-0.8.7/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/README.rst` & `musical_games-0.8.7/README.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/docs/Makefile` & `musical_games-0.8.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/docs/conf.py` & `musical_games-0.8.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/docs/contributing.rst` & `musical_games-0.8.7/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/docs/index.rst` & `musical_games-0.8.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/docs/make.bat` & `musical_games-0.8.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/docs/musical_games.converters.rst` & `musical_games-0.8.7/docs/musical_games.converters.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/docs/musical_games.dice_games.lilypond.rst` & `musical_games-0.8.7/docs/musical_games.dice_games.lilypond.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/docs/musical_games.dice_games.rst` & `musical_games-0.8.7/docs/musical_games.dice_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/docs/musical_games.rst` & `musical_games-0.8.7/docs/musical_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/__version__.py` & `musical_games-0.8.7/musical_games/__version__.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv` & `musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv` & `musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv` & `musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly` & `musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly` & `musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly` & `musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly` & `musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly` & `musical_games-0.8.7/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly` & `musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly`

 * *Files 22% similar despite different names*

```diff
@@ -42,27 +42,26 @@
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c \major
             }
             {
                 \clef bass
                 \time 2/4
+                \BLOCK{ set loop_data = namespace(previous_bar=None) }
                 \BLOCK{ for bar_ind, bar in bar_collections['dance'].get_bars('piano_left_hand').items() }
-                    \BLOCK{ if bar.lilypond_str.startswith('\clef "treble"') or bar.lilypond_str.startswith('\clefBracketed "treble"')}
+                    \BLOCK{ if bar.get_annotation().has_clef_change }
                         \set Staff.forceClef = ##t
                         \VAR{bar.lilypond_str}
-                        \BLOCK{ if not bar_collections['dance'].get_bars('piano_left_hand')[bar_ind + 1].lilypond_str.startswith('\clef') }
-                            \clefBracketed "bass"
-                        \BLOCK{ endif }
-                    \BLOCK{ elif bar.lilypond_str.startswith('\clef "bass"') }
-                        \set Staff.forceClef = ##t
+                    \BLOCK{ elif loop_data.previous_bar is not none and loop_data.previous_bar.get_annotation().has_clef_change }
+                        \clefBracketed "bass"
                         \VAR{bar.lilypond_str}
                     \BLOCK{ else }
-                    \VAR{bar.lilypond_str}
+                        \VAR{bar.lilypond_str}
                     \BLOCK{endif}
+                    \BLOCK{ set loop_data.previous_bar = bar }
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
     \layout {
         indent = #0
```

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly` & `musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly`

 * *Files 8% similar despite different names*

```diff
@@ -116,37 +116,21 @@
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
                 \time 2/4
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
-		                \BLOCK{ set bar = composition_bars['trio'][bar_index].get_bar('piano_left_hand') }
-		                \BLOCK{ if bar.lilypond_str.startswith('\clef') }
-                            \VAR{bar.lilypond_str}
-                            \BLOCK{ if bar_index != 7 and not composition_bars['trio'][bar_index + 1].get_bar('piano_left_hand').lilypond_str.startswith('\clef') }
-                                \clef "bass"
-                            \BLOCK{ endif }
-                        \BLOCK{ else }
-                        \VAR{bar.lilypond_str}
-                        \BLOCK{endif}
+    		            \VAR{composition_bars['trio'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 	        	\clef bass
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
-    		            \BLOCK{ set bar = composition_bars['trio'][bar_index].get_bar('piano_left_hand') }
-		                \BLOCK{ if bar.lilypond_str.startswith('\clef') }
-		                    \VAR{bar.lilypond_str}
-                            \BLOCK{ if bar_index != 15 and not composition_bars['trio'][bar_index + 1].get_bar('piano_left_hand').lilypond_str.startswith('\clef') }
-                                \clef "bass"
-                            \BLOCK{ endif }
-                        \BLOCK{ else }
-                        \VAR{bar.lilypond_str}
-                        \BLOCK{endif}
+    		            \VAR{composition_bars['trio'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
             }
         >>
     >>
     \midi { }
 }
```

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly` & `musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly`

 * *Files 16% similar despite different names*

```diff
@@ -113,42 +113,46 @@
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
                 \time 2/4
 		        \repeat volta 2{
+		            \BLOCK{ set loop_data = namespace(previous_bar=None) }
 		            \BLOCK{ for bar_index in range(8) }
 		                \BLOCK{ set bar = composition_bars['trio'][bar_index].get_bar('piano_left_hand') }
-		                \BLOCK{ if bar.lilypond_str.startswith('\clef') }
+		                \BLOCK{ if bar.get_annotation().has_clef_change }
                             \clefAfterBarOnce
                             \set Staff.forceClef = ##t
                             \VAR{bar.lilypond_str}
-                            \BLOCK{ if bar_index != 7 and not composition_bars['trio'][bar_index + 1].get_bar('piano_left_hand').lilypond_str.startswith('\clef') }
-                                \set Staff.forceClef = ##t \clefAfterBarOnce \clefBracketed "bass"
-                            \BLOCK{ endif }
+                        \BLOCK{ elif loop_data.previous_bar is not none and loop_data.previous_bar.get_annotation().has_clef_change }
+                            \set Staff.forceClef = ##t \clefAfterBarOnce \clefBracketed "bass"
+                            \VAR{bar.lilypond_str}
                         \BLOCK{ else }
-                        \VAR{bar.lilypond_str}
+                            \VAR{bar.lilypond_str}
                         \BLOCK{endif}
+                        \BLOCK{ set loop_data.previous_bar = bar}
     		        \BLOCK{ endfor }
 	        	}
 	        	\clef bass
 		        \repeat volta 2{
+		            \BLOCK{ set loop_data = namespace(previous_bar=None) }
     		        \BLOCK{ for bar_index in range(8, 16) }
     		            \BLOCK{ set bar = composition_bars['trio'][bar_index].get_bar('piano_left_hand') }
-		                \BLOCK{ if bar.lilypond_str.startswith('\clef') }
-		                    \clefAfterBarOnce
-		                    \set Staff.forceClef = ##t
-		                    \VAR{bar.lilypond_str}
-                            \BLOCK{ if bar_index != 15 and not composition_bars['trio'][bar_index + 1].get_bar('piano_left_hand').lilypond_str.startswith('\clef') }
-                                \set Staff.forceClef = ##t \clefAfterBarOnce \clefBracketed "bass"
-                            \BLOCK{ endif }
+		                \BLOCK{ if bar.get_annotation().has_clef_change }
+                            \clefAfterBarOnce
+                            \set Staff.forceClef = ##t
+                            \VAR{bar.lilypond_str}
+                        \BLOCK{ elif loop_data.previous_bar is not none and loop_data.previous_bar.get_annotation().has_clef_change }
+                            \set Staff.forceClef = ##t \clefAfterBarOnce \clefBracketed "bass"
+                            \VAR{bar.lilypond_str}
                         \BLOCK{ else }
-                        \VAR{bar.lilypond_str}
+                            \VAR{bar.lilypond_str}
                         \BLOCK{endif}
+                        \BLOCK{ set loop_data.previous_bar = bar}
     		        \BLOCK{ endfor }
 	        	}
 		        \once \override Score.RehearsalMark #'self-alignment-X = #right \mark \markup {\fontsize #-1 \italic "D.C. al Fine"}
             }
         >>
     >>
     \layout {
```

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly` & `musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly`

 * *Files 14% similar despite different names*

```diff
@@ -28,17 +28,17 @@
         >>
         \new Staff
         <<
             {
                 \key c \major
             }
             {
-                \BLOCK{ if synchronous_bar.get_bar('piano_left_hand').lilypond_str.startswith('\clef "treble"') }
+                \BLOCK{ if synchronous_bar.get_bar('piano_left_hand').get_annotation().clef == 'treble' }
                     \bassToTreble
-                \BLOCK{ elif synchronous_bar.get_bar('piano_left_hand').lilypond_str.startswith('\clef "bass"') }
+                \BLOCK{ elif synchronous_bar.get_bar('piano_left_hand').get_annotation().clef == 'bass' }
                     \bassToBass
                 \BLOCK{ else }
                     \bass
                 \BLOCK{ endif }
                 \time 2/4
                 \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
                 \bar "|."
```

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly` & `musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly`

 * *Files 18% similar despite different names*

```diff
@@ -30,33 +30,33 @@
         >>
         \new Staff
         <<
             {
                 \key c \major
             }
             {
-                \BLOCK{ if synchronous_bars|length > 0 and synchronous_bars[0].get_bar('piano_left_hand').lilypond_str.startswith('\clef "treble"') }
+                \BLOCK{ if synchronous_bars|length > 0 and synchronous_bars[0].get_bar('piano_left_hand').get_annotation().clef == 'treble' }
                     \bassToTreble
-                \BLOCK{ elif synchronous_bars|length > 0 and synchronous_bars[0].get_bar('piano_left_hand').lilypond_str.startswith('\clef "bass"') }
+                \BLOCK{ elif synchronous_bars|length > 0 and synchronous_bars[0].get_bar('piano_left_hand').get_annotation().clef == 'bass' }
                     \bassToBass
                 \BLOCK{ else }
                     \clef bass
                 \BLOCK{ endif }
                 \time 2/4
 
                 \BLOCK{ for synchronous_bar in synchronous_bars }
                 \BLOCK{ set bar = synchronous_bar.get_bar('piano_left_hand') }
                 \BLOCK{ set has_next = loop.index0 != synchronous_bars|length - 1 }
                 \BLOCK{ if has_next }
                 \BLOCK{ set next_bar = synchronous_bars[loop.index0 + 1].get_bar('piano_left_hand') }
                 \BLOCK{ endif }
-                \BLOCK{ if bar.lilypond_str.startswith('\clef') }
+                \BLOCK{ if bar.get_annotation().has_clef_change }
                     \set Staff.forceClef = ##t
                     \VAR{ bar.lilypond_str }
-                    \BLOCK{ if has_next and not next_bar.lilypond_str.startswith('\clef') }
+                    \BLOCK{ if has_next and not next_bar.get_annotation().has_clef_change }
                        \clefAfterBarOnce \clefBracketed "bass"
                     \BLOCK{ endif }
                 \BLOCK{ else }
                     \VAR{ bar.lilypond_str }
                 \BLOCK{endif}
                 \BLOCK{ endfor }
                 \bar "|."
```

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv` & `musical_games-0.8.7/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"bar_index",piano_right_hand,"piano_left_hand"
-"1",d''16 [e''16 f''16 d''16] b'8 [d''8],"{<<{\voiceOne r8 <b f'>8 <d' f'>8 [<b f'>8]} \new Voice {\voiceTwo g2}>>}"
-"2",a''16 [gis''16 a''16 b''16] c'''8 [d'''8],"a8 [<c' e'>8] d8 [<a d'>8]"
+"bar_index","piano_right_hand","piano_left_hand"
+"1","d''16 [e''16 f''16 d''16] b'8 [d''8]","{<<{\voiceOne r8 <b f'>8 <d' f'>8 [<b f'>8]} \new Voice {\voiceTwo g2}>>}"
+"2","a''16 [gis''16 a''16 b''16] c'''8 [d'''8]","a8 [<c' e'>8] d8 [<a d'>8]"
 "3","<c'' g''>8 [<c'' fis''>8] <b' g''>4","<g d'>8 [<a d'>8] <g d'>4"
 "4","g'8 [c''16 d''16] e''16 [f''16 g''8]","e8 [g8] c'8 [e'8]"
 "5",e''8. [d''16 b'8 b'8],"\clef ""treble"" {<<{\voiceOne r8 <b e'>8 <d' e'>8 [<d' e'>8]} \new Voice {\voiceTwo gis2}>>}"
 "6","cis''16 [cis''16 e''16 cis''16] a'8 [e''8]","\clef ""bass"" {<<{\voiceOne r8 <e' g'>8 <cis' g'>8 [<cis' g'>8]} \new Voice {\voiceTwo a2}>>}"
 "7","c''8 [<g' e''>8] <e' c''>4","<c' e'>8 [c'8] c4"
 "8","c''8 [c''16 b'16] a'8 [e'8]","a,8 [<a c'>8] <a c'>8 [<a c'>8]"
 "9","b'8 [a''8] g''8 [f''8]","{<<{\voiceOne r8 <b d'>8 <b d'>8 [<b d'>8]} \new Voice {\voiceTwo g2}>>}"
```

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv` & `musical_games-0.8.7/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv` & `musical_games-0.8.7/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly` & `musical_games-0.8.7/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly` & `musical_games-0.8.7/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly` & `musical_games-0.8.7/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly` & `musical_games-0.8.7/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly` & `musical_games-0.8.7/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly` & `musical_games-0.8.7/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly` & `musical_games-0.8.7/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly` & `musical_games-0.8.7/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly` & `musical_games-0.8.7/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly` & `musical_games-0.8.7/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv` & `musical_games-0.8.7/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly` & `musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv` & `musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv` & `musical_games-0.8.7/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/data/lilypond_utils/clef_changes.ly` & `musical_games-0.8.7/musical_games/data/lilypond_utils/clef_changes.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/dice_games/base.py` & `musical_games-0.8.7/musical_games/dice_games/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,14 +413,35 @@
     def lilypond_str(self) -> str:
         """Get a representation of this bar as a lilypond string.
 
         Returns:
             A lilypond string of a single bar.
         """
 
+    @abstractmethod
+    def get_annotation(self) -> BarAnnotation:
+        """Get annotation data for this bar.
+
+        In addition to the raw lilypond data, it is convenient to store some annotation data next to it. The exact
+        data may be dice game dependent, as long as is it inherits from :class:`BarAnnotation`.
+
+        Returns:
+            A bar annotation object.
+        """
+
+
+class BarAnnotation(metaclass=ABCMeta):
+    """Annotation data for a single bar.
+
+    A :class:`Bar` object contains a lilypond string representing the musical data for that bar. In addition, we may
+    store annotation data covering data about the lilypond data.
+
+    The exact implementation may be different for each dice game.
+    """
+
 
 class SynchronousBar(metaclass=ABCMeta):
     """Representation of a list of bars played synchronously across staffs.
 
     Suppose that a piece has a piano and a violin, then at each time point there are three bars being played, left and
     right hand piano and the violin. These synchronous bars are connected in this class. For clarity, the different
     bars should be stored in a dictionary with their staff name as key.
@@ -571,16 +592,21 @@
 
 @dataclass(frozen=True, slots=True)
 class SimpleBar(Bar):
     """Dataclass representation of a single bar, of a single staff.
 
     Args:
         lilypond_str: the lilypond string representation of this bar
+        annotation: optional bar annotation object.
     """
     lilypond_str: str
+    annotation: BarAnnotation | None = None
+
+    def get_annotation(self) -> BarAnnotation:
+        return self.annotation
 
 
 @dataclass(frozen=True, slots=True)
 class SimpleSynchronousBar(SynchronousBar):
     """Representation of a bar across staffs.
 
     Args:
```

### Comparing `musical_games-0.8.6/musical_games/dice_games/dice_games.py` & `musical_games-0.8.7/musical_games/dice_games/dice_games.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 __author__ = 'Robbert Harms'
 __date__ = '2024-04-09'
 __maintainer__ = 'Robbert Harms'
 __email__ = 'robbert@xkls.nl'
 __licence__ = 'LGPL v3'
 
+import json
 import re
+from dataclasses import dataclass
 from importlib import resources
 
-import jinja2
-
-from musical_games.dice_games.base import (SimpleDiceTable, SimpleMidiSettings, SimpleDiceGame)
-from musical_games.dice_games.data_csv import SimpleBarCollectionCSVReader
+from musical_games.dice_games.base import (SimpleDiceTable, SimpleMidiSettings, SimpleDiceGame, BarAnnotation)
+from musical_games.dice_games.data_csv import CSVBarCollectionLoader, AnnotationLoader
 
 
 class CPEBachCounterpoint(SimpleDiceGame):
 
     def __init__(self):
         """Implementation of a Counterpoint dice by C.P.E. Bach.
 
@@ -41,19 +41,18 @@
                 [6, 15, 24, 33, 42, 51],
                 [7, 16, 25, 34, 43, 52],
                 [8, 17, 26, 35, 44, 53],
                 [9, 18, 27, 36, 45, 54]]),
         }
         data_name = 'cpe_bach_counterpoint'
 
-        csv_reader = SimpleBarCollectionCSVReader()
-        treble_bars = csv_reader.read_csv(resources.files('musical_games')
-                                          / f'data/dice_games/{data_name}/bars_treble.csv')
-        bass_bars = csv_reader.read_csv(resources.files('musical_games')
-                                        / f'data/dice_games/{data_name}/bars_bass.csv')
+        treble_bars = CSVBarCollectionLoader(resources.files('musical_games')
+                                             / f'data/dice_games/{data_name}/bars_treble.csv').load_data()
+        bass_bars = CSVBarCollectionLoader(resources.files('musical_games')
+                                           / f'data/dice_games/{data_name}/bars_bass.csv').load_data()
 
         midi_settings = SimpleMidiSettings(
             {'treble': {'piano_right_hand': 'acoustic grand'}, 'bass': {'piano_left_hand': 'acoustic grand'}},
             {'treble': {'piano_right_hand': 0}, 'bass': {'piano_left_hand': 0}},
             {'treble': {'piano_right_hand': 1}, 'bass': {'piano_left_hand': 0.75}})
 
         super().__init__('C.P.E. Bach', 'Counterpoint', dice_tables, {'treble': treble_bars, 'bass': bass_bars},
@@ -81,19 +80,18 @@
                 [8, 69, 26, 53, 43, 95, 88, 63, 79, 5, 3, 60, 54, 21, 42, 82],
                 [84, 6, 4, 22, 51, 12, 83, 92, 58, 93, 66, 23, 15, 13, 27, 32],
                 [39, 28, 18, 35, 89, 75, 61, 96, 7, 91, 70, 1, 74, 44, 52, 50],
                 [59, 71, 37, 16, 86, 49, 77, 20, 38, 68, 19, 29, 80, 36, 34, 9]]),
         }
         data_name = 'kirnberger_menuet_trio'
 
-        csv_reader = SimpleBarCollectionCSVReader()
-        bar_collections = {'menuet': csv_reader.read_csv(resources.files('musical_games') /
-                                                         f'data/dice_games/{data_name}/menuet_bars.csv'),
-                           'trio': csv_reader.read_csv(resources.files('musical_games') /
-                                                       f'data/dice_games/{data_name}/trio_bars.csv')}
+        bar_collections = {'menuet': CSVBarCollectionLoader(resources.files('musical_games') /
+                                                            f'data/dice_games/{data_name}/menuet_bars.csv').load_data(),
+                           'trio': CSVBarCollectionLoader(resources.files('musical_games') /
+                                                          f'data/dice_games/{data_name}/trio_bars.csv').load_data()}
 
         midi_settings = SimpleMidiSettings(
             {'menuet': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'},
              'trio': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
             {'menuet': {'piano_right_hand': 0, 'piano_left_hand': 0},
              'trio': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'menuet': {'piano_right_hand': 1, 'piano_left_hand': 0.75},
@@ -122,17 +120,18 @@
                 [123, 116, 137, 110, 91, 98, 129, 99, 107, 122, 105, 93, 106, 121],
                 [131, 147, 143, 113, 101, 115, 103, 140, 111, 145, 133, 109, 117, 125],
                 [138, 151, 118, 124, 141, 127, 142, 149, 97, 134, 120, 100, 119, 132],
                 [144, 153, 146, 128, 150, 154, 152, 102, 135, 148, 136, 108, 130, 139]])
         }
         data_name = 'kirnberger_polonaise'
 
-        csv_reader = SimpleBarCollectionCSVReader()
-        bar_collections = {'polonaise': csv_reader.read_csv(resources.files('musical_games') /
-                                                            f'data/dice_games/{data_name}/polonaise_bars.csv')}
+        bar_collections = {
+            'polonaise': CSVBarCollectionLoader(resources.files('musical_games') /
+                                                f'data/dice_games/{data_name}/polonaise_bars.csv').load_data()
+        }
 
         midi_settings = SimpleMidiSettings(
             {'polonaise': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand',
                            'violin_1': 'Violin', 'violin_2': 'Violin'}},
             {'polonaise': {'piano_right_hand': 0, 'piano_left_hand': 0,
                            'violin_1': 0, 'violin_2': 0}},
             {'polonaise': {'piano_right_hand': 0.75, 'piano_left_hand': 0.6,
@@ -158,17 +157,18 @@
                 [142, 106, 40, 69, 43, 140, 23, 89, 66, 124, 26, 84, 75, 103, 96, 127],
                 [99, 68, 86, 139, 120, 92, 143, 83, 93, 55, 29, 51, 42, 110, 108, 98],
                 [85, 45, 90, 158, 82, 123, 78, 58, 61, 34, 119, 46, 59, 54, 60, 47],
                 [145, 97, 6, 121, 56, 67, 63, 16, 50, 79, 175, 76, 113, 88, 53, 118]])
         }
         data_name = 'mozart_contredanse'
 
-        csv_reader = SimpleBarCollectionCSVReader()
-        bar_collections = {'contredanse': csv_reader.read_csv(resources.files('musical_games') /
-                                                        f'data/dice_games/{data_name}/contredanse_bars.csv')}
+        bar_collections = {
+            'contredanse': CSVBarCollectionLoader(resources.files('musical_games') /
+                                                  f'data/dice_games/{data_name}/contredanse_bars.csv').load_data()
+        }
 
         midi_settings = SimpleMidiSettings(
             {'contredanse': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
             {'contredanse': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'contredanse': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
 
         def split_voices(voices):
@@ -197,17 +197,16 @@
                 [119, 84, 114, 50, 140, 86, 169, 94, 120, 88, 48, 166, 51, 115, 72, 111],
                 [98, 142, 42, 156, 75, 129, 62, 123, 65, 77, 19, 82, 137, 38, 149, 8],
                 [3, 87, 165, 61, 135, 47, 147, 33, 102, 4, 31, 164, 144, 59, 173, 78],
                 [54, 130, 10, 103, 28, 37, 106, 5, 35, 20, 108, 92, 12, 124, 44, 131]])
         }
         data_name = 'mozart_waltz'
 
-        csv_reader = SimpleBarCollectionCSVReader()
-        bar_collections = {'waltz': csv_reader.read_csv(resources.files('musical_games') /
-                                                        f'data/dice_games/{data_name}/waltz_bars.csv')}
+        bar_collections = {'waltz': CSVBarCollectionLoader(resources.files('musical_games') /
+                                                           f'data/dice_games/{data_name}/waltz_bars.csv').load_data()}
 
         midi_settings = SimpleMidiSettings(
             {'waltz': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
             {'waltz': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'waltz': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
 
         def split_voices(voices):
@@ -248,19 +247,18 @@
                 [75, 39, 54, 1, 65, 43, 15, 80, 9, 34, 93, 48, 69, 58, 90, 21],
                 [40, 73, 16, 68, 29, 55, 2, 61, 22, 67, 49, 77, 57, 87, 33, 10],
                 [83, 3, 28, 53, 37, 17, 44, 70, 63, 85, 32, 96, 12, 23, 50, 91],
                 [18, 45, 62, 38, 4, 27, 52, 94, 11, 92, 24, 86, 51, 60, 78, 31]]),
         }
         data_name = 'stadler_menuet_trio'
 
-        csv_reader = SimpleBarCollectionCSVReader()
-        bar_collections = {'menuet': csv_reader.read_csv(resources.files('musical_games') /
-                                                         f'data/dice_games/{data_name}/menuet_bars.csv'),
-                           'trio': csv_reader.read_csv(resources.files('musical_games') /
-                                                       f'data/dice_games/{data_name}/trio_bars.csv')}
+        bar_collections = {'menuet': CSVBarCollectionLoader(resources.files('musical_games') /
+                                                            f'data/dice_games/{data_name}/menuet_bars.csv').load_data(),
+                           'trio': CSVBarCollectionLoader(resources.files('musical_games') /
+                                                          f'data/dice_games/{data_name}/trio_bars.csv').load_data()}
 
         midi_settings = SimpleMidiSettings(
             {'menuet': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'},
              'trio': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
             {'menuet': {'piano_right_hand': 0, 'piano_left_hand': 0},
              'trio': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'menuet': {'piano_right_hand': 1, 'piano_left_hand': 0.75},
@@ -288,24 +286,49 @@
                 [(43, 57), (135, 188), (56, 18), (189, 163), (25, 38), (166, 122), (179, 123), (169, 53)],
                 [(181, 129), (131, 186), (115, 170), (62, 178), (183, 132), (168, 171), (81, 151), (158, 64)],
                 [(134, 26), (118, 184), (160, 140), (114, 34), (42, 164), (146, 83), (141, 162), (73, 153)],
                 [(79, 191), (121, 155), (138, 156), (16, 173), (133, 167), (142, 172), (147, 159), (152, 157)]]),
         }
         data_name = 'gerlach_scottish_dance'
 
-        csv_reader = SimpleBarCollectionCSVReader()
-        bars = csv_reader.read_csv(resources.files('musical_games') /
-                                   f'data/dice_games/{data_name}/scottish_dance_bars.csv')
+        csv_reader = CSVBarCollectionLoader(
+            resources.files('musical_games') / f'data/dice_games/{data_name}/scottish_dance_bars.csv',
+            annotation_data_csv=resources.files('musical_games') /
+                                f'data/dice_games/{data_name}/scottish_dance_bars_annotations.csv',
+            annotation_loader=GerlachScottishDance.GerlachAnnotationLoader()
+        )
+        bars = csv_reader.load_data()
 
         bar_collections = {'dance': bars,
                            'trio': bars}
 
         midi_settings = SimpleMidiSettings(
             {'dance': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'},
              'trio': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
             {'dance': {'piano_right_hand': 0, 'piano_left_hand': 0},
              'trio': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'dance': {'piano_right_hand': 1, 'piano_left_hand': 0.75},
              'trio': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
 
         super().__init__('Gerlach', 'Scottish dance', dice_tables, bar_collections,
                          self._generate_jinja2_environment(data_name), midi_settings)
+
+    @dataclass(frozen=True, slots=True)
+    class GerlachAnnotation(BarAnnotation):
+        """Annotation for a bar in the Gerlach dice game.
+
+        The only annotation is the presence of a clef change at the beginning of a bar.
+
+        Args:
+            has_clef_change: if the annotated bar has a clef change at the beginning
+            clef: a string literal if there is a clef change at the beginning of this bar
+        """
+        has_clef_change: bool
+        clef: str | None
+
+    class GerlachAnnotationLoader(AnnotationLoader):
+
+        def load_annotation(self, input_data: str) -> BarAnnotation:
+            if input_data == '':
+                return GerlachScottishDance.GerlachAnnotation(False, None)
+            else:
+                return GerlachScottishDance.GerlachAnnotation(True, json.loads(input_data)['clef'])
```

### Comparing `musical_games-0.8.6/musical_games/external/base.py` & `musical_games-0.8.7/musical_games/external/base.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/external/images.py` & `musical_games-0.8.7/musical_games/external/images.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/external/lilypond.py` & `musical_games-0.8.7/musical_games/external/lilypond.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/external/midi_converters.py` & `musical_games-0.8.7/musical_games/external/midi_converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,20 +123,21 @@
             # Set chorus and reverb by song & soundfont
             opt EFreverb=1
             opt EFchorus=1
 
             # Never kill voices to save CPU
             opt -k0
 
-            # Sustain fades after three seconds (3000ms)
+            # Sustain fades after three seconds (1500ms)
             opt -m3000
         ''')
         if self._soundfont:
             self._timidity_config += f'soundfont {str(self._soundfont)}'
 
     def call(self, midi_in: Path, wav_out: Path, gain: float | None = None) -> None:
+        gain = gain or 0.1
         wav_out.parent.mkdir(parents=True, exist_ok=True)
 
         with tempfile.NamedTemporaryFile('w') as tmp_file:
             tmp_file.write(self._timidity_config)
             tmp_file.flush()
-            run_command(['timidity', '-c', tmp_file.name, '--output-24bit', '-A120', '-Ow', '-o', wav_out, midi_in])
+            run_command(['timidity', '-c', tmp_file.name, '--output-24bit', f'-A{gain*2000}', '-Ow', '-o', wav_out, midi_in])
```

### Comparing `musical_games-0.8.6/musical_games/external/utils.py` & `musical_games-0.8.7/musical_games/external/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/external/wav_converters.py` & `musical_games-0.8.7/musical_games/external/wav_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/musical_games/utils.py` & `musical_games-0.8.7/musical_games/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/pyproject.toml` & `musical_games-0.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "musical_games"
 description = "Implementation of musical dice games from the 18th century."
 readme = "README.rst"
-version = "0.8.6"
+version = "0.8.7"
 requires-python = ">=3.11"
 keywords = ["Musical games", "Dice games", "Piano music"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
```

### Comparing `musical_games-0.8.6/scripts/demo_cpe_bach.py` & `musical_games-0.8.7/scripts/demo_cpe_bach.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/scripts/demo_gerlach_scottish_dance.py` & `musical_games-0.8.7/scripts/demo_gerlach_scottish_dance.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/scripts/demo_kirnberger_meneut_trio.py` & `musical_games-0.8.7/scripts/demo_kirnberger_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/scripts/demo_kirnberger_polonaise.py` & `musical_games-0.8.7/scripts/demo_kirnberger_polonaise.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/scripts/demo_mozart_contredanse.py` & `musical_games-0.8.7/scripts/demo_mozart_contredanse.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/scripts/demo_mozart_waltz.py` & `musical_games-0.8.7/scripts/demo_mozart_waltz.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/scripts/demo_stadler_meneut_trio.py` & `musical_games-0.8.7/scripts/demo_stadler_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/scripts/lilypond_copy.py` & `musical_games-0.8.7/scripts/lilypond_copy.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/scripts/lilypond_copy2.py` & `musical_games-0.8.7/scripts/lilypond_copy2.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/tox.ini` & `musical_games-0.8.7/tox.ini`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.6/PKG-INFO` & `musical_games-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musical_games
-Version: 0.8.6
+Version: 0.8.7
 Summary: Implementation of musical dice games from the 18th century.
 Keywords: Musical games,Dice games,Piano music
 Author-email: Robbert Harms <robbert@xkls.nl>
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

