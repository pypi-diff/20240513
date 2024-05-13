# Comparing `tmp/joserfc-0.8.0.tar.gz` & `tmp/joserfc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joserfc-0.8.0.tar", last modified: Wed Sep  6 13:10:17 2023, max compression
+gzip compressed data, was "joserfc-0.9.0.tar", last modified: Thu Nov 16 08:06:42 2023, max compression
```

## Comparing `joserfc-0.8.0.tar` & `joserfc-0.9.0.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.143231 joserfc-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (999)     1501 2023-09-06 13:10:07.000000 joserfc-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      142 2023-09-06 13:10:07.000000 joserfc-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     2456 2023-09-06 13:10:17.143231 joserfc-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1286 2023-09-06 13:10:07.000000 joserfc-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.119231 joserfc-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (999)      112 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.119231 joserfc-0.8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (999)      223 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (999)    17717 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/_static/dark-logo.svg
--rwxr-xr-x   0 runner    (1001) docker     (999)      674 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/_static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (999)    17719 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/_static/light-logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.119231 joserfc-0.8.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (999)       85 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)      151 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/api/jwe.rst
--rw-r--r--   0 runner    (1001) docker     (999)      151 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/api/jwk.rst
--rw-r--r--   0 runner    (1001) docker     (999)      151 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/api/jws.rst
--rw-r--r--   0 runner    (1001) docker     (999)      151 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/api/jwt.rst
--rw-r--r--   0 runner    (1001) docker     (999)     2423 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (999)     2898 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.119231 joserfc-0.8.0/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (999)       79 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/contributing/authors.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1605 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)       18 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/contributing/sponsors.rst
--rw-r--r--   0 runner    (1001) docker     (999)     2994 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/contributing/structure.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1189 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/contributing/translation.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.123231 joserfc-0.8.0/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (999)     6702 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/guide/algorithms.rst
--rw-r--r--   0 runner    (1001) docker     (999)     2358 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1978 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/guide/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (999)     7267 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/guide/jwe.rst
--rw-r--r--   0 runner    (1001) docker     (999)    11295 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/guide/jwk.rst
--rw-r--r--   0 runner    (1001) docker     (999)    13154 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/guide/jws.rst
--rw-r--r--   0 runner    (1001) docker     (999)     8413 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/guide/jwt.rst
--rw-r--r--   0 runner    (1001) docker     (999)     6287 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/guide/registry.rst
--rw-r--r--   0 runner    (1001) docker     (999)     2117 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1842 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.115231 joserfc-0.8.0/docs/locales/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.115231 joserfc-0.8.0/docs/locales/zh/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.123231 joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (999)    25085 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/api.po
--rw-r--r--   0 runner    (1001) docker     (999)     5173 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/changelog.po
--rw-r--r--   0 runner    (1001) docker     (999)     8499 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/contributing.po
--rw-r--r--   0 runner    (1001) docker     (999)    50862 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/guide.po
--rw-r--r--   0 runner    (1001) docker     (999)     3864 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/index.po
--rw-r--r--   0 runner    (1001) docker     (999)     3637 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/install.po
--rw-r--r--   0 runner    (1001) docker     (999)     7674 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/migrations.po
--rw-r--r--   0 runner    (1001) docker     (999)     1914 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/recipes.po
--rw-r--r--   0 runner    (1001) docker     (999)     2148 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/security.po
--rw-r--r--   0 runner    (1001) docker     (999)     2769 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/stability.po
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.123231 joserfc-0.8.0/docs/migrations/
--rw-r--r--   0 runner    (1001) docker     (999)     3857 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/migrations/authlib.rst
--rw-r--r--   0 runner    (1001) docker     (999)      149 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/migrations/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)     4552 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/migrations/pyjwt.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.123231 joserfc-0.8.0/docs/recipes/
--rw-r--r--   0 runner    (1001) docker     (999)      110 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/recipes/azure.rst
--rw-r--r--   0 runner    (1001) docker     (999)     2540 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/recipes/openssl.rst
--rw-r--r--   0 runner    (1001) docker     (999)      973 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/security.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1629 2023-09-06 13:10:07.000000 joserfc-0.8.0/docs/stability.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1832 2023-09-06 13:10:07.000000 joserfc-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-06 13:10:17.143231 joserfc-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-06 13:10:07.000000 joserfc-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.115231 joserfc-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.127231 joserfc-0.8.0/src/joserfc/
--rw-r--r--   0 runner    (1001) docker     (999)      141 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5647 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.127231 joserfc-0.8.0/src/joserfc/drafts/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/drafts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1470 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/drafts/jwe_chacha20.py
--rw-r--r--   0 runner    (1001) docker     (999)     5296 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/drafts/jwe_ecdh_1pu.py
--rw-r--r--   0 runner    (1001) docker     (999)     3149 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/errors.py
--rw-r--r--   0 runner    (1001) docker     (999)    10550 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/jwe.py
--rw-r--r--   0 runner    (1001) docker     (999)     1759 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/jwk.py
--rw-r--r--   0 runner    (1001) docker     (999)    10266 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/jws.py
--rw-r--r--   0 runner    (1001) docker     (999)     4090 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/jwt.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/py.typed
--rw-r--r--   0 runner    (1001) docker     (999)     6765 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.127231 joserfc-0.8.0/src/joserfc/rfc7515/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7515/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2108 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7515/compact.py
--rw-r--r--   0 runner    (1001) docker     (999)     5449 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7515/json.py
--rw-r--r--   0 runner    (1001) docker     (999)     3583 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7515/model.py
--rw-r--r--   0 runner    (1001) docker     (999)     2714 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7515/registry.py
--rw-r--r--   0 runner    (1001) docker     (999)      756 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7515/types.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.127231 joserfc-0.8.0/src/joserfc/rfc7516/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7516/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1760 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7516/compact.py
--rw-r--r--   0 runner    (1001) docker     (999)     3982 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7516/json.py
--rw-r--r--   0 runner    (1001) docker     (999)    10079 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7516/message.py
--rw-r--r--   0 runner    (1001) docker     (999)    10231 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7516/models.py
--rw-r--r--   0 runner    (1001) docker     (999)     3817 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7516/registry.py
--rw-r--r--   0 runner    (1001) docker     (999)      676 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7516/types.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.127231 joserfc-0.8.0/src/joserfc/rfc7517/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7517/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    10929 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7517/models.py
--rw-r--r--   0 runner    (1001) docker     (999)     4313 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7517/pem.py
--rw-r--r--   0 runner    (1001) docker     (999)      461 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7517/types.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.131231 joserfc-0.8.0/src/joserfc/rfc7518/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7518/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1570 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7518/derive_key.py
--rw-r--r--   0 runner    (1001) docker     (999)     5151 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7518/ec_key.py
--rw-r--r--   0 runner    (1001) docker     (999)    12602 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7518/jwe_algs.py
--rw-r--r--   0 runner    (1001) docker     (999)     4344 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7518/jwe_encs.py
--rw-r--r--   0 runner    (1001) docker     (999)      557 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7518/jwe_zips.py
--rw-r--r--   0 runner    (1001) docker     (999)     6605 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7518/jws_algs.py
--rw-r--r--   0 runner    (1001) docker     (999)     2302 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7518/oct_key.py
--rw-r--r--   0 runner    (1001) docker     (999)     5932 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7518/rsa_key.py
--rw-r--r--   0 runner    (1001) docker     (999)      298 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7518/util.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.131231 joserfc-0.8.0/src/joserfc/rfc7519/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7519/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1367 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7519/claims.py
--rw-r--r--   0 runner    (1001) docker     (999)     5459 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7519/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.131231 joserfc-0.8.0/src/joserfc/rfc7638/
--rw-r--r--   0 runner    (1001) docker     (999)      483 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7638/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.131231 joserfc-0.8.0/src/joserfc/rfc7797/
--rw-r--r--   0 runner    (1001) docker     (999)      277 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7797/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3784 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7797/compact.py
--rw-r--r--   0 runner    (1001) docker     (999)     3590 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7797/json.py
--rw-r--r--   0 runner    (1001) docker     (999)      761 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc7797/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.131231 joserfc-0.8.0/src/joserfc/rfc8037/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc8037/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      993 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc8037/jws_eddsa.py
--rw-r--r--   0 runner    (1001) docker     (999)     5953 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc8037/okp_key.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.131231 joserfc-0.8.0/src/joserfc/rfc8812/
--rw-r--r--   0 runner    (1001) docker     (999)      430 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/rfc8812/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1601 2023-09-06 13:10:07.000000 joserfc-0.8.0/src/joserfc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.127231 joserfc-0.8.0/src/joserfc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     2456 2023-09-06 13:10:17.000000 joserfc-0.8.0/src/joserfc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     4989 2023-09-06 13:10:17.000000 joserfc-0.8.0/src/joserfc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-06 13:10:17.000000 joserfc-0.8.0/src/joserfc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       36 2023-09-06 13:10:17.000000 joserfc-0.8.0/src/joserfc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        8 2023-09-06 13:10:17.000000 joserfc-0.8.0/src/joserfc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.131231 joserfc-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1475 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.135231 joserfc-0.8.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (999)     4154 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/fixtures/jwe_compact_ecdh_1pu.json
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/fixtures/jwe_compact_ecdh_es.json
--rw-r--r--   0 runner    (1001) docker     (999)    14321 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/fixtures/jwe_rfc7520.json
--rw-r--r--   0 runner    (1001) docker     (999)    11569 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/fixtures/jws_examples.json
--rw-r--r--   0 runner    (1001) docker     (999)     8670 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/fixtures/jws_rfc7520.json
--rw-r--r--   0 runner    (1001) docker     (999)     1961 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/fixtures/jws_rfc7797.json
--rw-r--r--   0 runner    (1001) docker     (999)     3591 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/fixtures/jwt_use_jws.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.135231 joserfc-0.8.0/tests/jwe/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2436 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwe/test_chacha20.py
--rw-r--r--   0 runner    (1001) docker     (999)     7840 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwe/test_compact.py
--rw-r--r--   0 runner    (1001) docker     (999)     8657 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwe/test_ecdh_1pu.py
--rw-r--r--   0 runner    (1001) docker     (999)     3905 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwe/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (999)    15944 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwe/test_example.py
--rw-r--r--   0 runner    (1001) docker     (999)     1924 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwe/test_json.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.135231 joserfc-0.8.0/tests/jwk/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2611 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwk/test_ec_key.py
--rw-r--r--   0 runner    (1001) docker     (999)     2535 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwk/test_jwk_set.py
--rw-r--r--   0 runner    (1001) docker     (999)     3766 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwk/test_key_methods.py
--rw-r--r--   0 runner    (1001) docker     (999)     2862 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwk/test_oct_key.py
--rw-r--r--   0 runner    (1001) docker     (999)     3874 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwk/test_okp_key.py
--rw-r--r--   0 runner    (1001) docker     (999)     5687 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwk/test_rsa_key.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.135231 joserfc-0.8.0/tests/jws/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2521 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jws/test_compact.py
--rw-r--r--   0 runner    (1001) docker     (999)     6075 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jws/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (999)     1566 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jws/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (999)     3984 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jws/test_json.py
--rw-r--r--   0 runner    (1001) docker     (999)     4087 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jws/test_rfc7797.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.135231 joserfc-0.8.0/tests/jwt/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4687 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwt/test_claims.py
--rw-r--r--   0 runner    (1001) docker     (999)      908 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwt/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (999)     2609 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/jwt/test_jwt.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.143231 joserfc-0.8.0/tests/keys/
--rw-r--r--   0 runner    (1001) docker     (999)     1653 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/RFC7516-A.1.3.json
--rw-r--r--   0 runner    (1001) docker     (999)     1653 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/RFC7516-A.2.3.json
--rw-r--r--   0 runner    (1001) docker     (999)      323 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/RFC7520-EC-108.json
--rw-r--r--   0 runner    (1001) docker     (999)      263 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/RFC7520-EC-120.json
--rw-r--r--   0 runner    (1001) docker     (999)      392 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/RFC7520-EC-private.json
--rw-r--r--   0 runner    (1001) docker     (999)      293 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/RFC7520-EC-public.json
--rw-r--r--   0 runner    (1001) docker     (999)     1712 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/RFC7520-RSA-73.json
--rw-r--r--   0 runner    (1001) docker     (999)     3271 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/RFC7520-RSA-84.json
--rw-r--r--   0 runner    (1001) docker     (999)     1712 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/RFC7520-RSA-private.json
--rw-r--r--   0 runner    (1001) docker     (999)      446 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/RFC7520-RSA-public.json
--rw-r--r--   0 runner    (1001) docker     (999)      137 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/RFC7520-oct-130.json
--rw-r--r--   0 runner    (1001) docker     (999)      158 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/RFC7520-oct-enc.json
--rw-r--r--   0 runner    (1001) docker     (999)      156 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/RFC7520-oct-sig.json
--rw-r--r--   0 runner    (1001) docker     (999)      287 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      198 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/ec-p256-alice.json
--rw-r--r--   0 runner    (1001) docker     (999)      198 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/ec-p256-bob.json
--rw-r--r--   0 runner    (1001) docker     (999)      227 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/ec-p256-private.pem
--rw-r--r--   0 runner    (1001) docker     (999)      178 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/ec-p256-public.pem
--rw-r--r--   0 runner    (1001) docker     (999)      288 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/ec-p384-private.pem
--rw-r--r--   0 runner    (1001) docker     (999)      215 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/ec-p384-public.pem
--rw-r--r--   0 runner    (1001) docker     (999)      361 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/ec-p512-private.pem
--rw-r--r--   0 runner    (1001) docker     (999)      268 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/ec-p512-public.pem
--rw-r--r--   0 runner    (1001) docker     (999)      223 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/ec-secp256k1-private.pem
--rw-r--r--   0 runner    (1001) docker     (999)      174 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/ec-secp256k1-public.pem
--rw-r--r--   0 runner    (1001) docker     (999)      191 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/okp-ed25519-private.json
--rw-r--r--   0 runner    (1001) docker     (999)      139 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/okp-ed25519-public.json
--rw-r--r--   0 runner    (1001) docker     (999)      156 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/okp-ed448-private.pem
--rw-r--r--   0 runner    (1001) docker     (999)      146 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/okp-ed448-public.pem
--rw-r--r--   0 runner    (1001) docker     (999)      146 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/okp-x25519-alice.json
--rw-r--r--   0 runner    (1001) docker     (999)      146 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/okp-x25519-bob.json
--rw-r--r--   0 runner    (1001) docker     (999)      146 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/okp-x25519-charlie.json
--rw-r--r--   0 runner    (1001) docker     (999)     3243 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/rsa-openssl-private.pem
--rw-r--r--   0 runner    (1001) docker     (999)      800 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/rsa-openssl-public.pem
--rw-r--r--   0 runner    (1001) docker     (999)     3381 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/ssh-rsa-private.pem
--rw-r--r--   0 runner    (1001) docker     (999)      738 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/keys/ssh-rsa-public.pem
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:17.143231 joserfc-0.8.0/tests/rfc7520/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/rfc7520/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     7022 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/rfc7520/test_jwe.py
--rw-r--r--   0 runner    (1001) docker     (999)     8925 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/rfc7520/test_jws.py
--rw-r--r--   0 runner    (1001) docker     (999)      717 2023-09-06 13:10:07.000000 joserfc-0.8.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.576036 joserfc-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-11-16 08:06:35.000000 joserfc-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-11-16 08:06:35.000000 joserfc-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2023-11-16 08:06:42.576036 joserfc-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-11-16 08:06:35.000000 joserfc-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.544036 joserfc-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.544036 joserfc-0.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    17717 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/_static/dark-logo.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      674 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/_static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    17719 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/_static/light-logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.544036 joserfc-0.9.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/api/jwe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/api/jwk.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/api/jws.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/api/jwt.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.548036 joserfc-0.9.0/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/contributing/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/contributing/sponsors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/contributing/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/contributing/translation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.548036 joserfc-0.9.0/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/guide/algorithms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/guide/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/guide/jwe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11295 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/guide/jwk.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/guide/jws.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/guide/jwt.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/guide/registry.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.540036 joserfc-0.9.0/docs/locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.540036 joserfc-0.9.0/docs/locales/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.552036 joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    25085 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/api.po
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/changelog.po
+-rw-r--r--   0 runner    (1001) docker     (127)     9548 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/contributing.po
+-rw-r--r--   0 runner    (1001) docker     (127)    50962 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/guide.po
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/index.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/install.po
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/migrations.po
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/recipes.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/security.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/stability.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.552036 joserfc-0.9.0/docs/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/migrations/authlib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/migrations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/migrations/pyjwt.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.552036 joserfc-0.9.0/docs/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/recipes/azure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/recipes/openssl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/security.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-11-16 08:06:35.000000 joserfc-0.9.0/docs/stability.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-11-16 08:06:35.000000 joserfc-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 08:06:42.576036 joserfc-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 08:06:35.000000 joserfc-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.540036 joserfc-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.552036 joserfc-0.9.0/src/joserfc/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.556036 joserfc-0.9.0/src/joserfc/drafts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/drafts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/drafts/jwe_chacha20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/drafts/jwe_ecdh_1pu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/jwe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/jwk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/jws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.556036 joserfc-0.9.0/src/joserfc/rfc7515/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7515/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7515/compact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5449 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7515/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7515/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7515/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7515/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.556036 joserfc-0.9.0/src/joserfc/rfc7516/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7516/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7516/compact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7516/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7516/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7516/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7516/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7516/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.556036 joserfc-0.9.0/src/joserfc/rfc7517/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7517/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7517/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7517/pem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7517/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.560036 joserfc-0.9.0/src/joserfc/rfc7518/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7518/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7518/derive_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7518/ec_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7518/jwe_algs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7518/jwe_encs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7518/jwe_zips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7518/jws_algs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7518/oct_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7518/rsa_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7518/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.560036 joserfc-0.9.0/src/joserfc/rfc7519/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7519/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7519/claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7519/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.560036 joserfc-0.9.0/src/joserfc/rfc7638/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7638/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.560036 joserfc-0.9.0/src/joserfc/rfc7797/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7797/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7797/compact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7797/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc7797/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.560036 joserfc-0.9.0/src/joserfc/rfc8037/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc8037/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc8037/jws_eddsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5953 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc8037/okp_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.564036 joserfc-0.9.0/src/joserfc/rfc8812/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/rfc8812/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2023-11-16 08:06:35.000000 joserfc-0.9.0/src/joserfc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.556036 joserfc-0.9.0/src/joserfc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2023-11-16 08:06:42.000000 joserfc-0.9.0/src/joserfc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2023-11-16 08:06:42.000000 joserfc-0.9.0/src/joserfc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 08:06:42.000000 joserfc-0.9.0/src/joserfc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-16 08:06:42.000000 joserfc-0.9.0/src/joserfc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-16 08:06:42.000000 joserfc-0.9.0/src/joserfc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.564036 joserfc-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.564036 joserfc-0.9.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/fixtures/jwe_compact_ecdh_1pu.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/fixtures/jwe_compact_ecdh_es.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14321 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/fixtures/jwe_rfc7520.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11569 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/fixtures/jws_examples.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/fixtures/jws_rfc7520.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/fixtures/jws_rfc7797.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/fixtures/jwt_use_jws.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.564036 joserfc-0.9.0/tests/jwe/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwe/test_chacha20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwe/test_compact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwe/test_ecdh_1pu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwe/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15944 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwe/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwe/test_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.568036 joserfc-0.9.0/tests/jwk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwk/test_ec_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwk/test_jwk_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwk/test_key_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwk/test_oct_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwk/test_okp_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwk/test_rsa_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.568036 joserfc-0.9.0/tests/jws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jws/test_compact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jws/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jws/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jws/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jws/test_rfc7797.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.568036 joserfc-0.9.0/tests/jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwt/test_claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwt/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/jwt/test_jwt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.572036 joserfc-0.9.0/tests/keys/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/RFC7516-A.1.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/RFC7516-A.2.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/RFC7520-EC-108.json
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/RFC7520-EC-120.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/RFC7520-EC-private.json
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/RFC7520-EC-public.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/RFC7520-RSA-73.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/RFC7520-RSA-84.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/RFC7520-RSA-private.json
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/RFC7520-RSA-public.json
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/RFC7520-oct-130.json
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/RFC7520-oct-enc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/RFC7520-oct-sig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/ec-p256-alice.json
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/ec-p256-bob.json
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/ec-p256-private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/ec-p256-public.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/ec-p384-private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/ec-p384-public.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/ec-p512-private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/ec-p512-public.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/ec-secp256k1-private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/ec-secp256k1-public.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/okp-ed25519-private.json
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/okp-ed25519-public.json
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/okp-ed448-private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/okp-ed448-public.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/okp-x25519-alice.json
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/okp-x25519-bob.json
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/okp-x25519-charlie.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/rsa-openssl-private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/rsa-openssl-public.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/ssh-rsa-private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/keys/ssh-rsa-public.pem
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:42.576036 joserfc-0.9.0/tests/rfc7520/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/rfc7520/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/rfc7520/test_jwe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/rfc7520/test_jws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2023-11-16 08:06:35.000000 joserfc-0.9.0/tests/test_util.py
```

### Comparing `joserfc-0.8.0/LICENSE` & `joserfc-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/PKG-INFO` & `joserfc-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joserfc
-Version: 0.8.0
+Version: 0.9.0
 Summary: The ultimate Python library for JOSE RFCs, including JWS, JWE, JWK, JWA, JWT
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Documentation, https://jose.authlib.org/
 Project-URL: Source, https://github.com/authlib/joserfc
 Project-URL: Blog, https://blog.authlib.org/
 Classifier: Development Status :: 4 - Beta
@@ -20,16 +20,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: drafts
 License-File: LICENSE
+Requires-Dist: cryptography
+Provides-Extra: drafts
+Requires-Dist: pycryptodome; extra == "drafts"
 
 JOSE RFC
 ========
 
 `·joserfc·` is a Python library that provides a comprehensive implementation of several
 essential JSON Object Signing and Encryption (JOSE) standards.
```

### Comparing `joserfc-0.8.0/README.rst` & `joserfc-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/_static/dark-logo.svg` & `joserfc-0.9.0/docs/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/_static/icon.svg` & `joserfc-0.9.0/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/_static/light-logo.svg` & `joserfc-0.9.0/docs/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/changelog.rst` & `joserfc-0.9.0/docs/changelog.rst`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,23 @@
 .. _joserfc: https://pypi.org/project/joserfc/
 
 ----
 
 .. module:: joserfc
     :noindex:
 
+0.9.0
+-----
+
+**Released on November 16, 2023**
+
+- Use ``os.urandom`` for ``OctKey.generate_key``.
+- Add ``allow_blank`` for ``JWTClaimsRegistry``.
+- Improve callable key for :meth:`~jwk.guess_key`.
+
 0.8.0
 -----
 
 **Released on September 06, 2023**
 
 - Add :ref:`ensure_kid` method on key models.
 - Add ``auto_kid`` parameter on key model ``.generate_key`` method.
```

### Comparing `joserfc-0.8.0/docs/conf.py` & `joserfc-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/contributing/index.rst` & `joserfc-0.9.0/docs/contributing/index.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/contributing/structure.rst` & `joserfc-0.9.0/docs/contributing/structure.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/contributing/translation.rst` & `joserfc-0.9.0/docs/contributing/translation.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/guide/algorithms.rst` & `joserfc-0.9.0/docs/guide/algorithms.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/guide/index.rst` & `joserfc-0.9.0/docs/guide/index.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/guide/introduction.rst` & `joserfc-0.9.0/docs/guide/introduction.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/guide/jwe.rst` & `joserfc-0.9.0/docs/guide/jwe.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/guide/jwk.rst` & `joserfc-0.9.0/docs/guide/jwk.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/guide/jws.rst` & `joserfc-0.9.0/docs/guide/jws.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/guide/jwt.rst` & `joserfc-0.9.0/docs/guide/jwt.rst`

 * *Files 3% similar despite different names*

```diff
@@ -90,23 +90,44 @@
 ``value``
   OPTIONAL. Requests that the Claim be returned with a particular value.
 
 ``values``
   OPTIONAL. Requests that the Claim be returned with one of a set of values,
   with the values appearing in order of preference.
 
+And we added one more field:
+
+``allow_blank``
+  OPTIONAL. Allow essential claims to be an empty string.
+
 Missing essential claims
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. code-block:: python
 
-    claims = {"iss": "https://authlib.org"}
     claims_requests = JWTClaimsRegistry(aud={"essential": True})
 
-    claims_requests.validate(claims)  # this will raise MissingClaimError
+    # this will raise MissingClaimError
+    claims = {"iss": "https://authlib.org"}
+    claims_requests.validate(claims)
+
+    # this will raise MissingClaimError
+    claims = {"iss": ""}
+    claims_requests.validate(claims)
+
+Allow empty essential claims
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    claims_requests = JWTClaimsRegistry(aud={"essential": True, "allow_blank": True})
+
+    # this will NOT raise MissingClaimError
+    claims = {"iss": ""}
+    claims_requests.validate(claims)
 
 Invalid claims values
 ~~~~~~~~~~~~~~~~~~~~~
 
 .. code-block:: python
 
     claims = {"iss": "https://authlib.org"}
```

### Comparing `joserfc-0.8.0/docs/guide/registry.rst` & `joserfc-0.9.0/docs/guide/registry.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/index.rst` & `joserfc-0.9.0/docs/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,20 @@
     >>> token.header
     {'alg': 'HS256', 'typ': 'JWT'}
     >>> token.claims
     {'k': 'value'}
 
 You would find more details and advanced usage in :ref:`jwt` section.
 
+.. important::
+
+    The string ``"secret"`` employed in the above example is solely intended for demonstration
+    purposes. In a production environment, it is crucial to use a highly secure secret key to
+    ensure robust security measures.
+
 RFCs
 ----
 
 It follows RFCs with extensible API. The module has implementations of:
 
 - RFC7515: :ref:`JSON Web Signature <jws>`
 - RFC7516: :ref:`JSON Web Encryption <jwe>`
```

### Comparing `joserfc-0.8.0/docs/install.rst` & `joserfc-0.9.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/api.po` & `joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/api.po`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/changelog.po` & `joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/changelog.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: joserfc 0.5.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-06 22:04+0900\n"
+"POT-Creation-Date: 2023-11-16 17:05+0900\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh\n"
 "Language-Team: zh <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -24,209 +24,230 @@
 msgstr "历史记录"
 
 #: ../../changelog.rst:6
 msgid "Here is the history of joserfc_ package releases."
 msgstr "这里记录了 joserfc_ 的发布历史。"
 
 #: ../../changelog.rst:16
-msgid "0.8.0"
+msgid "0.9.0"
 msgstr ""
 
 #: ../../changelog.rst:18
-msgid "**Released on September 06, 2023**"
+msgid "**Released on November 16, 2023**"
 msgstr ""
 
 #: ../../changelog.rst:20
-msgid "Add :ref:`ensure_kid` method on key models."
+msgid "Use ``os.urandom`` for ``OctKey.generate_key``."
 msgstr ""
 
 #: ../../changelog.rst:21
+msgid "Add ``allow_blank`` for ``JWTClaimsRegistry``."
+msgstr ""
+
+#: ../../changelog.rst:22
+msgid "Improve callable key for :meth:`~jwk.guess_key`."
+msgstr ""
+
+#: ../../changelog.rst:25
+msgid "0.8.0"
+msgstr ""
+
+#: ../../changelog.rst:27
+msgid "**Released on September 06, 2023**"
+msgstr ""
+
+#: ../../changelog.rst:29
+msgid "Add :ref:`ensure_kid` method on key models."
+msgstr ""
+
+#: ../../changelog.rst:30
 msgid "Add ``auto_kid`` parameter on key model ``.generate_key`` method."
 msgstr ""
 
-#: ../../changelog.rst:22 ../../changelog.rst:32
+#: ../../changelog.rst:31 ../../changelog.rst:41
 msgid "Improvements on type hints"
 msgstr ""
 
-#: ../../changelog.rst:25
+#: ../../changelog.rst:34
 msgid "0.7.0"
 msgstr ""
 
-#: ../../changelog.rst:27
+#: ../../changelog.rst:36
 msgid "**Released on August 14, 2023**"
 msgstr ""
 
-#: ../../changelog.rst:29
+#: ../../changelog.rst:38
 msgid "Add \"iat\" claims validation in JWT."
 msgstr ""
 
-#: ../../changelog.rst:30
+#: ../../changelog.rst:39
 msgid "Add ``__bool__`` magic method on :class:`jwk.KeySet`."
 msgstr ""
 
-#: ../../changelog.rst:31
+#: ../../changelog.rst:40
 msgid ""
 "Raise ``InvalidExchangeKeyError`` for ``exchange_derive_key`` on Curve "
 "key."
 msgstr ""
 
-#: ../../changelog.rst:35
+#: ../../changelog.rst:44
 msgid "0.6.0"
 msgstr ""
 
-#: ../../changelog.rst:37
+#: ../../changelog.rst:46
 msgid "**Released on July 20, 2023**"
 msgstr ""
 
-#: ../../changelog.rst:39
+#: ../../changelog.rst:48
 msgid "Huge improvements on type hints, via :user:`Viicos`."
 msgstr ""
 
-#: ../../changelog.rst:40
+#: ../../changelog.rst:49
 msgid "Do not mutate the header when ``jwt.encode``, via :issue:`6`."
 msgstr ""
 
-#: ../../changelog.rst:41
+#: ../../changelog.rst:50
 msgid "Register algorithms with their matched key types on key set."
 msgstr ""
 
-#: ../../changelog.rst:42
+#: ../../changelog.rst:51
 msgid "Improve error handling, raise proper errors."
 msgstr ""
 
-#: ../../changelog.rst:44
+#: ../../changelog.rst:53
 msgid "**Breaking changes**:"
 msgstr ""
 
-#: ../../changelog.rst:46
+#: ../../changelog.rst:55
 msgid ""
 "``jws.JSONSignature`` is replaced by :class:`jws.GeneralJSONSignature` "
 "and :class:`jws.FlattenedJSONSignature`."
 msgstr ""
 
-#: ../../changelog.rst:48
+#: ../../changelog.rst:57
 msgid ""
 "``jwe.JSONEncryption`` is replaced by :class:`jwe.GeneralJSONEncryption` "
 "and :class:`jwe.FlattenedJSONEncryption`."
 msgstr ""
 
-#: ../../changelog.rst:52
+#: ../../changelog.rst:61
 msgid "0.5.0"
 msgstr ""
 
-#: ../../changelog.rst:54
+#: ../../changelog.rst:63
 msgid "**Released on July 12, 2023**"
 msgstr ""
 
-#: ../../changelog.rst:56
+#: ../../changelog.rst:65
 msgid "Add RFC7797 JSON Web Signature (JWS) Unencoded Payload Option"
 msgstr ""
 
-#: ../../changelog.rst:57
+#: ../../changelog.rst:66
 msgid "Fix ``decrypt_json`` when there is no ``encrypted_key``"
 msgstr ""
 
-#: ../../changelog.rst:58
+#: ../../changelog.rst:67
 msgid "Rename JWE CompleteJSONSerialization to GeneralJSONSerialization"
 msgstr ""
 
-#: ../../changelog.rst:59
+#: ../../changelog.rst:68
 msgid "Rename ``JSONEncryption.flatten`` to ``.flattened``"
 msgstr ""
 
-#: ../../changelog.rst:60
+#: ../../changelog.rst:69
 msgid "Load and dump RSA, EC, and OKP key with password"
 msgstr ""
 
-#: ../../changelog.rst:61
+#: ../../changelog.rst:70
 msgid ""
 "Rename Curve key method: ``exchange_shared_key`` to "
 "``exchange_derive_key``"
 msgstr ""
 
-#: ../../changelog.rst:64
+#: ../../changelog.rst:73
 msgid "0.4.0"
 msgstr ""
 
-#: ../../changelog.rst:66
+#: ../../changelog.rst:75
 msgid "**Released on July 6, 2023**"
 msgstr ""
 
-#: ../../changelog.rst:68
+#: ../../changelog.rst:77
 msgid "Change ``options`` to ``parameters`` for JWK methods"
 msgstr ""
 
-#: ../../changelog.rst:69
+#: ../../changelog.rst:78
 msgid "Change ``JWSRegistry`` and ``JWERegistry`` parameters"
 msgstr ""
 
-#: ../../changelog.rst:70
+#: ../../changelog.rst:79
 msgid "Guess ``sender_key`` from JWKs in JWE"
 msgstr ""
 
-#: ../../changelog.rst:71
+#: ../../changelog.rst:80
 msgid "Add importing key from DER encoding bytes"
 msgstr ""
 
-#: ../../changelog.rst:72
+#: ../../changelog.rst:81
 msgid "Fix JWS JSON serialization when members have only unprotected headers"
 msgstr ""
 
-#: ../../changelog.rst:73
+#: ../../changelog.rst:82
 msgid "Check key type before processing algorithms of JWS and JWE"
 msgstr ""
 
-#: ../../changelog.rst:76
+#: ../../changelog.rst:85
 msgid "0.3.0"
 msgstr ""
 
-#: ../../changelog.rst:78
+#: ../../changelog.rst:87
 msgid "**Released on June 29, 2023**"
 msgstr ""
 
-#: ../../changelog.rst:80
+#: ../../changelog.rst:89
 msgid "Return ``str`` instead of ``bytes`` for JWS and JWE serializations"
 msgstr ""
 
-#: ../../changelog.rst:81
+#: ../../changelog.rst:90
 msgid "Add a ``detach_content`` method for JWS"
 msgstr ""
 
-#: ../../changelog.rst:82
+#: ../../changelog.rst:91
 msgid "Remove ``jwt.extract`` method, because ``extract`` won't work for JWE"
 msgstr ""
 
-#: ../../changelog.rst:83
+#: ../../changelog.rst:92
 msgid "Add ``JWKRegistry`` for JWK"
 msgstr ""
 
-#: ../../changelog.rst:84
+#: ../../changelog.rst:93
 msgid "Update ``JSONEncryption.add_recipient`` parameters"
 msgstr ""
 
-#: ../../changelog.rst:85
+#: ../../changelog.rst:94
 msgid "Export register methods for JWE drafts"
 msgstr ""
 
-#: ../../changelog.rst:88
+#: ../../changelog.rst:97
 msgid "0.2.0"
 msgstr ""
 
-#: ../../changelog.rst:90
+#: ../../changelog.rst:99
 msgid "**Released on June 25, 2023**"
 msgstr ""
 
-#: ../../changelog.rst:92
+#: ../../changelog.rst:101
 msgid "A beta release."
 msgstr ""
 
-#: ../../changelog.rst:95
+#: ../../changelog.rst:104
 msgid "0.1.0"
 msgstr ""
 
-#: ../../changelog.rst:97
+#: ../../changelog.rst:106
 msgid "**Released on March 5, 2023**"
 msgstr ""
 
-#: ../../changelog.rst:99
+#: ../../changelog.rst:108
 msgid "Initial release."
 msgstr ""
+
```

### Comparing `joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/contributing.po` & `joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/contributing.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,48 +4,62 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: joserfc 0.5.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-01 08:56+0900\n"
+"POT-Creation-Date: 2023-11-16 16:35+0900\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh\n"
 "Language-Team: zh <LL@li.org>\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.9.1\n"
 
 #: ../../contributing/authors.rst:2
 msgid "Authors"
 msgstr "作者列表"
 
-#: ../../contributing/authors.rst:5
-msgid "Owner"
-msgstr "所有者"
+#: ../../contributing/authors.rst:4
+msgid ""
+"``joserfc`` is written and maintained by `Hsiaoming Yang "
+"<https://lepture.com>`_."
+msgstr ""
 
 #: ../../contributing/authors.rst:8
-msgid "Maintainer"
-msgstr "维护者"
-
-#: ../../contributing/authors.rst:11
 msgid "Contributors"
 msgstr "贡献者"
 
+#: ../../contributing/authors.rst:10
+msgid "Here is the list of the main contributors:"
+msgstr ""
+
+#: ../../contributing/authors.rst:12
+msgid "`Viicos <https://github.com/Viicos>`_"
+msgstr ""
+
+#: ../../contributing/authors.rst:13
+msgid "`Alon Bar-Lev <https://github.com/alonbl>`_"
+msgstr ""
+
+#: ../../contributing/authors.rst:15
+msgid "And more on https://github.com/authlib/joserfc/graphs/contributors"
+msgstr ""
+
 #: ../../contributing/index.rst:2
 msgid "Contributing"
 msgstr "参与贡献"
 
 #: ../../contributing/index.rst:4
 msgid "Contributions are welcome, and they are greatly appreciated!"
-msgstr ""
+msgstr "欢迎贡献，我们非常感激你的参与！"
 
 #: ../../contributing/index.rst:7
 msgid "Types of contributions"
 msgstr "贡献类型"
 
 #: ../../contributing/index.rst:9
 msgid "There are many ways you can contribute."
@@ -55,47 +69,48 @@
 msgid "Report bugs"
 msgstr "报告错误"
 
 #: ../../contributing/index.rst:14
 msgid ""
 "You're welcome to report bugs at `GitHub Issues "
 "<https://github.com/authlib/joserfc/issues>`_."
-msgstr ""
+msgstr "欢迎使用 `GitHub Issues <https://github.com/authlib/joserfc/issues>`_ "
+"来报告错误。"
 
 #: ../../contributing/index.rst:17
 msgid ""
 "Before reporting a bug, please verify your bug against the latest code in"
 " ``main`` branch."
-msgstr ""
+msgstr "在向我们报告错误前，请先使用 ``main`` 分支的最新代码检查一下，也许该错误已修复。"
 
 #: ../../contributing/index.rst:20
 msgid "When reporting a bug, please including:"
-msgstr ""
+msgstr "报告错误时，请包含："
 
 #: ../../contributing/index.rst:22
 msgid "Your operating system name and version."
-msgstr ""
+msgstr "你的操作系统以及操作系统的版本。"
 
 #: ../../contributing/index.rst:23
 msgid "Your Python version."
-msgstr "你的 Python 版本"
+msgstr "你的 Python 版本。"
 
 #: ../../contributing/index.rst:24
 msgid "Details to reproduce the bug."
-msgstr ""
+msgstr "重现错误的步骤。"
 
 #: ../../contributing/index.rst:27
 msgid "Submit fixes"
-msgstr ""
+msgstr "提交修改"
 
 #: ../../contributing/index.rst:29
 msgid ""
 "Once you found a bug that you can fix, you're welcome to submit your pull"
 " request."
-msgstr ""
+msgstr "一旦你发现了一个可以修复的错误，欢迎向我们提交 Pull Request。"
 
 #: ../../contributing/index.rst:32
 msgid ""
 "Please follow our `git commit conventions "
 "<https://www.conventionalcommits.org/en/v1.0.0/>`_."
 msgstr ""
 
@@ -122,15 +137,15 @@
 
 #: ../../contributing/index.rst:50
 msgid "venv"
 msgstr ""
 
 #: ../../contributing/index.rst:52
 msgid "I strongly suggest you create a virtual environment with ``venv``:"
-msgstr ""
+msgstr "强烈建议你使用 ``venv`` 创建一个虚拟环境："
 
 #: ../../contributing/index.rst:60
 msgid "Install"
 msgstr "安装"
 
 #: ../../contributing/index.rst:62
 msgid "Then install the Python requirements for development:"
@@ -263,45 +278,40 @@
 "start by referring to the :ref:`development` guide, which will help you "
 "set up a suitable development environment. Afterward, navigate to the "
 "docs folder using the following command:"
 msgstr ""
 
 #: ../../contributing/translation.rst:16
 msgid "Generate .pot files"
-msgstr ""
+msgstr "生成 .pot 文件"
 
 #: ../../contributing/translation.rst:18
 msgid ""
 "Before creating translations in your desired languages, you need to "
 "generate the source ``.pot`` files. This can be accomplished using the "
 "following command:"
 msgstr ""
 
 #: ../../contributing/translation.rst:27
 msgid "Update languages"
-msgstr ""
+msgstr "更新语言包"
 
 #: ../../contributing/translation.rst:29
 msgid ""
 "Next, proceed to generate the ``.po`` files in your preferred languages "
 "using the ``sphinx-intl`` tool:"
-msgstr ""
+msgstr "下一步，使用 ``sphinx-intl`` 这个工具来生成你需要的语言的 ``.po`` 文件："
 
 #: ../../contributing/translation.rst:36
 msgid "In this example, we're using the language code ``de`` to represent German."
-msgstr ""
+msgstr "在这个例子中，我们使用语言代码 ``de`` 代表德语。"
 
 #: ../../contributing/translation.rst:39
-#, fuzzy
 msgid "Writing the Translations"
-msgstr "翻译"
+msgstr "更新翻译文件"
 
 #: ../../contributing/translation.rst:41
 msgid ""
 "Following the previous command, the ``.po`` files will be generated "
 "within the ``locales/de/LC_MESSAGES`` directory. You can now edit these "
 "files to add the German translations accordingly."
 msgstr ""
-
-#~ msgid "Then install the Python requirements for unit tests:"
-#~ msgstr ""
-
```

### Comparing `joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/guide.po` & `joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/guide.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: joserfc 0.5.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-01 08:26+0900\n"
+"POT-Creation-Date: 2023-10-07 09:32+0900\n"
 "PO-Revision-Date: 2023-07-15 14:44+0900\n"
 "Last-Translator: Hsiaoming Yang <me@lepture.com>\n"
 "Language: zh\n"
 "Language-Team: zh <LL@li.org>\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.9.1\n"
 
 #: ../../guide/algorithms.rst:6 ../../guide/jws.rst:252
 #: ../../guide/registry.rst:21
 msgid "Algorithms"
 msgstr "算法"
 
 #: ../../guide/algorithms.rst:10
@@ -475,15 +475,15 @@
 
 #: ../../guide/index.rst:73
 msgid "JSON Web Token (JWT) is built on top of :ref:`jws` or :ref:`jwe`."
 msgstr "JSON Web Token (JWT) 本质上是一种 :ref:`jws` 或者 :ref:`jwe`。"
 
 #: ../../guide/index.rst:79
 msgid "Most :ref:`jwt` are encoded with JWS in compact serialization."
-msgstr "通常我们见到的 :ref:`jwt` 都是基于 :ref:`jws` 的紧凑序列化编码。"
+msgstr "通常我们见到的 :ref:`jwt` 都是基于 JWS 的紧凑序列化编码。"
 
 #: ../../guide/index.rst:85
 #, fuzzy
 msgid ""
 "JSON Web Encryption (JWE) represents encrypted content using JSON-based "
 "data structures."
 msgstr "JSON Web Encryption (JWE) 使用基于 JSON 的数据结构表示加密内容。（参考 RFC7516_）"
@@ -691,15 +691,15 @@
 "construct a :class`jwe.FlattenedJSONEncryption` instead:"
 msgstr ""
 
 #: ../../guide/jwe.rst:206
 msgid "And make sure only adding one recipient."
 msgstr "同时注意，你只能增加一位成员。"
 
-#: ../../guide/jwe.rst:209 ../../guide/jwt.rst:267
+#: ../../guide/jwe.rst:209 ../../guide/jwt.rst:288
 msgid "Algorithms & Registry"
 msgstr "算法和注册表"
 
 #: ../../guide/jwe.rst:211
 msgid ""
 "``joserfc.jwe`` module would ONLY allow recommended algorithms by "
 "default, you can find which algorithm is recommended according to "
@@ -1397,184 +1397,200 @@
 
 #: ../../guide/jwt.rst:94
 msgid ""
 "OPTIONAL. Requests that the Claim be returned with one of a set of "
 "values, with the values appearing in order of preference."
 msgstr ""
 
-#: ../../guide/jwt.rst:98
+#: ../../guide/jwt.rst:97
+msgid "And we added one more field:"
+msgstr ""
+
+#: ../../guide/jwt.rst:100
+msgid "``allow_blank``"
+msgstr ""
+
+#: ../../guide/jwt.rst:100
+msgid "OPTIONAL. Allow essential claims to be an empty string."
+msgstr ""
+
+#: ../../guide/jwt.rst:103
 msgid "Missing essential claims"
 msgstr ""
 
-#: ../../guide/jwt.rst:108
+#: ../../guide/jwt.rst:118
+msgid "Allow empty essential claims"
+msgstr ""
+
+#: ../../guide/jwt.rst:129
 msgid "Invalid claims values"
 msgstr ""
 
-#: ../../guide/jwt.rst:118
+#: ../../guide/jwt.rst:139
 msgid "Default validators"
 msgstr ""
 
-#: ../../guide/jwt.rst:120
+#: ../../guide/jwt.rst:141
 msgid ""
 "The ``JWTClaimsRegistry`` has built-in validators for timing related "
 "fields:"
 msgstr ""
 
-#: ../../guide/jwt.rst:122
+#: ../../guide/jwt.rst:143
 msgid "``exp``: expiration time"
 msgstr ""
 
-#: ../../guide/jwt.rst:123
+#: ../../guide/jwt.rst:144
 msgid "``nbf``: not before"
 msgstr ""
 
-#: ../../guide/jwt.rst:124
+#: ../../guide/jwt.rst:145
 msgid "``iat``: issued at"
 msgstr ""
 
-#: ../../guide/jwt.rst:127
+#: ../../guide/jwt.rst:148
 msgid "JWS & JWE"
 msgstr ""
 
-#: ../../guide/jwt.rst:129
+#: ../../guide/jwt.rst:150
 msgid ""
 "JWT is built on top of JWS and JWE, all of the above examples are in JWS."
 " Here is an example of JWE:"
 msgstr ""
 
-#: ../../guide/jwt.rst:142
+#: ../../guide/jwt.rst:163
 msgid ""
 "The JWE formatted result contains 5 parts, while JWS only contains 3 "
 "parts, a JWE example would be something like this (line breaks for "
 "display only):"
 msgstr ""
 
-#: ../../guide/jwt.rst:153
+#: ../../guide/jwt.rst:174
 msgid "Another difference is the key used for ``encode`` and ``decode``."
 msgstr ""
 
-#: ../../guide/jwt.rst:155
+#: ../../guide/jwt.rst:176
 msgid ""
 "For :ref:`jws`, a private key is used for ``encode``, and a public key is"
 " used for ``decode``. The ``encode`` method will use a private key to "
 "sign, and the ``decode`` method will use a public key to verify."
 msgstr ""
 
-#: ../../guide/jwt.rst:159
+#: ../../guide/jwt.rst:180
 msgid ""
 "For :ref:`jwe`, it is the contrary, a public key is used for ``encode``, "
 "and a private key is used for ``decode``. The ``encode`` method  will use"
 " a public key to encrypt, and the ``decode`` method will use a private "
 "key to decrypt."
 msgstr ""
 
-#: ../../guide/jwt.rst:164
+#: ../../guide/jwt.rst:185
 msgid "The key parameter"
 msgstr ""
 
-#: ../../guide/jwt.rst:166
+#: ../../guide/jwt.rst:187
 msgid ""
 "In the above example, we're using :ref:`OctKey` only for simplicity. "
 "There are other types of keys in :ref:`jwk`."
 msgstr ""
 
-#: ../../guide/jwt.rst:170
+#: ../../guide/jwt.rst:191
 msgid "Key types"
 msgstr ""
 
-#: ../../guide/jwt.rst:172
+#: ../../guide/jwt.rst:193
 msgid ""
 "Each algorithm (``alg`` in header) requires a certain type of key. For "
 "example:"
 msgstr ""
 
-#: ../../guide/jwt.rst:174
+#: ../../guide/jwt.rst:195
 msgid "``HS256`` requires ``OctKey``"
 msgstr ""
 
-#: ../../guide/jwt.rst:175
+#: ../../guide/jwt.rst:196
 msgid "``RS256`` requires ``RSAKey``"
 msgstr ""
 
-#: ../../guide/jwt.rst:176
+#: ../../guide/jwt.rst:197
 msgid "``ES256`` requires ``ECKey`` or ``OKPKey``"
 msgstr ""
 
-#: ../../guide/jwt.rst:178
+#: ../../guide/jwt.rst:199
 msgid "You can find the correct key type for each algorithm at:"
 msgstr ""
 
-#: ../../guide/jwt.rst:180 ../../guide/jwt.rst:275
+#: ../../guide/jwt.rst:201 ../../guide/jwt.rst:296
 msgid ":ref:`JSON Web Signature Algorithms <jws_algorithms>`"
 msgstr ""
 
-#: ../../guide/jwt.rst:181 ../../guide/jwt.rst:276
+#: ../../guide/jwt.rst:202 ../../guide/jwt.rst:297
 msgid ":ref:`JSON Web Encryption Algorithms <jwe_algorithms>`"
 msgstr ""
 
-#: ../../guide/jwt.rst:183
+#: ../../guide/jwt.rst:204
 msgid "Here is an example of a JWT with \"alg\" of ``RS256`` in JWS type:"
 msgstr ""
 
-#: ../../guide/jwt.rst:202
+#: ../../guide/jwt.rst:223
 msgid ""
 "In production, ``jwt.encode`` is usually used by the *client* side, a "
 "client normally does not have the access to private keys. The server "
 "provider would usually expose the public keys in JWK Set."
 msgstr ""
 
-#: ../../guide/jwt.rst:207
+#: ../../guide/jwt.rst:228
 msgid "Use key set"
 msgstr ""
 
-#: ../../guide/jwt.rst:209
+#: ../../guide/jwt.rst:230
 msgid ""
 "You can also pass a JWK Set to the ``key`` parameter of :meth:`encode` "
 "and :meth:`decode` methods."
 msgstr ""
 
-#: ../../guide/jwt.rst:226
+#: ../../guide/jwt.rst:247
 msgid ""
 "The methods will find the correct key according to the ``kid`` you "
 "specified. If there is no ``kid`` in header, it will pick on randomly and"
 " add the ``kid`` of the key into header."
 msgstr ""
 
-#: ../../guide/jwt.rst:230
+#: ../../guide/jwt.rst:251
 msgid ""
 "A client would usually get the public key set from a public URL, normally"
 " the ``decode`` code would be something like:"
 msgstr ""
 
-#: ../../guide/jwt.rst:246
+#: ../../guide/jwt.rst:267
 msgid "Callable key"
 msgstr ""
 
-#: ../../guide/jwt.rst:248
+#: ../../guide/jwt.rst:269
 msgid "It is also possible to assign a callable function as the ``key``:"
 msgstr ""
 
-#: ../../guide/jwt.rst:269
+#: ../../guide/jwt.rst:290
 msgid ""
 "The :meth:`encode` and :meth:`decode` accept an ``algorithms`` parameter "
 "for specifying the allowed algorithms. By default, it only allows your to"
 " use recommended algorithms."
 msgstr ""
 
-#: ../../guide/jwt.rst:273
+#: ../../guide/jwt.rst:294
 msgid "You can find out the recommended algorithms at:"
 msgstr ""
 
-#: ../../guide/jwt.rst:278
+#: ../../guide/jwt.rst:299
 msgid ""
 "For instance, ``HS386`` is not a recommended algorithm, and you want to "
 "use this algorithm:"
 msgstr ""
 
-#: ../../guide/jwt.rst:289
+#: ../../guide/jwt.rst:310
 msgid ""
 "If not specifying the ``algorithms`` parameter, the ``encode`` method "
 "will raise an error."
 msgstr ""
 
 #: ../../guide/registry.rst:6
 msgid "Registry"
@@ -1636,15 +1652,15 @@
 "By default, the ``JWSRegistry`` only permits the usage of registered "
 "header parameters. Additionally, it verifies the validity of the header "
 "parameter values before allowing their usage."
 msgstr ""
 
 #: ../../guide/registry.rst:63
 msgid "Type checking"
-msgstr ""
+msgstr "类型检查"
 
 #: ../../guide/registry.rst:65
 msgid ""
 "The header parameter registry for JWS and JWE performs an initial check "
 "on the value type."
 msgstr ""
 
@@ -1706,26 +1722,7 @@
 #: ../../guide/registry.rst:164
 msgid ""
 "JSON Web Token (JWT) is built on top of :ref:`jws` or :ref:`jwe`. The "
 "``encode`` and ``decode`` methods accept a ``registry`` parameter. "
 "Depending on the algorithm of the JWT, you need to decide whether to use "
 "``JWSRegistry`` or ``JWERegistry``."
 msgstr ""
-
-#~ msgid "A128CBC-HS256"
-#~ msgstr ""
-
-#~ msgid "A192CBC-HS384"
-#~ msgstr ""
-
-#~ msgid "A256CBC-HS512"
-#~ msgstr ""
-
-#~ msgid "A128GCM"
-#~ msgstr ""
-
-#~ msgid "A192GCM"
-#~ msgstr ""
-
-#~ msgid "A256GCM"
-#~ msgstr ""
-
```

### Comparing `joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/index.po` & `joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/index.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: joserfc 0.5.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-15 14:44+0900\n"
+"POT-Creation-Date: 2023-11-16 16:35+0900\n"
 "PO-Revision-Date: 2023-07-15 14:44+0900\n"
 "Last-Translator: Hsiaoming Yang <me@lepture.com>\n"
 "Language: zh\n"
 "Language-Team: zh <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.1\n"
 
-#: ../../index.rst:59
+#: ../../index.rst:65
 msgid "Getting started"
 msgstr "开始上手"
 
-#: ../../index.rst:66
+#: ../../index.rst:72
 msgid "Essentials"
 msgstr "必读文档"
 
-#: ../../index.rst:75
+#: ../../index.rst:81
 msgid "Recipes"
 msgstr "小技巧"
 
-#: ../../index.rst:83
+#: ../../index.rst:89
 msgid "Development"
 msgstr "开发者文档"
 
 #: ../../index.rst:2
 msgid "JOSE RFC"
 msgstr ""
 
@@ -43,106 +43,111 @@
 msgid ""
 "``joserfc`` is a Python library that provides a comprehensive "
 "implementation of several essential JSON Object Signing and Encryption "
 "(JOSE) standards, including JWS (JSON Web Signature), JWE (JSON Web "
 "Encryption), JWK (JSON Web Key), JWA (JSON Web Algorithms), and JWT (JSON"
 " Web Tokens)."
 msgstr ""
-"``joserfc`` 是一个提供了多个重要 JSON Object Signing and Encryption (JOSE) "
-"标准的全面实现的 Python 库，包括 JWS (JSON Web Signature)，JWE (JSON Web Encryption)，"
-"JWK (JSON Web Key)，JWA (JSON Web Algorithms)，和 JWT (JSON Web Tokens)。"
-
+"``joserfc`` 是一个提供了多个重要 JSON Object Signing and Encryption (JOSE) 标准的全面实现的"
+" Python 库，包括 JWS (JSON Web Signature)，JWE (JSON Web Encryption)，JWK (JSON"
+" Web Key)，JWA (JSON Web Algorithms)，和 JWT (JSON Web Tokens)。"
 
 #: ../../index.rst:9
 msgid ""
 "It is derived from Authlib_, but features a redesigned API specific to "
 "JOSE functionality."
-msgstr ""
-"它源于 Authlib_，但我们专门为 JOSE 功能重新设计了 API。"
+msgstr "它源于 Authlib_，但我们专门为 JOSE 功能重新设计了 API。"
 
 #: ../../index.rst:14
 msgid "Usage"
 msgstr "使用方法"
 
 #: ../../index.rst:16
 msgid ""
 "A quick and simple JWT encoding and decoding would look something like "
 "this:"
-msgstr ""
-"一个快速而简单的 JWT 编码和解码的示例如下："
+msgstr "一个快速而简单的 JWT 编码和解码的示例如下："
 
 #: ../../index.rst:30
 msgid "You would find more details and advanced usage in :ref:`jwt` section."
 msgstr "您可以在 :ref:`jwt` 部分找到更多详细信息和高级用法。"
 
-#: ../../index.rst:33
+#: ../../index.rst:34
+msgid ""
+"The string ``\"secret\"`` employed in the above example is solely "
+"intended for demonstration purposes. In a production environment, it is "
+"crucial to use a highly secure secret key to ensure robust security "
+"measures."
+msgstr ""
+
+#: ../../index.rst:39
 msgid "RFCs"
 msgstr ""
 
-#: ../../index.rst:35
+#: ../../index.rst:41
 msgid "It follows RFCs with extensible API. The module has implementations of:"
 msgstr "它遵循可扩展的 API，并遵循 RFC 标准。该模块包含以下实现："
 
-#: ../../index.rst:37
+#: ../../index.rst:43
 msgid "RFC7515: :ref:`JSON Web Signature <jws>`"
 msgstr ""
 
-#: ../../index.rst:38
+#: ../../index.rst:44
 msgid "RFC7516: :ref:`JSON Web Encryption <jwe>`"
 msgstr ""
 
-#: ../../index.rst:39
+#: ../../index.rst:45
 msgid "RFC7517: :ref:`JSON Web Key <jwk>`"
 msgstr ""
 
-#: ../../index.rst:40
+#: ../../index.rst:46
 msgid "RFC7518: :ref:`JSON Web Algorithms <jwa>`"
 msgstr ""
 
-#: ../../index.rst:41
+#: ../../index.rst:47
 msgid "RFC7519: :ref:`JSON Web Token <jwt>`"
 msgstr ""
 
-#: ../../index.rst:42
+#: ../../index.rst:48
 msgid ""
 "RFC7520: Examples of Protecting Content Using JSON Object Signing and "
 "Encryption"
 msgstr ""
 
-#: ../../index.rst:43
+#: ../../index.rst:49
 msgid "RFC7638: ``thumbprint`` for JWK"
 msgstr ""
 
-#: ../../index.rst:44
+#: ../../index.rst:50
 msgid "RFC8037: ``OKP`` Key and ``EdDSA`` algorithm"
 msgstr ""
 
-#: ../../index.rst:45
+#: ../../index.rst:51
 msgid "RFC8812: ``ES256K`` algorithm"
 msgstr ""
 
-#: ../../index.rst:47
+#: ../../index.rst:53
 msgid "And draft RFCs implementation of:"
 msgstr "同时包含如下 JOSE 草案的实现："
 
-#: ../../index.rst:49
+#: ../../index.rst:55
 msgid ":ref:`chacha20`"
 msgstr ""
 
-#: ../../index.rst:50
+#: ../../index.rst:56
 msgid ":ref:`ecdh1pu`"
 msgstr ""
 
-#: ../../index.rst:52
+#: ../../index.rst:58
 msgid "RFC7520 is implemented as test cases."
 msgstr "RFC7520 是测试案例，详情请参考源码里的 tests 部分。"
 
-#: ../../index.rst:55
+#: ../../index.rst:61
 msgid "Next"
 msgstr "继续阅读"
 
-#: ../../index.rst:57
+#: ../../index.rst:63
 msgid ""
 "Explore the following sections to discover more about ``joserfc`` and its"
 " features."
-msgstr ""
-"浏览以下部分，了解更多关于 ``joserfc`` 及其特性的内容。"
+msgstr "浏览以下部分，了解更多关于 ``joserfc`` 及其特性的内容。"
+
```

### Comparing `joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/install.po` & `joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/install.po`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/migrations.po` & `joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/migrations.po`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/security.po` & `joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/security.po`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/locales/zh/LC_MESSAGES/stability.po` & `joserfc-0.9.0/docs/locales/zh/LC_MESSAGES/stability.po`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/migrations/authlib.rst` & `joserfc-0.9.0/docs/migrations/authlib.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/migrations/pyjwt.rst` & `joserfc-0.9.0/docs/migrations/pyjwt.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/recipes/openssl.rst` & `joserfc-0.9.0/docs/recipes/openssl.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/security.rst` & `joserfc-0.9.0/docs/security.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/docs/stability.rst` & `joserfc-0.9.0/docs/stability.rst`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/pyproject.toml` & `joserfc-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/_keys.py` & `joserfc-0.9.0/src/joserfc/_keys.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/drafts/jwe_chacha20.py` & `joserfc-0.9.0/src/joserfc/drafts/jwe_chacha20.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/drafts/jwe_ecdh_1pu.py` & `joserfc-0.9.0/src/joserfc/drafts/jwe_ecdh_1pu.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/errors.py` & `joserfc-0.9.0/src/joserfc/errors.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/jwe.py` & `joserfc-0.9.0/src/joserfc/jwe.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/jws.py` & `joserfc-0.9.0/src/joserfc/jws.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/jwt.py` & `joserfc-0.9.0/src/joserfc/jwt.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/registry.py` & `joserfc-0.9.0/src/joserfc/registry.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7515/compact.py` & `joserfc-0.9.0/src/joserfc/rfc7515/compact.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7515/json.py` & `joserfc-0.9.0/src/joserfc/rfc7515/json.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7515/model.py` & `joserfc-0.9.0/src/joserfc/rfc7515/model.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7515/registry.py` & `joserfc-0.9.0/src/joserfc/rfc7515/registry.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7515/types.py` & `joserfc-0.9.0/src/joserfc/rfc7515/types.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7516/compact.py` & `joserfc-0.9.0/src/joserfc/rfc7516/compact.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7516/json.py` & `joserfc-0.9.0/src/joserfc/rfc7516/json.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7516/message.py` & `joserfc-0.9.0/src/joserfc/rfc7516/message.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7516/models.py` & `joserfc-0.9.0/src/joserfc/rfc7516/models.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7516/registry.py` & `joserfc-0.9.0/src/joserfc/rfc7516/registry.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7516/types.py` & `joserfc-0.9.0/src/joserfc/rfc7516/types.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7517/models.py` & `joserfc-0.9.0/src/joserfc/rfc7517/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,17 +111,23 @@
         it will generate the kid with ``.thumbprint`` method, which is defined
         by RFC7638."""
         if "kid" not in self.dict_value:
             self._dict_value["kid"] = self.thumbprint()
 
     @property
     def kid(self) -> t.Optional[str]:
+        """The "kid" value of the JSON Web Key."""
         return self.get("kid")
 
     @property
+    def alg(self) -> t.Optional[str]:
+        """The "alg" value of the JSON Web Key."""
+        return self.get("alg")
+
+    @property
     def raw_value(self):
         raise NotImplementedError()
 
     @property
     def is_private(self) -> bool:
         raise NotImplementedError()
```

### Comparing `joserfc-0.8.0/src/joserfc/rfc7517/pem.py` & `joserfc-0.9.0/src/joserfc/rfc7517/pem.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7518/derive_key.py` & `joserfc-0.9.0/src/joserfc/rfc7518/derive_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7518/ec_key.py` & `joserfc-0.9.0/src/joserfc/rfc7518/ec_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7518/jwe_algs.py` & `joserfc-0.9.0/src/joserfc/rfc7518/jwe_algs.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7518/jwe_encs.py` & `joserfc-0.9.0/src/joserfc/rfc7518/jwe_encs.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7518/jwe_zips.py` & `joserfc-0.9.0/src/joserfc/rfc7518/jwe_zips.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7518/jws_algs.py` & `joserfc-0.9.0/src/joserfc/rfc7518/jws_algs.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7518/oct_key.py` & `joserfc-0.9.0/src/joserfc/rfc7518/oct_key.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import random
-import string
+import os
 import typing as t
 from ..util import (
     to_bytes,
     urlsafe_b64decode,
     urlsafe_b64encode,
 )
 from ..registry import KeyParameter
@@ -62,16 +61,13 @@
         """
         if not private:
             raise ValueError("oct key can not be generated as public")
 
         if key_size % 8 != 0:
             raise ValueError("Invalid bit size for oct key")
 
-        length = key_size // 8
-        rand = random.SystemRandom()
-        chars = string.ascii_letters + string.digits
-        value = "".join(rand.choice(chars) for _ in range(length))
+        value = os.urandom(key_size // 8)
         raw_key = to_bytes(value)
         key: OctKey = cls(raw_key, raw_key, parameters)
         if auto_kid:
             key.ensure_kid()
         return key
```

### Comparing `joserfc-0.8.0/src/joserfc/rfc7518/rsa_key.py` & `joserfc-0.9.0/src/joserfc/rfc7518/rsa_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7519/claims.py` & `joserfc-0.9.0/src/joserfc/rfc7519/claims.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7519/registry.py` & `joserfc-0.9.0/src/joserfc/rfc7519/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,40 +7,45 @@
     InvalidTokenError,
 )
 
 
 #: http://openid.net/specs/openid-connect-core-1_0.html#IndividualClaimsRequests
 class ClaimsOption(TypedDict, total=False):
     essential: bool
+    allow_blank: Optional[bool]
     value: Union[str, int]
-    values: List[Union[str, int]]
+    values: Union[List[Union[str, int]], List[str], List[int]]
 
 
 class ClaimsRegistry:
     """Requesting "claims" for JWT with the given conditions."""
 
     def __init__(self, **kwargs: ClaimsOption):
         self.options = kwargs
         self.essential_keys = {key for key in kwargs if kwargs[key].get("essential")}
 
     def check_value(self, claim_name: str, value: Any) -> None:
         option = self.options.get(claim_name)
         if option:
+            allow_blank = option.get("allow_blank")
+            if not allow_blank and not value:
+                raise InvalidClaimError(claim_name)
+
             option_value = option.get("value")
             if option_value and value != option_value:
                 raise InvalidClaimError(claim_name)
 
             option_values = option.get("values")
             if option_values and value not in option_values:
                 raise InvalidClaimError(claim_name)
 
     def validate(self, claims: Dict[str, Any]) -> None:
-        missed_key = self.essential_keys - set(claims.keys())
-        if missed_key:
-            raise MissingClaimError(",".join(missed_key))
+        missed_keys = {key for key in self.essential_keys if claims.get(key) is None}
+        if missed_keys:
+            raise MissingClaimError(",".join(sorted(missed_keys)))
 
         for key in claims:
             value = claims[key]
             func = getattr(self, "validate_" + key, None)
             if func:
                 func(value)
             elif key in self.options:
```

### Comparing `joserfc-0.8.0/src/joserfc/rfc7797/compact.py` & `joserfc-0.9.0/src/joserfc/rfc7797/compact.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7797/json.py` & `joserfc-0.9.0/src/joserfc/rfc7797/json.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc7797/registry.py` & `joserfc-0.9.0/src/joserfc/rfc7797/registry.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc8037/jws_eddsa.py` & `joserfc-0.9.0/src/joserfc/rfc8037/jws_eddsa.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/rfc8037/okp_key.py` & `joserfc-0.9.0/src/joserfc/rfc8037/okp_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc/util.py` & `joserfc-0.9.0/src/joserfc/util.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/src/joserfc.egg-info/PKG-INFO` & `joserfc-0.9.0/src/joserfc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joserfc
-Version: 0.8.0
+Version: 0.9.0
 Summary: The ultimate Python library for JOSE RFCs, including JWS, JWE, JWK, JWA, JWT
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Documentation, https://jose.authlib.org/
 Project-URL: Source, https://github.com/authlib/joserfc
 Project-URL: Blog, https://blog.authlib.org/
 Classifier: Development Status :: 4 - Beta
@@ -20,16 +20,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: drafts
 License-File: LICENSE
+Requires-Dist: cryptography
+Provides-Extra: drafts
+Requires-Dist: pycryptodome; extra == "drafts"
 
 JOSE RFC
 ========
 
 `·joserfc·` is a Python library that provides a comprehensive implementation of several
 essential JSON Object Signing and Encryption (JOSE) standards.
```

### Comparing `joserfc-0.8.0/src/joserfc.egg-info/SOURCES.txt` & `joserfc-0.9.0/src/joserfc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/base.py` & `joserfc-0.9.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/fixtures/jwe_compact_ecdh_1pu.json` & `joserfc-0.9.0/tests/fixtures/jwe_compact_ecdh_1pu.json`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/fixtures/jwe_rfc7520.json` & `joserfc-0.9.0/tests/fixtures/jwe_rfc7520.json`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/fixtures/jws_examples.json` & `joserfc-0.9.0/tests/fixtures/jws_examples.json`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/fixtures/jws_rfc7520.json` & `joserfc-0.9.0/tests/fixtures/jws_rfc7520.json`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/fixtures/jws_rfc7797.json` & `joserfc-0.9.0/tests/fixtures/jws_rfc7797.json`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/fixtures/jwt_use_jws.json` & `joserfc-0.9.0/tests/fixtures/jwt_use_jws.json`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jwe/test_chacha20.py` & `joserfc-0.9.0/tests/jwe/test_chacha20.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jwe/test_compact.py` & `joserfc-0.9.0/tests/jwe/test_compact.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jwe/test_ecdh_1pu.py` & `joserfc-0.9.0/tests/jwe/test_ecdh_1pu.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             value,
             private_key=key,
             registry=ecdh_registry,
             sender_key=key,
         )
         self.assertEqual(obj.plaintext, b'hello')
 
-    def test_sender_key_not_found(self):
+    def test_sender_key_not_found_via_kid(self):
         alice_key = load_key("ec-p256-alice.json", {"kid": "alice"})
         bob_key = load_key("ec-p256-bob.json", {"kid": "bob"})
         protected = {"alg": "ECDH-1PU+A128KW", "enc": "A128CBC-HS256"}
         value = encrypt_compact(
             protected, b'hello',
             public_key=bob_key,
             registry=ecdh_registry,
@@ -147,14 +147,27 @@
         self.assertRaises(
             ValueError, decrypt_compact, value,
             private_key=bob_key,
             registry=ecdh_registry,
             sender_key=key_set,
         )
 
+    def test_sender_key_not_found_via_alg(self):
+        alice_key = load_key("ec-p256-alice.json", {"kid": "alice"})
+        protected = {"alg": "ECDH-1PU+A128KW", "enc": "A128CBC-HS256"}
+        bob_key = load_key("RFC7520-RSA-private.json")
+        key_set = KeySet([bob_key])
+        self.assertRaises(
+            ValueError, encrypt_compact,
+            protected, b'hello',
+            public_key=alice_key,
+            registry=ecdh_registry,
+            sender_key=key_set,
+        )
+
 
 TestECDH1PUCompact.load_fixture('jwe_compact_ecdh_1pu.json')
 
 
 class TestECDH1PUJSON(TestCase):
     def test_example_B(self):
         # https://datatracker.ietf.org/doc/html/draft-madden-jose-ecdh-1pu-04#appendix-B.11
```

### Comparing `joserfc-0.8.0/tests/jwe/test_errors.py` & `joserfc-0.9.0/tests/jwe/test_errors.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jwe/test_example.py` & `joserfc-0.9.0/tests/jwe/test_example.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jwe/test_json.py` & `joserfc-0.9.0/tests/jwe/test_json.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jwk/test_ec_key.py` & `joserfc-0.9.0/tests/jwk/test_ec_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jwk/test_jwk_set.py` & `joserfc-0.9.0/tests/jwk/test_jwk_set.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jwk/test_key_methods.py` & `joserfc-0.9.0/tests/jwk/test_key_methods.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,20 +28,37 @@
         self.assertIsInstance(key, OctKey)
 
     def test_guess_bytes_key(self):
         key = guess_key(b"key", Guest())
         self.assertIsInstance(key, OctKey)
 
     def test_guess_callable_key(self):
-        def key_func(obj):
-            return OctKey.import_key("key")
+        oct_key = OctKey.generate_key(parameters={'kid': '1'})
+        rsa_key = RSAKey.generate_key(parameters={'kid': '2'})
 
-        key = guess_key(key_func, Guest())
+        def key_func1(obj):
+            return "key"
+
+        def key_func2(obj):
+            return rsa_key
+
+        def key_func3(obj):
+            return KeySet([oct_key, rsa_key])
+
+        key = guess_key(key_func1, Guest())
         self.assertIsInstance(key, OctKey)
 
+        key = guess_key(key_func2, Guest())
+        self.assertIsInstance(key, RSAKey)
+
+        guest = Guest()
+        guest.set_kid('2')
+        key = guess_key(key_func3, guest)
+        self.assertIsInstance(key, RSAKey)
+
     def test_guess_key_set(self):
         key_set = KeySet([OctKey.generate_key(), RSAKey.generate_key()])
         guest = Guest()
         guest._headers["alg"] = "HS256"
         self.assertRaises(ValueError, guess_key, key_set, guest)
         key = guess_key(key_set, guest, True)
         self.assertIsInstance(key, OctKey)
@@ -100,14 +117,21 @@
         key.check_alg("HS256")
         self.assertRaises(
             UnsupportedKeyAlgorithmError,
             key.check_alg,
             "RS256"
         )
 
+    def test_alg_property(self):
+        key = OctKey.import_key("secret")
+        self.assertIsNone(key.alg)
+
+        key = OctKey.import_key("secret", {"alg": "HS256"})
+        self.assertEqual(key.alg, "HS256")
+
     def test_check_ops(self):
         key = OctKey.import_key("secret", {"key_ops": ["sign", "verify"]})
         key.check_key_op("sign")
         self.assertRaises(
             UnsupportedKeyOperationError,
             key.check_key_op,
             "wrapKey"
```

### Comparing `joserfc-0.8.0/tests/jwk/test_oct_key.py` & `joserfc-0.9.0/tests/jwk/test_oct_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jwk/test_okp_key.py` & `joserfc-0.9.0/tests/jwk/test_okp_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jwk/test_rsa_key.py` & `joserfc-0.9.0/tests/jwk/test_rsa_key.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jws/test_compact.py` & `joserfc-0.9.0/tests/jws/test_compact.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jws/test_errors.py` & `joserfc-0.9.0/tests/jws/test_errors.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jws/test_examples.py` & `joserfc-0.9.0/tests/jws/test_examples.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jws/test_json.py` & `joserfc-0.9.0/tests/jws/test_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,21 @@
         member = {'protected': {'alg': 'ES256'}}
         value = serialize_json(member, b'hello', keys)
         self.assertIn('header', value)
         self.assertIn('kid', value['header'])
 
         # this will always pick alice key
         member = {'protected': {'alg': 'ES256'}, 'header': {'kid': 'alice'}}
-        serialize_json(member, b'hello', keys)
+        value = serialize_json(member, b'hello', keys)
+        self.assertEqual(value['header'], {'kid': 'alice'})
+
+        # header can also be an empty value
+        member = {'protected': {'alg': 'ES256'}, 'header': {}}
+        value = serialize_json(member, b'hello', keys)
+        self.assertIn('kid', value['header'])
 
     def test_detach_content(self):
         member = {'protected': {'alg': 'ES256'}}
         key = load_key("ec-p256-alice.json")
         value = serialize_json(member, b'hello', key)
         self.assertIn('payload', value)
         new_value = detach_content(value)
@@ -97,13 +103,13 @@
             BadSignatureError,
             deserialize_json,
             value, key2
         )
 
     def test_with_public_header(self):
         key: RSAKey = load_key('rsa-openssl-private.pem')
-        member = {'protected': {'alg': 'RS256'}, 'header': {'kid': 'abc'}}
+        member = {'header': {'alg': 'RS256', 'kid': 'abc'}}
         value = serialize_json(member, b'hello', key)
         self.assertIn('header', value)
         obj = deserialize_json(value, key)
         self.assertEqual(obj.payload, b'hello')
         self.assertEqual(obj.headers(), {'alg': 'RS256', 'kid': 'abc'})
```

### Comparing `joserfc-0.8.0/tests/jws/test_rfc7797.py` & `joserfc-0.9.0/tests/jws/test_rfc7797.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jwt/test_claims.py` & `joserfc-0.9.0/tests/jwt/test_claims.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,22 @@
         self.assertRaises(MissingClaimError, claims_requests.validate, {"iss": "a"})
 
         claims_requests = jwt.JWTClaimsRegistry(sub={"essential": True}, iss={"essential": True})
         self.assertRaises(MissingClaimError, claims_requests.validate, {"sub": "a"})
 
         claims_requests.validate({"sub": "a", "iss": "a", "name": "joserfc"})
 
+    def test_essential_empty_value(self):
+        claims_requests = jwt.JWTClaimsRegistry(sub={"essential": True})
+        self.assertRaises(MissingClaimError, claims_requests.validate, {"sub": None})
+        self.assertRaises(InvalidClaimError, claims_requests.validate, {"sub": ""})
+        claims_requests = jwt.JWTClaimsRegistry(sub={"essential": True, "allow_blank": True})
+        self.assertRaises(MissingClaimError, claims_requests.validate, {"sub": None})
+        claims_requests.validate({"sub": ""})
+
     def test_option_value(self):
         claims_requests = jwt.JWTClaimsRegistry(sub={"essential": True, "value": "123"})
         self.assertRaises(InvalidClaimError, claims_requests.validate, {"sub": "a"})
         claims_requests.validate({"sub": "123"})
 
     def test_option_values(self):
         claims_requests = jwt.JWTClaimsRegistry(sub={"essential": True, "values": ["1", "2"]})
```

### Comparing `joserfc-0.8.0/tests/jwt/test_fixtures.py` & `joserfc-0.9.0/tests/jwt/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/jwt/test_jwt.py` & `joserfc-0.9.0/tests/jwt/test_jwt.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/keys/RFC7516-A.1.3.json` & `joserfc-0.9.0/tests/keys/RFC7516-A.1.3.json`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/keys/RFC7516-A.2.3.json` & `joserfc-0.9.0/tests/keys/RFC7516-A.2.3.json`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/keys/RFC7520-RSA-73.json` & `joserfc-0.9.0/tests/keys/RFC7520-RSA-73.json`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/keys/RFC7520-RSA-84.json` & `joserfc-0.9.0/tests/keys/RFC7520-RSA-84.json`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/keys/RFC7520-RSA-private.json` & `joserfc-0.9.0/tests/keys/RFC7520-RSA-private.json`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/keys/rsa-openssl-private.pem` & `joserfc-0.9.0/tests/keys/rsa-openssl-private.pem`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/keys/rsa-openssl-public.pem` & `joserfc-0.9.0/tests/keys/rsa-openssl-public.pem`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/keys/ssh-rsa-private.pem` & `joserfc-0.9.0/tests/keys/ssh-rsa-private.pem`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/keys/ssh-rsa-public.pem` & `joserfc-0.9.0/tests/keys/ssh-rsa-public.pem`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/rfc7520/test_jwe.py` & `joserfc-0.9.0/tests/rfc7520/test_jwe.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/rfc7520/test_jws.py` & `joserfc-0.9.0/tests/rfc7520/test_jws.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.8.0/tests/test_util.py` & `joserfc-0.9.0/tests/test_util.py`

 * *Files identical despite different names*

