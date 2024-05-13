# Comparing `tmp/PDKMaster-0.9.5.tar.gz` & `tmp/PDKMaster-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDKMaster-0.9.5.tar", last modified: Tue Aug  8 13:57:39 2023, max compression
+gzip compressed data, was "PDKMaster-0.9.6.tar", last modified: Sun Oct 22 15:16:51 2023, max compression
```

## Comparing `PDKMaster-0.9.5.tar` & `PDKMaster-0.9.6.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.657629 PDKMaster-0.9.5/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.625629 PDKMaster-0.9.5/.ci/
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1069 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/.ci/check-dco.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      155 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2183 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/.gitlab-ci.yml
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6586 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/Contributing.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/LICENSE.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.625629 PDKMaster-0.9.5/LICENSES/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/LICENSES/agpl-3.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/LICENSES/apache-2.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/LICENSES/cern_ohl_s_v2.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/LICENSES/gpl-2.0.txt
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.629629 PDKMaster-0.9.5/PDKMaster.egg-info/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10060 2023-08-08 13:57:39.000000 PDKMaster-0.9.5/PDKMaster.egg-info/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3966 2023-08-08 13:57:39.000000 PDKMaster-0.9.5/PDKMaster.egg-info/SOURCES.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-08-08 13:57:39.000000 PDKMaster-0.9.5/PDKMaster.egg-info/dependency_links.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-08-08 13:57:39.000000 PDKMaster-0.9.5/PDKMaster.egg-info/requires.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       15 2023-08-08 13:57:39.000000 PDKMaster-0.9.5/PDKMaster.egg-info/top_level.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10060 2023-08-08 13:57:39.657629 PDKMaster-0.9.5/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9592 2023-08-08 13:50:43.000000 PDKMaster-0.9.5/README.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.629629 PDKMaster-0.9.5/ReleaseNotes/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      442 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/ReleaseNotes/v0.1.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1234 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/ReleaseNotes/v0.2.0.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1471 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/ReleaseNotes/v0.3.0.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2547 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/ReleaseNotes/v0.9.0.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.629629 PDKMaster-0.9.5/assura_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/assura_yaml/.keepme
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      595 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/checkskill.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       14 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/ci-requirements.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/dev-requirements.txt
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.629629 PDKMaster-0.9.5/display_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/display_yaml/.keepme
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.617629 PDKMaster-0.9.5/docs/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.633629 PDKMaster-0.9.5/docs/src/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6063 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/conf.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      456 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/index.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      141 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster._util.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      560 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.design.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      443 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.dispatch.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      312 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.io.coriolis.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.io.klayout.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      934 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.io.parsing.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      318 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.io.pdkmaster.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      262 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.io.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      449 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.io.spice.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      290 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1556 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.technology.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3746 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/dodo.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     4469 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/extract_rules.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    26261 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/files.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.633629 PDKMaster-0.9.5/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      709 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18133 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/_util.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.633629 PDKMaster-0.9.5/pdkmaster/design/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      237 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6045 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/cell.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10199 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/circuit.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8637 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/factory.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.637629 PDKMaster-0.9.5/pdkmaster/design/layout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      664 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/layout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    28707 2023-07-26 08:56:45.000000 PDKMaster-0.9.5/pdkmaster/design/layout/_circuitlayouter.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    48505 2023-08-08 13:50:43.000000 PDKMaster-0.9.5/pdkmaster/design/layout/_primitivelayouter.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3335 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/layout/factory_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    22622 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/layout/layout_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2887 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/library.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2600 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/routinggauge.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.637629 PDKMaster-0.9.5/pdkmaster/dispatch/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1375 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/dispatch/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1378 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/dispatch/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1956 2023-07-24 14:24:09.000000 PDKMaster-0.9.5/pdkmaster/dispatch/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8101 2023-07-26 08:56:38.000000 PDKMaster-0.9.5/pdkmaster/dispatch/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2803 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/dispatch/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3801 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/dispatch/shape.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.637629 PDKMaster-0.9.5/pdkmaster/io/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.637629 PDKMaster-0.9.5/pdkmaster/io/coriolis/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/coriolis/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    58632 2023-07-26 08:24:56.000000 PDKMaster-0.9.5/pdkmaster/io/coriolis/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.641629 PDKMaster-0.9.5/pdkmaster/io/klayout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      142 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/klayout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37919 2023-07-26 08:57:55.000000 PDKMaster-0.9.5/pdkmaster/io/klayout/export.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    23519 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/klayout/merge_.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.641629 PDKMaster-0.9.5/pdkmaster/io/lefdef/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      261 2023-07-25 08:57:03.000000 PDKMaster-0.9.5/pdkmaster/io/lefdef/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9948 2023-07-26 08:24:48.000000 PDKMaster-0.9.5/pdkmaster/io/lefdef/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.641629 PDKMaster-0.9.5/pdkmaster/io/notebook/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      121 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/notebook/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1253 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/notebook/plotter.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.641629 PDKMaster-0.9.5/pdkmaster/io/parsing/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      214 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/parsing/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18847 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/parsing/assura.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      422 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/parsing/display.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      822 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/parsing/layermap.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17548 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/parsing/skill_grammar.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24374 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/parsing/tf.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.641629 PDKMaster-0.9.5/pdkmaster/io/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18067 2023-07-26 08:56:38.000000 PDKMaster-0.9.5/pdkmaster/io/pdkmaster/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.645629 PDKMaster-0.9.5/pdkmaster/io/spice/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      165 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/spice/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    15809 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/spice/pyspice.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     5904 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/spice/spice_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      181 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/spice/typing.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.645629 PDKMaster-0.9.5/pdkmaster/technology/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      276 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4032 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    77846 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/geometry.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18203 2023-07-26 09:02:44.000000 PDKMaster-0.9.5/pdkmaster/technology/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      627 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/net.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.649629 PDKMaster-0.9.5/pdkmaster/technology/primitive/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      466 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10122 2023-07-26 08:56:45.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/_core.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2421 2023-07-26 08:56:45.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/_derived.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1176 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/_param.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24164 2023-07-26 08:57:55.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/conductors.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    44812 2023-08-08 13:50:33.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/devices.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4914 2023-07-26 12:04:52.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/layers.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6752 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/rules.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9109 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/property_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2138 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    25167 2023-07-26 12:04:52.000000 PDKMaster-0.9.5/pdkmaster/technology/technology_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2246 2023-07-26 12:04:52.000000 PDKMaster-0.9.5/pdkmaster/technology/wafer_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3344 2023-07-26 08:24:56.000000 PDKMaster-0.9.5/pdkmaster/typing.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-08-08 13:57:39.657629 PDKMaster-0.9.5/setup.cfg
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1410 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/setup.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      863 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/skill.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1278 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/skill2yaml.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.649629 PDKMaster-0.9.5/test/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.649629 PDKMaster-0.9.5/test/unit/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7946 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/_util.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.649629 PDKMaster-0.9.5/test/unit/design/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/design/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3025 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/design/cell.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2470 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/design/circuit.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3664 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/design/factory.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37661 2023-07-26 08:56:45.000000 PDKMaster-0.9.5/test/unit/design/layout.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4584 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/design/library.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.653629 PDKMaster-0.9.5/test/unit/dispatch/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/dispatch/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1343 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/dispatch/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1397 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/dispatch/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1752 2023-07-26 08:56:38.000000 PDKMaster-0.9.5/test/unit/dispatch/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1531 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/dispatch/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3403 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/dispatch/shape.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13201 2023-07-26 08:56:45.000000 PDKMaster-0.9.5/test/unit/dummy.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.653629 PDKMaster-0.9.5/test/unit/io/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.653629 PDKMaster-0.9.5/test/unit/io/klayout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/klayout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13480 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/klayout/export.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20839 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/klayout/merge.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.653629 PDKMaster-0.9.5/test/unit/io/lefdef/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-25 08:57:03.000000 PDKMaster-0.9.5/test/unit/io/lefdef/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1573 2023-07-25 08:57:03.000000 PDKMaster-0.9.5/test/unit/io/lefdef/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.653629 PDKMaster-0.9.5/test/unit/io/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1862 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/pdkmaster/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.653629 PDKMaster-0.9.5/test/unit/io/spice/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/spice/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7947 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/spice/pyspice.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1317 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/spice/spice_.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.657629 PDKMaster-0.9.5/test/unit/technology/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/technology/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1313 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/technology/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    56025 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/technology/geometry.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6370 2023-07-26 09:02:44.000000 PDKMaster-0.9.5/test/unit/technology/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    53229 2023-08-08 13:50:33.000000 PDKMaster-0.9.5/test/unit/technology/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2775 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/technology/property.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2072 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/technology/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17588 2023-08-08 13:50:33.000000 PDKMaster-0.9.5/test/unit/technology/technology.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1052 2023-07-26 12:04:52.000000 PDKMaster-0.9.5/test/unit/technology/wafer.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1438 2023-07-26 09:02:44.000000 PDKMaster-0.9.5/test/unit/typing.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      673 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test.tf
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.657629 PDKMaster-0.9.5/tf_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/tf_yaml/.keepme
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.201441 PDKMaster-0.9.6/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.169441 PDKMaster-0.9.6/.ci/
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1069 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/.ci/check-dco.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      155 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2183 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/.gitlab-ci.yml
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6586 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/Contributing.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/LICENSE.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.169441 PDKMaster-0.9.6/LICENSES/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/LICENSES/agpl-3.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/LICENSES/apache-2.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/LICENSES/cern_ohl_s_v2.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/LICENSES/gpl-2.0.txt
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.169441 PDKMaster-0.9.6/PDKMaster.egg-info/
+-rw-r--r--   0 verhaegs   (500) verhaegs   (500)    10657 2023-10-22 15:16:51.000000 PDKMaster-0.9.6/PDKMaster.egg-info/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3966 2023-10-22 15:16:51.000000 PDKMaster-0.9.6/PDKMaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-10-22 15:16:51.000000 PDKMaster-0.9.6/PDKMaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-10-22 15:16:51.000000 PDKMaster-0.9.6/PDKMaster.egg-info/requires.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       15 2023-10-22 15:16:51.000000 PDKMaster-0.9.6/PDKMaster.egg-info/top_level.txt
+-rw-r--r--   0 verhaegs   (500) verhaegs   (500)    10657 2023-10-22 15:16:51.197441 PDKMaster-0.9.6/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10038 2023-10-22 15:04:57.000000 PDKMaster-0.9.6/README.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.169441 PDKMaster-0.9.6/ReleaseNotes/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      442 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/ReleaseNotes/v0.1.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1234 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/ReleaseNotes/v0.2.0.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1471 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/ReleaseNotes/v0.3.0.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2547 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/ReleaseNotes/v0.9.0.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.169441 PDKMaster-0.9.6/assura_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/assura_yaml/.keepme
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      595 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/checkskill.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       14 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/ci-requirements.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/dev-requirements.txt
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.173441 PDKMaster-0.9.6/display_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/display_yaml/.keepme
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.161441 PDKMaster-0.9.6/docs/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.173441 PDKMaster-0.9.6/docs/src/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6063 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/docs/src/conf.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      456 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/docs/src/index.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      141 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/docs/src/pdkmaster._util.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      560 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/docs/src/pdkmaster.design.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      443 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/docs/src/pdkmaster.dispatch.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      312 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/docs/src/pdkmaster.io.coriolis.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/docs/src/pdkmaster.io.klayout.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      934 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/docs/src/pdkmaster.io.parsing.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      318 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/docs/src/pdkmaster.io.pdkmaster.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      262 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/docs/src/pdkmaster.io.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      449 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/docs/src/pdkmaster.io.spice.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      290 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/docs/src/pdkmaster.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1556 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/docs/src/pdkmaster.technology.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3746 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/dodo.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     4469 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/extract_rules.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    26261 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/files.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.173441 PDKMaster-0.9.6/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      709 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18133 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/_util.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.177441 PDKMaster-0.9.6/pdkmaster/design/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      237 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/design/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6045 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/design/cell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10199 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/design/circuit.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8637 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/design/factory.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.177441 PDKMaster-0.9.6/pdkmaster/design/layout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      664 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/design/layout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    29592 2023-10-19 15:24:16.000000 PDKMaster-0.9.6/pdkmaster/design/layout/_circuitlayouter.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    47505 2023-10-11 15:54:39.000000 PDKMaster-0.9.6/pdkmaster/design/layout/_primitivelayouter.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3335 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/design/layout/factory_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    22622 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/design/layout/layout_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2887 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/design/library.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2600 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/design/routinggauge.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.177441 PDKMaster-0.9.6/pdkmaster/dispatch/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1375 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/dispatch/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1378 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/dispatch/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1956 2023-07-24 14:24:09.000000 PDKMaster-0.9.6/pdkmaster/dispatch/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8101 2023-07-26 08:56:38.000000 PDKMaster-0.9.6/pdkmaster/dispatch/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2803 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/dispatch/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3801 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/dispatch/shape.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.181441 PDKMaster-0.9.6/pdkmaster/io/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.181441 PDKMaster-0.9.6/pdkmaster/io/coriolis/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/coriolis/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    58544 2023-10-11 15:53:51.000000 PDKMaster-0.9.6/pdkmaster/io/coriolis/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.181441 PDKMaster-0.9.6/pdkmaster/io/klayout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      142 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/klayout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    38056 2023-10-11 15:54:39.000000 PDKMaster-0.9.6/pdkmaster/io/klayout/export.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    23519 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/klayout/merge_.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.181441 PDKMaster-0.9.6/pdkmaster/io/lefdef/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      261 2023-07-25 08:57:03.000000 PDKMaster-0.9.6/pdkmaster/io/lefdef/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9948 2023-07-26 08:24:48.000000 PDKMaster-0.9.6/pdkmaster/io/lefdef/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.181441 PDKMaster-0.9.6/pdkmaster/io/notebook/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      121 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/notebook/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1253 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/notebook/plotter.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.181441 PDKMaster-0.9.6/pdkmaster/io/parsing/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      214 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/parsing/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18847 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/parsing/assura.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      422 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/parsing/display.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      822 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/parsing/layermap.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17548 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/parsing/skill_grammar.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24374 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/parsing/tf.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.185441 PDKMaster-0.9.6/pdkmaster/io/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18102 2023-10-11 15:54:39.000000 PDKMaster-0.9.6/pdkmaster/io/pdkmaster/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.185441 PDKMaster-0.9.6/pdkmaster/io/spice/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      165 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/spice/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    15809 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/spice/pyspice.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     5904 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/spice/spice_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      181 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/io/spice/typing.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.185441 PDKMaster-0.9.6/pdkmaster/technology/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      276 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/technology/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4032 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/technology/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    77846 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/technology/geometry.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18203 2023-07-26 09:02:44.000000 PDKMaster-0.9.6/pdkmaster/technology/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      627 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/technology/net.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.189441 PDKMaster-0.9.6/pdkmaster/technology/primitive/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      466 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/technology/primitive/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10162 2023-10-11 15:53:51.000000 PDKMaster-0.9.6/pdkmaster/technology/primitive/_core.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2421 2023-07-26 08:56:45.000000 PDKMaster-0.9.6/pdkmaster/technology/primitive/_derived.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1176 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/technology/primitive/_param.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24544 2023-10-11 15:53:51.000000 PDKMaster-0.9.6/pdkmaster/technology/primitive/conductors.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    46349 2023-10-22 14:58:33.000000 PDKMaster-0.9.6/pdkmaster/technology/primitive/devices.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4914 2023-10-22 14:58:33.000000 PDKMaster-0.9.6/pdkmaster/technology/primitive/layers.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6752 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/technology/primitive/rules.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9109 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/technology/property_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2138 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/pdkmaster/technology/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    25272 2023-10-22 14:58:33.000000 PDKMaster-0.9.6/pdkmaster/technology/technology_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2246 2023-10-22 14:58:33.000000 PDKMaster-0.9.6/pdkmaster/technology/wafer_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3344 2023-07-26 08:24:56.000000 PDKMaster-0.9.6/pdkmaster/typing.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-10-22 15:16:51.201441 PDKMaster-0.9.6/setup.cfg
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1410 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/setup.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      863 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/skill.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1278 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/skill2yaml.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.189441 PDKMaster-0.9.6/test/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.189441 PDKMaster-0.9.6/test/unit/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7946 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/_util.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.193441 PDKMaster-0.9.6/test/unit/design/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/design/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3025 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/design/cell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2470 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/design/circuit.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3664 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/design/factory.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    38035 2023-10-11 15:54:39.000000 PDKMaster-0.9.6/test/unit/design/layout.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4584 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/design/library.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.193441 PDKMaster-0.9.6/test/unit/dispatch/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/dispatch/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1343 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/dispatch/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1397 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/dispatch/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1752 2023-07-26 08:56:38.000000 PDKMaster-0.9.6/test/unit/dispatch/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1531 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/dispatch/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3403 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/dispatch/shape.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13201 2023-10-22 14:58:33.000000 PDKMaster-0.9.6/test/unit/dummy.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.193441 PDKMaster-0.9.6/test/unit/io/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/io/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.193441 PDKMaster-0.9.6/test/unit/io/klayout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/io/klayout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13480 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/io/klayout/export.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20839 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/io/klayout/merge.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.193441 PDKMaster-0.9.6/test/unit/io/lefdef/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-25 08:57:03.000000 PDKMaster-0.9.6/test/unit/io/lefdef/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1573 2023-07-25 08:57:03.000000 PDKMaster-0.9.6/test/unit/io/lefdef/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.197441 PDKMaster-0.9.6/test/unit/io/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/io/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1862 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/io/pdkmaster/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.197441 PDKMaster-0.9.6/test/unit/io/spice/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/io/spice/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7947 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/io/spice/pyspice.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1317 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/io/spice/spice_.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.197441 PDKMaster-0.9.6/test/unit/technology/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/technology/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1313 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/technology/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    56025 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/technology/geometry.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6370 2023-07-26 09:02:44.000000 PDKMaster-0.9.6/test/unit/technology/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    53812 2023-10-22 14:58:33.000000 PDKMaster-0.9.6/test/unit/technology/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2775 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/technology/property.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2072 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test/unit/technology/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17588 2023-10-22 14:58:33.000000 PDKMaster-0.9.6/test/unit/technology/technology.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1052 2023-10-22 14:58:33.000000 PDKMaster-0.9.6/test/unit/technology/wafer.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1438 2023-07-26 09:02:44.000000 PDKMaster-0.9.6/test/unit/typing.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      673 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/test.tf
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-10-22 15:16:51.197441 PDKMaster-0.9.6/tf_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.6/tf_yaml/.keepme
```

### Comparing `PDKMaster-0.9.5/.ci/check-dco.py` & `PDKMaster-0.9.6/.ci/check-dco.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/.gitlab-ci.yml` & `PDKMaster-0.9.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/Contributing.md` & `PDKMaster-0.9.6/Contributing.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/LICENSE.md` & `PDKMaster-0.9.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/LICENSES/agpl-3.0.txt` & `PDKMaster-0.9.6/LICENSES/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/LICENSES/apache-2.0.txt` & `PDKMaster-0.9.6/LICENSES/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/LICENSES/cern_ohl_s_v2.txt` & `PDKMaster-0.9.6/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/LICENSES/gpl-2.0.txt` & `PDKMaster-0.9.6/LICENSES/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/PDKMaster.egg-info/PKG-INFO` & `PDKMaster-0.9.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,20 @@
-Metadata-Version: 2.1
-Name: PDKMaster
-Version: 0.9.5
-Summary: ASIC PDK Manager and Design Framework
-Author: Staf Verhaegen
-Author-email: staf@fibraservi.eu
-License: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
-Project-URL: Source Code, https://gitlab.com/Chips4Makers/PDKMaster
-Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/PDKMaster/issues
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.6: Release of several changes used in improved version of c4m-flexcell and c4m-flexio
+  Mostly small changes or bug fixes. One bigger change is that now more than one implant layer
+  can be drawn around a WaferWire interconnect. Resistor and Diode primitives now allow to
+  define them with multiple implant layers and generate the layout for these multiple implant
+  layers.
+  After this release some API breaking changes will be merged.
 * v0.9.5: allow use of MOSFET.gate4mosfet attribute before MOSFET is added to Technology.
   This allows having rules added to the technology that are using the gate of a specific
   MOSFET.
 * v0.9.4:
   * Support for WaferWire without an implant for diode, MOSFET etc.
   * Roadworks on layer manipulation
   * API improvements, unification and deprecation
```

### Comparing `PDKMaster-0.9.5/PDKMaster.egg-info/SOURCES.txt` & `PDKMaster-0.9.6/PDKMaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/PKG-INFO` & `PDKMaster-0.9.6/PDKMaster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 Metadata-Version: 2.1
 Name: PDKMaster
-Version: 0.9.5
+Version: 0.9.6
 Summary: ASIC PDK Manager and Design Framework
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/PDKMaster
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/PDKMaster/issues
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: setuptools
+Requires-Dist: modgrammar
+Requires-Dist: shapely
+Requires-Dist: descartes
+Requires-Dist: PySpice>=1.5
+Requires-Dist: klayout
 
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.6: Release of several changes used in improved version of c4m-flexcell and c4m-flexio
+  Mostly small changes or bug fixes. One bigger change is that now more than one implant layer
+  can be drawn around a WaferWire interconnect. Resistor and Diode primitives now allow to
+  define them with multiple implant layers and generate the layout for these multiple implant
+  layers.
+  After this release some API breaking changes will be merged.
 * v0.9.5: allow use of MOSFET.gate4mosfet attribute before MOSFET is added to Technology.
   This allows having rules added to the technology that are using the gate of a specific
   MOSFET.
 * v0.9.4:
   * Support for WaferWire without an implant for diode, MOSFET etc.
   * Roadworks on layer manipulation
   * API improvements, unification and deprecation
```

### Comparing `PDKMaster-0.9.5/README.md` & `PDKMaster-0.9.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,39 @@
+Metadata-Version: 2.1
+Name: PDKMaster
+Version: 0.9.6
+Summary: ASIC PDK Manager and Design Framework
+Author: Staf Verhaegen
+Author-email: staf@fibraservi.eu
+License: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
+Project-URL: Source Code, https://gitlab.com/Chips4Makers/PDKMaster
+Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/PDKMaster/issues
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: setuptools
+Requires-Dist: modgrammar
+Requires-Dist: shapely
+Requires-Dist: descartes
+Requires-Dist: PySpice>=1.5
+Requires-Dist: klayout
+
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.6: Release of several changes used in improved version of c4m-flexcell and c4m-flexio
+  Mostly small changes or bug fixes. One bigger change is that now more than one implant layer
+  can be drawn around a WaferWire interconnect. Resistor and Diode primitives now allow to
+  define them with multiple implant layers and generate the layout for these multiple implant
+  layers.
+  After this release some API breaking changes will be merged.
 * v0.9.5: allow use of MOSFET.gate4mosfet attribute before MOSFET is added to Technology.
   This allows having rules added to the technology that are using the gate of a specific
   MOSFET.
 * v0.9.4:
   * Support for WaferWire without an implant for diode, MOSFET etc.
   * Roadworks on layer manipulation
   * API improvements, unification and deprecation
```

### Comparing `PDKMaster-0.9.5/ReleaseNotes/v0.2.0.md` & `PDKMaster-0.9.6/ReleaseNotes/v0.2.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/ReleaseNotes/v0.3.0.md` & `PDKMaster-0.9.6/ReleaseNotes/v0.3.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/ReleaseNotes/v0.9.0.md` & `PDKMaster-0.9.6/ReleaseNotes/v0.9.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/checkskill.py` & `PDKMaster-0.9.6/checkskill.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/docs/src/conf.py` & `PDKMaster-0.9.6/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/docs/src/pdkmaster.design.rst` & `PDKMaster-0.9.6/docs/src/pdkmaster.design.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/docs/src/pdkmaster.io.parsing.rst` & `PDKMaster-0.9.6/docs/src/pdkmaster.io.parsing.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/docs/src/pdkmaster.technology.rst` & `PDKMaster-0.9.6/docs/src/pdkmaster.technology.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/dodo.py` & `PDKMaster-0.9.6/dodo.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/extract_rules.py` & `PDKMaster-0.9.6/extract_rules.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/files.py` & `PDKMaster-0.9.6/files.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/__init__.py` & `PDKMaster-0.9.6/pdkmaster/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/_util.py` & `PDKMaster-0.9.6/pdkmaster/_util.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/design/cell.py` & `PDKMaster-0.9.6/pdkmaster/design/cell.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/design/circuit.py` & `PDKMaster-0.9.6/pdkmaster/design/circuit.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/design/factory.py` & `PDKMaster-0.9.6/pdkmaster/design/factory.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/design/layout/__init__.py` & `PDKMaster-0.9.6/pdkmaster/design/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/design/layout/_circuitlayouter.py` & `PDKMaster-0.9.6/pdkmaster/design/layout/_circuitlayouter.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,24 +49,14 @@
                 )
         if contact_right is not None:
             if len(contact_right.top) != 1:
                 raise NotImplementedError(
                     f"Multiple top layers for Via '{contact_right.name}'",
                 )
 
-        impls = tuple(filter(
-            lambda impl: isinstance(impl, _prm.Implant) and impl.type_ != _prm.adjImpl,
-            mosfet.implant,
-        ))
-        if len(impls) != 1:
-            raise NotImplementedError(
-                f"Multiple implant for MOSFET '{inst.prim.name}'",
-            )
-        self._implant = impls[0]
-
     @property
     def inst(self) -> _ckt._PrimitiveInstance:
         return self._inst
     @property
     def contact_left(self) -> Optional[_prm.Via]:
         return self._contact_left
     @property
@@ -208,46 +198,80 @@
                     f"Active specification mismatch between transistor spec {i} and {i+1}",
                 )
 
         # Create the layout
 
         layout = self.fab.new_layout()
         x = 0.0
+
+        spec = None
+        mosfet = None
+        active = None
+        oxide = None
+        ox_enc = None
+        bottom_enc = ()
+        well_args = {}
         for i, spec in enumerate(specs):
             prev_spec = specs[i - 1] if (i > 0) else None
             next_spec = specs[i + 1] if (i < (len(specs) - 1)) else None
             mosfet = cast(_prm.MOSFET, spec.inst.prim)
+            gate = mosfet.gate
+            active = gate.active
+            oxide = gate.oxide
 
             # First generate, so the port net checks are run now.
             l_trans = self.inst_layout(inst=spec.inst)
 
+            # For contacts also draw implant around bottom,
+            # extend top and bottom enclosure to use the gate enclosure
+            def comb_enc(impl):
+                idx = active.implant.index(impl)
+                min_enc = active.min_implant_enclosure[idx]
+                idx = mosfet.implant.index(impl)
+                gate_enc = mosfet.min_gateimplant_enclosure[idx]
+                if (gate_enc.second + _geo.epsilon) > min_enc.max():
+                    return _prp.Enclosure((min_enc.min(), gate_enc.second))
+                else:
+                    return _prp.Enclosure((min_enc.max(), gate_enc.second))
+
+            bottom_enc = tuple(comb_enc(impl) for impl in mosfet.implant)
+
+            if oxide is None:
+                ox_enc = None
+            else:
+                idx = active.oxide.index(oxide)
+                ox_enc = gate.min_gateoxide_enclosure
+                min_enc = active.min_oxide_enclosure[idx]
+                if ox_enc is None:
+                    ox_enc = min_enc
+                elif min_enc is not None:
+                    ox_enc = _prp.Enclosure((min_enc.min(), ox_enc.second))
+
             # Draw left sd
             if spec.contact_left is not None:
                 w = spec.inst.params["w"]
                 if prev_spec is not None:
                     w = min(w, prev_spec.inst.params["w"])
                 if mosfet.well is None:
                     well_args = {}
                 else:
                     well_args = {
                         "bottom_well": mosfet.well,
                         "well_net": spec.inst.ports["bulk"],
                     }
-                if (i > 0):
-                    # Add oxide layer on first contact
-                    oxide_args = {}
-                else:
-                    oxide_args = {"bottom_oxide": mosfet.gate.oxide}
                 l = self.wire_layout(
                     wire=spec.contact_left,
                     net=self.circuit.net_lookup(port=spec.inst.ports["sourcedrain1"]),
-                    bottom_height=w, bottom=mosfet.gate.active,
-                    bottom_implant=spec._implant, **oxide_args, **well_args,
+                    bottom_height=w, bottom=active,
+                    bottom_implant=mosfet.implant, bottom_implant_enclosure=bottom_enc,
+                    bottom_oxide=oxide, bottom_oxide_enclosure=ox_enc,
+                    **well_args,
                 ).moved(dxy=_geo.Point(x=x, y=0.0))
                 layout += l
+
                 spc = cast(_prm.MOSFET, spec.inst.prim).computed.min_contactgate_space
                 x += (
                     0.5*spec.contact_left.width + spc + 0.5*spec.inst.params["l"]
                 )
             else:
                 gate_space = cast(_prm.MOSFET, spec.inst.prim).computed.min_gate_space
                 if prev_spec is not None:
@@ -270,31 +294,28 @@
                 gate_space = cast(_prm.MOSFET, spec.inst.prim).computed.min_gate_space
                 if next_spec is not None:
                     gate_space = max(
                         gate_space,
                         cast(_prm.MOSFET, next_spec.inst.prim).computed.min_gate_space,
                     )
                 x += 0.5*spec.inst.params["l"] + 0.5*gate_space
+        assert spec is not None
+        assert mosfet is not None
+        assert active is not None
 
         # Draw last contact if needed
-        spec = specs[-1]
+        # spec and other variables are already set from last run of previous for loop
         if spec.contact_right is not None:
-            mosfet = cast(_prm.MOSFET, spec.inst.prim)
-            if mosfet.well is None:
-                well_args = {}
-            else:
-                well_args = {
-                    "bottom_well": mosfet.well,
-                    "well_net": spec.inst.ports["bulk"],
-                }
             l = self.wire_layout(
                 wire=spec.contact_right,
                 net=self.circuit.net_lookup(port=spec.inst.ports["sourcedrain2"]),
-                bottom_height=spec.inst.params["w"], bottom=mosfet.gate.active,
-                bottom_implant=spec._implant, bottom_oxide=mosfet.gate.oxide, **well_args,
+                bottom_height=spec.inst.params["w"], bottom=active,
+                bottom_implant=mosfet.implant, bottom_implant_enclosure=bottom_enc,
+                bottom_oxide=oxide, bottom_oxide_enclosure=ox_enc,
+                **well_args,
             ).moved(dxy=_geo.Point(x=x, y=0.0))
             layout += l
 
         return layout
 
     @overload
     def place(self, object_: _ckt._Instance, *,
@@ -595,25 +616,25 @@
             if bottom_right is not None:
                 if top_right is not None:
                     via_right = min(bottom_right - bottom_henc, top_right - top_henc)
                 else:
                     via_right = bottom_right - bottom_henc
             else:
                 if top_right is not None:
-                    via_right = top_right + top_henc
+                    via_right = top_right - top_henc
                 else:
                     via_right = None
             if bottom_top is not None:
                 if top_top is not None:
                     via_top = min(bottom_top - bottom_venc, top_top - top_venc)
                 else:
                     via_top = bottom_top - bottom_venc
             else:
                 if top_top is not None:
-                    via_top = top_top + top_venc
+                    via_top = top_top - top_venc
                 else:
                     via_top = None
 
             if (via_left is None) != (via_right is None):
                 raise NotImplementedError(
                     "left or right edge specification of Via but not both"
                 )
```

### Comparing `PDKMaster-0.9.5/pdkmaster/design/layout/_primitivelayouter.py` & `PDKMaster-0.9.6/pdkmaster/design/layout/_primitivelayouter.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,52 @@
                     f"Param '{self.name}' value '{value}' is not one of the allowed values:\n"
                     f"    {self.choices}"
             )
 
         return value
 
 
+class _PrimitivesLayoutParam(_LayoutParam):
+    value_type_str = "iterable of '_Primitive'"
+
+    def __init__(self, *,
+        primitive: _prm.PrimitiveT, name: str,
+        default: MultiT[_prm.PrimitiveT]=(),
+        choices: OptMultiT[_prm.PrimitiveT]=None,
+    ):
+        self.choices = cast_OptMultiT(choices)
+        super().__init__(
+            primitive=primitive, name=name, allow_none=True,
+            default=cast_MultiT(default),
+        )
+
+    def cast(self, value):
+        err = (
+            f"param '{self.name}' has to be a `_Primitive` or an iterable \n"
+            "of type `_Primitive'"
+        )
+
+        def check_elem(elem):
+            if not isinstance(elem, _prm.PrimitiveT):
+                raise TypeError(err)
+            if (self.choices is not None) and (elem not in self.choices):
+                raise ValueError(
+                    f"param '{elem.name}' is not one of {self.choices!r}"
+                )
+            return elem
+
+        if value is None:
+            value = self.default
+        elif not _util.is_iterable(value):
+            value = (check_elem(value),)
+        else:
+            value = tuple(check_elem(elem) for elem in value)
+        return value
+
+
 class _EnclosureLayoutParam(_LayoutParam):
     value_type = (_prp.Enclosure, float, Iterable[float])
     value_type_str = "'Enclosure'"
 
     def cast(self, value):
         if value is None:
             if hasattr(self, "default"):
@@ -137,42 +175,52 @@
     ):
         self.n = n
         super().__init__(
             primitive=primitive, name=name, allow_none=allow_none, default=default,
         )
 
     def cast(self, value):
+        err = (
+            f"param '{self.name}' has to be an enclosure value or an iterable \n"
+            "of type 'Enclosure'"
+        )
+        if self.n > 0:
+            err += f" with length {self.n}"
+
         if value is None:
             if hasattr(self, "default"):
                 value = self.default
             elif not self.allow_none:
                 raise TypeError(
                     f"'None' value not allowed for parameter '{self.name}'"
                 )
+        elif isinstance(value, _prp.Enclosure) or (value in ("wide", "tall")):
+            value = max(self.n, 1)*(value,)
         elif not _util.is_iterable(value):
             try:
-                value = self.n*(_prp.Enclosure(value),)
+                value = (_prp.Enclosure(value),)
             except:
-                raise TypeError(
-                    f"param '{self.name}' has to be an enclosure value or an iterable \n"
-                    f"of type 'Enclosure' with length {self.n}"
-                )
+                raise TypeError(err)
+            else:
+                if self.n > 1: # Not needed for 0 or 1
+                    value *= self.n
         else:
             try:
                 value = tuple(
                     (None if elem is None
-                     else elem if isinstance(elem, _prp.Enclosure)
+                     else elem if isinstance(elem, _prp.Enclosure) or (elem in ("wide", "tall"))
                      else _prp.Enclosure(elem)
                     ) for elem in value
                 )
             except:
-                raise TypeError(
-                    f"param '{self.name}' has to be an enclosure value or an iterable \n"
-                    f"of type 'Enclosure' with length {self.n}"
-                )
+                raise TypeError(err)
+            else:
+                if self.n != 0:
+                    if len(value) != self.n:
+                        raise TypeError(err)
         return value
 
 
 class _NetLayoutParam(_LayoutParam):
     value_type = _net.NetT
     value_type_str = "Net"
 
@@ -197,18 +245,22 @@
         return {
             param.name: param.cast(prim_params.pop(param.name, None))
             for param in layout_params
         }
 
     def _Primitive(self, prim: _prm.PrimitiveT, **params: Any) -> Dict[str, Any]:
         out = {}
-        if isinstance(prim, _prm.PinAttrPrimitiveT) and prim.pin is not None:
+        try:
+            pin: _prm.Marker = prim.pin # type: ignore
+        except AttributeError:
+            pass
+        else:
             out.update(self.cast_params(
                 layout_params=_PrimitiveLayoutParam(
-                    primitive=prim, name="pin", allow_none=True, choices=prim.pin,
+                    primitive=prim, name="pin", allow_none=True, choices=pin,
                 ),
                 prim_params=params,
             ))
 
         if len(prim.ports) > 0:
             try:
                 portnets = params.pop("portnets")
@@ -272,21 +324,22 @@
         super_params.update(marker_params)
 
         return super_params
 
     def WaferWire(self, prim: _prm.WaferWire, **params) -> Dict[str, Any]:
         layparams = []
         ww_params = {}
+
         layparams.extend((
-            _PrimitiveLayoutParam(
+            _PrimitivesLayoutParam(
                 primitive=prim, name="implant", choices=prim.implant,
-                allow_none=True,
+                default=(),
             ),
-            _EnclosureLayoutParam(
-                primitive=prim, name="implant_enclosure", allow_none=True,
+            _EnclosuresLayoutParam(
+                primitive=prim, name="implant_enclosure", default=(), allow_none=True, n=0,
             ),
         ))
         if (len(prim.well) > 1) or prim.allow_in_substrate:
             layparams.extend((
                 _PrimitiveLayoutParam(
                     primitive=prim, name="well", allow_none=prim.allow_in_substrate,
                     choices=prim.well
@@ -313,21 +366,83 @@
                 _EnclosureLayoutParam(
                     primitive=prim, name="oxide_enclosure", allow_none=True,
                 ),
             ))
         ww_params.update(self.cast_params(layout_params=layparams, prim_params=params))
 
         implant = ww_params["implant"]
-        enc = ww_params["implant_enclosure"]
-        if (implant is not None) and (enc is None):
-            idx = prim.implant.index(implant)
-            ww_params["implant_enclosure"] = prim.min_implant_enclosure[idx]
+        enclosure = ww_params["implant_enclosure"]
+        if len(implant) != len(enclosure):
+            if len(implant) == 0:
+                raise TypeError(
+                    f"Enclusore specified without an implant layer for WaferWire `{prim.name}`"
+                )
+            elif len(enclosure) == 0:
+                # Use minimum enclosure for all implants
+                enclosure = len(implant)*(None,)
+            elif len(enclosure) == 1:
+                enclosure = len(implant)*enclosure
+            else:
+                raise ValueError(
+                    f"Parameter number mismatch for WaferWire `{prim.name}`\n"
+                    f"{len(implant)} implant layers and {len(enclosure)} enclosures"
+                )
+        # Replace None enclosure values with minimal enclosure values
+        assert len(implant) == len(enclosure), "Internal error"
+        def min_enc(impl, enc):
+            if (enc is None) or enc in ("wide", "tall"):
+                idx = prim.implant.index(impl)
+                if enc is None:
+                    enc = prim.min_implant_enclosure[idx]
+                elif enc == "wide":
+                    enc = prim.min_implant_enclosure[idx].wide()
+                elif enc == "tall":
+                    enc = prim.min_implant_enclosure[idx].tall()
+                else: # pragma: no cover
+                    assert False, "Internal error"
+            return enc
+        enclosure = tuple(min_enc(implant[i], enc) for i, enc in enumerate(enclosure))
+        ww_params["implant"] = implant
+        ww_params["implant_enclosure"] = enclosure
+
+        well = cast(_prm.Well, ww_params["well"])
+        enclosure = ww_params["well_enclosure"]
+        well_net = ww_params["well_net"]
+        if well is not None:
+            if "portnets" in params:
+                net = params["portnets"]["conn"]
+            else:
+                net = prim.ports["conn"]
+            for main_impl in implant:
+                if main_impl.type_ in (_prm.nImpl, _prm.pImpl):
+                    break
+            else:
+                main_impl = None
+            if well_net is None:
+                if (
+                    (main_impl is not None)
+                    and (main_impl.type_ == well.type_)
+                ):
+                    ww_params["well_net"] = net
+                else:
+                    raise TypeError("well_net needs to be provided if well is specified")
+            else:
+                if (
+                    (main_impl is not None) and (main_impl.type_ == well.type_)
+                    and (net != well_net)
+                ):
+                    raise ValueError(
+                        f"Net '{well_net}' for well '{well.name}' of WaferWire"
+                        f" {prim.name} is different from net '{net}''\n"
+                        f"\tbut implant '{main_impl.name}' have same type as the well"
+                    )
 
-        if (ww_params["well"] is not None) and (ww_params["well_net"] is None):
-            raise ValueError("well_net needs to be provided if well is specified")
+            if enclosure is None:
+                idx = prim.well.index(well)
+                ww_params["well_enclosure"] = prim.min_well_enclosure[idx]
 
         if ("oxide" in ww_params):
             oxide = ww_params["oxide"]
             if oxide is not None:
                 oxide_enclosure = ww_params["oxide_enclosure"]
                 if oxide_enclosure is None:
                     idx = prim.oxide.index(oxide)
@@ -365,29 +480,27 @@
         choices = sum(
             (cast(_prm.WaferWire, wire).implant for wire in filter(
                 lambda w: isinstance(w, _prm.WaferWire),
                 prim.bottom,
             )),
             tuple(),
         )
-        if choices:
-            layparams.extend((
-                _PrimitiveLayoutParam(
-                    primitive=prim, name="bottom_implant",
-                    allow_none=True, choices=choices,
-                ),
-                _EnclosureLayoutParam(
-                    primitive=prim, name="bottom_implant_enclosure", allow_none=True,
-                ),
-                _PrimitiveLayoutParam(primitive=prim, name="bottom_well", allow_none=True),
-                _NetLayoutParam(primitive=prim, name="well_net", allow_none=True),
-                _EnclosureLayoutParam(
-                    primitive=prim, name="bottom_well_enclosure", allow_none=True,
-                ),
-            ))
+        layparams.extend((
+            _PrimitivesLayoutParam(
+                primitive=prim, name="bottom_implant", choices=choices,
+            ),
+            _EnclosuresLayoutParam(
+                primitive=prim, name="bottom_implant_enclosure", default=(), allow_none=True, n=0,
+            ),
+            _PrimitiveLayoutParam(primitive=prim, name="bottom_well", allow_none=True),
+            _NetLayoutParam(primitive=prim, name="well_net", allow_none=True),
+            _EnclosureLayoutParam(
+                primitive=prim, name="bottom_well_enclosure", allow_none=True,
+            ),
+        ))
 
         choices = sum(
             (
                 cast(_prm.WaferWire, wire).oxide
                 for wire in filter(
                     lambda w: isinstance(w, _prm.WaferWire),
                     prim.bottom,
@@ -412,83 +525,30 @@
                 primitive=prim, name="top", default=default, choices=prim.top,
             ))
         else:
             via_params["top"] = prim.top[0]
 
         via_params.update(self.cast_params(layout_params=layparams, prim_params=params))
 
-        def get_via_param(name: str):
-            try:
-                return via_params[name]
-            except KeyError:
-                return None
+        super_params = super().Via(prim, **params)
+        super_params.update(via_params)
 
-        bottom = via_params["bottom"]
-        bottom_impl = get_via_param("bottom_implant")
-        bottom_impl_enc = get_via_param("bottom_implant_enclosure")
-        bottom_well = get_via_param("bottom_well")
-        well_net = get_via_param("well_net")
-        bottom_well_enc = get_via_param("bottom_well_enclosure")
-        if isinstance(bottom, _prm.WaferWire):
-            if bottom_impl is None:
-                if bottom_impl_enc is not None:
+        bottom = super_params["bottom"]
+        if not isinstance(bottom, _prm.WaferWire):
+            for param, value in (
+                ("bottom_implant", ()),
+                ("bottom_implant_enclosure", ()),
+                ("bottom_well", None),
+                ("bottom_well_enclosure", None),
+                ("well_net", None),
+            ):
+                if super_params[param] != value:
                     raise TypeError(
-                        "bottom_implant_enclosure provided for bottom "
-                        f"'{bottom.name}' of via {prim.name} without a bottom_implant"
+                        f"param '{param}' not valid for bottom '{bottom.name}'"
                     )
-            else:
-                if bottom_impl_enc is None:
-                    idx = bottom.implant.index(bottom_impl)
-                    via_params["bottom_implant_enclosure"] = bottom.min_implant_enclosure[idx]
-
-            if bottom_well is not None:
-                if bottom_well not in bottom.well:
-                    raise ValueError(
-                        f"bottom_well '{bottom_well.name}' not a valid well for "
-                        f"bottom wire '{bottom.name}'"
-                    )
-                if bottom_well_enc is None:
-                    idx = bottom.well.index(bottom_well)
-                    via_params["bottom_well_enclosure"] = (
-                        bottom.min_well_enclosure[idx]
-                    )
-                # well_net will be checked during layout generation
-            elif not bottom.allow_in_substrate:
-                raise TypeError(
-                    f"bottom wire '{bottom.name}' needs a well"
-                )
-        else:
-            if bottom_impl is not None:
-                raise TypeError(
-                    f"bottom_implant '{bottom_impl.name}' not a valid implant for "
-                    f"bottom wire '{bottom.name}'"
-                )
-            if bottom_impl_enc is not None:
-                raise TypeError(
-                    "bottom_implant_enclosure wrongly provided for bottom wire "
-                    f"'{bottom.name}'"
-                )
-            if bottom_well is not None:
-                raise TypeError(
-                    f"bottom_well '{bottom_well.name}' not a valid well for "
-                    f"bottom wire '{bottom.name}'"
-                )
-            if bottom_well_enc is not None:
-                raise TypeError(
-                    "bottom_well_enclosure wrongly provided for bottom wire "
-                    f"'{bottom.name}'"
-                )
-            if well_net is not None:
-                raise TypeError(
-                    "well_net wrongly provided for bottom wire "
-                    f"'{bottom.name}'"
-                )
-
-        super_params = super().Via(prim, **params)
-        super_params.update(via_params)
 
         return super_params
 
     def MIMCapacitor(self, prim: _prm.MIMCapacitor, **params) -> Dict[str, Any]:
         mim_params = self.cast_params(
             layout_params=_BoolLayoutParam(
                 primitive=prim, name="bottom_connect_up", default=True,
@@ -627,27 +687,27 @@
 
     def WaferWire(self, prim: _prm.WaferWire, **waferwire_params) -> LayoutT:
         width = waferwire_params["width"]
         height = waferwire_params["height"]
 
         implant = waferwire_params.pop("implant")
         implant_enclosure = waferwire_params.pop("implant_enclosure")
-        assert (implant is None) or (implant_enclosure is not None)
 
         well = waferwire_params.pop("well", None)
         well_enclosure = waferwire_params.pop("well_enclosure", None)
 
         oxide = waferwire_params.pop("oxide", None)
         oxide_enclosure = waferwire_params.pop("oxide_enclosure", None)
 
         layout = self._WidthSpaceConductor(prim, **waferwire_params)
-        if (implant is not None):
-            layout.add_shape(layer=implant, net=None, shape=_rect(
+        for i, impl in enumerate(implant):
+            enc = implant_enclosure[i]
+            layout.add_shape(layer=impl, net=None, shape=_rect(
                 -0.5*width, -0.5*height, 0.5*width, 0.5*height,
-                enclosure=implant_enclosure,
+                enclosure=enc,
             ))
         if well is not None:
             well_net = waferwire_params["well_net"]
             assert well_net is not None, "Internal error"
             layout.add_shape(layer=well, net=well_net, shape=_rect(
                 -0.5*width, -0.5*height, 0.5*width, 0.5*height,
                 enclosure=well_enclosure,
@@ -655,17 +715,14 @@
         if oxide is not None:
             layout.add_shape(layer=oxide, net=None, shape=_rect(
                 -0.5*width, -0.5*height, 0.5*width, 0.5*height,
                 enclosure=oxide_enclosure,
             ))
         return layout
 
-    def MIMTop(self, prim: _prm.MIMTop, **_) -> LayoutT:
-        raise ValueError("No generation of MIMTop layer; use MIMCapacitor instead")
-
     def Via(self, prim: _prm.Via, **via_params) -> LayoutT:
         tech = self.tech
 
         try:
             portnets = via_params["portnets"]
         except KeyError:
             net = prim.ports["conn"]
@@ -797,80 +854,35 @@
         )
 
         via_bottom = tech.on_grid(-0.5*via_height)
         via_left = tech.on_grid(-0.5*via_width)
 
         layout = self.fab.new_layout()
 
-        layout.add_shape(layer=bottom, net=net, shape=bottom_rect)
+        if isinstance(bottom, _prm.WaferWire):
+            bottom_args = {
+                param: via_params[f"bottom_{param}"]
+                for param in (
+                    "implant", "implant_enclosure",
+                    "oxide", "oxide_enclosure",
+                    "well", "well_enclosure",
+                )
+            }
+            bottom_args["well_net"] = via_params["well_net"]
+        else:
+            bottom_args = {}
+        layout.add_primitive(
+            prim=bottom, portnets={"conn": net}, origin=bottom_rect.center,
+            width=bottom_rect.width, height=bottom_rect.height,
+            **bottom_args,
+        )
         layout.add_shape(layer=prim, net=net, shape=_via_array(
             via_left, via_bottom, width, pitch, rows, columns,
         ))
         layout.add_shape(layer=top, net=net, shape=top_rect)
-        try:
-            impl = via_params["bottom_implant"]
-        except KeyError:
-            impl = None
-        else:
-            if impl is not None:
-                enc = cast(_prp.Enclosure, via_params["bottom_implant_enclosure"])
-                assert enc is not None, "Internal error"
-                if enc in ("wide", "tall"):
-                    idx = bottom.implant.index(impl)
-                    enc2 = bottom.min_implant_enclosure[idx]
-                    if enc == "wide":
-                        enc = enc2.wide()
-                    else:
-                        assert enc == "tall", "Internal error"
-                        enc = enc2.tall()
-                layout.add_shape(layer=impl, net=None, shape=_geo.Rect.from_rect(
-                    rect=bottom_rect, bias=enc,
-                ))
-        try:
-            oxide = via_params["bottom_oxide"]
-        except KeyError:
-            oxide = None
-        else:
-            if oxide is not None:
-                assert isinstance(bottom, _prm.WaferWire)
-                enc = cast(_prp.Enclosure, via_params["bottom_oxide_enclosure"])
-                if enc is None:
-                    idx = bottom.oxide.index(oxide)
-                    enc = bottom.min_oxide_enclosure[idx]
-                assert (enc is not None), "Unknown enclosure"
-                layout.add_shape(layer=oxide, net=None, shape=_geo.Rect.from_rect(
-                    rect=bottom_rect, bias=enc,
-                ))
-        try:
-            well = via_params["bottom_well"]
-        except KeyError:
-            well = None
-        else:
-            if well is not None:
-                well_net = via_params.get("well_net", None)
-                enc = via_params["bottom_well_enclosure"]
-                assert enc is not None, "Internal error"
-                if (impl is not None) and (impl.type_ == well.type_):
-                    if well_net is not None:
-                        if well_net != net:
-                            raise ValueError(
-                                f"Net '{well_net}' for well '{well.name}' of WaferWire"
-                                f" {bottom.name} is different from net '{net}''\n"
-                                f"\tbut implant '{impl.name}' is same type as the well"
-                            )
-                    else:
-                        well_net = net
-                elif well_net is None:
-                    raise TypeError(
-                        f"No well_net specified for WaferWire '{bottom.name}' in"
-                        f" well '{well.name}'"
-                    )
-                layout.add_shape(layer=well, net=well_net, shape=_geo.Rect.from_rect(
-                    rect=bottom_rect, bias=enc,
-                ))
 
         return layout
 
     def DeepWell(self, prim: _prm.DeepWell, **deepwell_params) -> LayoutT:
         raise NotImplementedError("layout generation for DeepWell primitive")
 
     def Resistor(self, prim: _prm.Resistor, **resistor_params) -> LayoutT:
@@ -881,16 +893,16 @@
             port2 = prim.ports.port2
         else:
             port1 = portnets["port1"]
             port2 = portnets["port2"]
         if prim.contact is None:
             raise NotImplementedError("Resistor layout without contact layer")
 
-        res_width = resistor_params["width"]
-        res_length = resistor_params["length"]
+        res_width = cast(float, resistor_params["width"])
+        res_length = cast(float, resistor_params["length"])
 
         wire = prim.wire
 
         cont = prim.contact
         cont_space = prim.min_contact_space
         assert cont_space is not None
         try:
@@ -903,20 +915,18 @@
                 raise AssertionError("Internal error")
             else:
                 cont_enc = cont.min_top_enclosure[wire_idx]
                 cont_args = {"top": wire, "x": 0.0, "top_width": res_width}
         else:
             cont_enc = cont.min_bottom_enclosure[wire_idx]
             cont_args = {"bottom": wire, "x": 0.0, "bottom_width": res_width}
-        if (prim.implant is not None) and isinstance(wire, _prm.WaferWire):
-            cont_args["bottom_implant"] = prim.implant
         cont_y1 = -0.5*res_length - cont_space - 0.5*cont.width
         cont_y2 = -cont_y1
 
-        wire_ext = cont_space + cont.width + cont_enc.min()
+        wire_ext = cont_space + cont.width + cont_enc.max()
 
         layout = self.fab.new_layout()
 
         # Draw indicator layers
         for idx, ind in enumerate(prim.indicator):
             ext = prim.min_indicator_extension[idx]
             layout += self(ind, width=(res_width + 2*ext), height=res_length)
@@ -974,24 +984,18 @@
                     if msl.mask == wire.mask:
                         assert isinstance(msl.shape, _geo.Rect)
                         msl._shape = _geo.Rect.from_rect(
                             rect=msl.shape, bottom=(0.5*res_length + self.tech.grid)
                         )
         layout += _l_cont
 
-        if prim.implant is not None:
-            impl = prim.implant
-            try:
-                enc = prim.min_implant_enclosure.max() # type: ignore
-            except AttributeError:
-                assert isinstance(wire, _prm.WaferWire), "Internal error"
-                idx = wire.implant.index(impl)
-                enc = wire.min_implant_enclosure[idx].max()
-            impl_width = res_width + 2*enc
-            impl_height = res_length + 2*wire_ext + 2*enc
+        for i, impl in enumerate(prim.implant):
+            enc = prim.min_implant_enclosure[i]
+            impl_width = res_width + 2*enc.first
+            impl_height = res_length + 2*wire_ext + 2*enc.second
             layout.add_shape(
                 layer=impl, net=None, shape=_geo.Rect.from_size(width=impl_width, height=impl_height),
             )
 
         return layout
 
     def MIMCapacitor(self, prim: _prm.MIMCapacitor, **mimcapargs) -> LayoutT:
@@ -1110,35 +1114,35 @@
         except KeyError:
             an = prim.ports.anode
             cath = prim.ports.cathode
         else:
             an = portnets["anode"]
             cath = portnets["cathode"]
 
-        wirenet_args = {
+        is_p = any(impl.type_ == _prm.pImpl for impl in prim.implant)
+
+        wirenet_args: Dict[str, Any] = {
             "implant": prim.implant,
-            "portnets": {"conn": an if prim.implant.type_ == _prm.pImpl else cath},
+            "portnets": {"conn": an if is_p else cath},
         }
-        if prim.min_implant_enclosure is not None:
-            wirenet_args["implant_enclosure"] = prim.min_implant_enclosure
         if prim.well is not None:
             wirenet_args.update({
                 "well": prim.well,
-                "well_net": cath if prim.implant.type_ == _prm.pImpl else an,
+                "well_net": cath if is_p else an,
             })
 
         layout = self.fab.new_layout()
         layout.add_primitive(prim=prim.wire, **wirenet_args, **diode_params)
         wireact_bounds = layout.bounds(mask=prim.wire.mask)
         act_width = wireact_bounds.right - wireact_bounds.left
         act_height = wireact_bounds.top - wireact_bounds.bottom
 
         for i, ind in enumerate(prim.indicator):
-            enc = prim.min_indicator_enclosure[i].max()
-            layout += self(ind, width=(act_width + 2*enc), height=(act_height + 2*enc))
+            enc = prim.min_indicator_enclosure[i]
+            layout += self(ind, width=(act_width + 2*enc.first), height=(act_height + 2*enc.second))
 
         return layout
 
     def MOSFET(self, prim: _prm.MOSFET, **mos_params) -> LayoutT:
         l = mos_params["l"]
         w = mos_params["w"]
         gate_encs = mos_params["gateimplant_enclosures"]
```

### Comparing `PDKMaster-0.9.5/pdkmaster/design/layout/factory_.py` & `PDKMaster-0.9.6/pdkmaster/design/layout/factory_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/design/layout/layout_.py` & `PDKMaster-0.9.6/pdkmaster/design/layout/layout_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/design/library.py` & `PDKMaster-0.9.6/pdkmaster/design/library.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/design/routinggauge.py` & `PDKMaster-0.9.6/pdkmaster/design/routinggauge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/dispatch/__init__.py` & `PDKMaster-0.9.6/pdkmaster/dispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/dispatch/edge.py` & `PDKMaster-0.9.6/pdkmaster/dispatch/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/dispatch/mask.py` & `PDKMaster-0.9.6/pdkmaster/dispatch/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/dispatch/primitive.py` & `PDKMaster-0.9.6/pdkmaster/dispatch/primitive.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/dispatch/rule.py` & `PDKMaster-0.9.6/pdkmaster/dispatch/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/dispatch/shape.py` & `PDKMaster-0.9.6/pdkmaster/dispatch/shape.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/io/coriolis/export.py` & `PDKMaster-0.9.6/pdkmaster/io/coriolis/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,18 +99,18 @@
         self.poly_layers = {
             gate.poly for gate in tech.primitives.__iter_type__(_prm.MOSFETGate)
         }
         self.via_conns = via_conns = cast(Set[_prm.PrimitiveT], set())
         for via in tech.primitives.__iter_type__(_prm.Via):
             via_conns.update(via.bottom)
             via_conns.update(via.top)
-        self.blockages = {prim.blockage for prim in filter(
-            lambda p: p.blockage is not None,
-            tech.primitives.__iter_type__(_prm.BlockageAttrPrimitiveT),
-        )}
+        self.blockages = {
+            cast(_prm.BlockageAttrPrimitiveT, prim).blockage
+            for prim in filter(lambda p: hasattr(p, "blockage"), tech.primitives)
+        }
 
     def _Primitive(self, prim: _prm.PrimitiveT):
         raise NotImplementedError(
             f"layer code generation for '{prim.__class__.__name__}'"
         )
 
     def Marker(self, prim: _prm.Marker):
@@ -477,18 +477,18 @@
         self.metals: Tuple[_prm.MetalWire, ...] = tuple(filter(
             lambda m: not isinstance(m, _prm.MIMTop),
             tech.primitives.__iter_type__(_prm.MetalWire),
         ))
         self.vias: Tuple[_prm.Via, ...] = tuple(tech.primitives.__iter_type__(_prm.Via))
         assert len(self.metals) == len(self.vias)
         self.pinmasks = pinmasks = {}
-        for prim in tech.primitives.__iter_type__(_prm.PinAttrPrimitiveT):
-            if prim.pin is not None:
+        for prim in tech.primitives:
+            if hasattr(prim, "pin"):
                 assert isinstance(prim, _prm.DesignMaskPrimitiveT)
-                pinmasks[prim.pin.mask] = prim.mask
+                pinmasks[cast(_prm.PinAttrPrimitiveT, prim).pin.mask] = prim.mask
 
         self.metalsdir: Optional[Tuple[Optional[str], ...]] = None
 
     def __call__(self, lib: _lbry.Library, *, routinggauge: Optional[_rg.RoutingGauge]):
         def otherdir(dir_):
             return "vertical" if dir_ == "horizontal" else "horizontal"
 
@@ -1172,21 +1172,18 @@
             )
 
         s_prims += "\n# ViaLayers\n"
         for via in vias:
             s_prims += gen(via, via_layer=True)
 
         s_prims += "\n# Blockages\n"
-        for prim in filter(
-            lambda p: p.blockage is not None,
-            self.tech.primitives.__iter_type__(_prm.BlockageAttrPrimitiveT),
-        ):
+        for prim in filter(lambda p: hasattr(p, "blockage"), self.tech.primitives):
             s_prims += dedent(f"""
                 tech.getLayer('{prim.name}').setBlockageLayer(
-                    tech.getLayer('{cast(_prm.Marker, prim.blockage).name}')
+                    tech.getLayer('{cast(_prm.BlockageAttrPrimitiveT, prim).blockage.name}')
                 )
             """[1:])
 
         s_prims += "\n# Coriolis internal layers\n"
         for name, mat in (
             ("text.cell", "other"),
             ("text.instance", "other"),
@@ -1295,29 +1292,29 @@
             )
         for prim in self.tech.primitives.__iter_type__(_prm.WaferWire):
             s += (
                 f"    style.addDrawingStyle(group='Active Layers', name='{prim.name}'"
                 ", color=toRGB('White'), pattern=toHexa('antihash0.8'), border=1"
                 ", threshold=threshold)\n"
             )
-            if prim.pin is not None:
+            if hasattr(prim, "pin"):
                 s += (
                     "    style.addDrawingStyle(group='Active Layers'"
                     f", name='{prim.pin.name}', color=toRGB('White')"
                     ", pattern=toHexa('antihash0.8'), border=2"
                     ", threshold=threshold)\n"
                 )
         for i, prim in enumerate(self.tech.primitives.__iter_type__(_prm.GateWire)):
             rgb = "Red" if i == 0 else "Orange"
             s += (
                 f"    style.addDrawingStyle(group='Active Layers', name='{prim.name}'"
                 f", color=toRGB('{rgb}'), pattern=toHexa('antihash0.8'), border=1"
                 ", threshold=threshold)\n"
             )
-            if prim.pin is not None:
+            if hasattr(prim, "pin"):
                 s += (
                     "    style.addDrawingStyle(group='Active Layers'"
                     f", name='{prim.pin.name}', color=toRGB('{rgb}')"
                     ", pattern=toHexa('antihash0.8'), border=2"
                     ", threshold=threshold)\n"
                 )
 
@@ -1326,15 +1323,15 @@
             rgb = clrs[i%len(clrs)]
             hexa = "slash.8" if i == 0 else "poids4.8"
             s += (
                 f"    style.addDrawingStyle(group='Routing Layers', name='{prim.name}'"
                 f", color=toRGB('{rgb}'), pattern=toHexa('{hexa}'), border=1"
                 ", threshold=threshold)\n"
             )
-            if prim.pin is not None:
+            if hasattr(prim, "pin"):
                 s += (
                     f"    style.addDrawingStyle(group='Routing Layers'"
                     f", name='{prim.pin.name}', color=toRGB('{rgb}'), pattern=toHexa('{hexa}')"
                     ", border=2, threshold=threshold)\n"
                 )
 
         s += "\n    # Cuts (VIA holes).\n"
@@ -1344,18 +1341,18 @@
             rgb = clrs[i%len(clrs)] if i > 0 else "0,150,150"
             s += (
                 f"    style.addDrawingStyle(group='Cuts (VIA holes', name='{prim.name}'"
                 f", color=toRGB('{rgb}'), threshold=threshold)\n"
             )
 
         s += "\n    # Blockages.\n"
-        blockages = {prim.blockage for prim in filter(
-            lambda p: p.blockage is not None,
-            self.tech.primitives.__iter_type__(_prm.BlockageAttrPrimitiveT),
-        )}
+        blockages = {
+            cast(_prm.BlockageAttrPrimitiveT, prim).blockage
+            for prim in filter(lambda p: hasattr(p, "blockage"), self.tech.primitives)
+        }
         for i, prim in enumerate(filter(
             lambda p: p in blockages, self.tech.primitives.__iter_type__(_prm.Marker)
         )):
             rgb = clrs[i%len(clrs)]
             hexa = "slash.8" if i == 0 else "poids4.8"
             s += (
                 f"    style.addDrawingStyle(group='Blockages', name='{prim.name}'"
```

### Comparing `PDKMaster-0.9.5/pdkmaster/io/klayout/export.py` & `PDKMaster-0.9.6/pdkmaster/io/klayout/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 from textwrap import dedent
 from itertools import product
 from xml.etree import ElementTree as ET
-from typing import Any, Tuple, Dict, Set, Iterable, Optional, Union, cast, overload
+from typing import Any, Tuple, List, Dict, Set, Iterable, Optional, Union, cast, overload
 
 from ... import _util, dispatch as _dsp
 from ...typing import GDSLayerSpecDict
 from ...technology import (
     property_ as _prp, rule as _rle, wafer_ as _wfr, mask as _msk, edge as _edg,
     geometry as _geo, primitive as _prm, net as _net, technology_ as _tch,
 )
@@ -317,15 +317,15 @@
 
     return s
 
 
 def _str_lvsdiode(tech: _tch.Technology, diode: _prm.Diode, spice_params: SpicePrimParamsT):
     s = f"# {diode.name}\n"
 
-    is_n = diode.implant.type_ == _prm.nImpl
+    is_n = any(impl.type_ == _prm.nImpl for impl in diode.implant)
 
     s_diode = _mask_conv(diode.mask)
     s_conn = _mask_conv(diode.wire.conn_mask)
     s_well = _mask_conv(
         diode.well.mask if diode.well is not None
         else tech.substrate_prim.mask
     )
@@ -861,18 +861,22 @@
                             point = _util.get_first_of(ps.points)
                         shapes.insert(pya.DText(net.name, point.x, point.y))
         elif isinstance(o, _geo.MaskShapes):
             for ms in o:
                 self._add(ms, add_pin_label=add_pin_label, net=net)
         elif isinstance(o, _lay.LayoutT):
             prims = o.fab.tech.primitives
-            pinmasks = []
-            for prim in prims.__iter_type__(_prm.PinAttrPrimitiveT):
-                if prim.pin is not None:
-                    pinmasks.append(prim.pin.mask)
+            pinmasks: List[_msk.DesignMask] = []
+            for prim in prims:
+                try:
+                    pin: _prm.Marker = prim.pin # type: ignore
+                except AttributeError:
+                    pass
+                else:
+                    pinmasks.append(pin.mask)
             self.pinmasks = tuple(pinmasks)
             for sl in o._sublayouts:
                 if isinstance(sl, _laylay._MaskShapesSubLayout):
                     self._add(sl.shapes, add_pin_label=add_pin_label, net=sl.net)
                 elif isinstance(sl, _laylay._InstanceSubLayout):
                     assert self.cell is not None
                     instcell = self._register_cell(sl.inst.cell)
```

### Comparing `PDKMaster-0.9.5/pdkmaster/io/klayout/merge_.py` & `PDKMaster-0.9.6/pdkmaster/io/klayout/merge_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/io/lefdef/export.py` & `PDKMaster-0.9.6/pdkmaster/io/lefdef/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/io/notebook/plotter.py` & `PDKMaster-0.9.6/pdkmaster/io/notebook/plotter.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/io/parsing/assura.py` & `PDKMaster-0.9.6/pdkmaster/io/parsing/assura.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/io/parsing/layermap.py` & `PDKMaster-0.9.6/pdkmaster/io/parsing/layermap.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/io/parsing/skill_grammar.py` & `PDKMaster-0.9.6/pdkmaster/io/parsing/skill_grammar.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/io/parsing/tf.py` & `PDKMaster-0.9.6/pdkmaster/io/parsing/tf.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/io/pdkmaster/export.py` & `PDKMaster-0.9.6/pdkmaster/io/pdkmaster/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,18 +73,22 @@
     def _params_unhandled(self, prim): # pragma: no cover
         raise RuntimeError(f"Internal error: unhandled params for {prim.__class__.__name__}")
 
     def _params_designmask(self, prim: _prm.DesignMaskPrimitiveT):
         s = ""
         if prim.grid is not None:
             s += f"grid={prim.grid},"
-        if isinstance(prim, _prm.BlockageAttrPrimitiveT) and prim.blockage is not None:
+        try:
+            blockage: _prm.Marker = prim.blockage # type: ignore
+        except AttributeError:
+            pass
+        else:
             if s:
                 s += " "
-            s += f"blockage={_str_prim(prim.blockage)},"
+            s += f"blockage={_str_prim(blockage)},"
         s += "\n"
 
         return s
 
     def _params_widthspace(self, prim: _prm.WidthSpacePrimitiveT):
         s = f"min_width={prim.min_width}, min_space={prim.min_space},\n"
         if prim.space_table is not None:
@@ -93,16 +97,20 @@
                 s += f"    {row},\n"
             s += "),\n"
         s += f"min_area={prim.min_area},\n"
         if prim.min_density is not None:
             s += f"min_density={prim.min_density},\n"
         if prim.max_density is not None:
             s += f"max_density={prim.max_density},\n"
-        if isinstance(prim, _prm.PinAttrPrimitiveT) and prim.pin is not None:
-            s += f"pin={_str_prim(prim.pin)},\n"
+        try:
+            pin: _prm.Marker = prim.pin # type: ignore
+        except AttributeError:
+            pass
+        else:
+            s += f"pin={_str_prim(pin)},\n"
 
         return s
 
     def _params_widthspacedesignmask(self, prim: _prm.WidthSpaceDesignMaskPrimitiveT):
         return self._params_widthspace(prim) + self._params_designmask(prim)
 
     def _params_Base(self, prim: _prm.Base):
@@ -189,19 +197,18 @@
         if prim.contact is not None:
             assert prim.min_contact_space is not None
             s += (
                 f"contact={_str_prim(prim.contact)},"
                 f" min_contact_space={prim.min_contact_space},\n"
             )
         if prim.implant is not None:
-            s += f"implant={_str_prim(prim.implant)}"
-            if prim.min_implant_enclosure is not None:
-                s += f", min_implant_enclosure={_str_enclosure(prim.min_implant_enclosure)},\n"
-            else:
-                s += ",\n"
+            s += (
+                f"implant={_str_primtuple(prim.implant)}, "
+                f", min_implant_enclosure={_str_enclosures(prim.min_implant_enclosure)},\n"
+            )
         return s
 
     def _params_MIMCapacitor(self, prim: _prm.MIMCapacitor):
         return (
             f"bottom={_str_prim(prim.bottom)},\n"
             f"top={_str_prim(prim.top)},\n"
             f"via={_str_prim(prim.via)},\n"
@@ -213,17 +220,17 @@
             f"min_top2bottom_space={prim.min_top2bottom_space},\n"
         )
 
     def _params_Diode(self, prim: _prm.Diode):
         s = f"wire={_str_prim(prim.wire)}, indicator={_str_primtuple(prim.indicator)},\n"
         s += f"min_width={prim.min_width},\n"
         s += f"min_indicator_enclosure={_str_enclosures(prim.min_indicator_enclosure)},\n"
-        s += f"implant={_str_prim(prim.implant)}"
+        s += f"implant={_str_primtuple(prim.implant)}"
         if prim.min_implant_enclosure is not None:
-            s += f", min_implant_enclosure={_str_enclosure(prim.min_implant_enclosure)}"
+            s += f", min_implant_enclosure={_str_enclosures(prim.min_implant_enclosure)}"
         s += ",\n"
         if prim.well is not None:
             s += f"well={_str_prim(prim.well)}"
             if prim.min_well_enclosure is not None:
                 s += f", min_well_enclosure={_str_enclosure(prim.min_well_enclosure)}"
             s += ",\n"
         return s
```

### Comparing `PDKMaster-0.9.5/pdkmaster/io/spice/pyspice.py` & `PDKMaster-0.9.6/pdkmaster/io/spice/pyspice.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/io/spice/spice_.py` & `PDKMaster-0.9.6/pdkmaster/io/spice/spice_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/edge.py` & `PDKMaster-0.9.6/pdkmaster/technology/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/geometry.py` & `PDKMaster-0.9.6/pdkmaster/technology/geometry.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/mask.py` & `PDKMaster-0.9.6/pdkmaster/technology/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/net.py` & `PDKMaster-0.9.6/pdkmaster/technology/net.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/primitive/_core.py` & `PDKMaster-0.9.6/pdkmaster/technology/primitive/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 
         super().__init__(**maskprimitive_args)
 
     @abc.abstractmethod
     def _generate_rules(self, *,
         tech: "_tch.Technology",
     ) -> Iterable[_rle.RuleT]:
-        from .conductors import _PinAttribute
+        from .layers import Marker
 
         yield from super()._generate_rules(tech=tech)
 
         yield from (
             self.mask.width >= self.min_width,
             self.mask.space >= self.min_space,
         )
@@ -265,16 +265,20 @@
                     )
                 else:
                     submask = self.mask.parts_with(condition=(
                         self.mask.width >= w[0],
                         self.mask.length >= w[1],
                     ))
                 yield _msk.Spacing(submask, self.mask) >= row[1]
-        if isinstance(self, _PinAttribute) and self.pin is not None:
-            yield _msk.Connect(self.mask, self.pin.mask)
+        try:
+            pin: Marker = self.pin # type: ignore
+        except AttributeError:
+            pass
+        else:
+            yield _msk.Connect(self.mask, pin.mask)
 WidthSpacePrimitiveT = _WidthSpacePrimitive
 
 
 class _WidthSpaceDesignMaskPrimitive(_DesignMaskPrimitive, _WidthSpacePrimitive):
     """_WidthSpacePrimitive that is also a _DesignMaskPrimitive
     """
     pass
```

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/primitive/_derived.py` & `PDKMaster-0.9.6/pdkmaster/technology/primitive/_derived.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/primitive/_param.py` & `PDKMaster-0.9.6/pdkmaster/technology/primitive/_param.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/primitive/conductors.py` & `PDKMaster-0.9.6/pdkmaster/technology/primitive/conductors.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,33 +34,45 @@
 
     The blockage layer is a layer to indicate areas where no base layer
     shapes should be added. This is often used by place-and-route to
     not add routing in certain places. The blockage layer can then also be
     used to have abstract view of cells that don't contain the real
     shapes but just the area where the router should not add shapes.
     """
-    def __init__(self, *, blockage: Optional["Marker"]=None, **super_args):
-        self.blockage = blockage
+    def __init__(self, *, blockage: Optional[Marker]=None, **super_args):
+        self._blockage = blockage
         super().__init__(**super_args)
+
+    @property
+    def blockage(self) -> Marker:
+        if self._blockage is None:
+            raise AttributeError(f"Primitive '{self.name}' has no blockage attribute")
+        return self._blockage
 BlockageAttrPrimitiveT = _BlockageAttribute
 
 
 class _PinAttribute(_Primitive):
     """Mixin class for primitives with a pin attribute
 
     The pin layer is a layer that can indicate where external signals
     of a cell can be connected. The exact rules of how to use this pin
     layer are PDK specific.
     """
     def __init__(self, *,
-        pin: Optional["Marker"]=None,
+        pin: Optional[Marker]=None,
         **super_args,
     ):
-        self.pin = pin
+        self._pin = pin
         super().__init__(**super_args)
+
+    @property
+    def pin(self) -> Marker:
+        if self._pin is None:
+            raise AttributeError(f"Primitive '{self.name}' has no pin attribute")
+        return self._pin
 PinAttrPrimitiveT = _PinAttribute
 
 
 class _Conductor(_BlockageAttribute, _PinAttribute, _DesignMaskPrimitive):
     """Primitive that acts as a conductor.
 
     This primitive is assumed to use a DesignMask as it's mask. And will
```

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/primitive/devices.py` & `PDKMaster-0.9.6/pdkmaster/technology/primitive/devices.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,16 +104,16 @@
     def __init__(self, *, name: str,
         wire: ResistorWireT,
         min_width: Optional[float]=None, min_length: Optional[float]=None,
         min_space: Optional[float]=None,
         contact: Optional[Via], min_contact_space: Optional[float]=None,
         indicator: MultiT[ResistorIndicatorT],
         min_indicator_extension: MultiT[float],
-        implant: Optional[Implant]=None,
-        min_implant_enclosure: Optional[_prp.Enclosure]=None,
+        implant: OptMultiT[Implant]=(),
+        min_implant_enclosure: OptMultiT[_prp.Enclosure]=(),
         **super_args,
     ):
         # If both model and sheetres are specified, sheetres will be used for
         # LVS circuit generation in pyspice export.
         self.wire = wire
 
         if min_width is None:
@@ -135,40 +135,48 @@
         self.min_space = min_space
 
         self.indicator = indicator = cast_MultiT(indicator)
         self.min_indicator_extension = min_indicator_extension = cast_MultiT_n(
             _util.i2f_recursive(min_indicator_extension), n=len(indicator),
         )
 
-        if implant is not None:
-            if isinstance(implant, Well):
+        if implant is None:
+            implant = ()
+        implant = cast_MultiT(implant)
+        for impl in implant:
+            if isinstance(impl, Well):
                 raise TypeError(
-                    f"Resistor implant may not be Well '{implant.name}'",
+                    f"Resistor implant may not be Well '{impl.name}'",
                 )
             if isinstance(wire, WaferWire):
-                if implant not in wire.implant:
+                if impl not in wire.implant:
                     raise ValueError(
-                        f"implant '{implant.name}' is not valid for waferwire '{wire.name}'"
+                        f"implant '{impl.name}' is not valid for waferwire '{wire.name}'"
                     )
             elif not isinstance(wire, GateWire):
                 raise ValueError(
                     f"Resistor {name}: "
                     "implant may only be provided for a wire of type "
                     "'WaferWire' or 'GateWire'"
                 )
-        elif min_implant_enclosure is not None:
-            raise TypeError(
-                "min_implant_enclosure has to be 'None' if no implant is given"
-            )
         self.implant = implant
+        if min_implant_enclosure is None:
+            min_implant_enclosure = ()
+        if implant and not min_implant_enclosure:
+            def get_enc(impl: Implant):
+                if isinstance(wire, WaferWire):
+                    idx = wire.implant.index(impl)
+                    return wire.min_implant_enclosure[idx]
+                else:
+                    return _prp.Enclosure(0.0)
+            min_implant_enclosure = tuple(get_enc(impl) for impl in implant)
+        min_implant_enclosure = cast_MultiT_n(min_implant_enclosure, n=len(implant))
         self.min_implant_enclosure = min_implant_enclosure
 
-        prims = (wire, *indicator)
-        if implant:
-            prims += (implant,)
+        prims = (wire, *indicator, *implant)
         mask = _msk.Intersect(prim.mask for prim in prims).alias(f"resistor:{name}")
 
         super().__init__(name=name, mask=mask, **super_args)
 
         self.ports += (
             _PrimitiveNet(prim=self, name=name)
             for name in ("port1", "port2")
@@ -226,17 +234,21 @@
 
         if self.min_length > (self.wire.min_width + _geo.epsilon):
             length_edge = _edg.Intersect((resistorbody_edge, wire_edge))
             yield length_edge.length >= self.min_length
 
         for i, ind in enumerate(self.indicator):
             ext = self.min_indicator_extension[i]
-            mask = self.wire.mask.remove(ind.mask)
+            mask = ind.mask.remove(self.wire.mask)
             yield mask.width >= ext
 
+        for i, implant in enumerate(self.implant):
+            enc = self.min_implant_enclosure[i]
+            yield self.mask.enclosed_by(implant.mask) >= enc
+
 
 class _Capacitor(_DevicePrimitive):
     """This is a abstract base class for all capacitor types.
     It needs to be subclassed.
     """
     pass
 CapacitorT = _Capacitor
@@ -328,20 +340,22 @@
 DiodeIndicatorT = Union[Marker, ExtraProcess]
 class Diode(_DevicePrimitive, _MaskPrimitive):
     """`Diode` represent a diode device made up of a WaferWire object.
     A diode device needs a pn-junction which does need to be achieved by
     implants.
 
     Arguments:
-        name: optional name for the diode; otherwise a unique name starting
-            with "diode:" will be generated.
+        name: name for the diode
         wire: the base layer for the diode
+        min_width: minimum width of the diode.
+            The minimum width of the wire layer is taken as default value.
         indicator: list of indicator layers for the Diode. Only the
             overlapping area of all the indicator layers will be seen as
-            the Resistor device.
+            the Resistor device. At least one indicator layer has to be given;
+            diodes without indicators are considered to be parasitic devices.
             Both ExtraProcess and Marker are valid indicator layers.
         min_indicator_extension: minimum required enclosure of the base wire
             by the indicator. If only one value is given it will
             be used for all the indicators.
         implant: the implant layer of the WaferWire forming the diode.
             The implant layer has to be a valid implant layer for the
             base WaferWire primitive.
@@ -357,49 +371,59 @@
         min_well_enclosure: optional minimum required enclosure of the
             base wire by the well. If no well is specified no
             min_well_enclosure may be specified either. If a well is
             specified but no min_well_enclosure the minimum well enclosure
             from the base WaferWire will be used.
     """
     def __init__(self, *, name: str,
-        wire: WaferWire, indicator: MultiT[DiodeIndicatorT],
-        min_width: Optional[float]=None,
-        min_indicator_enclosure: MultiT[_prp.Enclosure],
-        implant: Implant, min_implant_enclosure: Optional[_prp.Enclosure]=None,
+        wire: WaferWire, min_width: Optional[float]=None,
+        indicator: MultiT[DiodeIndicatorT], min_indicator_enclosure: MultiT[_prp.Enclosure],
+        implant: MultiT[Implant], min_implant_enclosure: OptMultiT[_prp.Enclosure]=(),
         well: Optional[Well]=None, min_well_enclosure: Optional[_prp.Enclosure]=None,
         **super_args,
     ):
         self.wire = wire
 
-        self.indicator = indicator = cast_MultiT(indicator)
-
         if min_width is None:
             min_width = wire.min_width
         elif min_width < wire.min_width:
             raise ValueError("min_width may not be smaller than base wire min_width")
         self.min_width = min_width
 
+        self.indicator = indicator = cast_MultiT(indicator)
+        if not indicator:
+            raise ValueError(f"No indicator(s) given for Diode `{name}`")
+
         self.min_indicator_enclosure = min_indicator_enclosure = cast_MultiT_n(
             min_indicator_enclosure, n=len(indicator),
         )
 
-        if isinstance(implant, Well):
-            raise TypeError(f"implant '{implant.name}' is a well")
-        if not implant in wire.implant:
-            raise ValueError(
-                f"implant '{implant.name}' is not valid for waferwire '{wire.name}'"
-            )
-        self.implant = implant
+        self.implant = implant = cast_MultiT(implant)
+        for impl in implant:
+            if isinstance(impl, Well):
+                raise TypeError(f"implant '{impl.name}' is a well")
+            if impl not in wire.implant:
+                raise ValueError(
+                    f"implant '{impl.name}' is not valid for waferwire '{wire.name}'"
+                )
+        if min_implant_enclosure is None:
+            min_implant_enclosure=()
+        if implant and not min_implant_enclosure:
+            def get_enc(impl: Implant) -> _prp.Enclosure:
+                idx = wire.implant.index(impl)
+                return wire.min_implant_enclosure[idx]
+            min_implant_enclosure = tuple(get_enc(impl) for impl in implant)
+        min_implant_enclosure = cast_MultiT_n(min_implant_enclosure, n=len(implant))
         self.min_implant_enclosure = min_implant_enclosure
 
         if "mask" in super_args:
             raise TypeError("Diode got an unexpected keyword argument 'mask'")
         else:
             super_args["mask"] = _msk.Intersect(
-                prim.mask for prim in (wire, *indicator, implant)
+                prim.mask for prim in (wire, *indicator, *implant)
             ).alias(f"diode:{name}")
 
         super().__init__(name=name, **super_args)
 
         self.ports += (
             _PrimitiveNet(prim=self, name=name)
             for name in ("anode", "cathode")
@@ -412,31 +436,33 @@
             if min_well_enclosure is not None:
                 raise TypeError("min_well_enclosure given without a well")
         else:
             if well not in wire.well:
                 raise ValueError(
                     f"well '{well.name}' is not a valid well for wire '{wire.name}'"
                 )
-            if well.type_ == implant.type_:
-                raise ValueError(
-                    f"type of implant '{implant.name}' may not be the same as"
-                    " type of well '{well.name}' for a diode"
-                )
+            for impl in implant:
+                if well.type_ == impl.type_:
+                    raise ValueError(
+                        f"type of implant '{impl.name}' may not be the same as"
+                        " type of well '{well.name}' for a diode"
+                    )
         self.well = well
         self.min_well_enclosure = min_well_enclosure
 
         self.params += (
             _DeviceParam(primitive=self, name="width", default=self.min_width),
             _DeviceParam(primitive=self, name="height", default=self.min_width),
         )
 
     @property
     def designmasks(self) -> Iterable[_msk.DesignMask]:
         yield from self.wire.designmasks
-        yield from self.implant.designmasks
+        for impl in self.implant:
+            yield from impl.designmasks
         if self.well is not None:
             yield from self.well.designmasks
         yield from super().designmasks
 
     def _generate_rules(self, *,
         tech: _tch.Technology,
     ) -> Iterable[_rle.RuleT]:
@@ -447,16 +473,18 @@
         yield cast(_msk._MaskAlias, self.mask)
         if self.min_width > self.wire.min_width:
             yield self.mask.width >= self.min_width
         for i, ind in enumerate(self.indicator):
             enc = self.min_indicator_enclosure[i]
             yield self.wire.mask.enclosed_by(ind.mask) >= enc
         if self.min_implant_enclosure is not None:
-            enc = self.min_implant_enclosure
-            yield self.mask.enclosed_by(self.implant.mask) >= enc
+            for i, impl in enumerate(self.implant):
+                idx = self.implant.index(impl)
+                enc = self.min_implant_enclosure[idx]
+                yield self.mask.enclosed_by(impl.mask) >= enc
 
 
 class MOSFETGate(_WidthSpacePrimitive):
     """MOSFETGate is a primitive representing the gate of a MOSFET transistor.
     A self-aligned process is assumed for the MOSFET so the gate is basically
     the area where a gate layer crosses the active layer. A dielectric layer
     in between the two layers is forming the gate capacitor the is part of the
```

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/primitive/layers.py` & `PDKMaster-0.9.6/pdkmaster/technology/primitive/layers.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/primitive/rules.py` & `PDKMaster-0.9.6/pdkmaster/technology/primitive/rules.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/property_.py` & `PDKMaster-0.9.6/pdkmaster/technology/property_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/rule.py` & `PDKMaster-0.9.6/pdkmaster/technology/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/technology_.py` & `PDKMaster-0.9.6/pdkmaster/technology/technology_.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 from math import floor, ceil
 import abc
-from typing import Dict, Optional, Union, Iterable, cast, overload
+from typing import List, Dict, Optional, Union, Iterable, cast, overload
 
 from . import (
     property_ as _prp, rule as _rle, mask as _msk, wafer_ as _wfr, geometry as _geo,
     primitive as _prm,
 )
 
 
@@ -170,20 +170,20 @@
                 ww2 = primitive2.waferwire
 
                 spaces.extend((
                     self.min_space(ww1, primitive2),
                     self.min_space(ww2, primitive1),
                 ))
 
-                e1s = []
+                e1s: List[float] = []
                 for prim in primitive1.prim:
                     enc = get_enc(ww=ww1, prim=prim)
                     if enc is not None:
                         e1s.append(enc)
-                e2s = []
+                e2s: List[float] = []
                 for prim in primitive2.prim:
                     enc = get_enc(ww=ww2, prim=prim)
                     if enc is not None:
                         e2s.append(enc)
                 if (len(e1s) > 0) and (len(e2s) > 0):
                     spaces.append(max(e1s) + max(e2s))
 
@@ -372,16 +372,14 @@
 
     def _build_interconnect(self) -> None:
         prims = self._primitives
 
         neworder = []
         def add_prims(prims2):
             for prim in prims2:
-                if prim is None:
-                    continue
                 idx = prims.index(prim)
                 if idx not in neworder:
                     neworder.append(idx)
 
         def get_name(prim):
             return prim.name
 
@@ -426,18 +424,22 @@
         # process vias
         vias = set(prims.__iter_type__(_prm.Via))
 
         def allwires(wire):
             if isinstance(wire, _prm.Resistor):
                 yield from allwires(wire.wire)
                 yield from wire.indicator
-            if isinstance(wire, _prm.PinAttrPrimitiveT) and wire.pin is not None:
-                yield wire.pin
-            if isinstance(wire, _prm.BlockageAttrPrimitiveT) and wire.blockage is not None:
-                yield wire.blockage
+            try:
+                yield wire.pin # type: ignore
+            except AttributeError:
+                pass
+            try:
+                yield wire.blockage # type: ignore
+            except AttributeError:
+                pass
             yield wire
 
         connvias = set(filter(lambda via: any(w in via.bottom for w in bottomwires), vias))
         if connvias:
             viatops = set()
             while connvias:
                 viabottoms = set()
@@ -473,15 +475,18 @@
             raise Technology.ConnectionError(
                 f"vias ({', '.join(via.name for via in vias)}) have no connection to"
                 " a technology bottom wire"
             )
 
         # Add via and it's blockage layers
         vias = tuple(prims.__iter_type__(_prm.Via))
-        add_prims(prim.blockage for prim in vias)
+        add_prims(prim.blockage for prim in filter(
+            lambda v: hasattr(v, "blockage"),
+            vias
+        ))
         # Now add all vias
         add_prims(vias)
 
         # process mosfets
         mosfets = set(prims.__iter_type__(_prm.MOSFET))
         gates = {mosfet.gate for mosfet in mosfets}
         allgates = set(prims.__iter_type__(_prm.MOSFETGate))
@@ -534,14 +539,15 @@
         # process top metal wires
         add_prims(prims.__iter_type__(_prm.TopMetalWire))
 
         # process resistors
         resistors = set(prims.__iter_type__(_prm.Resistor))
         for resistor in resistors:
             markers.update(resistor.indicator)
+            implants.update(resistor.implant)
 
         # process capacitors
         mimtops = set(prims.__iter_type__(_prm.MIMTop))
         mimcaps = tuple(prims.__iter_type__(_prm.MIMCapacitor))
         usedtops = set(c.top for c in mimcaps)
         unusedtops = mimtops - usedtops
         if unusedtops:
@@ -559,15 +565,15 @@
         bipolars = set(prims.__iter_type__(_prm.Bipolar))
         for bipolar in bipolars:
             markers.update(bipolar.indicator)
 
         # extra rules
         rules = set(prims.__iter_type__(_prm.RulePrimitiveT))
 
-        add_prims((*markers, *resistors, *mimcaps, *diodes, *bipolars, *rules))
+        add_prims((*implants, *markers, *resistors, *mimcaps, *diodes, *bipolars, *rules))
 
         # process auxiliary
         def aux_key(aux: _prm.Auxiliary) -> str:
             return aux.name
         add_prims(sorted(prims.__iter_type__(_prm.Auxiliary), key=aux_key))
 
         # reorder primitives
```

### Comparing `PDKMaster-0.9.5/pdkmaster/technology/wafer_.py` & `PDKMaster-0.9.6/pdkmaster/technology/wafer_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/pdkmaster/typing.py` & `PDKMaster-0.9.6/pdkmaster/typing.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/setup.py` & `PDKMaster-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/skill.py` & `PDKMaster-0.9.6/skill.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/skill2yaml.py` & `PDKMaster-0.9.6/skill2yaml.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/_util.py` & `PDKMaster-0.9.6/test/unit/_util.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/design/cell.py` & `PDKMaster-0.9.6/test/unit/design/cell.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/design/circuit.py` & `PDKMaster-0.9.6/test/unit/design/circuit.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/design/factory.py` & `PDKMaster-0.9.6/test/unit/design/factory.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/design/layout.py` & `PDKMaster-0.9.6/test/unit/design/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,27 @@
         hvox = prims.hvox
         ch = prims.contact
         metal = prims.metal
         metalpin = prims.metalpin
         metal2 = prims.metal2
         metal2pin = prims.metal2pin
         ndiode = prims.ndiode
+        nmos = prims.nmos
+
+        # WaferWire with single implant
+        active2 = _prm.WaferWire(
+            name="active2", min_width=0.2, min_space=0.5,
+            allow_in_substrate=False,
+            implant=nplus, min_implant_enclosure=_prp.Enclosure(0.05),
+            implant_abut=nplus, allow_contactless_implant=False,
+            well=nwell, min_well_enclosure=_prp.Enclosure(0.1),
+            min_well_enclosure_same_type=_prp.Enclosure(0.08),
+            allow_well_crossing=False,
+            oxide=hvox, min_oxide_enclosure=_prp.Enclosure(0.08),
+        )
 
         class MyNet(_net._Net):
             def __init__(self, name: str):
                 super().__init__(name)
         net = MyNet("net")
 
         # Unexpected parameter
@@ -103,37 +116,46 @@
 
         self.assertAlmostEqual(params["width"], 2.0)
         self.assertIsNone(params["height"])
 
         with self.assertRaises(ValueError):
             caster(prim=metal, pin=metal2pin)
 
-        # WaferWire with single implant
-        active2 = _prm.WaferWire(
-            name="active2", min_width=0.2, min_space=0.5,
-            allow_in_substrate=False,
-            implant=nplus, min_implant_enclosure=_prp.Enclosure(0.05),
-            implant_abut=nplus, allow_contactless_implant=False,
-            well=nwell, min_well_enclosure=_prp.Enclosure(0.1),
-            min_well_enclosure_same_type=_prp.Enclosure(0.08),
-            allow_well_crossing=False,
-            oxide=hvox, min_oxide_enclosure=_prp.Enclosure(0.08),
+        ### WaferWire
+        enc = _prp.Enclosure(1.0)
+        params = caster(prim=active, implant=(nplus, pplus), implant_enclosure=enc)
+        self.assertEqual(
+            params["implant_enclosure"], (enc, enc),
         )
-        params = caster(prim=active2, well_net=net, oxide=hvox)
 
-        self.assertEqual(params["implant"], None)
-        self.assertAlmostEqual(params["implant_enclosure"], None)
+        params = caster(prim=active2, well_net=net, oxide=hvox)
+        self.assertEqual(params["implant"], ())
+        self.assertEqual(params["implant_enclosure"], ())
         self.assertEqual(params["well"], nwell)
         self.assertAlmostEqual(params["oxide_enclosure"].first, 0.08)
 
-        ### Via errors
+        # Wrong implant type
+        with self.assertRaises(TypeError):
+            caster(prim=active2, implant=5, well_net=net)
+        with self.assertRaises(TypeError):
+            caster(prim=active2, implant=(5,), well_net=net)
+        with self.assertRaises(ValueError):
+            caster(prim=active2, implant=metal, well_net=net)
+        with self.assertRaises(ValueError):
+            caster(prim=active2, implant=(metal,), well_net=net)
+
+        # implant_enclosure without implant
+        with self.assertRaises(TypeError):
+            caster(prim=active, implant_enclosure=1.0)
 
-        # wrong bottom_well
+        # Wrong number of enclosures
         with self.assertRaises(ValueError):
-            caster(prim=ch, bottom=active, bottom_implant=nplus, bottom_well=deepwell)
+            caster(prim=active, implant=(nplus, pplus), implant_enclosure=3*(enc,))
+
+        ### Via errors
 
         # bottom WaferWire parameters given for GateWire bottom
         with self.assertRaises(TypeError):
             caster(prim=ch, bottom=poly, bottom_implant=nplus)
         with self.assertRaises(TypeError):
             caster(prim=ch, bottom=poly, bottom_implant_enclosure=0.3)
         with self.assertRaises(TypeError):
@@ -146,26 +168,14 @@
         ### Via coverage
 
         # default bottom_well_enclosure
         params = caster(
             prim=ch, bottom=active, bottom_implant=pplus, bottom_well=nwell,
         )
 
-        self.assertEqual(params["bottom_well_enclosure"], active.min_well_enclosure[0])
-
-        # ch with active not allowed in substrate
-        ch2 = _prm.Via(
-            name="contact2", width=0.2, min_space=0.2,
-            bottom=(active2, poly), top=metal,
-            min_bottom_enclosure=_prp.Enclosure(0.2), min_top_enclosure=_prp.Enclosure(0.15),
-        )
-        # no bottom_well for waferwire not allowed in substrate
-        with self.assertRaises(TypeError):
-            caster(prim=ch2, bottom=active2, bottom_implant=nplus)
-
         # via with one bottom and one top
         via2 = _prm.Via(
             name="via2", width=0.35, min_space=0.35,
             bottom=metal, top=metal2,
             min_bottom_enclosure=_prp.Enclosure(0.2), min_top_enclosure=_prp.Enclosure(0.15),
         )
         # default bottom & top
@@ -176,14 +186,19 @@
 
         # Diode to cover _DevicePrimitive
 
         params = caster(prim=ndiode, width=2.0, height=None)
         self.assertAlmostEqual(params["width"], 2.0)
         self.assertAlmostEqual(params["height"], active.min_width)
 
+        # Wrong number of implant enclosures for MOSFET gate
+
+        with self.assertRaises(TypeError):
+            caster(prim=nmos, gateimplant_enclosures=(1.0, 2.0))
+
 
 class LayoutTest(unittest.TestCase):
     def test__rect(self):
 
         self.assertEqual(
             _layprim._rect(left=0.0, bottom=0.0, right=1.0, top=1.0, enclosure=1.0),
             _layprim._rect(
@@ -615,25 +630,21 @@
                         _geo.MaskShape(mask=prims.hvox.mask, shape=rect_enc),
                     ))
                 ),
             )),
         )
 
         # WaferWire with well but no well_net
-        with self.assertRaises(ValueError):
+        with self.assertRaises(TypeError):
             lay = layouter(
                 prims.active, width=1.0, height=1.0,
-                implant=prims.nplus, implant_enclosure=_prp.Enclosure(0.2),
+                implant=prims.pplus, implant_enclosure=_prp.Enclosure(0.2),
                 well=prims.nwell, well_enclosure=_prp.Enclosure(1.0),
             )
 
-        # MIMTop
-        with self.assertRaises(ValueError):
-            layouter(prims.MIMTop)
-
         # Via with bottom/top_enclosure as value
         lay = layouter(
             prims.via, space=0.35, rows=1, columns=1,
             bottom=prims.metal, bottom_enclosure=enc,
             bottom_width=None, bottom_height=None,
             top=prims.metal2, top_enclosure=enc,
             top_width=None, top_height=None,
```

### Comparing `PDKMaster-0.9.5/test/unit/design/library.py` & `PDKMaster-0.9.6/test/unit/design/library.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/dispatch/edge.py` & `PDKMaster-0.9.6/test/unit/dispatch/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/dispatch/mask.py` & `PDKMaster-0.9.6/test/unit/dispatch/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/dispatch/primitive.py` & `PDKMaster-0.9.6/test/unit/dispatch/primitive.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/dispatch/rule.py` & `PDKMaster-0.9.6/test/unit/dispatch/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/dispatch/shape.py` & `PDKMaster-0.9.6/test/unit/dispatch/shape.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/dummy.py` & `PDKMaster-0.9.6/test/unit/dummy.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/io/klayout/export.py` & `PDKMaster-0.9.6/test/unit/io/klayout/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/io/klayout/merge.py` & `PDKMaster-0.9.6/test/unit/io/klayout/merge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/io/lefdef/export.py` & `PDKMaster-0.9.6/test/unit/io/lefdef/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/io/pdkmaster/export.py` & `PDKMaster-0.9.6/test/unit/io/pdkmaster/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/io/spice/pyspice.py` & `PDKMaster-0.9.6/test/unit/io/spice/pyspice.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/io/spice/spice_.py` & `PDKMaster-0.9.6/test/unit/io/spice/spice_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/technology/edge.py` & `PDKMaster-0.9.6/test/unit/technology/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/technology/geometry.py` & `PDKMaster-0.9.6/test/unit/technology/geometry.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/technology/mask.py` & `PDKMaster-0.9.6/test/unit/technology/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/technology/primitive.py` & `PDKMaster-0.9.6/test/unit/technology/primitive.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,14 +417,15 @@
                 name="prim1", min_width=1.0, min_space=1.0, space_table=(
                     (2.0, 2.0),
                     ((10.0, 3.0), 3.0),
                 ),
                 min_area=2.0, min_density=0.4, max_density=80,
             )
 
+        pin = _prm.Marker(name="pin")
         prim1 = _prm.MetalWire(
             name="prim1", min_width=1.0, min_space=1.0, space_table=(
                 (2.0, 2.0),
                 ((10.0, 3.0), 3.0),
             ),
             min_area=2.0, min_density=0.4, max_density=0.8,
         )
@@ -432,20 +433,24 @@
             name="prim1", min_width=1.0, min_space=1.0, space_table=(
                 (2.0, 2.0),
                 ((10.0, 3.0), 3.0),
             ),
             min_area=2.0, min_density=0.4, max_density=0.8,
         )
         prim2 = _prm.MetalWire(
-            name="prim2", min_width=1.0, min_space=1.0, grid=0.2,
+            name="prim2", min_width=1.0, min_space=1.0, grid=0.2, pin=pin,
         )
 
         self.assertEqual(prim1, prim1bis)
         self.assertNotEqual(prim1, prim2)
 
+        with self.assertRaises(AttributeError):
+            prim1.pin
+        self.assertEqual(prim2.pin, pin)
+
         rules = tuple(prim1._generate_rules(tech=dummy_tech))
         self.assertIn(prim1.mask, rules)
         rules = tuple(prim2._generate_rules(tech=dummy_tech))
         self.assertIn(prim2.mask, rules)
 
     def test_via(self):
         nimpl = _prm.Implant(
@@ -662,60 +667,61 @@
         with self.assertRaises(ValueError):
             # implant for wire that is not WaferWire or GateWire
             _prm.Resistor(
                 name="error",
                 wire=m1, contact=None, indicator=m1res, min_indicator_extension=0.5,
                 implant=nimpl,
             )
-        with self.assertRaises(TypeError):
+        with self.assertRaises(ValueError):
             # min_implant_enclosure without implant
             prim1 = _prm.Resistor(
                 name="error", min_width=1.2,
                 wire=poly, contact=None, indicator=polyres, min_indicator_extension=0.5,
                 min_implant_enclosure=_prp.Enclosure(0.2),
             )
         with self.assertRaises(ValueError):
             # wire not in via bottom or top
             _prm.Resistor(
                 name="error", min_width=1.2,
                 wire=active, contact=via, min_contact_space=0.1,
                 indicator=polyres, min_indicator_extension=0.5,
-                implant=nimpl,
+                implant=nimpl, min_implant_enclosure=_prp.Enclosure(0.1),
             )
         with self.assertRaises(TypeError):
             # min_contact_space without contact
             _prm.Resistor(
                 name="error", min_width=1.2,
                 wire=poly, contact=None, indicator=polyres, min_indicator_extension=0.5,
                 min_contact_space=0.1,
             )
         with self.assertRaises(TypeError):
             # min_contact_space missing with given contact
             _prm.Resistor(
                 name="error", min_width=1.2,
                 wire=poly, contact=via,
                 indicator=polyres, min_indicator_extension=0.5,
-                implant=nimpl,
+                implant=nimpl, min_implant_enclosure=_prp.Enclosure(0.1),
             )
 
         prim1 = _prm.Resistor(
             name="prim1", min_width=1.2,
             wire=poly, contact=via, min_contact_space=0.1,
             indicator=polyres, min_indicator_extension=0.5,
             implant=nimpl,
         )
         prim1bis = _prm.Resistor(
             name="prim1",
             wire=poly, contact=via, min_contact_space=0.1,
             indicator=polyres, min_indicator_extension=0.5,
-            implant=nimpl,
+            implant=nimpl, min_implant_enclosure=None,
         )
         prim2 = _prm.Resistor(
             name="prim2", min_width=1.0, min_space=1.5,
-            wire=m1, contact=None, indicator=m1res, min_indicator_extension=0.5,
+            wire=m1, contact=None, implant=None,
+            indicator=m1res, min_indicator_extension=0.5,
         )
 
         self.assertEqual(prim1, prim1bis)
         self.assertNotEqual(prim1, prim2)
 
         rules = tuple(prim1._generate_rules(tech=dummy_tech))
         self.assertIn(prim1.mask, rules)
@@ -869,14 +875,20 @@
             # grid parameter given
             _prm.Diode(
                 name="error", wire=active, grid=0.01,
                 indicator=actdiode, min_indicator_enclosure=_prp.Enclosure(0.05),
                 implant=pimpl,
             )
         with self.assertRaises(ValueError):
+            prim1 = _prm.Diode(
+                name="prim1", wire=active, min_width=1.2,
+                indicator=(), min_indicator_enclosure=_prp.Enclosure(0.05),
+                implant=pimpl,
+            )
+        with self.assertRaises(ValueError):
             # min_width too small
             _prm.Diode(
                 name="error", wire=active, min_width=0.5,
                 indicator=actdiode, min_indicator_enclosure=_prp.Enclosure(0.05),
                 implant=pimpl,
             )
         with self.assertRaises(TypeError):
@@ -928,15 +940,15 @@
                 indicator=actdiode, min_indicator_enclosure=_prp.Enclosure(0.05),
                 implant=pimpl, well=pwell,
             )
 
         prim1 = _prm.Diode(
             name="prim1", wire=active, min_width=1.2,
             indicator=actdiode, min_indicator_enclosure=_prp.Enclosure(0.05),
-            implant=pimpl,
+            implant=pimpl, min_implant_enclosure=None,
         )
         prim1bis = _prm.Diode(
             name="prim1", wire=active, min_width=1.2,
             indicator=actdiode, min_indicator_enclosure=_prp.Enclosure(0.05),
             implant=pimpl,
         )
         prim2 = _prm.Diode(
```

### Comparing `PDKMaster-0.9.5/test/unit/technology/property.py` & `PDKMaster-0.9.6/test/unit/technology/property.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/technology/rule.py` & `PDKMaster-0.9.6/test/unit/technology/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/technology/technology.py` & `PDKMaster-0.9.6/test/unit/technology/technology.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/technology/wafer.py` & `PDKMaster-0.9.6/test/unit/technology/wafer.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test/unit/typing.py` & `PDKMaster-0.9.6/test/unit/typing.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.5/test.tf` & `PDKMaster-0.9.6/test.tf`

 * *Files identical despite different names*

