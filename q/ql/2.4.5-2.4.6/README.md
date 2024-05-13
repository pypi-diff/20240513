# Comparing `tmp/ql-2.4.5.tar.gz` & `tmp/ql-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ql-2.4.5.tar", last modified: Mon May  6 18:42:55 2024, max compression
+gzip compressed data, was "ql-2.4.6.tar", last modified: Mon May 13 11:09:41 2024, max compression
```

## Comparing `ql-2.4.5.tar` & `ql-2.4.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1069 2023-12-02 10:49:28.147259 ql-2.4.5/LICENSE
--rw-r--r--   0        0        0    30438 2023-12-02 17:17:28.643589 ql-2.4.5/README.md
--rw-r--r--   0        0        0     1532 2024-05-06 18:42:55.133989 ql-2.4.5/pyproject.toml
--rw-r--r--   0        0        0      112 2024-05-06 18:42:03.102094 ql-2.4.5/src/quill/__init__.py
--rw-r--r--   0        0        0     1281 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/__share__.py
--rw-r--r--   0        0        0       53 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/cyl.ini
--rw-r--r--   0        0        0      547 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/README.md
--rw-r--r--   0        0        0      379 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/__init__.py
--rw-r--r--   0        0        0     9622 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/auditing.py
--rw-r--r--   0        0        0     1311 2023-12-03 23:27:45.026188 ql-2.4.5/src/quill/fold/cli.py
--rw-r--r--   0        0        0       40 2023-12-03 23:24:33.221746 ql-2.4.5/src/quill/fold/cut/__init__.py
--rw-r--r--   0        0        0     3420 2023-12-03 22:41:19.940279 ql-2.4.5/src/quill/fold/cut/audit_checking.py
--rw-r--r--   0        0        0      352 2023-12-03 22:52:13.019343 ql-2.4.5/src/quill/fold/cut/contexts/__init__.py
--rw-r--r--   0        0        0     3579 2023-12-04 09:21:20.771070 ql-2.4.5/src/quill/fold/cut/contexts/article.py
--rw-r--r--   0        0        0      541 2023-12-04 08:43:02.463200 ql-2.4.5/src/quill/fold/cut/contexts/base.py
--rw-r--r--   0        0        0     1214 2023-12-03 22:26:40.726878 ql-2.4.5/src/quill/fold/cut/contexts/helpers.py
--rw-r--r--   0        0        0      299 2023-12-03 22:48:22.507731 ql-2.4.5/src/quill/fold/cut/contexts/index.py
--rw-r--r--   0        0        0     1755 2023-12-04 08:42:44.667686 ql-2.4.5/src/quill/fold/cut/contexts/md.py
--rw-r--r--   0        0        0     2618 2023-12-04 10:01:17.310506 ql-2.4.5/src/quill/fold/cut/contexts/models.py
--rw-r--r--   0        0        0      252 2023-12-03 23:20:05.734748 ql-2.4.5/src/quill/fold/cut/ctx.py
--rw-r--r--   0        0        0     1705 2023-12-03 23:15:49.287613 ql-2.4.5/src/quill/fold/cut/ctx_building.py
--rw-r--r--   0        0        0      251 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/cut/datetime_util.py
--rw-r--r--   0        0        0     1363 2023-12-02 17:06:43.927655 ql-2.4.5/src/quill/fold/cut/interface.py
--rw-r--r--   0        0        0     2381 2023-12-02 16:32:27.062293 ql-2.4.5/src/quill/fold/cut/main.py
--rw-r--r--   0        0        0      250 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/cut/name_config.py
--rw-r--r--   0        0        0      506 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/cut/pymd_engine.py
--rw-r--r--   0        0        0     7056 2023-12-03 23:32:56.952432 ql-2.4.5/src/quill/fold/cut/rules.py
--rw-r--r--   0        0        0     5068 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/cut/templater.py
--rw-r--r--   0        0        0     1999 2024-05-06 18:07:48.726730 ql-2.4.5/src/quill/fold/distrib_setup.py
--rw-r--r--   0        0        0    10795 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/git.py
--rw-r--r--   0        0        0     1242 2024-05-06 18:10:31.424806 ql-2.4.5/src/quill/fold/man.py
--rw-r--r--   0        0        0     2027 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/ns_util.py
--rw-r--r--   0        0        0    11481 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/site_yaml.py
--rw-r--r--   0        0        0      668 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/subdomain.py
--rw-r--r--   0        0        0       40 2023-12-03 23:24:42.617572 ql-2.4.5/src/quill/fold/wire/__init__.py
--rw-r--r--   0        0        0       27 2023-12-02 10:49:28.331261 ql-2.4.5/src/quill/fold/wire/emitters.ini
--rw-r--r--   0        0        0     7595 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/wire/emitters.py
--rw-r--r--   0        0        0     2212 2023-12-02 10:49:28.331261 ql-2.4.5/src/quill/fold/wire/html_elem_util.py
--rw-r--r--   0        0        0     5858 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/wire/html_index_util.py
--rw-r--r--   0        0        0     3937 2023-12-02 10:49:28.331261 ql-2.4.5/src/quill/fold/wire/html_page_util.py
--rw-r--r--   0        0        0      880 2023-12-02 10:49:28.331261 ql-2.4.5/src/quill/fold/wire/html_util.py
--rw-r--r--   0        0        0     1533 2023-12-02 16:32:12.422569 ql-2.4.5/src/quill/fold/wire/main.py
--rw-r--r--   0        0        0     3083 2023-12-02 10:49:28.331261 ql-2.4.5/src/quill/fold/wire/sinks.py
--rw-r--r--   0        0        0     3443 2023-12-02 10:49:28.331261 ql-2.4.5/src/quill/fold/wire/transforms.py
--rw-r--r--   0        0        0     4940 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/fold/yaml_util.py
--rw-r--r--   0        0        0       59 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/manifest/README.md
--rw-r--r--   0        0        0       42 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/manifest/__init__.py
--rw-r--r--   0        0        0      475 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/manifest/man.py
--rw-r--r--   0        0        0      850 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/manifest/namings.py
--rw-r--r--   0        0        0     1223 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/manifest/parsing.py
--rw-r--r--   0        0        0     2212 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/README.md
--rw-r--r--   0        0        0       62 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/__init__.py
--rw-r--r--   0        0        0       44 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/address/__init__.py
--rw-r--r--   0        0        0     9734 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/address/paths.py
--rw-r--r--   0        0        0      863 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/address/routing.py
--rw-r--r--   0        0        0      208 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/io.py
--rw-r--r--   0        0        0      102 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/lever/__init__.py
--rw-r--r--   0        0        0     1121 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/lever/blockelems.py
--rw-r--r--   0        0        0     1383 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/lever/docelems.py
--rw-r--r--   0        0        0      244 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/lever/elems.py
--rw-r--r--   0        0        0      627 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/lever/git.py
--rw-r--r--   0        0        0     5830 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/lever/lists.py
--rw-r--r--   0        0        0      265 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/lever/mmd.py
--rw-r--r--   0        0        0     5056 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/lever/parser.py
--rw-r--r--   0        0        0     2607 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/lever/structure.py
--rw-r--r--   0        0        0     9463 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/scan/lever/tokens.py
--rw-r--r--   0        0        0       52 2023-12-02 10:49:28.335261 ql-2.4.5/src/quill/spin.ini
--rw-r--r--   0        0        0    31710 1970-01-01 00:00:00.000000 ql-2.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-12-02 10:49:28.147259 ql-2.4.6/LICENSE
+-rw-r--r--   0        0        0    30438 2023-12-02 17:17:28.643589 ql-2.4.6/README.md
+-rw-r--r--   0        0        0     1554 2024-05-13 11:09:41.643882 ql-2.4.6/pyproject.toml
+-rw-r--r--   0        0        0      112 2024-05-13 11:08:58.540632 ql-2.4.6/src/quill/__init__.py
+-rw-r--r--   0        0        0     1281 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/__share__.py
+-rw-r--r--   0        0        0       53 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/cyl.ini
+-rw-r--r--   0        0        0      547 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/fold/README.md
+-rw-r--r--   0        0        0      379 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/fold/__init__.py
+-rw-r--r--   0        0        0     9622 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/fold/auditing.py
+-rw-r--r--   0        0        0     1311 2023-12-03 23:27:45.026188 ql-2.4.6/src/quill/fold/cli.py
+-rw-r--r--   0        0        0       40 2023-12-03 23:24:33.221746 ql-2.4.6/src/quill/fold/cut/__init__.py
+-rw-r--r--   0        0        0     3420 2023-12-03 22:41:19.940279 ql-2.4.6/src/quill/fold/cut/audit_checking.py
+-rw-r--r--   0        0        0      352 2023-12-03 22:52:13.019343 ql-2.4.6/src/quill/fold/cut/contexts/__init__.py
+-rw-r--r--   0        0        0     3579 2023-12-04 09:21:20.771070 ql-2.4.6/src/quill/fold/cut/contexts/article.py
+-rw-r--r--   0        0        0      541 2023-12-04 08:43:02.463200 ql-2.4.6/src/quill/fold/cut/contexts/base.py
+-rw-r--r--   0        0        0     1214 2023-12-03 22:26:40.726878 ql-2.4.6/src/quill/fold/cut/contexts/helpers.py
+-rw-r--r--   0        0        0      299 2023-12-03 22:48:22.507731 ql-2.4.6/src/quill/fold/cut/contexts/index.py
+-rw-r--r--   0        0        0     1755 2023-12-04 08:42:44.667686 ql-2.4.6/src/quill/fold/cut/contexts/md.py
+-rw-r--r--   0        0        0     2618 2023-12-04 10:01:17.310506 ql-2.4.6/src/quill/fold/cut/contexts/models.py
+-rw-r--r--   0        0        0      252 2023-12-03 23:20:05.734748 ql-2.4.6/src/quill/fold/cut/ctx.py
+-rw-r--r--   0        0        0     1705 2023-12-03 23:15:49.287613 ql-2.4.6/src/quill/fold/cut/ctx_building.py
+-rw-r--r--   0        0        0      251 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/fold/cut/datetime_util.py
+-rw-r--r--   0        0        0     1363 2023-12-02 17:06:43.927655 ql-2.4.6/src/quill/fold/cut/interface.py
+-rw-r--r--   0        0        0     2381 2023-12-02 16:32:27.062293 ql-2.4.6/src/quill/fold/cut/main.py
+-rw-r--r--   0        0        0      250 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/fold/cut/name_config.py
+-rw-r--r--   0        0        0      506 2024-05-13 11:05:23.680380 ql-2.4.6/src/quill/fold/cut/pymd_engine.py
+-rw-r--r--   0        0        0     7056 2024-05-08 12:31:32.796225 ql-2.4.6/src/quill/fold/cut/rules.py
+-rw-r--r--   0        0        0     5068 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/fold/cut/templater.py
+-rw-r--r--   0        0        0     1999 2024-05-06 18:07:48.726730 ql-2.4.6/src/quill/fold/distrib_setup.py
+-rw-r--r--   0        0        0    10795 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/fold/git.py
+-rw-r--r--   0        0        0     1242 2024-05-06 18:10:31.424806 ql-2.4.6/src/quill/fold/man.py
+-rw-r--r--   0        0        0     2027 2024-05-08 12:27:13.515747 ql-2.4.6/src/quill/fold/ns_util.py
+-rw-r--r--   0        0        0    11481 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/fold/site_yaml.py
+-rw-r--r--   0        0        0      668 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/fold/subdomain.py
+-rw-r--r--   0        0        0       40 2023-12-03 23:24:42.617572 ql-2.4.6/src/quill/fold/wire/__init__.py
+-rw-r--r--   0        0        0       27 2023-12-02 10:49:28.331261 ql-2.4.6/src/quill/fold/wire/emitters.ini
+-rw-r--r--   0        0        0     7595 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/fold/wire/emitters.py
+-rw-r--r--   0        0        0     2212 2023-12-02 10:49:28.331261 ql-2.4.6/src/quill/fold/wire/html_elem_util.py
+-rw-r--r--   0        0        0     5858 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/fold/wire/html_index_util.py
+-rw-r--r--   0        0        0     3937 2023-12-02 10:49:28.331261 ql-2.4.6/src/quill/fold/wire/html_page_util.py
+-rw-r--r--   0        0        0      880 2023-12-02 10:49:28.331261 ql-2.4.6/src/quill/fold/wire/html_util.py
+-rw-r--r--   0        0        0     1533 2023-12-02 16:32:12.422569 ql-2.4.6/src/quill/fold/wire/main.py
+-rw-r--r--   0        0        0     3083 2023-12-02 10:49:28.331261 ql-2.4.6/src/quill/fold/wire/sinks.py
+-rw-r--r--   0        0        0     3443 2023-12-02 10:49:28.331261 ql-2.4.6/src/quill/fold/wire/transforms.py
+-rw-r--r--   0        0        0     4940 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/fold/yaml_util.py
+-rw-r--r--   0        0        0       59 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/manifest/README.md
+-rw-r--r--   0        0        0       42 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/manifest/__init__.py
+-rw-r--r--   0        0        0      475 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/manifest/man.py
+-rw-r--r--   0        0        0      850 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/manifest/namings.py
+-rw-r--r--   0        0        0     1223 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/manifest/parsing.py
+-rw-r--r--   0        0        0     2212 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/README.md
+-rw-r--r--   0        0        0       62 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/__init__.py
+-rw-r--r--   0        0        0       44 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/address/__init__.py
+-rw-r--r--   0        0        0     9734 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/address/paths.py
+-rw-r--r--   0        0        0      863 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/address/routing.py
+-rw-r--r--   0        0        0      208 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/io.py
+-rw-r--r--   0        0        0      102 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/lever/__init__.py
+-rw-r--r--   0        0        0     1121 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/lever/blockelems.py
+-rw-r--r--   0        0        0     1383 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/lever/docelems.py
+-rw-r--r--   0        0        0      244 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/lever/elems.py
+-rw-r--r--   0        0        0      627 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/lever/git.py
+-rw-r--r--   0        0        0     5830 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/lever/lists.py
+-rw-r--r--   0        0        0      265 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/lever/mmd.py
+-rw-r--r--   0        0        0     5056 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/lever/parser.py
+-rw-r--r--   0        0        0     2607 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/lever/structure.py
+-rw-r--r--   0        0        0     9463 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/scan/lever/tokens.py
+-rw-r--r--   0        0        0       52 2023-12-02 10:49:28.335261 ql-2.4.6/src/quill/spin.ini
+-rw-r--r--   0        0        0    31740 1970-01-01 00:00:00.000000 ql-2.4.6/PKG-INFO
```

### Comparing `ql-2.4.5/LICENSE` & `ql-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/README.md` & `ql-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/pyproject.toml` & `ql-2.4.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -34,18 +34,19 @@
     "markdown",
     "pygments",
     "python-frontmatter",
     "dateparser",
     "markdown-katex>=202112.1034",
     "pathlib2",
     "pydantic>=2.5.2",
+    "ocxsect>=0.1.5",
 ]
 requires-python = ">=3.10,<3.13"
 readme = "README.md"
-version = "2.4.5"
+version = "2.4.6"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/spin-systems/quill"
 Repository = "https://github.com/spin-systems/quill.git"
```

### Comparing `ql-2.4.5/src/quill/__share__.py` & `ql-2.4.6/src/quill/__share__.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/README.md` & `ql-2.4.6/src/quill/fold/README.md`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/auditing.py` & `ql-2.4.6/src/quill/fold/auditing.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/cli.py` & `ql-2.4.6/src/quill/fold/cli.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/cut/audit_checking.py` & `ql-2.4.6/src/quill/fold/cut/audit_checking.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/cut/contexts/article.py` & `ql-2.4.6/src/quill/fold/cut/contexts/article.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/cut/contexts/base.py` & `ql-2.4.6/src/quill/fold/cut/contexts/base.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/cut/contexts/helpers.py` & `ql-2.4.6/src/quill/fold/cut/contexts/helpers.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/cut/contexts/md.py` & `ql-2.4.6/src/quill/fold/cut/contexts/md.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/cut/contexts/models.py` & `ql-2.4.6/src/quill/fold/cut/contexts/models.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/cut/ctx_building.py` & `ql-2.4.6/src/quill/fold/cut/ctx_building.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/cut/interface.py` & `ql-2.4.6/src/quill/fold/cut/interface.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/cut/main.py` & `ql-2.4.6/src/quill/fold/cut/main.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/cut/rules.py` & `ql-2.4.6/src/quill/fold/cut/rules.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/cut/templater.py` & `ql-2.4.6/src/quill/fold/cut/templater.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/distrib_setup.py` & `ql-2.4.6/src/quill/fold/distrib_setup.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/git.py` & `ql-2.4.6/src/quill/fold/git.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/man.py` & `ql-2.4.6/src/quill/fold/man.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/ns_util.py` & `ql-2.4.6/src/quill/fold/ns_util.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/site_yaml.py` & `ql-2.4.6/src/quill/fold/site_yaml.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/subdomain.py` & `ql-2.4.6/src/quill/fold/subdomain.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/wire/emitters.py` & `ql-2.4.6/src/quill/fold/wire/emitters.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/wire/html_elem_util.py` & `ql-2.4.6/src/quill/fold/wire/html_elem_util.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/wire/html_index_util.py` & `ql-2.4.6/src/quill/fold/wire/html_index_util.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/wire/html_page_util.py` & `ql-2.4.6/src/quill/fold/wire/html_page_util.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/wire/html_util.py` & `ql-2.4.6/src/quill/fold/wire/html_util.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/wire/main.py` & `ql-2.4.6/src/quill/fold/wire/main.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/wire/sinks.py` & `ql-2.4.6/src/quill/fold/wire/sinks.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/wire/transforms.py` & `ql-2.4.6/src/quill/fold/wire/transforms.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/fold/yaml_util.py` & `ql-2.4.6/src/quill/fold/yaml_util.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/manifest/namings.py` & `ql-2.4.6/src/quill/manifest/namings.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/manifest/parsing.py` & `ql-2.4.6/src/quill/manifest/parsing.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/scan/README.md` & `ql-2.4.6/src/quill/scan/README.md`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/scan/address/paths.py` & `ql-2.4.6/src/quill/scan/address/paths.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/scan/address/routing.py` & `ql-2.4.6/src/quill/scan/address/routing.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/scan/lever/blockelems.py` & `ql-2.4.6/src/quill/scan/lever/blockelems.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/scan/lever/docelems.py` & `ql-2.4.6/src/quill/scan/lever/docelems.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/scan/lever/git.py` & `ql-2.4.6/src/quill/scan/lever/git.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/scan/lever/lists.py` & `ql-2.4.6/src/quill/scan/lever/lists.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/scan/lever/parser.py` & `ql-2.4.6/src/quill/scan/lever/parser.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/scan/lever/structure.py` & `ql-2.4.6/src/quill/scan/lever/structure.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/src/quill/scan/lever/tokens.py` & `ql-2.4.6/src/quill/scan/lever/tokens.py`

 * *Files identical despite different names*

### Comparing `ql-2.4.5/PKG-INFO` & `ql-2.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ql
-Version: 2.4.5
+Version: 2.4.6
 Summary: spin.systems generator and driver
 Keywords: website,staticjinja
 Author-Email: Louis Maddox <louismmx@gmail.com>
 License: MIT
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,14 +30,15 @@
 Requires-Dist: markdown
 Requires-Dist: pygments
 Requires-Dist: python-frontmatter
 Requires-Dist: dateparser
 Requires-Dist: markdown-katex>=202112.1034
 Requires-Dist: pathlib2
 Requires-Dist: pydantic>=2.5.2
+Requires-Dist: ocxsect>=0.1.5
 Description-Content-Type: text/markdown
 
 # quill
 
 [![PyPI](https://img.shields.io/pypi/v/ql?logo=python&logoColor=%23cccccc)](https://pypi.org/project/ql)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/spin-systems/quill/master.svg)](https://results.pre-commit.ci/latest/github/spin-systems/quill/master)
```

