# Comparing `tmp/eea.api.dataconnector-8.5.zip` & `tmp/eea.api.dataconnector-9.0.zip`

## zipinfo {}

```diff
@@ -1,310 +1,310 @@
-Zip file size: 122762 bytes, number of entries: 308
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/docs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/
--rw-r--r--  2.0 unx       38 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/setup.cfg
--rw-r--r--  2.0 unx     2291 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/CONTRIBUTING.md
--rw-r--r--  2.0 unx     9624 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/PKG-INFO
--rw-r--r--  2.0 unx     3234 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/README.rst
--rw-r--r--  2.0 unx     2580 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/setup.py
--rw-r--r--  2.0 unx      126 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/MANIFEST.in
--rw-r--r--  2.0 unx       40 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     9624 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       12 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/namespace_packages.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/not-zip-safe
--rw-r--r--  2.0 unx      106 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/requires.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/top_level.txt
--rw-r--r--  2.0 unx    10916 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx     5492 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/docs/HISTORY.txt
--rw-r--r--  2.0 unx      920 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/docs/LICENSE.txt
--rw-r--r--  2.0 unx    18092 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/docs/LICENSE.GPL
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/
--rw-r--r--  2.0 unx       93 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/
--rw-r--r--  2.0 unx       93 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/browser/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/api/
--rw-r--r--  2.0 unx     4272 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/behavior.zcml
--rw-r--r--  2.0 unx        4 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/version.txt
--rw-r--r--  2.0 unx      543 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/configure.zcml
--rw-r--r--  2.0 unx      781 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/setuphandlers.py
--rw-r--r--  2.0 unx     3094 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/adapter.py
--rw-r--r--  2.0 unx     5244 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/interfaces.py
--rw-r--r--  2.0 unx      811 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/README.txt
--rw-r--r--  2.0 unx      521 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/utils.py
--rw-r--r--  2.0 unx     4466 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/behavior.py
--rw-r--r--  2.0 unx     1763 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles.zcml
--rw-r--r--  2.0 unx      832 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/permissions.zcml
--rw-r--r--  2.0 unx     9218 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/queryparser.py
--rw-r--r--  2.0 unx      217 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/__init__.py
--rw-r--r--  2.0 unx     5095 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/queryfilter.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/zh_TW/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/en/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hr/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/es/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt_BR/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ro/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eu/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/el/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/it/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ru/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/is/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lt/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hu/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/nl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fi/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lv/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/mt/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/tr/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/no/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sv/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/bg/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/kl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/et/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sk/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/cs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/da/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fr/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/de/
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eea.pot
--rwxr-xr-x  2.0 unx      218 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/update.sh
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/plone-manual.pot
--rw-r--r--  2.0 unx       13 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/en/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/en/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/en/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/en/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/es/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/es/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/es/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/es/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/es/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ro/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ro/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ro/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ro/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ro/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eu/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eu/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/el/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/el/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/el/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/el/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/el/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/it/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/it/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/it/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/it/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/it/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ru/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ru/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ru/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ru/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ru/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/is/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/is/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/is/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/is/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/is/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hu/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hu/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/nl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/nl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/nl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/nl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/nl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fi/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fi/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fi/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fi/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fi/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lv/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lv/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/mt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/mt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/mt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/mt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/mt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/tr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/tr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/tr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/tr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/tr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/no/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/no/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/no/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/no/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/no/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sv/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sv/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/bg/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/bg/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/bg/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/bg/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/bg/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/kl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/kl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/kl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/kl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/kl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/et/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/et/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/et/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/et/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/et/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sk/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sk/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sk/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sk/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sk/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/cs/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/cs/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/cs/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/cs/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/cs/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/da/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/da/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/da/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/da/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/da/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/de/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/de/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/de/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/de/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/locales/de/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/2/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/3/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/4/
--rw-r--r--  2.0 unx     2103 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/configure.zcml
--rw-r--r--  2.0 unx      263 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/to2.py
--rw-r--r--  2.0 unx     1287 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/evolve84.py
--rw-r--r--  2.0 unx      263 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/to4.py
--rw-r--r--  2.0 unx       17 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/2/types/
--rw-r--r--  2.0 unx      153 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/2/types.xml
--rw-r--r--  2.0 unx     2454 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/2/types/map_visualization.xml
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/3/types/
--rw-r--r--  2.0 unx      221 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/3/types.xml
--rw-r--r--  2.0 unx     2465 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/3/types/tableau_visualization.xml
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/4/types/
--rw-r--r--  2.0 unx      157 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/4/types.xml
--rw-r--r--  2.0 unx     2465 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/4/types/tableau_visualization.xml
--rw-r--r--  2.0 unx     1779 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/tests/base.py
--rw-r--r--  2.0 unx      735 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/tests/test_doctests.py
--rw-r--r--  2.0 unx       14 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/tests/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/
--rw-r--r--  2.0 unx     2750 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/browser/configure.zcml
--rw-r--r--  2.0 unx    14543 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/browser/blocks.py
--rw-r--r--  2.0 unx     1650 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/browser/dataprovider.py
--rw-r--r--  2.0 unx       16 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/browser/__init__.py
--rw-r--r--  2.0 unx      664 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/data_connector_view.pt
--rw-r--r--  2.0 unx      527 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/visualization_view.pt
--rw-r--r--  2.0 unx      522 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/arcgis_map_view.pt
--rw-r--r--  2.0 unx      526 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/tableau_view.pt
--rw-r--r--  2.0 unx      343 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/provided_data.pt
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/uninstall/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/
--rw-r--r--  2.0 unx      131 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/uninstall/browserlayer.xml
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_50/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_50/types/
--rw-r--r--  2.0 unx      286 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_50/types.xml
--rw-r--r--  2.0 unx      194 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_50/types/visualization.xml
--rw-r--r--  2.0 unx      189 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_50/types/map_visualization.xml
--rw-r--r--  2.0 unx      189 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_50/types/tableau_visualization.xml
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/
--rw-r--r--  2.0 unx      471 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types.xml
--rw-r--r--  2.0 unx     1369 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/rolemap.xml
--rw-r--r--  2.0 unx      178 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/visualization.xml
--rw-r--r--  2.0 unx      191 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/elasticconnector.xml
--rw-r--r--  2.0 unx      188 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/map_interactive.xml
--rw-r--r--  2.0 unx      188 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/map_visualization.xml
--rw-r--r--  2.0 unx      187 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/tableau_visualization.xml
--rw-r--r--  2.0 unx      195 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/discodataconnector.xml
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/
--rw-r--r--  2.0 unx      151 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types.xml
--rw-r--r--  2.0 unx     2749 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/visualization.xml
--rw-r--r--  2.0 unx     2409 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/map_interactive.xml
--rw-r--r--  2.0 unx     2649 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/map_visualization.xml
--rw-r--r--  2.0 unx     2714 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/tableau_visualization.xml
-drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/
--rw-r--r--  2.0 unx      522 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types.xml
--rw-r--r--  2.0 unx      181 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/metadata.xml
--rw-r--r--  2.0 unx     1369 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/rolemap.xml
--rw-r--r--  2.0 unx      187 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/browserlayer.xml
--rw-r--r--  2.0 unx     2685 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/visualization.xml
--rw-r--r--  2.0 unx      417 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/File.xml
--rw-r--r--  2.0 unx     2249 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/elasticconnector.xml
--rw-r--r--  2.0 unx     2424 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/map_interactive.xml
--rw-r--r--  2.0 unx     2700 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/map_visualization.xml
--rw-r--r--  2.0 unx     2708 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/tableau_visualization.xml
--rw-r--r--  2.0 unx     2201 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/discodataconnector.xml
--rw-r--r--  2.0 unx     1633 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/api/visualization.py
--rw-r--r--  2.0 unx     1721 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/api/configure.zcml
--rw-r--r--  2.0 unx     8522 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/api/dataconnector.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-10 09:00 eea.api.dataconnector-8.5/eea/api/dataconnector/api/__init__.py
-308 files, 182179 bytes uncompressed, 55110 bytes compressed:  69.7%
+Zip file size: 123562 bytes, number of entries: 308
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/
+-rw-r--r--  2.0 unx       38 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/setup.cfg
+-rw-r--r--  2.0 unx     2291 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/CONTRIBUTING.md
+-rw-r--r--  2.0 unx     9750 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/PKG-INFO
+-rw-r--r--  2.0 unx     3234 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/README.rst
+-rw-r--r--  2.0 unx     2580 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/setup.py
+-rw-r--r--  2.0 unx      126 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/MANIFEST.in
+-rw-r--r--  2.0 unx       40 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     9750 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       12 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx      106 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/requires.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/top_level.txt
+-rw-r--r--  2.0 unx    10916 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx     5618 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/docs/HISTORY.txt
+-rw-r--r--  2.0 unx      920 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/docs/LICENSE.txt
+-rw-r--r--  2.0 unx    18092 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/docs/LICENSE.GPL
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/
+-rw-r--r--  2.0 unx       93 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/
+-rw-r--r--  2.0 unx       93 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/browser/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/api/
+-rw-r--r--  2.0 unx     4272 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/behavior.zcml
+-rw-r--r--  2.0 unx        4 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/version.txt
+-rw-r--r--  2.0 unx      543 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/configure.zcml
+-rw-r--r--  2.0 unx      781 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/setuphandlers.py
+-rw-r--r--  2.0 unx     3094 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/adapter.py
+-rw-r--r--  2.0 unx     5244 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/interfaces.py
+-rw-r--r--  2.0 unx      811 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/README.txt
+-rw-r--r--  2.0 unx      521 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/utils.py
+-rw-r--r--  2.0 unx     4466 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/behavior.py
+-rw-r--r--  2.0 unx     1763 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles.zcml
+-rw-r--r--  2.0 unx      832 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/permissions.zcml
+-rw-r--r--  2.0 unx     9218 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/queryparser.py
+-rw-r--r--  2.0 unx      217 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/__init__.py
+-rw-r--r--  2.0 unx     5095 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/queryfilter.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/zh_TW/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/en/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hr/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/es/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt_BR/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ro/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eu/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/el/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/it/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ru/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/is/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lt/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hu/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/nl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fi/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lv/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/mt/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/tr/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/no/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sv/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/bg/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/kl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/et/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sk/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/cs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/da/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fr/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/de/
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eea.pot
+-rwxr-xr-x  2.0 unx      218 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/update.sh
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/plone-manual.pot
+-rw-r--r--  2.0 unx       13 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/en/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/en/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/en/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/en/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/es/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/es/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/es/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/es/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ro/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ro/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ro/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ro/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ro/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/el/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/el/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/el/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/el/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/el/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/it/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/it/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/it/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/it/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/it/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ru/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ru/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ru/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ru/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ru/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/is/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/is/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/is/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/is/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/is/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/nl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/nl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/nl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/nl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/nl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fi/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fi/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fi/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fi/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fi/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/mt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/mt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/mt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/mt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/mt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/tr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/tr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/tr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/tr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/tr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/no/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/no/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/no/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/no/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/no/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/bg/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/bg/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/bg/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/bg/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/bg/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/kl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/kl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/kl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/kl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/kl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/et/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/et/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/et/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/et/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/et/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sk/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sk/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sk/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sk/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sk/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/cs/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/cs/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/cs/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/cs/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/cs/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/da/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/da/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/da/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/da/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/da/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/de/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/de/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/de/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/de/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/locales/de/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/2/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/3/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/4/
+-rw-r--r--  2.0 unx     2103 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/configure.zcml
+-rw-r--r--  2.0 unx      263 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/to2.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/evolve84.py
+-rw-r--r--  2.0 unx      263 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/to4.py
+-rw-r--r--  2.0 unx       17 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/2/types/
+-rw-r--r--  2.0 unx      153 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/2/types.xml
+-rw-r--r--  2.0 unx     2454 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/2/types/map_visualization.xml
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/3/types/
+-rw-r--r--  2.0 unx      221 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/3/types.xml
+-rw-r--r--  2.0 unx     2465 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/3/types/tableau_visualization.xml
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/4/types/
+-rw-r--r--  2.0 unx      157 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/4/types.xml
+-rw-r--r--  2.0 unx     2465 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/4/types/tableau_visualization.xml
+-rw-r--r--  2.0 unx     1779 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/tests/base.py
+-rw-r--r--  2.0 unx      735 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/tests/test_doctests.py
+-rw-r--r--  2.0 unx       14 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/
+-rw-r--r--  2.0 unx     2750 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/browser/configure.zcml
+-rw-r--r--  2.0 unx    20985 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/browser/blocks.py
+-rw-r--r--  2.0 unx     1650 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/browser/dataprovider.py
+-rw-r--r--  2.0 unx       16 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/browser/__init__.py
+-rw-r--r--  2.0 unx      664 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/data_connector_view.pt
+-rw-r--r--  2.0 unx      527 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/visualization_view.pt
+-rw-r--r--  2.0 unx      522 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/arcgis_map_view.pt
+-rw-r--r--  2.0 unx      526 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/tableau_view.pt
+-rw-r--r--  2.0 unx      343 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/provided_data.pt
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/uninstall/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/
+-rw-r--r--  2.0 unx      131 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/uninstall/browserlayer.xml
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_50/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_50/types/
+-rw-r--r--  2.0 unx      286 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_50/types.xml
+-rw-r--r--  2.0 unx      194 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_50/types/visualization.xml
+-rw-r--r--  2.0 unx      189 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_50/types/map_visualization.xml
+-rw-r--r--  2.0 unx      189 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_50/types/tableau_visualization.xml
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/
+-rw-r--r--  2.0 unx      471 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types.xml
+-rw-r--r--  2.0 unx     1369 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/rolemap.xml
+-rw-r--r--  2.0 unx      178 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/visualization.xml
+-rw-r--r--  2.0 unx      191 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/elasticconnector.xml
+-rw-r--r--  2.0 unx      188 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/map_interactive.xml
+-rw-r--r--  2.0 unx      188 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/map_visualization.xml
+-rw-r--r--  2.0 unx      187 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/tableau_visualization.xml
+-rw-r--r--  2.0 unx      195 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/discodataconnector.xml
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/
+-rw-r--r--  2.0 unx      151 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types.xml
+-rw-r--r--  2.0 unx     2749 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/visualization.xml
+-rw-r--r--  2.0 unx     2409 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/map_interactive.xml
+-rw-r--r--  2.0 unx     2649 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/map_visualization.xml
+-rw-r--r--  2.0 unx     2714 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/tableau_visualization.xml
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/
+-rw-r--r--  2.0 unx      522 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types.xml
+-rw-r--r--  2.0 unx      181 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/metadata.xml
+-rw-r--r--  2.0 unx     1369 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/rolemap.xml
+-rw-r--r--  2.0 unx      187 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/browserlayer.xml
+-rw-r--r--  2.0 unx     2685 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/visualization.xml
+-rw-r--r--  2.0 unx      417 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/File.xml
+-rw-r--r--  2.0 unx     2249 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/elasticconnector.xml
+-rw-r--r--  2.0 unx     2424 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/map_interactive.xml
+-rw-r--r--  2.0 unx     2700 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/map_visualization.xml
+-rw-r--r--  2.0 unx     2708 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/tableau_visualization.xml
+-rw-r--r--  2.0 unx     2201 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/discodataconnector.xml
+-rw-r--r--  2.0 unx     1633 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/api/visualization.py
+-rw-r--r--  2.0 unx     1721 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/api/configure.zcml
+-rw-r--r--  2.0 unx     8522 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/api/dataconnector.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:34 eea.api.dataconnector-9.0/eea/api/dataconnector/api/__init__.py
+308 files, 188999 bytes uncompressed, 55910 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -1,925 +1,925 @@
-Filename: eea.api.dataconnector-8.5/
+Filename: eea.api.dataconnector-9.0/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/
+Filename: eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/docs/
+Filename: eea.api.dataconnector-9.0/docs/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/
+Filename: eea.api.dataconnector-9.0/eea/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/setup.cfg
+Filename: eea.api.dataconnector-9.0/setup.cfg
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/CONTRIBUTING.md
+Filename: eea.api.dataconnector-9.0/CONTRIBUTING.md
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/PKG-INFO
+Filename: eea.api.dataconnector-9.0/PKG-INFO
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/README.rst
+Filename: eea.api.dataconnector-9.0/README.rst
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/setup.py
+Filename: eea.api.dataconnector-9.0/setup.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/MANIFEST.in
+Filename: eea.api.dataconnector-9.0/MANIFEST.in
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/entry_points.txt
+Filename: eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/entry_points.txt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/dependency_links.txt
+Filename: eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/dependency_links.txt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/PKG-INFO
+Filename: eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/PKG-INFO
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/namespace_packages.txt
+Filename: eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/namespace_packages.txt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/not-zip-safe
+Filename: eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/not-zip-safe
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/requires.txt
+Filename: eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/requires.txt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/top_level.txt
+Filename: eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/top_level.txt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/SOURCES.txt
+Filename: eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/SOURCES.txt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/docs/HISTORY.txt
+Filename: eea.api.dataconnector-9.0/docs/HISTORY.txt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/docs/LICENSE.txt
+Filename: eea.api.dataconnector-9.0/docs/LICENSE.txt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/docs/LICENSE.GPL
+Filename: eea.api.dataconnector-9.0/docs/LICENSE.GPL
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/
+Filename: eea.api.dataconnector-9.0/eea/api/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/__init__.py
+Filename: eea.api.dataconnector-9.0/eea/__init__.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/__init__.py
+Filename: eea.api.dataconnector-9.0/eea/api/__init__.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/tests/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/tests/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/browser/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/browser/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/api/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/api/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/behavior.zcml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/behavior.zcml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/version.txt
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/version.txt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/configure.zcml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/configure.zcml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/setuphandlers.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/setuphandlers.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/adapter.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/adapter.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/interfaces.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/interfaces.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/README.txt
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/README.txt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/utils.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/utils.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/behavior.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/behavior.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles.zcml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles.zcml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/permissions.zcml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/permissions.zcml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/queryparser.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/queryparser.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/__init__.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/__init__.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/queryfilter.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/queryfilter.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/zh_TW/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/zh_TW/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/en/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/en/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hr/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hr/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/es/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/es/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt_BR/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt_BR/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ro/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ro/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eu/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eu/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/el/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/el/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/it/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/it/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ru/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ru/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/is/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/is/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lt/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lt/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hu/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hu/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/nl/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/nl/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fi/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fi/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lv/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lv/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sl/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sl/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/mt/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/mt/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/tr/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/tr/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/no/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/no/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sv/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sv/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/bg/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/bg/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/kl/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/kl/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/et/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/et/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sk/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sk/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pl/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pl/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/cs/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/cs/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/da/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/da/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fr/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fr/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/de/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/de/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eea.pot
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eea.pot
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/update.sh
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/update.sh
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/plone-manual.pot
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/plone-manual.pot
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/__init__.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/__init__.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/zh_TW/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/en/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/en/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/en/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/en/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/en/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/en/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/en/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/en/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/en/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/en/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hr/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hr/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hr/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hr/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hr/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/es/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/es/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/es/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/es/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/es/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/es/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/es/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/es/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/es/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/es/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt_BR/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ro/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ro/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ro/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ro/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ro/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ro/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ro/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ro/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ro/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ro/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eu/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eu/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eu/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eu/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/eu/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/eu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/el/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/el/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/el/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/el/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/el/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/el/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/el/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/el/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/el/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/el/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/it/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/it/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/it/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/it/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/it/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/it/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/it/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/it/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/it/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/it/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ru/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ru/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ru/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ru/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ru/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ru/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ru/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ru/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/ru/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/ru/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/is/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/is/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/is/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/is/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/is/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/is/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/is/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/is/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/is/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/is/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lt/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lt/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lt/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lt/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lt/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hu/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hu/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hu/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hu/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/hu/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/hu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/nl/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/nl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/nl/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/nl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/nl/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/nl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/nl/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/nl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/nl/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/nl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pt/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fi/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fi/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fi/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fi/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fi/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fi/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fi/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fi/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fi/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fi/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lv/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lv/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lv/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lv/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/lv/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/lv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sl/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sl/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sl/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sl/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sl/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/mt/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/mt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/mt/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/mt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/mt/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/mt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/mt/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/mt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/mt/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/mt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/tr/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/tr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/tr/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/tr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/tr/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/tr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/tr/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/tr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/tr/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/tr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/no/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/no/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/no/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/no/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/no/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/no/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/no/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/no/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/no/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/no/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sv/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sv/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sv/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sv/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sv/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/bg/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/bg/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/bg/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/bg/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/bg/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/bg/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/bg/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/bg/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/bg/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/bg/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/kl/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/kl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/kl/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/kl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/kl/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/kl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/kl/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/kl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/kl/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/kl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/et/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/et/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/et/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/et/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/et/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/et/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/et/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/et/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/et/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/et/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sk/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sk/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sk/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sk/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sk/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sk/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sk/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sk/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/sk/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/sk/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pl/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pl/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pl/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pl/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/pl/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/pl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/cs/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/cs/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/cs/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/cs/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/cs/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/cs/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/cs/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/cs/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/cs/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/cs/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/da/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/da/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/da/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/da/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/da/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/da/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/da/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/da/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/da/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/da/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fr/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fr/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fr/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fr/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/fr/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/fr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/de/LC_MESSAGES/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/de/LC_MESSAGES/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/de/LC_MESSAGES/plone.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/de/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/de/LC_MESSAGES/eea.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/de/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/de/LC_MESSAGES/eea.mo
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/de/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/locales/de/LC_MESSAGES/plone.po
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/locales/de/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/2/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/2/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/3/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/3/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/4/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/4/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/configure.zcml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/configure.zcml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/to2.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/to2.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/evolve84.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/evolve84.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/to4.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/to4.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/__init__.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/__init__.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/2/types/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/2/types/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/2/types.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/2/types.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/2/types/map_visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/2/types/map_visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/3/types/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/3/types/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/3/types.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/3/types.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/3/types/tableau_visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/3/types/tableau_visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/4/types/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/4/types/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/4/types.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/4/types.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/4/types/tableau_visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/4/types/tableau_visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/tests/base.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/tests/base.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/tests/test_doctests.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/tests/test_doctests.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/tests/__init__.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/tests/__init__.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/browser/configure.zcml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/browser/configure.zcml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/browser/blocks.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/browser/blocks.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/browser/dataprovider.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/browser/dataprovider.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/browser/__init__.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/browser/__init__.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/data_connector_view.pt
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/data_connector_view.pt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/visualization_view.pt
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/visualization_view.pt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/arcgis_map_view.pt
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/arcgis_map_view.pt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/tableau_view.pt
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/tableau_view.pt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/provided_data.pt
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/provided_data.pt
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/uninstall/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/uninstall/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/uninstall/browserlayer.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/uninstall/browserlayer.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_50/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_50/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_50/types/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_50/types/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_50/types.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_50/types.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_50/types/visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_50/types/visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_50/types/map_visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_50/types/map_visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_50/types/tableau_visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_50/types/tableau_visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/rolemap.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/rolemap.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/elasticconnector.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/elasticconnector.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/map_interactive.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/map_interactive.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/map_visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/map_visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/tableau_visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/tableau_visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/types/discodataconnector.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/types/discodataconnector.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/map_interactive.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/map_interactive.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/map_visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/map_visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/tableau_visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/tableau_visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/metadata.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/metadata.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/rolemap.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/rolemap.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/browserlayer.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/browserlayer.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/File.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/File.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/elasticconnector.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/elasticconnector.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/map_interactive.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/map_interactive.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/map_visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/map_visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/tableau_visualization.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/tableau_visualization.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/discodataconnector.xml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/discodataconnector.xml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/api/visualization.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/api/visualization.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/api/configure.zcml
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/api/configure.zcml
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/api/dataconnector.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/api/dataconnector.py
 Comment: 
 
-Filename: eea.api.dataconnector-8.5/eea/api/dataconnector/api/__init__.py
+Filename: eea.api.dataconnector-9.0/eea/api/dataconnector/api/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `eea.api.dataconnector-8.5/CONTRIBUTING.md` & `eea.api.dataconnector-9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/PKG-INFO` & `eea.api.dataconnector-9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eea.api.dataconnector
-Version: 8.5
+Version: 9.0
 Summary: eea.api.dataconnector integration for Plone
 Home-page: https://github.com/eea/eea.api.dataconnector
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
 Classifier: Environment :: Web Environment
@@ -129,14 +129,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+9.0 - (2024-01-12)
+---------------------------
+* Change: feat: improve plotlychart visualization serialization
+  [razvanMiu]
+
 8.5 - (2024-01-09)
 ---------------------------
 * Change: fix: don't break visualizations if selected content is not a viz
   [razvanMiu]
 
 8.4 - (2023-12-15)
 ---------------------------
```

## Comparing `eea.api.dataconnector-8.5/README.rst` & `eea.api.dataconnector-9.0/README.rst`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/setup.py` & `eea.api.dataconnector-9.0/setup.py`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/PKG-INFO` & `eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eea.api.dataconnector
-Version: 8.5
+Version: 9.0
 Summary: eea.api.dataconnector integration for Plone
 Home-page: https://github.com/eea/eea.api.dataconnector
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
 Classifier: Environment :: Web Environment
@@ -129,14 +129,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+9.0 - (2024-01-12)
+---------------------------
+* Change: feat: improve plotlychart visualization serialization
+  [razvanMiu]
+
 8.5 - (2024-01-09)
 ---------------------------
 * Change: fix: don't break visualizations if selected content is not a viz
   [razvanMiu]
 
 8.4 - (2023-12-15)
 ---------------------------
```

## Comparing `eea.api.dataconnector-8.5/eea.api.dataconnector.egg-info/SOURCES.txt` & `eea.api.dataconnector-9.0/eea.api.dataconnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/docs/HISTORY.txt` & `eea.api.dataconnector-9.0/docs/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+9.0 - (2024-01-12)
+---------------------------
+* Change: feat: improve plotlychart visualization serialization
+  [razvanMiu]
+
 8.5 - (2024-01-09)
 ---------------------------
 * Change: fix: don't break visualizations if selected content is not a viz
   [razvanMiu]
 
 8.4 - (2023-12-15)
 ---------------------------
```

## Comparing `eea.api.dataconnector-8.5/docs/LICENSE.txt` & `eea.api.dataconnector-9.0/docs/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/docs/LICENSE.GPL` & `eea.api.dataconnector-9.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/behavior.zcml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/behavior.zcml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/configure.zcml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/setuphandlers.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/setuphandlers.py`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/adapter.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/adapter.py`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/interfaces.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/interfaces.py`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/README.txt` & `eea.api.dataconnector-9.0/eea/api/dataconnector/README.txt`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/utils.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/utils.py`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/behavior.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/behavior.py`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles.zcml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles.zcml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/permissions.zcml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/permissions.zcml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/queryparser.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/queryparser.py`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/queryfilter.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/queryfilter.py`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/configure.zcml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/evolve84.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/evolve84.py`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/2/types/map_visualization.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/2/types/map_visualization.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/3/types/tableau_visualization.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/3/types/tableau_visualization.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/upgrades/4/types/tableau_visualization.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/upgrades/4/types/tableau_visualization.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/tests/base.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/tests/base.py`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/tests/test_doctests.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/tests/test_doctests.py`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/browser/configure.zcml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/browser/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/browser/blocks.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/browser/blocks.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,104 +1,134 @@
 """ block-related utils """
 
 import re
 from urllib.parse import urlparse
+from AccessControl import Unauthorized
 from plone import api
 from plone.restapi.behaviors import IBlocks
 from plone.restapi.interfaces import ISerializeToJson
 from plone.restapi.interfaces import IBlockFieldSerializationTransformer
 from plone.restapi.interfaces import IBlockFieldDeserializationTransformer
 from plone.restapi.deserializer.utils import path2uid
 from plone.restapi.serializer.utils import RESOLVEUID_RE, uid_to_url
+from zExceptions import Forbidden
 from zope.component import adapter
 from zope.component import queryMultiAdapter
 from zope.interface import implementer
 from zope.publisher.interfaces.browser import IBrowserRequest
 
 
-def getLink(path):
+def getLinkHTML(url, text=None):
     """
-    Get link
+      Get link HTML
+      """
+
+    if not url:
+        return url
+
+    if not text:
+        text = url
+
+    return '<a href="' + url + '" target="_blank">' + text + '</a>'
+
+
+def getLink(path):
     """
+      Get link
+      """
 
     URL = urlparse(path)
 
     if URL.netloc.startswith('localhost') and URL.scheme:
         return path.replace(URL.scheme + "://" + URL.netloc, "")
     return path
 
 
 def getUid(context, link, retry=True):
     """
-    Get the UID corresponding to a given link.
+      Get the UID corresponding to a given link.
 
-    Parameters:
-    - context: The context or object providing the link.
-    - link (str): The link for which to retrieve the UID.
-    - retry (bool, optional): If True, attempt to resolve the UID
-      even if the initial attempt fails. Defaults to True.
-
-    Returns:
-    - str or None: The UID corresponding to the provided link,
-      or None if the link is empty or cannot be resolved.
-
-    If the link is empty, the function returns the link itself.
-    If the link cannot be resolved in the initial attempt and retry
-    is True, the function retries resolving the link by calling itself
-    with retry set to False.
-
-    The function uses the RESOLVEUID_RE regular expression to match
-    and extract the UID from the link.
-    """
+      Parameters:
+      - context: The context or object providing the link.
+      - link (str): The link for which to retrieve the UID.
+      - retry (bool, optional): If True, attempt to resolve the UID
+        even if the initial attempt fails. Defaults to True.
+
+      Returns:
+      - str or None: The UID corresponding to the provided link,
+        or None if the link is empty or cannot be resolved.
+
+      If the link is empty, the function returns the link itself.
+      If the link cannot be resolved in the initial attempt and retry
+      is True, the function retries resolving the link by calling itself
+      with retry set to False.
+
+      The function uses the RESOLVEUID_RE regular expression to match
+      and extract the UID from the link.
+      """
 
     if not link:
         return link
     match = RESOLVEUID_RE.match(link)
     if match is None:
         if not retry:
             return link
         # Alin Voinea a zis sa las asa
-        return getUid(
-            context,
-            path2uid(
-                context=context, link=getLink(link)),
-            False)
+        return getUid(context, path2uid(context=context, link=getLink(link)),
+                      False)
 
     uid, _ = match.groups()
     return uid
 
 
-def getMetadata(serializer):
+def getUrlUid(self, value, field):
     """
-    Extract metadata information from a serializer.
+    Get URL and UID based on the provided value and field.
 
-    Parameters:
-    - serializer: The serializer providing metadata information.
+    :param value: The input value.
+    :param field: The field to extract the URL from in the value.
 
-    Returns:
-    - dict: A dictionary containing metadata information with
-    the following keys:
-      - "@id": The identifier.
-      - "title": The title.
-      - "publisher": The publisher.
-      - "geo_coverage": The geographic coverage.
-      - "temporal_coverage": The temporal coverage.
-      - "other_organisations": Other organizations involved.
-      - "data_provenance": Data provenance information.
-      - "figure_note": Additional notes related to the figure.
-
-    The function retrieves metadata information from the provided
-    serializer and returns it as a dictionary. If a specific metadata
-    field is not present in the serializer, the corresponding key in
-    the dictionary will have a value of None.
+    :return: A tuple containing the URL and UID.
     """
 
+    url = value.get(field)
+    uid = getUid(self.context, url)
+    url = uid_to_url(url)
+    return url, uid
+
+
+def getMetadata(serializer):
+    """
+      Extract metadata information from a serializer.
+
+      Parameters:
+      - serializer: The serializer providing metadata information.
+
+      Returns:
+      - dict: A dictionary containing metadata information with
+      the following keys:
+        - "@id": The identifier.
+        - "title": The title.
+        - "publisher": The publisher.
+        - "geo_coverage": The geographic coverage.
+        - "temporal_coverage": The temporal coverage.
+        - "other_organisations": Other organizations involved.
+        - "data_provenance": Data provenance information.
+        - "figure_note": Additional notes related to the figure.
+
+      The function retrieves metadata information from the provided
+      serializer and returns it as a dictionary. If a specific metadata
+      field is not present in the serializer, the corresponding key in
+      the dictionary will have a value of None.
+      """
+
     return {
         "@id": serializer.get("@id"),
         "title": serializer.get("title"),
+        "description": serializer.get("description"),
         "publisher": serializer.get("publisher"),
         "geo_coverage": serializer.get("geo_coverage"),
         "temporal_coverage": serializer.get("temporal_coverage"),
         "other_organisations": serializer.get("other_organisations"),
         "data_provenance": serializer.get("data_provenance"),
         "figure_note": serializer.get("figure_note")
     }
@@ -124,52 +154,63 @@
     chartData["data"] = newData
 
     return chartData
 
 
 def getVisualization(serializer, layout=True):
     """
-    Extract visualization information from a serializer.
+      Extract visualization information from a serializer.
 
-    Parameters:
-    - serializer: The serializer providing visualization information.
-    - layout (bool, optional): If True, apply layout adjustments to the
-      visualization data. Defaults to True.
-
-    Returns:
-    - dict or None: A dictionary containing visualization information
-    with the following keys:
-      - "chartData": The chart data.
-      - "provider_url": The provider URL.
-      Returns None if the visualization information is not present.
-
-    The function retrieves visualization information from the provided
-    serializer, including chart data and provider URL. If layout is set
-    to True (default), it applies layout adjustments to the chart data using
-    the getVisualizationLayout function.
-    If visualization information is not present, the function returns None.
-    """
+      Parameters:
+      - serializer: The serializer providing visualization information.
+      - layout (bool, optional): If True, apply layout adjustments to the
+        visualization data. Defaults to True.
+
+      Returns:
+      - dict or None: A dictionary containing visualization information
+      with the following keys:
+        - "chartData": The chart data.
+        - "provider_url": The provider URL.
+        Returns None if the visualization information is not present.
+
+      The function retrieves visualization information from the provided
+      serializer, including chart data and provider URL. If layout is set
+      to True (default), it applies layout adjustments to the chart data using
+      the getVisualizationLayout function.
+      If visualization information is not present, the function returns None.
+      """
+
+    visualization = serializer.get("visualization", None)
+
+    if not visualization:
+        return {}
 
-    visualization = serializer.get("visualization", {})
     chartData = visualization.get("chartData", {})
-    provider_url = chartData.get("provider_url")
+    use_data_sources = visualization.get("use_data_sources", layout)
+    provider_url = visualization.get("provider_url", None)
 
-    if layout:
+    if use_data_sources:
         chartData = getVisualizationLayout(chartData)
 
-    if chartData and "provider_url" in chartData:
-        del chartData["provider_url"]
+    response = {
+        "chartData": {
+            "data": chartData.get("data", []),
+            "layout": chartData.get("layout", {}),
+            "frames": chartData.get("frames", [])
+        },
+        "use_data_sources": use_data_sources
+    }
 
-    if not visualization:
-        return {}
+    if use_data_sources and provider_url:
+        response["provider_url"] = provider_url
 
-    return {
-        "chartData": chartData,
-        "provider_url": provider_url
-    }
+    if use_data_sources and "data_source" in visualization:
+        response["data_source"] = visualization.get("data_source")
+
+    return response
 
 
 @implementer(IBlockFieldSerializationTransformer)
 @adapter(IBlocks, IBrowserRequest)
 class EmbedVisualizationSerializationTransformer:
     """Embed visualization serialization"""
 
@@ -177,47 +218,83 @@
     block_type = "embed_visualization"
 
     def __init__(self, context, request):
         self.context = context
         self.request = request
 
     def __call__(self, value):
-        uid = getUid(self.context, value.get('vis_url'))
+        vis_url, uid = getUrlUid(self, value, 'vis_url')
 
         if 'visualization' in value:
             del value['visualization']
 
         if not uid:
             return value
-        doc = api.content.get(UID=uid)
-        doc_serializer = queryMultiAdapter(
-            (doc, self.request),
-            ISerializeToJson
-        ) if doc else None
+
+        doc = None
+
+        try:
+            doc = api.content.get(UID=uid)
+        except Unauthorized:
+            return {
+                **value, "vis_url": vis_url,
+                "visualization": {
+                    "error":
+                    "Apologies, it seems this " +
+                    getLinkHTML(vis_url, 'Chart (Interactive)') +
+                    " has not been published yet."
+                }
+            }
+        except Forbidden:
+            return {
+                **value, "vis_url": vis_url,
+                "visualization": {
+                    "error":
+                    "Apologies, it seems you do not have " +
+                    "permissions to see this " +
+                    getLinkHTML(vis_url, 'Chart (Interactive)') + "."
+                }
+            }
+
+        doc_serializer = self._get_doc_serializer(doc)
         if doc_serializer:
-            doc_serializer = doc_serializer(
-                version=self.request.get("version"))
-            use_live_data = value.get('use_live_data', True)
+            use_data_sources = value.get('use_data_sources', True)
 
             return {
-                **value,
-                "vis_url":  uid_to_url(value.get('vis_url')),
+                **value, "vis_url": vis_url,
                 "visualization": {
                     **getMetadata(doc_serializer),
-                    **doc_serializer.get('visualization', {}),
-                    **getVisualization(
-                        serializer=doc_serializer,
-                        layout=use_live_data
-                    ),
+                    **getVisualization(serializer=doc_serializer,
+                                       layout=use_data_sources),
                 }
             }
-        return {
-            **value,
-            "vis_url":  uid_to_url(value.get('vis_url'))
-        }
+        return {**value, "vis_url": uid_to_url(value.get('vis_url'))}
+
+    def _get_doc_serializer(self, doc):
+        """
+        Get a serializer for the given document.
+
+        This method queries for a JSON serializer adapter for the provided
+        document and request. If a serializer is found, it is instantiated
+        with the version from the request and returned.
+
+        :param doc: The document for which to get a serializer.
+        :type doc: object
+
+        :return: An instantiated JSON serializer if available, or None if
+                 not found.
+        :rtype: object or None
+        """
+        if doc:
+            doc_serializer = queryMultiAdapter(
+                (doc, self.request), ISerializeToJson)
+            if doc_serializer:
+                return doc_serializer(
+                    version=self.request.get("version"))
+        return None
 
 
 @implementer(IBlockFieldDeserializationTransformer)
 @adapter(IBlocks, IBrowserRequest)
 class EmbedVisualizationDeserializationTransformer:
     """Embed visualization deserialization"""
 
@@ -228,16 +305,16 @@
         self.context = context
         self.request = request
 
     def __call__(self, value):
         if 'visualization' in value:
             del value['visualization']
         if 'vis_url' in value:
-            value['vis_url'] = path2uid(
-                context=self.context, link=getLink(value['vis_url']))
+            value['vis_url'] = path2uid(context=self.context,
+                                        link=getLink(value['vis_url']))
         return value
 
 
 @implementer(IBlockFieldSerializationTransformer)
 @adapter(IBlocks, IBrowserRequest)
 class EmbedTableauVisualizationSerializationTransformer:
     """Embed tableau visualization serialization"""
@@ -246,44 +323,84 @@
     block_type = "embed_tableau_visualization"
 
     def __init__(self, context, request):
         self.context = context
         self.request = request
 
     def __call__(self, value):
-        tableau_vis_url = value.get('tableau_vis_url')
-        uid = getUid(self.context, tableau_vis_url)
+        tableau_vis_url, uid = getUrlUid(self, value, 'tableau_vis_url')
 
         if 'tableau_visualization' in value:
             del value['tableau_visualization']
 
         if not uid:
             return value
 
-        doc = api.content.get(UID=uid)
-        doc_serializer = queryMultiAdapter(
-            (doc, self.request),
-            ISerializeToJson
-        ) if doc else None
+        doc = None
+
+        try:
+            doc = api.content.get(UID=uid)
+        except Unauthorized:
+            return {
+                **value, "tableau_vis_url": tableau_vis_url,
+                "tableau_visualization": {
+                    "error":
+                    "Apologies, it seems this " +
+                    getLinkHTML(tableau_vis_url, 'Dashboard') +
+                    " has not been published yet."
+                }
+            }
+        except Forbidden:
+            return {
+                **value, "tableau_vis_url": tableau_vis_url,
+                "tableau_visualization": {
+                    "error":
+                    "Apologies, it seems you do not have " +
+                    "permissions to see this " +
+                    getLinkHTML(tableau_vis_url, 'Dashboard') + "."
+                }
+            }
+
+        doc_serializer = self._get_doc_serializer(doc)
         if doc_serializer:
-            doc_serializer = doc_serializer(
-                version=self.request.get("version"))
             return {
-                **value,
-                "tableau_vis_url":  uid_to_url(tableau_vis_url),
+                **value, "tableau_vis_url": tableau_vis_url,
                 "tableau_visualization": {
                     **getMetadata(doc_serializer),
                     **doc_serializer.get('tableau_visualization', {}),
                 }
             }
         return {
             **value,
-            "tableau_vis_url":  uid_to_url(tableau_vis_url),
+            "tableau_vis_url": tableau_vis_url,
         }
 
+    def _get_doc_serializer(self, doc):
+        """
+        Get a serializer for the given document.
+
+        This method queries for a JSON serializer adapter for the provided
+        document and request. If a serializer is found, it is instantiated
+        with the version from the request and returned.
+
+        :param doc: The document for which to get a serializer.
+        :type doc: object
+
+        :return: An instantiated JSON serializer if available, or None if
+                 not found.
+        :rtype: object or None
+        """
+        if doc:
+            doc_serializer = queryMultiAdapter(
+                (doc, self.request), ISerializeToJson)
+            if doc_serializer:
+                return doc_serializer(
+                    version=self.request.get("version"))
+        return None
+
 
 @implementer(IBlockFieldDeserializationTransformer)
 @adapter(IBlocks, IBrowserRequest)
 class EmbedTableauVisualizationDeserializationTransformer:
     """Embed Tableau visualization deserialization"""
 
     order = 9999
@@ -293,16 +410,16 @@
         self.context = context
         self.request = request
 
     def __call__(self, value):
         if 'tableau_visualization' in value:
             del value['tableau_visualization']
         if 'tableau_vis_url' in value:
-            value['tableau_vis_url'] = path2uid(
-                context=self.context, link=value['tableau_vis_url'])
+            value['tableau_vis_url'] = path2uid(context=self.context,
+                                                link=value['tableau_vis_url'])
         return value
 
 
 @implementer(IBlockFieldSerializationTransformer)
 @adapter(IBlocks, IBrowserRequest)
 class EmbedEEAMapBlockSerializationTransformer:
     """Embed eea map block serializer"""
@@ -311,44 +428,84 @@
     block_type = "embed_eea_map_block"
 
     def __init__(self, context, request):
         self.context = context
         self.request = request
 
     def __call__(self, value):
-        vis_url = value.get('vis_url')
-        uid = getUid(self.context, vis_url)
+        vis_url, uid = getUrlUid(self, value, 'vis_url')
 
         if 'map_visualization_data' in value:
             del value['map_visualization_data']
 
         if not uid:
             return value
 
-        doc = api.content.get(UID=uid)
-        doc_serializer = queryMultiAdapter(
-            (doc, self.request),
-            ISerializeToJson
-        ) if doc else None
+        doc = None
+
+        try:
+            doc = api.content.get(UID=uid)
+        except Unauthorized:
+            return {
+                **value, "tableau_vis_url": vis_url,
+                "map_visualization_data": {
+                    "error":
+                    "Apologies, it seems this " +
+                    getLinkHTML(vis_url, 'Map (Simple)') +
+                    " has not been published yet."
+                }
+            }
+        except Forbidden:
+            return {
+                **value, "tableau_vis_url": vis_url,
+                "map_visualization_data": {
+                    "error":
+                    "Apologies, it seems you do not have " +
+                    "permissions to see this " +
+                    getLinkHTML(vis_url, 'Map (Simple)') + "."
+                }
+            }
+
+        doc_serializer = self._get_doc_serializer(doc)
         if doc_serializer:
-            doc_serializer = doc_serializer(
-                version=self.request.get("version"))
             return {
-                **value,
-                "vis_url":  uid_to_url(vis_url),
+                **value, "vis_url": vis_url,
                 "map_visualization_data": {
                     **getMetadata(doc_serializer),
                     **doc_serializer.get('map_visualization_data', {}),
                 }
             }
         return {
             **value,
-            "vis_url":  uid_to_url(vis_url),
+            "vis_url": vis_url,
         }
 
+    def _get_doc_serializer(self, doc):
+        """
+        Get a serializer for the given document.
+
+        This method queries for a JSON serializer adapter for the provided
+        document and request. If a serializer is found, it is instantiated
+        with the version from the request and returned.
+
+        :param doc: The document for which to get a serializer.
+        :type doc: object
+
+        :return: An instantiated JSON serializer if available, or None if
+                 not found.
+        :rtype: object or None
+        """
+        if doc:
+            doc_serializer = queryMultiAdapter(
+                (doc, self.request), ISerializeToJson)
+            if doc_serializer:
+                return doc_serializer(
+                    version=self.request.get("version"))
+        return None
+
 
 @implementer(IBlockFieldDeserializationTransformer)
 @adapter(IBlocks, IBrowserRequest)
 class EmbedEEAMapBlockDeserializationTransformer:
     """Embed eea map block deserialization"""
 
     order = 9999
@@ -358,16 +515,16 @@
         self.context = context
         self.request = request
 
     def __call__(self, value):
         if 'map_visualization_data' in value:
             del value['map_visualization_data']
         if 'vis_url' in value:
-            value['vis_url'] = path2uid(
-                context=self.context, link=value['vis_url'])
+            value['vis_url'] = path2uid(context=self.context,
+                                        link=value['vis_url'])
         return value
 
 
 @implementer(IBlockFieldSerializationTransformer)
 @adapter(IBlocks, IBrowserRequest)
 class EmbedMapsSerializationTransformer:
     """Embed maps serializer"""
@@ -376,39 +533,76 @@
     block_type = "embed_maps"
 
     def __init__(self, context, request):
         self.context = context
         self.request = request
 
     def __call__(self, value):
-        uid = getUid(self.context, value.get('url'))
+        url, uid = getUrlUid(self, value, 'url')
 
         if 'maps' in value:
             del value['maps']
 
         if not uid:
             return value
 
-        doc = api.content.get(UID=uid)
-        doc_serializer = queryMultiAdapter(
-            (doc, self.request),
-            ISerializeToJson
-        ) if doc else None
+        try:
+            doc = api.content.get(UID=uid)
+        except Unauthorized:
+            return {
+                **value, "maps": {
+                    "error":
+                    "Apologies, it seems this " +
+                    getLinkHTML(url, 'Map (Interactive)') +
+                    " has not been published yet."
+                }
+            }
+        except Forbidden:
+            return {
+                **value, "maps": {
+                    "error":
+                    "Apologies, it seems you do not have " +
+                    "permissions to see this " +
+                    getLinkHTML(url, 'Map (Interactive)') + "."
+                }
+            }
+
+        doc_serializer = self._get_doc_serializer(doc)
         if doc_serializer:
-            doc_serializer = doc_serializer(
-                version=self.request.get("version"))
             return {
-                **value,
-                "maps": {
+                **value, "maps": {
                     **getMetadata(doc_serializer),
                     **doc_serializer.get('maps', {}),
                 }
             }
         return value
 
+    def _get_doc_serializer(self, doc):
+        """
+        Get a serializer for the given document.
+
+        This method queries for a JSON serializer adapter for the provided
+        document and request. If a serializer is found, it is instantiated
+        with the version from the request and returned.
+
+        :param doc: The document for which to get a serializer.
+        :type doc: object
+
+        :return: An instantiated JSON serializer if available, or None if
+                 not found.
+        :rtype: object or None
+        """
+        if doc:
+            doc_serializer = queryMultiAdapter(
+                (doc, self.request), ISerializeToJson)
+            if doc_serializer:
+                return doc_serializer(
+                    version=self.request.get("version"))
+        return None
+
 
 @implementer(IBlockFieldDeserializationTransformer)
 @adapter(IBlocks, IBrowserRequest)
 class EmbedMapsDeserializationTransformer:
     """Embed maps deserialization"""
 
     order = 9999
@@ -440,29 +634,25 @@
     #     # if value.get("visualization", {}).get("provider_url"):
     #     #     value["visualization"]["provider_url"] = self.url_to_path(
     #     #         value["visualization"]["provider_url"]
     #     #     )
     #     return value
 
     def __call__(self, value):
-        if value.get("use_live_data", True):
-            newData = (
-                value.get("visualization", {})
-                .get("chartData", {})
-                .get("data", None)
-            )
+        if value.get("use_data_sources", True):
+            newData = (value.get("visualization",
+                                 {}).get("chartData", {}).get("data", None))
             if not newData:
                 return value
             for traceIndex, trace in enumerate(newData):
                 for tk in trace:
                     originalColumn = re.sub("src$", "", tk)
                     if tk.endswith("src") and originalColumn in trace:
                         newData[traceIndex][originalColumn] = []
                 if not trace.get("transforms"):
                     continue
                 for transformIndex, _ in enumerate(trace.get("transforms")):
                     newData[traceIndex]["transforms"][transformIndex][
-                        "target"
-                    ] = []
+                        "target"] = []
             value["visualization"]["chartData"]["data"] = newData
 
         return value
```

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/browser/dataprovider.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/browser/dataprovider.py`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/data_connector_view.pt` & `eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/data_connector_view.pt`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/visualization_view.pt` & `eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/visualization_view.pt`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/arcgis_map_view.pt` & `eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/arcgis_map_view.pt`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/browser/pt/tableau_view.pt` & `eea.api.dataconnector-9.0/eea/api/dataconnector/browser/pt/tableau_view.pt`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_82/rolemap.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_82/rolemap.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/visualization.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/visualization.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/map_interactive.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/map_interactive.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/map_visualization.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/map_visualization.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/upgrades/to_60/types/tableau_visualization.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/upgrades/to_60/types/tableau_visualization.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/rolemap.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/rolemap.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/visualization.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/visualization.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/elasticconnector.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/elasticconnector.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/map_interactive.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/map_interactive.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/map_visualization.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/map_visualization.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/tableau_visualization.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/tableau_visualization.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/profiles/default/types/discodataconnector.xml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/profiles/default/types/discodataconnector.xml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/api/visualization.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/api/visualization.py`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/api/configure.zcml` & `eea.api.dataconnector-9.0/eea/api/dataconnector/api/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.api.dataconnector-8.5/eea/api/dataconnector/api/dataconnector.py` & `eea.api.dataconnector-9.0/eea/api/dataconnector/api/dataconnector.py`

 * *Files identical despite different names*

