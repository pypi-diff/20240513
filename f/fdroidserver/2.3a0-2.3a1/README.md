# Comparing `tmp/fdroidserver-2.3a0.tar.gz` & `tmp/fdroidserver-2.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdroidserver-2.3a0.tar", last modified: Wed Apr 10 14:57:56 2024, max compression
+gzip compressed data, was "fdroidserver-2.3a1.tar", last modified: Mon May 13 08:46:29 2024, max compression
```

## Comparing `fdroidserver-2.3a0.tar` & `fdroidserver-2.3a1.tar`

### file list

```diff
@@ -1,1295 +1,1302 @@
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/
--rw-r--r--   0 hans      (1000) hans      (1000)    10971 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/CHANGELOG.md
--rw-r--r--   0 hans      (1000) hans      (1000)    34520 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/LICENSE
--rw-r--r--   0 hans      (1000) hans      (1000)    61991 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/MANIFEST.in
--rw-r--r--   0 hans      (1000) hans      (1000)     5342 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/PKG-INFO
--rw-r--r--   0 hans      (1000) hans      (1000)     4486 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/README.md
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/buildserver/
--rw-r--r--   0 hans      (1000) hans      (1000)     3934 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/buildserver/Vagrantfile
--rw-r--r--   0 hans      (1000) hans      (1000)       68 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/buildserver/config.buildserver.yml
--rw-r--r--   0 hans      (1000) hans      (1000)      711 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/buildserver/provision-android-ndk
--rw-r--r--   0 hans      (1000) hans      (1000)     4547 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/buildserver/provision-android-sdk
--rw-r--r--   0 hans      (1000) hans      (1000)     2887 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/buildserver/provision-apt-get-install
--rw-r--r--   0 hans      (1000) hans      (1000)      298 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/buildserver/provision-apt-proxy
--rw-r--r--   0 hans      (1000) hans      (1000)     1463 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/buildserver/provision-gradle
--rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/buildserver/setup-env-vars
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/completion/
--rw-r--r--   0 hans      (1000) hans      (1000)     6221 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/completion/bash-completion
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/examples/
--rw-r--r--   0 hans      (1000) hans      (1000)     1892 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/examples/Vagrantfile.yaml
--rw-r--r--   0 hans      (1000) hans      (1000)    15338 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/examples/config.yml
--rw-r--r--   0 hans      (1000) hans      (1000)     2276 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/examples/fdroid_export_keystore_to_nitrokey.py
--rw-r--r--   0 hans      (1000) hans      (1000)     2015 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/examples/fdroid_exportkeystore.py
--rw-r--r--   0 hans      (1000) hans      (1000)      544 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/examples/fdroid_extract_repo_pubkey.py
--rw-r--r--   0 hans      (1000) hans      (1000)     1589 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/examples/fdroid_fetchsrclibs.py
--rw-r--r--   0 hans      (1000) hans      (1000)     1552 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/examples/fdroid_nitrokeyimport.py
--rw-r--r--   0 hans      (1000) hans      (1000)      123 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/examples/opensc-fdroid.cfg
--rw-r--r--   0 hans      (1000) hans      (1000)      237 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/examples/public-read-only-s3-bucket-policy.json
--rw-r--r--   0 hans      (1000) hans      (1000)      244 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/examples/template.yml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/fdroidserver/
--rw-r--r--   0 hans      (1000) hans      (1000)     2284 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/__init__.py
--rwxr-xr-x   0 hans      (1000) hans      (1000)     8941 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/__main__.py
--rw-r--r--   0 hans      (1000) hans      (1000)    37993 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/apksigcopier.py
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/fdroidserver/asynchronousfilereader/
--rw-r--r--   0 hans      (1000) hans      (1000)     1350 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/asynchronousfilereader/__init__.py
--rwxr-xr-x   0 hans      (1000) hans      (1000)     8928 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/btlog.py
--rw-r--r--   0 hans      (1000) hans      (1000)    55318 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/build.py
--rw-r--r--   0 hans      (1000) hans      (1000)    26736 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/checkupdates.py
--rw-r--r--   0 hans      (1000) hans      (1000)   164601 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/common.py
--rw-r--r--   0 hans      (1000) hans      (1000)    36816 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/deploy.py
--rw-r--r--   0 hans      (1000) hans      (1000)     1202 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/exception.py
--rw-r--r--   0 hans      (1000) hans      (1000)     2921 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/gpgsign.py
--rw-r--r--   0 hans      (1000) hans      (1000)    13174 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/import_subcommand.py
--rw-r--r--   0 hans      (1000) hans      (1000)    65741 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/index.py
--rw-r--r--   0 hans      (1000) hans      (1000)    11732 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/init.py
--rw-r--r--   0 hans      (1000) hans      (1000)     4751 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/install.py
--rw-r--r--   0 hans      (1000) hans      (1000)    34097 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/lint.py
--rw-r--r--   0 hans      (1000) hans      (1000)    12123 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/looseversion.py
--rw-r--r--   0 hans      (1000) hans      (1000)    41680 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/metadata.py
--rw-r--r--   0 hans      (1000) hans      (1000)     8929 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/mirror.py
--rw-r--r--   0 hans      (1000) hans      (1000)     4002 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/net.py
--rw-r--r--   0 hans      (1000) hans      (1000)    19772 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/nightly.py
--rw-r--r--   0 hans      (1000) hans      (1000)    17416 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/publish.py
--rw-r--r--   0 hans      (1000) hans      (1000)     1178 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/readmeta.py
--rw-r--r--   0 hans      (1000) hans      (1000)     3635 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/rewritemeta.py
--rw-r--r--   0 hans      (1000) hans      (1000)    45770 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/scanner.py
--rw-r--r--   0 hans      (1000) hans      (1000)     3949 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/signatures.py
--rw-r--r--   0 hans      (1000) hans      (1000)     8214 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/signindex.py
--rw-r--r--   0 hans      (1000) hans      (1000)     3299 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/tail.py
--rw-r--r--   0 hans      (1000) hans      (1000)   106630 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/update.py
--rw-r--r--   0 hans      (1000) hans      (1000)     8508 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/verify.py
--rw-r--r--   0 hans      (1000) hans      (1000)    16140 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/fdroidserver/vmtools.py
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/fdroidserver.egg-info/
--rw-r--r--   0 hans      (1000) hans      (1000)     5342 2024-04-10 14:57:56.000000 fdroidserver-2.3a0/fdroidserver.egg-info/PKG-INFO
--rw-r--r--   0 hans      (1000) hans      (1000)    56021 2024-04-10 14:57:56.000000 fdroidserver-2.3a0/fdroidserver.egg-info/SOURCES.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        1 2024-04-10 14:57:56.000000 fdroidserver-2.3a0/fdroidserver.egg-info/dependency_links.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       54 2024-04-10 14:57:56.000000 fdroidserver-2.3a0/fdroidserver.egg-info/entry_points.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      392 2024-04-10 14:57:56.000000 fdroidserver-2.3a0/fdroidserver.egg-info/requires.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       13 2024-04-10 14:57:56.000000 fdroidserver-2.3a0/fdroidserver.egg-info/top_level.txt
--rwxr-xr-x   0 hans      (1000) hans      (1000)    18504 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/gradlew-fdroid
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/locale/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.885981 fdroidserver-2.3a0/locale/bo/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/bo/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)   111110 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/bo/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.885981 fdroidserver-2.3a0/locale/cs/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/cs/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    95055 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/cs/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.885981 fdroidserver-2.3a0/locale/de/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/de/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    96478 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/de/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.885981 fdroidserver-2.3a0/locale/es/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/es/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    96283 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/es/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.885981 fdroidserver-2.3a0/locale/fr/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/fr/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    98956 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/fr/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.885981 fdroidserver-2.3a0/locale/hu/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/hu/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    84888 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/hu/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.885981 fdroidserver-2.3a0/locale/it/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/it/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    95184 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/it/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.885981 fdroidserver-2.3a0/locale/ko/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/ko/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    75849 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/ko/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.885981 fdroidserver-2.3a0/locale/nb_NO/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/nb_NO/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    89381 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/nb_NO/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.885981 fdroidserver-2.3a0/locale/pl/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/pl/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    95727 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/pl/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.885981 fdroidserver-2.3a0/locale/pt/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/pt/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    95243 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/pt/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/locale/pt_BR/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    95892 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/pt_BR/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/locale/pt_PT/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    95319 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/pt_PT/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/locale/ro/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.897981 fdroidserver-2.3a0/locale/ro/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    96228 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/ro/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/locale/ru/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.901981 fdroidserver-2.3a0/locale/ru/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)   115785 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/ru/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/locale/sq/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.901981 fdroidserver-2.3a0/locale/sq/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    94894 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/sq/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/locale/tr/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.901981 fdroidserver-2.3a0/locale/tr/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    94250 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/tr/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/locale/uk/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.901981 fdroidserver-2.3a0/locale/uk/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)   111258 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/uk/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/locale/zh_Hans/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.901981 fdroidserver-2.3a0/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    86319 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/zh_Hans/LC_MESSAGES/fdroidserver.po
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/locale/zh_Hant/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.901981 fdroidserver-2.3a0/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 hans      (1000) hans      (1000)    88340 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/locale/zh_Hant/LC_MESSAGES/fdroidserver.po
--rwxr-xr-x   0 hans      (1000) hans      (1000)    18661 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/makebuildserver
--rw-r--r--   0 hans      (1000) hans      (1000)     5302 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/pyproject.toml
--rw-r--r--   0 hans      (1000) hans      (1000)      771 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/setup.cfg
--rwxr-xr-x   0 hans      (1000) hans      (1000)     4161 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/setup.py
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.901981 fdroidserver-2.3a0/tests/
--rw-r--r--   0 hans      (1000) hans      (1000)      750 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/IsMD5Disabled.java
--rw-r--r--   0 hans      (1000) hans      (1000)    12227 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/Norway_bouvet_europe_2.obf.zip
--rw-r--r--   0 hans      (1000) hans      (1000)     7299 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/SpeedoMeterApp.main_1.apk
--rw-r--r--   0 hans      (1000) hans      (1000)     2557 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/aosp_testkey_debug.keystore
--rw-r--r--   0 hans      (1000) hans      (1000)    16876 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/apk.embedded_1.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    11471 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/bad-unicode-πÇÇ现代通用字-български-عربي1.apk
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.901981 fdroidserver-2.3a0/tests/build-tools/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.905981 fdroidserver-2.3a0/tests/build-tools/17.0.0/
--rw-r--r--   0 hans      (1000) hans      (1000)     6221 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      921 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      937 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1442 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      848 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      635 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1334 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      646 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      649 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1496 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.905981 fdroidserver-2.3a0/tests/build-tools/18.1.1/
--rw-r--r--   0 hans      (1000) hans      (1000)     6221 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      921 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      937 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1442 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      848 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      635 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1334 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      646 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      649 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1496 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.905981 fdroidserver-2.3a0/tests/build-tools/19.0.0/
--rw-r--r--   0 hans      (1000) hans      (1000)     6221 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      921 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      937 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1442 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      848 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      635 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1334 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      646 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      649 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1496 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.905981 fdroidserver-2.3a0/tests/build-tools/19.1.0/
--rw-r--r--   0 hans      (1000) hans      (1000)     6221 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      921 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      937 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1442 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      848 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      635 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1334 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      646 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      649 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1496 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.905981 fdroidserver-2.3a0/tests/build-tools/20.0.0/
--rw-r--r--   0 hans      (1000) hans      (1000)     6221 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      921 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      937 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1442 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      848 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      635 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1334 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      646 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      649 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1496 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.905981 fdroidserver-2.3a0/tests/build-tools/21.1.1/
--rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1475 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1223 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.905981 fdroidserver-2.3a0/tests/build-tools/21.1.2/
--rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1475 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1223 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.905981 fdroidserver-2.3a0/tests/build-tools/22.0.0/
--rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1635 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1529 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.909981 fdroidserver-2.3a0/tests/build-tools/22.0.1/
--rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1635 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1529 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.909981 fdroidserver-2.3a0/tests/build-tools/23.0.0/
--rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1635 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1529 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.909981 fdroidserver-2.3a0/tests/build-tools/23.0.1/
--rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1635 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1529 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.909981 fdroidserver-2.3a0/tests/build-tools/23.0.2/
--rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1635 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1529 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.909981 fdroidserver-2.3a0/tests/build-tools/23.0.3/
--rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1816 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.909981 fdroidserver-2.3a0/tests/build-tools/24.0.0/
--rw-r--r--   0 hans      (1000) hans      (1000)     6497 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1379 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1379 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      917 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      946 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      727 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      628 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      675 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      675 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      675 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      657 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      666 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1563 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.909981 fdroidserver-2.3a0/tests/build-tools/24.0.1/
--rw-r--r--   0 hans      (1000) hans      (1000)     6497 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1379 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1379 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      917 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      946 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      727 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      628 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      675 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      675 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      675 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      657 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      666 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1563 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.909981 fdroidserver-2.3a0/tests/build-tools/24.0.2/
--rw-r--r--   0 hans      (1000) hans      (1000)     6493 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      913 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      942 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      624 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      662 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1559 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.913981 fdroidserver-2.3a0/tests/build-tools/24.0.3/
--rw-r--r--   0 hans      (1000) hans      (1000)     6493 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      913 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      942 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      624 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      662 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1559 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.913981 fdroidserver-2.3a0/tests/build-tools/25.0.0/
--rw-r--r--   0 hans      (1000) hans      (1000)     6493 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      913 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      942 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      624 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      662 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1559 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.913981 fdroidserver-2.3a0/tests/build-tools/25.0.1/
--rw-r--r--   0 hans      (1000) hans      (1000)     6493 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      913 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      942 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      624 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      662 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1559 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.913981 fdroidserver-2.3a0/tests/build-tools/25.0.2/
--rw-r--r--   0 hans      (1000) hans      (1000)     6493 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      913 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      942 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      624 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      662 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1559 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.913981 fdroidserver-2.3a0/tests/build-tools/25.0.3/
--rw-r--r--   0 hans      (1000) hans      (1000)     6493 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      913 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      942 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1804 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      624 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      662 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1559 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.913981 fdroidserver-2.3a0/tests/build-tools/26.0.0/
--rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.913981 fdroidserver-2.3a0/tests/build-tools/26.0.1/
--rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.917981 fdroidserver-2.3a0/tests/build-tools/26.0.2/
--rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.917981 fdroidserver-2.3a0/tests/build-tools/26.0.3/
--rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.917981 fdroidserver-2.3a0/tests/build-tools/27.0.0/
--rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.917981 fdroidserver-2.3a0/tests/build-tools/27.0.1/
--rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.917981 fdroidserver-2.3a0/tests/build-tools/27.0.2/
--rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/build-tools/27.0.3/
--rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/build-tools/28.0.0/
--rw-r--r--   0 hans      (1000) hans      (1000)     6580 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      938 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      734 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1586 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/build-tools/28.0.1/
--rw-r--r--   0 hans      (1000) hans      (1000)     6580 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-com.moez.QKSMS_182.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      938 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      734 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1586 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/build-tools/28.0.2/
--rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      938 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      734 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-org.droidtr.keyboard_34.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1586 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-souch.smsbypass_9.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/build-tools/28.0.3/
--rw-r--r--   0 hans      (1000) hans      (1000)      655 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-com.example.test.helloworld_1.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-com.politedroid_3.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-com.politedroid_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      938 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-com.politedroid_5.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-com.politedroid_6.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-duplicate.permisssions_9999999.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-info.guardianproject.urzip_100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1230 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-no.min.target.sdk_987.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-obb.main.oldversion_1444412523.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-obb.main.twoversions_1101613.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-obb.main.twoversions_1101615.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-obb.main.twoversions_1101617.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-obb.mainpatch.current_1619.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1586 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-souch.smsbypass_9.txt
--rwxr-xr-x   0 hans      (1000) hans      (1000)      645 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build-tools/generate.sh
--rwxr-xr-x   0 hans      (1000) hans      (1000)    44562 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/build.TestCase
--rwxr-xr-x   0 hans      (1000) hans      (1000)    18340 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/check-fdroid-apk
--rwxr-xr-x   0 hans      (1000) hans      (1000)    13879 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/checkupdates.TestCase
--rw-r--r--   0 hans      (1000) hans      (1000)     1722 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/com.fake.IpaApp_1000000000001.ipa
--rwxr-xr-x   0 hans      (1000) hans      (1000)   131907 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/common.TestCase
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/config/
--rw-r--r--   0 hans      (1000) hans      (1000)     1547 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/antiFeatures.yml
--rw-r--r--   0 hans      (1000) hans      (1000)      208 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/categories.yml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/config/de/
--rw-r--r--   0 hans      (1000) hans      (1000)     1648 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/de/antiFeatures.yml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/config/fa/
--rw-r--r--   0 hans      (1000) hans      (1000)     1956 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/fa/antiFeatures.yml
--rw-r--r--   0 hans      (1000) hans      (1000)     1564 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/ic_antifeature_ads.xml
--rw-r--r--   0 hans      (1000) hans      (1000)     2313 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/ic_antifeature_disabledalgorithm.xml
--rw-r--r--   0 hans      (1000) hans      (1000)     1415 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/ic_antifeature_knownvuln.xml
--rw-r--r--   0 hans      (1000) hans      (1000)     1846 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/ic_antifeature_nonfreeadd.xml
--rw-r--r--   0 hans      (1000) hans      (1000)     1784 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/ic_antifeature_nonfreeassets.xml
--rw-r--r--   0 hans      (1000) hans      (1000)     1396 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/ic_antifeature_nonfreedep.xml
--rw-r--r--   0 hans      (1000) hans      (1000)     3038 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/ic_antifeature_nonfreenet.xml
--rw-r--r--   0 hans      (1000) hans      (1000)     1102 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/ic_antifeature_nosourcesince.xml
--rw-r--r--   0 hans      (1000) hans      (1000)      871 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/ic_antifeature_nsfw.xml
--rw-r--r--   0 hans      (1000) hans      (1000)     2493 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/ic_antifeature_tracking.xml
--rw-r--r--   0 hans      (1000) hans      (1000)     1442 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/ic_antifeature_upstreamnonfree.xml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/config/ro/
--rw-r--r--   0 hans      (1000) hans      (1000)     1692 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/ro/antiFeatures.yml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/config/zh-rCN/
--rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config/zh-rCN/antiFeatures.yml
--rw-r--r--   0 hans      (1000) hans      (1000)     1170 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/config.py
--rw-r--r--   0 hans      (1000) hans      (1000)   443812 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/corrupt-featureGraphic.png
--rwxr-xr-x   0 hans      (1000) hans      (1000)    15110 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/deploy.TestCase
--rw-r--r--   0 hans      (1000) hans      (1000)    10349 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/dummy-keystore.jks
--rwxr-xr-x   0 hans      (1000) hans      (1000)     2488 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/dump_internal_metadata_format.py
--rwxr-xr-x   0 hans      (1000) hans      (1000)     2093 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/exception.TestCase
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/extra/
--rwxr-xr-x   0 hans      (1000) hans      (1000)     5352 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/extra/manual-vmtools-test.py
--rw-r--r--   0 hans      (1000) hans      (1000)     4395 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/funding-usernames.yaml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/get_android_tools_versions/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-ndk-r10e/
--rw-r--r--   0 hans      (1000) hans      (1000)       18 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/get_android_tools_versions/android-ndk-r10e/RELEASE.TXT
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/ndk/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/ndk/11.2.2725575/
--rw-r--r--   0 hans      (1000) hans      (1000)       51 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/ndk/11.2.2725575/source.properties
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/ndk/17.2.4988734/
--rw-r--r--   0 hans      (1000) hans      (1000)       51 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/ndk/17.2.4988734/source.properties
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/ndk/21.3.6528147/
--rw-r--r--   0 hans      (1000) hans      (1000)       51 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/ndk/21.3.6528147/source.properties
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/ndk-bundle/
--rw-r--r--   0 hans      (1000) hans      (1000)      795 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/ndk-bundle/package.xml
--rw-r--r--   0 hans      (1000) hans      (1000)       51 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/ndk-bundle/source.properties
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/patcher/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/patcher/v4/
--rw-r--r--   0 hans      (1000) hans      (1000)      668 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/patcher/v4/source.properties
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/platforms/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/platforms/android-30/
--rw-r--r--   0 hans      (1000) hans      (1000)      194 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/platforms/android-30/source.properties
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/skiaparser/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/skiaparser/1/
--rwxr-xr-x   0 hans      (1000) hans      (1000)       90 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/skiaparser/1/source.properties
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/tools/
--rw-r--r--   0 hans      (1000) hans      (1000)      138 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/tools/source.properties
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/gnupghome/
--rw-r--r--   0 hans      (1000) hans      (1000)      724 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/gnupghome/pubring.gpg
--rw-r--r--   0 hans      (1000) hans      (1000)      600 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/gnupghome/random_seed
--rw-r--r--   0 hans      (1000) hans      (1000)     1388 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/gnupghome/secring.gpg
--rw-r--r--   0 hans      (1000) hans      (1000)     1280 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/gnupghome/trustdb.gpg
--rw-r--r--   0 hans      (1000) hans      (1000)    49211 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/gradle-maven-blocks.yaml
--rwxr-xr-x   0 hans      (1000) hans      (1000)     5887 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/gradle-release-checksums.py
--rwxr-xr-x   0 hans      (1000) hans      (1000)     6495 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/import_subcommand.TestCase
--rwxr-xr-x   0 hans      (1000) hans      (1000)    35711 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/index.TestCase
--rwxr-xr-x   0 hans      (1000) hans      (1000)     2888 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/init.TestCase
--rwxr-xr-x   0 hans      (1000) hans      (1000)     1608 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/install.TestCase
--rw-r--r--   0 hans      (1000) hans      (1000)    10067 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/janus.apk
--rwxr-xr-x   0 hans      (1000) hans      (1000)      802 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/key-tricks.py
--rw-r--r--   0 hans      (1000) hans      (1000)     5967 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/keystore.jks
--rwxr-xr-x   0 hans      (1000) hans      (1000)    18927 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/lint.TestCase
--rwxr-xr-x   0 hans      (1000) hans      (1000)    10676 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/main.TestCase
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/metadata/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/metadata/apk/
--rw-r--r--   0 hans      (1000) hans      (1000)      704 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/apk/info.guardianproject.urzip.yaml
--rw-r--r--   0 hans      (1000) hans      (1000)     1266 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/apk/org.dyndns.fules.ck.yaml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/metadata/app.with.special.build.params/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/metadata/app.with.special.build.params/en-US/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/metadata/app.with.special.build.params/en-US/antifeatures/
--rw-r--r--   0 hans      (1000) hans      (1000)       16 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/app.with.special.build.params/en-US/antifeatures/50_Ads.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       18 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/app.with.special.build.params/en-US/antifeatures/50_Tracking.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        9 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/app.with.special.build.params/en-US/antifeatures/Ads.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       12 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/app.with.special.build.params/en-US/antifeatures/NoSourceSince.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/metadata/app.with.special.build.params/zh-CN/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/metadata/app.with.special.build.params/zh-CN/antifeatures/
--rw-r--r--   0 hans      (1000) hans      (1000)       31 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/app.with.special.build.params/zh-CN/antifeatures/49_Tracking.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       22 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/app.with.special.build.params/zh-CN/antifeatures/50_Ads.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     2707 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/app.with.special.build.params.yml
--rw-r--r--   0 hans      (1000) hans      (1000)     1150 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/com.politedroid.yml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/metadata/dump/
--rw-r--r--   0 hans      (1000) hans      (1000)     7008 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/dump/app.with.special.build.params.yaml
--rw-r--r--   0 hans      (1000) hans      (1000)     3525 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/dump/com.politedroid.yaml
--rw-r--r--   0 hans      (1000) hans      (1000)    20962 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/dump/org.adaway.yaml
--rw-r--r--   0 hans      (1000) hans      (1000)     8374 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/dump/org.smssecure.smssecure.yaml
--rw-r--r--   0 hans      (1000) hans      (1000)    50353 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/dump/org.videolan.vlc.yaml
--rw-r--r--   0 hans      (1000) hans      (1000)      105 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/duplicate.permisssions.yml
--rw-r--r--   0 hans      (1000) hans      (1000)     1580 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/fake.ota.update.yml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/metadata/info.guardianproject.checkey/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/metadata/info.guardianproject.checkey/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)      470 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.checkey/en-US/description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       28 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.checkey/en-US/name.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/metadata/info.guardianproject.checkey/en-US/phoneScreenshots/
--rw-r--r--   0 hans      (1000) hans      (1000)   129240 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.checkey/en-US/phoneScreenshots/checkey-phone.png
--rw-r--r--   0 hans      (1000) hans      (1000)   169405 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.checkey/en-US/phoneScreenshots/checkey.png
--rw-r--r--   0 hans      (1000) hans      (1000)       19 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.checkey/en-US/summary.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/metadata/info.guardianproject.checkey/ja-JP/
--rw-r--r--   0 hans      (1000) hans      (1000)       40 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.checkey/ja-JP/name.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      491 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.checkey.yml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/en-US/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/en-US/changelogs/
--rw-r--r--   0 hans      (1000) hans      (1000)        4 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/en-US/changelogs/100.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/en-US/changelogs/default.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       17 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/en-US/full_description.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/en-US/images/
--rw-r--r--   0 hans      (1000) hans      (1000)    37877 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/en-US/images/featureGraphic.png
--rw-r--r--   0 hans      (1000) hans      (1000)     1413 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/en-US/images/icon.png
--rw-r--r--   0 hans      (1000) hans      (1000)       18 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/en-US/short_description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/en-US/title.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/en-US/video.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     1571 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip.yml
--rw-r--r--   0 hans      (1000) hans      (1000)      112 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/info.zwanenburg.caffeinetile.yml
--rw-r--r--   0 hans      (1000) hans      (1000)      137 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/no.min.target.sdk.yml
--rw-r--r--   0 hans      (1000) hans      (1000)      323 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/obb.main.oldversion.yml
--rw-r--r--   0 hans      (1000) hans      (1000)      302 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/obb.main.twoversions.yml
--rw-r--r--   0 hans      (1000) hans      (1000)      316 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/obb.mainpatch.current.yml
--rw-r--r--   0 hans      (1000) hans      (1000)     8505 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/org.adaway.yml
--rw-r--r--   0 hans      (1000) hans      (1000)      123 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/org.fdroid.ci.test.app.yml
--rw-r--r--   0 hans      (1000) hans      (1000)    18495 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/org.fdroid.fdroid.yml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/134/
--rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/134/28969C09.RSA
--rw-r--r--   0 hans      (1000) hans      (1000)   233459 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/134/28969C09.SF
--rw-r--r--   0 hans      (1000) hans      (1000)   233338 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/134/MANIFEST.MF
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/135/
--rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/135/28969C09.RSA
--rw-r--r--   0 hans      (1000) hans      (1000)   232264 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/135/28969C09.SF
--rw-r--r--   0 hans      (1000) hans      (1000)   232161 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/135/MANIFEST.MF
--rw-r--r--   0 hans      (1000) hans      (1000)     4751 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure.yml
--rw-r--r--   0 hans      (1000) hans      (1000)    23138 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/org.videolan.vlc.yml
--rw-r--r--   0 hans      (1000) hans      (1000)      102 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/raw.template.yml
--rw-r--r--   0 hans      (1000) hans      (1000)     1690 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata/souch.smsbypass.yml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.921981 fdroidserver-2.3a0/tests/metadata-rewrite-yml/
--rw-r--r--   0 hans      (1000) hans      (1000)     2722 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata-rewrite-yml/app.with.special.build.params.yml
--rw-r--r--   0 hans      (1000) hans      (1000)     1552 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata-rewrite-yml/fake.ota.update.yml
--rw-r--r--   0 hans      (1000) hans      (1000)    18466 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata-rewrite-yml/org.fdroid.fdroid.yml
--rwxr-xr-x   0 hans      (1000) hans      (1000)    95395 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/metadata.TestCase
--rw-r--r--   0 hans      (1000) hans      (1000)     2294 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/minimal_targetsdk_30_unsigned.apk
--rwxr-xr-x   0 hans      (1000) hans      (1000)    19343 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/nightly.TestCase
--rw-r--r--   0 hans      (1000) hans      (1000)     2266 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/no_targetsdk_minsdk1_unsigned.apk
--rw-r--r--   0 hans      (1000) hans      (1000)     2310 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/no_targetsdk_minsdk30_unsigned.apk
--rwxr-xr-x   0 hans      (1000) hans      (1000)      919 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/openssl-version-check-test.py
--rw-r--r--   0 hans      (1000) hans      (1000)     7173 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/org.bitbucket.tickytacky.mirrormirror_1.apk
--rw-r--r--   0 hans      (1000) hans      (1000)     7084 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/org.bitbucket.tickytacky.mirrormirror_2.apk
--rw-r--r--   0 hans      (1000) hans      (1000)     7126 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/org.bitbucket.tickytacky.mirrormirror_3.apk
--rw-r--r--   0 hans      (1000) hans      (1000)     6588 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/org.bitbucket.tickytacky.mirrormirror_4.apk
--rw-r--r--   0 hans      (1000) hans      (1000)   132453 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/org.dyndns.fules.ck_20.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    49715 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/org.sajeg.fallingblocks_3.apk
--rwxr-xr-x   0 hans      (1000) hans      (1000)    17071 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/publish.TestCase
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/repo/
--rw-r--r--   0 hans      (1000) hans      (1000)    14236 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/com.example.test.helloworld_1.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    17552 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/com.politedroid_3.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    18489 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/com.politedroid_4.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    18817 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/com.politedroid_5.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    16578 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/com.politedroid_6.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    27446 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/duplicate.permisssions_9999999.apk
--rw-r--r--   0 hans      (1000) hans      (1000)      238 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/entry.json
--rw-r--r--   0 hans      (1000) hans      (1000)      233 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/fake.ota.update_1234.zip
--rw-r--r--   0 hans      (1000) hans      (1000)    25399 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/index-v1.json
--rw-r--r--   0 hans      (1000) hans      (1000)    53527 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/index-v2.json
--rw-r--r--   0 hans      (1000) hans      (1000)    20519 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/index.xml
--rw-r--r--   0 hans      (1000) hans      (1000)    11740 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/info.zwanenburg.caffeinetile_4.apk
--rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/main.1101613.obb.main.twoversions.obb
--rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/main.1101615.obb.main.twoversions.obb
--rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/main.1434483388.obb.main.oldversion.obb
--rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/main.1619.obb.mainpatch.current.obb
--rw-r--r--   0 hans      (1000) hans      (1000)    14102 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/no.min.target.sdk_987.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    14323 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/obb.main.oldversion_1444412523.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    11477 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/obb.main.twoversions_1101613.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    11480 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/obb.main.twoversions_1101615.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    11481 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/obb.main.twoversions_1101617.apk
--rw-r--r--   0 hans      (1000) hans      (1000)      150 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/obb.main.twoversions_1101617_src.tar.gz
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/repo/obb.mainpatch.current/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/repo/obb.mainpatch.current/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)    24336 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/obb.mainpatch.current/en-US/featureGraphic.png
--rw-r--r--   0 hans      (1000) hans      (1000)   260113 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/obb.mainpatch.current/en-US/icon.png
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/repo/obb.mainpatch.current/en-US/phoneScreenshots/
--rw-r--r--   0 hans      (1000) hans      (1000)    44990 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/obb.mainpatch.current/en-US/phoneScreenshots/screenshot-main.png
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/repo/obb.mainpatch.current/en-US/sevenInchScreenshots/
--rw-r--r--   0 hans      (1000) hans      (1000)    56049 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/obb.mainpatch.current/en-US/sevenInchScreenshots/screenshot-tablet-main.png
--rw-r--r--   0 hans      (1000) hans      (1000)    11479 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/obb.mainpatch.current_1619.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    10541 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/obb.mainpatch.current_1619_another-release-key.apk
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)    16660 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/icon.png
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.925982 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/
--rw-r--r--   0 hans      (1000) hans      (1000)     9272 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot10.png
--rw-r--r--   0 hans      (1000) hans      (1000)    19938 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot12.png
--rw-r--r--   0 hans      (1000) hans      (1000)    43014 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot15.png
--rw-r--r--   0 hans      (1000) hans      (1000)    73703 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot18.png
--rw-r--r--   0 hans      (1000) hans      (1000)    17626 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot20.png
--rw-r--r--   0 hans      (1000) hans      (1000)    16417 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot22.png
--rw-r--r--   0 hans      (1000) hans      (1000)    21486 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot4.png
--rw-r--r--   0 hans      (1000) hans      (1000)    19667 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot7.png
--rw-r--r--   0 hans      (1000) hans      (1000)    37518 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot9.png
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/
--rw-r--r--   0 hans      (1000) hans      (1000)    68918 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot0.png
--rw-r--r--   0 hans      (1000) hans      (1000)   191534 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot1.png
--rw-r--r--   0 hans      (1000) hans      (1000)   125878 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot11.png
--rw-r--r--   0 hans      (1000) hans      (1000)    67178 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot13.png
--rw-r--r--   0 hans      (1000) hans      (1000)   139199 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot14.png
--rw-r--r--   0 hans      (1000) hans      (1000)   214383 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot16.png
--rw-r--r--   0 hans      (1000) hans      (1000)    16876 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot17.png
--rw-r--r--   0 hans      (1000) hans      (1000)    16876 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot19.png
--rw-r--r--   0 hans      (1000) hans      (1000)   133244 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot2.png
--rw-r--r--   0 hans      (1000) hans      (1000)    36011 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot21.png
--rw-r--r--   0 hans      (1000) hans      (1000)   234480 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot23.png
--rw-r--r--   0 hans      (1000) hans      (1000)   154254 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot3.png
--rw-r--r--   0 hans      (1000) hans      (1000)   133546 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot5.png
--rw-r--r--   0 hans      (1000) hans      (1000)   144451 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot6.png
--rw-r--r--   0 hans      (1000) hans      (1000)    77587 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot8.png
--rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/patch.1619.obb.mainpatch.current.obb
--rw-r--r--   0 hans      (1000) hans      (1000)    81295 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/souch.smsbypass_9.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    11471 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/urzip-; Рахма́, [rɐxˈmanʲɪnəf] سيرجي_رخمانينوف 谢·.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    13493 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/repo/v1.v2.sig_1020.apk
--rwxr-xr-x   0 hans      (1000) hans      (1000)     8857 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/rewritemeta.TestCase
--rwxr-xr-x   0 hans      (1000) hans      (1000)    51904 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/run-tests
--rwxr-xr-x   0 hans      (1000) hans      (1000)    32762 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/scanner.TestCase
--rwxr-xr-x   0 hans      (1000) hans      (1000)     2663 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/signatures.TestCase
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/signindex/
--rw-r--r--   0 hans      (1000) hans      (1000)    19941 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/signindex/guardianproject-v1.jar
--rw-r--r--   0 hans      (1000) hans      (1000)    15703 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/signindex/guardianproject.jar
--rw-r--r--   0 hans      (1000) hans      (1000)    22091 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/signindex/testy.jar
--rw-r--r--   0 hans      (1000) hans      (1000)    20068 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/signindex/unsigned.jar
--rwxr-xr-x   0 hans      (1000) hans      (1000)     7848 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/signindex.TestCase
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/Zillode/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/Zillode/syncthing-silk/
--rw-r--r--   0 hans      (1000) hans      (1000)     1984 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/Zillode/syncthing-silk/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/at.bitfire.davdroid/
--rw-r--r--   0 hans      (1000) hans      (1000)     3574 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/at.bitfire.davdroid/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/avenginekit/
--rw-r--r--   0 hans      (1000) hans      (1000)       87 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/avenginekit/build.gradle
--rw-r--r--   0 hans      (1000) hans      (1000)      971 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/chat/
--rw-r--r--   0 hans      (1000) hans      (1000)     4055 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/chat/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/client/
--rw-r--r--   0 hans      (1000) hans      (1000)     1317 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/client/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/client/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/client/src/main/
--rw-r--r--   0 hans      (1000) hans      (1000)     1303 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/client/src/main/AndroidManifest.xml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/emojilibrary/
--rwxr-xr-x   0 hans      (1000) hans      (1000)      685 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/emojilibrary/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/gradle/
--rw-r--r--   0 hans      (1000) hans      (1000)     1138 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/gradle/build_libraries.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/imagepicker/
--rwxr-xr-x   0 hans      (1000) hans      (1000)      716 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/imagepicker/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/mars-core-release/
--rw-r--r--   0 hans      (1000) hans      (1000)       93 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/mars-core-release/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/push/
--rw-r--r--   0 hans      (1000) hans      (1000)     1458 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/push/build.gradle
--rw-r--r--   0 hans      (1000) hans      (1000)      155 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/settings.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.anpmech.launcher/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.anpmech.launcher/app/
--rw-r--r--   0 hans      (1000) hans      (1000)     2258 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.anpmech.launcher/app/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.anpmech.launcher/app/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.anpmech.launcher/app/src/main/
--rw-r--r--   0 hans      (1000) hans      (1000)     2779 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.anpmech.launcher/app/src/main/AndroidManifest.xml
--rw-r--r--   0 hans      (1000) hans      (1000)     1203 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.anpmech.launcher/build.gradle
--rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.anpmech.launcher/settings.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.github.jameshnsears.quoteunquote/
--rw-r--r--   0 hans      (1000) hans      (1000)     7817 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.github.jameshnsears.quoteunquote/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/
--rw-r--r--   0 hans      (1000) hans      (1000)      358 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/gradle/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/gradle/wrapper/
--rw-r--r--   0 hans      (1000) hans      (1000)      230 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/gradle/wrapper/gradle-wrapper.properties
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/localeapi/
--rw-r--r--   0 hans      (1000) hans      (1000)      433 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/localeapi/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/localeapi/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/localeapi/src/main/
--rw-r--r--   0 hans      (1000) hans      (1000)      273 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/localeapi/src/main/AndroidManifest.xml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/oneSheeld/
--rw-r--r--   0 hans      (1000) hans      (1000)     4085 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/oneSheeld/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/oneSheeld/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/oneSheeld/src/main/
--rw-r--r--   0 hans      (1000) hans      (1000)    12491 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/oneSheeld/src/main/AndroidManifest.xml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/pagerIndicator/
--rw-r--r--   0 hans      (1000) hans      (1000)      432 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/pagerIndicator/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/pagerIndicator/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/pagerIndicator/src/main/
--rw-r--r--   0 hans      (1000) hans      (1000)      264 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/pagerIndicator/src/main/AndroidManifest.xml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/pullToRefreshlibrary/
--rw-r--r--   0 hans      (1000) hans      (1000)      378 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/pullToRefreshlibrary/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/pullToRefreshlibrary/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/pullToRefreshlibrary/src/main/
--rw-r--r--   0 hans      (1000) hans      (1000)      299 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/pullToRefreshlibrary/src/main/AndroidManifest.xml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/quickReturnHeader/
--rw-r--r--   0 hans      (1000) hans      (1000)      433 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/quickReturnHeader/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/quickReturnHeader/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/quickReturnHeader/src/main/
--rw-r--r--   0 hans      (1000) hans      (1000)      322 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/quickReturnHeader/src/main/AndroidManifest.xml
--rw-r--r--   0 hans      (1000) hans      (1000)      129 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/settings.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.jens.automation2/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.jens.automation2/app/
--rw-r--r--   0 hans      (1000) hans      (1000)     2439 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.jens.automation2/app/build.gradle
--rw-r--r--   0 hans      (1000) hans      (1000)     2166 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.jens.automation2/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.kunzisoft.testcase/
--rw-r--r--   0 hans      (1000) hans      (1000)     3053 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.kunzisoft.testcase/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/
--rw-r--r--   0 hans      (1000) hans      (1000)     8769 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/generic/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/generic/fastlane/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/android/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/android/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)     1073 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/android/en-US/full_description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       78 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/android/en-US/short_description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        9 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/android/en-US/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/versionDev/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/android/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/android/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)      586 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/android/en-US/full_description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       79 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/android/en-US/short_description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       13 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/android/en-US/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/generic/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/android/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/android/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)     1073 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/android/en-US/full_description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       78 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/android/en-US/short_description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        9 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/android/en-US/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/versionDev/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.889981 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/android/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/android/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)      586 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/android/en-US/full_description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       79 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/android/en-US/short_description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       13 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/android/en-US/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/com.seafile.seadroid2/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.seafile.seadroid2/app/
--rw-r--r--   0 hans      (1000) hans      (1000)     5178 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.seafile.seadroid2/app/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/com.ubergeek42.WeechatAndroid/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.ubergeek42.WeechatAndroid/app/
--rw-r--r--   0 hans      (1000) hans      (1000)    11566 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.ubergeek42.WeechatAndroid/app/build.gradle.kts
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/com.ubergeek42.WeechatAndroid/app/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/com.ubergeek42.WeechatAndroid/app/src/main/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/com.ubergeek42.WeechatAndroid/app/src/main/res/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/com.ubergeek42.WeechatAndroid/app/src/main/res/values/
--rw-r--r--   0 hans      (1000) hans      (1000)    50651 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/com.ubergeek42.WeechatAndroid/app/src/main/res/values/strings.xml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/de.varengold.activeTAN/
--rw-r--r--   0 hans      (1000) hans      (1000)     3711 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/de.varengold.activeTAN/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/dev.patrickgold.florisboard/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/dev.patrickgold.florisboard/app/
--rw-r--r--   0 hans      (1000) hans      (1000)     3693 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/dev.patrickgold.florisboard/app/build.gradle.kts
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/eu.siacs.conversations/
--rw-r--r--   0 hans      (1000) hans      (1000)     3564 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/eu.siacs.conversations/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/eu.siacs.conversations/metadata/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/eu.siacs.conversations/metadata/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)       13 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/eu.siacs.conversations/metadata/en-US/name.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/fdroid/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/fdroid/fdroidclient/
--rw-r--r--   0 hans      (1000) hans      (1000)    20507 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/fdroid/fdroidclient/AndroidManifest.xml
--rw-r--r--   0 hans      (1000) hans      (1000)     8314 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/fdroid/fdroidclient/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/firebase-allowlisted/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/firebase-allowlisted/app/
--rw-r--r--   0 hans      (1000) hans      (1000)      109 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/firebase-allowlisted/app/build.gradle
--rw-r--r--   0 hans      (1000) hans      (1000)      201 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/firebase-allowlisted/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/firebase-suspect/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/firebase-suspect/app/
--rw-r--r--   0 hans      (1000) hans      (1000)      108 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/firebase-suspect/app/build.gradle
--rw-r--r--   0 hans      (1000) hans      (1000)      189 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/firebase-suspect/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/info.guardianproject.ripple/
--rw-r--r--   0 hans      (1000) hans      (1000)      405 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/info.guardianproject.ripple/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/open-keychain/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/open-keychain/open-keychain/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/open-keychain/open-keychain/OpenKeychain/
--rw-r--r--   0 hans      (1000) hans      (1000)    11841 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/open-keychain/open-keychain/OpenKeychain/build.gradle
--rw-r--r--   0 hans      (1000) hans      (1000)     1304 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/open-keychain/open-keychain/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/org.mozilla.rocket/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/org.mozilla.rocket/app/
--rw-r--r--   0 hans      (1000) hans      (1000)    16741 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/org.mozilla.rocket/app/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/org.noise_planet.noisecapture/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/org.noise_planet.noisecapture/app/
--rw-r--r--   0 hans      (1000) hans      (1000)     4194 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/org.noise_planet.noisecapture/app/build.gradle
--rw-r--r--   0 hans      (1000) hans      (1000)       27 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/org.noise_planet.noisecapture/settings.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.929982 fdroidserver-2.3a0/tests/source-files/org.noise_planet.noisecapture/sosfilter/
--rw-r--r--   0 hans      (1000) hans      (1000)      814 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/org.noise_planet.noisecapture/sosfilter/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/org.tasks/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/org.tasks/app/
--rw-r--r--   0 hans      (1000) hans      (1000)     8530 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/org.tasks/app/build.gradle.kts
--rw-r--r--   0 hans      (1000) hans      (1000)      232 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/org.tasks/build.gradle
--rw-r--r--   0 hans      (1000) hans      (1000)      826 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/org.tasks/build.gradle.kts
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/org.tasks/buildSrc/
--rw-r--r--   0 hans      (1000) hans      (1000)       60 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/org.tasks/buildSrc/build.gradle.kts
--rw-r--r--   0 hans      (1000) hans      (1000)       16 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/org.tasks/settings.gradle.kts
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/osmandapp/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/osmandapp/osmand/
--rw-r--r--   0 hans      (1000) hans      (1000)     8372 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/osmandapp/osmand/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/osmandapp/osmand/gradle/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/osmandapp/osmand/gradle/wrapper/
--rw-r--r--   0 hans      (1000) hans      (1000)      233 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/osmandapp/osmand/gradle/wrapper/gradle-wrapper.properties
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/realm/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/realm/react-native/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/realm/react-native/android/
--rw-r--r--   0 hans      (1000) hans      (1000)    13331 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/realm/react-native/android/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/se.manyver/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/se.manyver/android/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/se.manyver/android/app/
--rw-r--r--   0 hans      (1000) hans      (1000)    10781 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/se.manyver/android/app/build.gradle
--rw-r--r--   0 hans      (1000) hans      (1000)     2006 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/se.manyver/android/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/se.manyver/android/gradle/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/se.manyver/android/gradle/wrapper/
--rw-r--r--   0 hans      (1000) hans      (1000)      199 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/se.manyver/android/gradle/wrapper/gradle-wrapper.properties
--rw-r--r--   0 hans      (1000) hans      (1000)      938 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/se.manyver/android/gradle.properties
--rw-r--r--   0 hans      (1000) hans      (1000)     3487 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/se.manyver/android/settings.gradle
--rw-r--r--   0 hans      (1000) hans      (1000)       56 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/se.manyver/app.json
--rw-r--r--   0 hans      (1000) hans      (1000)      571 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/se.manyver/index.android.js
--rw-r--r--   0 hans      (1000) hans      (1000)     5237 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/se.manyver/package.json
--rw-r--r--   0 hans      (1000) hans      (1000)      531 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/se.manyver/react-native.config.js
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/ut.ewh.audiometrytest/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/ut.ewh.audiometrytest/app/
--rw-r--r--   0 hans      (1000) hans      (1000)     1127 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/ut.ewh.audiometrytest/app/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/ut.ewh.audiometrytest/app/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/ut.ewh.audiometrytest/app/src/main/
--rw-r--r--   0 hans      (1000) hans      (1000)     5729 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/ut.ewh.audiometrytest/app/src/main/AndroidManifest.xml
--rw-r--r--   0 hans      (1000) hans      (1000)      548 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/ut.ewh.audiometrytest/build.gradle
--rw-r--r--   0 hans      (1000) hans      (1000)       15 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/ut.ewh.audiometrytest/settings.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/yuriykulikov/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/yuriykulikov/AlarmClock/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/source-files/yuriykulikov/AlarmClock/gradle/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/source-files/yuriykulikov/AlarmClock/gradle/wrapper/
--rw-r--r--   0 hans      (1000) hans      (1000)      238 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/source-files/yuriykulikov/AlarmClock/gradle/wrapper/gradle-wrapper.properties
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/stats/
--rw-r--r--   0 hans      (1000) hans      (1000)     1138 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/stats/known_apks.txt
--rwxr-xr-x   0 hans      (1000) hans      (1000)     2067 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/test-gradlew-fdroid
--rw-r--r--   0 hans      (1000) hans      (1000)     1897 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/testcommon.py
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-2/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-2/build/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/
--rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/.gitignore
--rw-r--r--   0 hans      (1000) hans      (1000)     5496 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/build.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/debug/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/debug/res/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/debug/res/values/
--rw-r--r--   0 hans      (1000) hans      (1000)      114 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/debug/res/values/constants.xml
--rw-r--r--   0 hans      (1000) hans      (1000)       96 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/debug/res/values/strings.xml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/java/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/java/org/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/java/org/piwigo/
--rw-r--r--   0 hans      (1000) hans      (1000)     4061 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/java/org/piwigo/PiwigoApplication.java
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/
--rw-r--r--   0 hans      (1000) hans      (1000)       19 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/contact-email.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       23 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/contact-website.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/default-language.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/de-DE/
--rw-r--r--   0 hans      (1000) hans      (1000)      518 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/de-DE/full-description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       58 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/de-DE/short-description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/de-DE/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)      478 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/full-description.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/feature-graphic/
--rw-r--r--   0 hans      (1000) hans      (1000)     1221 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/feature-graphic/piwigo-full.png
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/icon/
--rw-r--r--   0 hans      (1000) hans      (1000)     1110 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/icon/piwigo-icon.png
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/
--rw-r--r--   0 hans      (1000) hans      (1000)      964 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/01_Login.jpg
--rw-r--r--   0 hans      (1000) hans      (1000)     1108 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/02_Albums.jpg
--rw-r--r--   0 hans      (1000) hans      (1000)     1131 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/03_Photos.jpg
--rw-r--r--   0 hans      (1000) hans      (1000)     1052 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/04_Albums_horizontal.jpg
--rw-r--r--   0 hans      (1000) hans      (1000)      985 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/05_Menu.jpg
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/tablet-screenshots/
--rw-r--r--   0 hans      (1000) hans      (1000)      748 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/tablet-screenshots/01_Login.png
--rw-r--r--   0 hans      (1000) hans      (1000)       44 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/short-description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/fr-FR/
--rw-r--r--   0 hans      (1000) hans      (1000)      646 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/fr-FR/full-description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       57 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/fr-FR/short-description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/fr-FR/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/kn-IN/
--rw-r--r--   0 hans      (1000) hans      (1000)      478 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/kn-IN/full-description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       44 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/kn-IN/short-description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/kn-IN/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/de-DE/
--rw-r--r--   0 hans      (1000) hans      (1000)      475 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/de-DE/default.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)      482 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/en-US/default.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/fr-FR/
--rw-r--r--   0 hans      (1000) hans      (1000)      495 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/fr-FR/default.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/kn-IN/
--rw-r--r--   0 hans      (1000) hans      (1000)      482 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/kn-IN/default.txt
--rw-r--r--   0 hans      (1000) hans      (1000)      422 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/build.gradle
--rw-r--r--   0 hans      (1000) hans      (1000)       51 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/settings.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-2/metadata/
--rw-r--r--   0 hans      (1000) hans      (1000)      673 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-2/metadata/org.piwigo.android.yml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/src/main/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/src/main/play/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/src/main/play/listings/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/src/main/play/listings/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)       26 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/src/main/play/listings/en-US/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/src/main/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/src/main/play/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/src/main/play/listings/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/src/main/play/listings/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)       16 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/src/main/play/listings/en-US/title.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     4549 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/settings.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/src/main/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/src/main/play/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/src/main/play/listings/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/src/main/play/listings/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)       26 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/src/main/play/listings/en-US/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/src/main/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/src/main/play/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/src/main/play/listings/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/src/main/play/listings/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)       16 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/src/main/play/listings/en-US/title.txt
--rw-r--r--   0 hans      (1000) hans      (1000)     4549 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/settings.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/metadata/
--rw-r--r--   0 hans      (1000) hans      (1000)     2907 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/metadata/com.anysoftkeyboard.languagepack.dutch.yml
--rw-r--r--   0 hans      (1000) hans      (1000)    15227 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/metadata/com.menny.android.anysoftkeyboard.yml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-flutter/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-flutter/build/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-flutter/build/fr.emersion.goguma/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-flutter/build/fr.emersion.goguma/android/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/
--rw-r--r--   0 hans      (1000) hans      (1000)       20 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/contact-website.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/listings/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/listings/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)      577 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/listings/en-US/full-description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)       33 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/listings/en-US/short-description.txt
--rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/listings/en-US/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-flutter/metadata/
--rw-r--r--   0 hans      (1000) hans      (1000)      868 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-flutter/metadata/fr.emersion.goguma.yml
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/
--rw-r--r--   0 hans      (1000) hans      (1000)       56 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/settings.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/src/main/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/src/main/play/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/src/main/play/listings/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/src/main/play/listings/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)       23 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/src/main/play/listings/en-US/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/src/main/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/src/main/play/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/src/main/play/listings/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/src/main/play/listings/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)       17 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/src/main/play/listings/en-US/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/
--rw-r--r--   0 hans      (1000) hans      (1000)       56 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/settings.gradle
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/src/main/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/src/main/play/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/src/main/play/listings/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/src/main/play/listings/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)       23 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/src/main/play/listings/en-US/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/src/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/src/main/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/src/main/play/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.893981 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/src/main/play/listings/
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/src/main/play/listings/en-US/
--rw-r--r--   0 hans      (1000) hans      (1000)       17 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/src/main/play/listings/en-US/title.txt
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/triple-t-multiple/metadata/
--rw-r--r--   0 hans      (1000) hans      (1000)     1761 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-multiple/metadata/ch.admin.bag.covidcertificate.verifier.yml
--rw-r--r--   0 hans      (1000) hans      (1000)     1741 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/triple-t-multiple/metadata/ch.admin.bag.covidcertificate.wallet.yml
--rwxr-xr-x   0 hans      (1000) hans      (1000)    99607 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/update.TestCase
--rw-r--r--   0 hans      (1000) hans      (1000)     9925 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/urzip-badcert.apk
--rw-r--r--   0 hans      (1000) hans      (1000)     9923 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/urzip-badsig.apk
--rw-r--r--   0 hans      (1000) hans      (1000)     8471 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/urzip-release-unsigned.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    11406 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/urzip-release.apk
--rw-r--r--   0 hans      (1000) hans      (1000)     9969 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/urzip.apk
--rw-r--r--   0 hans      (1000) hans      (1000)    12086 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/v2.only.sig_2.apk
-drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-04-10 14:57:56.933982 fdroidserver-2.3a0/tests/valid-package-names/
--rw-r--r--   0 hans      (1000) hans      (1000)     8815 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/valid-package-names/RandomPackageNames.java
--rwxr-xr-x   0 hans      (1000) hans      (1000)      196 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/valid-package-names/random-package-names
--rwxr-xr-x   0 hans      (1000) hans      (1000)      885 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/valid-package-names/test.py
--rwxr-xr-x   0 hans      (1000) hans      (1000)     3416 2024-04-10 14:57:40.000000 fdroidserver-2.3a0/tests/vcs.TestCase
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/
+-rw-r--r--   0 hans      (1000) hans      (1000)    11126 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/CHANGELOG.md
+-rw-r--r--   0 hans      (1000) hans      (1000)    34520 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/LICENSE
+-rw-r--r--   0 hans      (1000) hans      (1000)    62226 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/MANIFEST.in
+-rw-r--r--   0 hans      (1000) hans      (1000)     5342 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/PKG-INFO
+-rw-r--r--   0 hans      (1000) hans      (1000)     4486 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/README.md
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/buildserver/
+-rw-r--r--   0 hans      (1000) hans      (1000)     3934 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/buildserver/Vagrantfile
+-rw-r--r--   0 hans      (1000) hans      (1000)       68 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/buildserver/config.buildserver.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)      711 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/buildserver/provision-android-ndk
+-rw-r--r--   0 hans      (1000) hans      (1000)     4547 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/buildserver/provision-android-sdk
+-rw-r--r--   0 hans      (1000) hans      (1000)     2887 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/buildserver/provision-apt-get-install
+-rw-r--r--   0 hans      (1000) hans      (1000)      298 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/buildserver/provision-apt-proxy
+-rw-r--r--   0 hans      (1000) hans      (1000)     1463 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/buildserver/provision-gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/buildserver/setup-env-vars
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/completion/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6221 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/completion/bash-completion
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/examples/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1892 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/examples/Vagrantfile.yaml
+-rw-r--r--   0 hans      (1000) hans      (1000)    15338 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/examples/config.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)     2265 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/examples/fdroid_export_keystore_to_nitrokey.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     2004 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/examples/fdroid_exportkeystore.py
+-rw-r--r--   0 hans      (1000) hans      (1000)      517 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/examples/fdroid_extract_repo_pubkey.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     1559 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/examples/fdroid_fetchsrclibs.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     1541 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/examples/fdroid_nitrokeyimport.py
+-rw-r--r--   0 hans      (1000) hans      (1000)      123 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/examples/opensc-fdroid.cfg
+-rw-r--r--   0 hans      (1000) hans      (1000)      237 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/examples/public-read-only-s3-bucket-policy.json
+-rw-r--r--   0 hans      (1000) hans      (1000)      244 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/examples/template.yml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/fdroidserver/
+-rw-r--r--   0 hans      (1000) hans      (1000)     2284 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/__init__.py
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     8941 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/__main__.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    37993 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/apksigcopier.py
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/fdroidserver/asynchronousfilereader/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1350 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/asynchronousfilereader/__init__.py
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     9831 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/btlog.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    60939 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/build.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    26800 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/checkupdates.py
+-rw-r--r--   0 hans      (1000) hans      (1000)   175233 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/common.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    37776 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/deploy.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     1202 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/exception.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     2886 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/gpgsign.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    14805 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/import_subcommand.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    69874 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/index.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    11707 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/init.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     4726 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/install.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    34407 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/lint.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    12123 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/looseversion.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    41680 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/metadata.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     9209 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/mirror.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     4002 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/net.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    21175 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/nightly.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    17391 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/publish.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     1158 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/readmeta.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     3610 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/rewritemeta.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    45810 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/scanner.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     3922 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/signatures.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     8179 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/signindex.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     3299 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/tail.py
+-rw-r--r--   0 hans      (1000) hans      (1000)   112507 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/update.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     8483 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/verify.py
+-rw-r--r--   0 hans      (1000) hans      (1000)    16140 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/fdroidserver/vmtools.py
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/fdroidserver.egg-info/
+-rw-r--r--   0 hans      (1000) hans      (1000)     5342 2024-05-13 08:46:29.000000 fdroidserver-2.3a1/fdroidserver.egg-info/PKG-INFO
+-rw-r--r--   0 hans      (1000) hans      (1000)    56200 2024-05-13 08:46:29.000000 fdroidserver-2.3a1/fdroidserver.egg-info/SOURCES.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        1 2024-05-13 08:46:29.000000 fdroidserver-2.3a1/fdroidserver.egg-info/dependency_links.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       54 2024-05-13 08:46:29.000000 fdroidserver-2.3a1/fdroidserver.egg-info/entry_points.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      349 2024-05-13 08:46:29.000000 fdroidserver-2.3a1/fdroidserver.egg-info/requires.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       13 2024-05-13 08:46:29.000000 fdroidserver-2.3a1/fdroidserver.egg-info/top_level.txt
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    18504 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/gradlew-fdroid
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/bo/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/bo/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)   111110 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/bo/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/cs/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    95081 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/cs/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/de/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/de/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    96478 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/de/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/es/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/es/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    96256 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/es/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/fr/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    98956 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/fr/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/hu/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    84888 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/hu/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/it/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/it/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    95189 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/it/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/ko/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    75849 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/ko/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/nb_NO/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    89381 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/nb_NO/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/pl/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    95734 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/pl/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/pt/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    95243 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/pt/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/pt_BR/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    95892 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/pt_BR/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/pt_PT/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    95319 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/pt_PT/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/ro/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    96228 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/ro/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/ru/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)   115785 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/ru/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/sq/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    94894 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/sq/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/tr/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    94251 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/tr/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/uk/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)   111258 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/uk/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/zh_Hans/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    86843 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/zh_Hans/LC_MESSAGES/fdroidserver.po
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/locale/zh_Hant/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.888382 fdroidserver-2.3a1/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 hans      (1000) hans      (1000)    88340 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/locale/zh_Hant/LC_MESSAGES/fdroidserver.po
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    18661 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/makebuildserver
+-rw-r--r--   0 hans      (1000) hans      (1000)     5274 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/pyproject.toml
+-rw-r--r--   0 hans      (1000) hans      (1000)      771 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/setup.cfg
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     4108 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/setup.py
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.892382 fdroidserver-2.3a1/tests/
+-rw-r--r--   0 hans      (1000) hans      (1000)      750 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/IsMD5Disabled.java
+-rw-r--r--   0 hans      (1000) hans      (1000)    12227 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/Norway_bouvet_europe_2.obf.zip
+-rw-r--r--   0 hans      (1000) hans      (1000)     4060 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/SANAPPSI.RSA
+-rw-r--r--   0 hans      (1000) hans      (1000)    63316 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/SANAPPSI.SF
+-rw-r--r--   0 hans      (1000) hans      (1000)     7299 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/SpeedoMeterApp.main_1.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)     2557 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/aosp_testkey_debug.keystore
+-rw-r--r--   0 hans      (1000) hans      (1000)    16876 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/apk.embedded_1.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    11471 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/bad-unicode-πÇÇ现代通用字-български-عربي1.apk
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.892382 fdroidserver-2.3a1/tests/build-tools/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.892382 fdroidserver-2.3a1/tests/build-tools/17.0.0/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6221 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      921 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      937 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1442 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      848 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      635 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1334 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      646 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      649 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1496 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.892382 fdroidserver-2.3a1/tests/build-tools/18.1.1/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6221 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      921 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      937 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1442 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      848 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      635 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1334 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      646 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      649 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1496 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.892382 fdroidserver-2.3a1/tests/build-tools/19.0.0/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6221 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      921 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      937 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1442 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      848 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      635 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1334 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      646 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      649 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1496 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.892382 fdroidserver-2.3a1/tests/build-tools/19.1.0/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6221 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      921 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      937 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1442 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      848 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      635 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1334 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      646 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      649 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1496 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.892382 fdroidserver-2.3a1/tests/build-tools/20.0.0/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6221 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      921 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      937 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1442 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      848 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      635 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1334 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      646 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      649 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1496 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.896382 fdroidserver-2.3a1/tests/build-tools/21.1.1/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1475 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1223 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.896382 fdroidserver-2.3a1/tests/build-tools/21.1.2/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1475 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1223 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.896382 fdroidserver-2.3a1/tests/build-tools/22.0.0/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1635 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1529 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.896382 fdroidserver-2.3a1/tests/build-tools/22.0.1/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1635 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1529 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.896382 fdroidserver-2.3a1/tests/build-tools/23.0.0/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1635 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1529 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.896382 fdroidserver-2.3a1/tests/build-tools/23.0.1/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1635 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1529 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.908382 fdroidserver-2.3a1/tests/build-tools/23.0.2/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1635 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1529 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.908382 fdroidserver-2.3a1/tests/build-tools/23.0.3/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6531 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      970 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      999 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1816 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      898 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      683 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      746 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      696 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      713 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1618 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.908382 fdroidserver-2.3a1/tests/build-tools/24.0.0/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6497 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1379 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1379 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      917 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      946 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      727 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      628 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      675 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      675 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      675 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      657 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      666 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1563 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.912382 fdroidserver-2.3a1/tests/build-tools/24.0.1/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6497 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1379 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1379 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      917 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      946 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      727 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      628 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      675 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      675 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      675 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      657 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      666 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1563 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.912382 fdroidserver-2.3a1/tests/build-tools/24.0.2/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6493 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      913 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      942 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      624 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      662 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1559 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.912382 fdroidserver-2.3a1/tests/build-tools/24.0.3/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6493 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      913 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      942 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      624 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      662 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1559 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.912382 fdroidserver-2.3a1/tests/build-tools/25.0.0/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6493 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      913 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      942 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      624 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      662 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1559 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.912382 fdroidserver-2.3a1/tests/build-tools/25.0.1/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6493 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      913 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      942 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      624 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      662 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1559 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.912382 fdroidserver-2.3a1/tests/build-tools/25.0.2/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6493 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      913 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      942 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1766 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      624 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      662 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1559 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.912382 fdroidserver-2.3a1/tests/build-tools/25.0.3/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6493 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      913 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      942 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1804 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      723 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      624 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1617 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      671 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      662 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1559 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.916382 fdroidserver-2.3a1/tests/build-tools/26.0.0/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.916382 fdroidserver-2.3a1/tests/build-tools/26.0.1/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.916382 fdroidserver-2.3a1/tests/build-tools/26.0.2/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.916382 fdroidserver-2.3a1/tests/build-tools/26.0.3/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.916382 fdroidserver-2.3a1/tests/build-tools/27.0.0/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.916382 fdroidserver-2.3a1/tests/build-tools/27.0.1/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.916382 fdroidserver-2.3a1/tests/build-tools/27.0.2/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.916382 fdroidserver-2.3a1/tests/build-tools/27.0.3/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6527 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1428 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      966 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      709 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1614 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/build-tools/28.0.0/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6580 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      938 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      734 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1586 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/build-tools/28.0.1/
+-rw-r--r--   0 hans      (1000) hans      (1000)     6580 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-com.moez.QKSMS_182.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      938 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      734 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1586 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/build-tools/28.0.2/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      938 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      734 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-org.droidtr.keyboard_34.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1586 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-souch.smsbypass_9.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/build-tools/28.0.3/
+-rw-r--r--   0 hans      (1000) hans      (1000)      655 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-com.example.test.helloworld_1.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-com.politedroid_3.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1400 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-com.politedroid_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      938 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-com.politedroid_5.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      995 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-com.politedroid_6.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1854 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-duplicate.permisssions_9999999.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      894 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-info.guardianproject.urzip_100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      679 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1230 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-no.min.target.sdk_987.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1686 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-obb.main.oldversion_1444412523.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-obb.main.twoversions_1101613.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-obb.main.twoversions_1101615.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      742 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-obb.main.twoversions_1101617.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      692 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-obb.mainpatch.current_1619.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1586 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-souch.smsbypass_9.txt
+-rwxr-xr-x   0 hans      (1000) hans      (1000)      645 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build-tools/generate.sh
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    44436 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/build.TestCase
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    18340 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/check-fdroid-apk
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    13259 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/checkupdates.TestCase
+-rw-r--r--   0 hans      (1000) hans      (1000)     1722 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/com.fake.IpaApp_1000000000001.ipa
+-rwxr-xr-x   0 hans      (1000) hans      (1000)   147208 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/common.TestCase
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/config/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1547 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/antiFeatures.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)      208 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/categories.yml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/config/de/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1648 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/de/antiFeatures.yml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/config/fa/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1956 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/fa/antiFeatures.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1564 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/ic_antifeature_ads.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)     2313 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/ic_antifeature_disabledalgorithm.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1415 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/ic_antifeature_knownvuln.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1846 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/ic_antifeature_nonfreeadd.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1784 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/ic_antifeature_nonfreeassets.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1396 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/ic_antifeature_nonfreedep.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)     3038 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/ic_antifeature_nonfreenet.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1102 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/ic_antifeature_nosourcesince.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)      871 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/ic_antifeature_nsfw.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)     2493 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/ic_antifeature_tracking.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1442 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/ic_antifeature_upstreamnonfree.xml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/config/ro/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1692 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/ro/antiFeatures.yml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/config/zh-rCN/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1375 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config/zh-rCN/antiFeatures.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1170 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/config.py
+-rw-r--r--   0 hans      (1000) hans      (1000)   443812 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/corrupt-featureGraphic.png
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    15317 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/deploy.TestCase
+-rw-r--r--   0 hans      (1000) hans      (1000)    10349 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/dummy-keystore.jks
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     2503 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/dump_internal_metadata_format.py
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     2048 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/exception.TestCase
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/extra/
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     5352 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/extra/manual-vmtools-test.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     4395 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/funding-usernames.yaml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/tests/get_android_tools_versions/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/get_android_tools_versions/android-ndk-r10e/
+-rw-r--r--   0 hans      (1000) hans      (1000)       18 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/get_android_tools_versions/android-ndk-r10e/RELEASE.TXT
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/ndk/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/ndk/11.2.2725575/
+-rw-r--r--   0 hans      (1000) hans      (1000)       51 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/ndk/11.2.2725575/source.properties
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/ndk/17.2.4988734/
+-rw-r--r--   0 hans      (1000) hans      (1000)       51 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/ndk/17.2.4988734/source.properties
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/ndk/21.3.6528147/
+-rw-r--r--   0 hans      (1000) hans      (1000)       51 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/ndk/21.3.6528147/source.properties
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/ndk-bundle/
+-rw-r--r--   0 hans      (1000) hans      (1000)      795 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/ndk-bundle/package.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)       51 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/ndk-bundle/source.properties
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/patcher/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/patcher/v4/
+-rw-r--r--   0 hans      (1000) hans      (1000)      668 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/patcher/v4/source.properties
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/platforms/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/platforms/android-30/
+-rw-r--r--   0 hans      (1000) hans      (1000)      194 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/platforms/android-30/source.properties
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/skiaparser/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/skiaparser/1/
+-rwxr-xr-x   0 hans      (1000) hans      (1000)       90 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/skiaparser/1/source.properties
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/tools/
+-rw-r--r--   0 hans      (1000) hans      (1000)      138 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/tools/source.properties
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/gnupghome/
+-rw-r--r--   0 hans      (1000) hans      (1000)      724 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/gnupghome/pubring.gpg
+-rw-r--r--   0 hans      (1000) hans      (1000)      600 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/gnupghome/random_seed
+-rw-r--r--   0 hans      (1000) hans      (1000)     1388 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/gnupghome/secring.gpg
+-rw-r--r--   0 hans      (1000) hans      (1000)     1280 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/gnupghome/trustdb.gpg
+-rw-r--r--   0 hans      (1000) hans      (1000)    49211 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/gradle-maven-blocks.yaml
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     5887 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/gradle-release-checksums.py
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     6390 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/import_subcommand.TestCase
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    40047 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/index.TestCase
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     2861 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/init.TestCase
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     1598 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/install.TestCase
+-rw-r--r--   0 hans      (1000) hans      (1000)    10728 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/issue-1128-min-sdk-30-poc.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)     6896 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/issue-1128-poc1.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)     9781 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/issue-1128-poc2.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)     8822 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/issue-1128-poc3a.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)     8821 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/issue-1128-poc3b.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    10067 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/janus.apk
+-rwxr-xr-x   0 hans      (1000) hans      (1000)      788 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/key-tricks.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     5967 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/keystore.jks
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    20501 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/lint.TestCase
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    10670 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/main.TestCase
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.920383 fdroidserver-2.3a1/tests/metadata/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/metadata/apk/
+-rw-r--r--   0 hans      (1000) hans      (1000)      704 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/apk/info.guardianproject.urzip.yaml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1266 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/apk/org.dyndns.fules.ck.yaml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/tests/metadata/app.with.special.build.params/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/tests/metadata/app.with.special.build.params/en-US/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/metadata/app.with.special.build.params/en-US/antifeatures/
+-rw-r--r--   0 hans      (1000) hans      (1000)       16 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/app.with.special.build.params/en-US/antifeatures/50_Ads.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       18 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/app.with.special.build.params/en-US/antifeatures/50_Tracking.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        9 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/app.with.special.build.params/en-US/antifeatures/Ads.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       12 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/app.with.special.build.params/en-US/antifeatures/NoSourceSince.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/tests/metadata/app.with.special.build.params/zh-CN/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/metadata/app.with.special.build.params/zh-CN/antifeatures/
+-rw-r--r--   0 hans      (1000) hans      (1000)       31 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/app.with.special.build.params/zh-CN/antifeatures/49_Tracking.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       22 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/app.with.special.build.params/zh-CN/antifeatures/50_Ads.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     2707 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/app.with.special.build.params.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1150 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/com.politedroid.yml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/metadata/dump/
+-rw-r--r--   0 hans      (1000) hans      (1000)     7008 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/dump/app.with.special.build.params.yaml
+-rw-r--r--   0 hans      (1000) hans      (1000)     3525 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/dump/com.politedroid.yaml
+-rw-r--r--   0 hans      (1000) hans      (1000)    20962 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/dump/org.adaway.yaml
+-rw-r--r--   0 hans      (1000) hans      (1000)     8374 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/dump/org.smssecure.smssecure.yaml
+-rw-r--r--   0 hans      (1000) hans      (1000)    50353 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/dump/org.videolan.vlc.yaml
+-rw-r--r--   0 hans      (1000) hans      (1000)      105 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/duplicate.permisssions.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1580 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/fake.ota.update.yml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.876381 fdroidserver-2.3a1/tests/metadata/info.guardianproject.checkey/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/metadata/info.guardianproject.checkey/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)      470 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.checkey/en-US/description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       28 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.checkey/en-US/name.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/metadata/info.guardianproject.checkey/en-US/phoneScreenshots/
+-rw-r--r--   0 hans      (1000) hans      (1000)   129240 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.checkey/en-US/phoneScreenshots/checkey-phone.png
+-rw-r--r--   0 hans      (1000) hans      (1000)   169405 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.checkey/en-US/phoneScreenshots/checkey.png
+-rw-r--r--   0 hans      (1000) hans      (1000)       19 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.checkey/en-US/summary.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/metadata/info.guardianproject.checkey/ja-JP/
+-rw-r--r--   0 hans      (1000) hans      (1000)       40 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.checkey/ja-JP/name.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      491 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.checkey.yml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/en-US/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/en-US/changelogs/
+-rw-r--r--   0 hans      (1000) hans      (1000)        4 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/en-US/changelogs/100.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/en-US/changelogs/default.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       17 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/en-US/full_description.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/en-US/images/
+-rw-r--r--   0 hans      (1000) hans      (1000)    37877 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/en-US/images/featureGraphic.png
+-rw-r--r--   0 hans      (1000) hans      (1000)     1413 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/en-US/images/icon.png
+-rw-r--r--   0 hans      (1000) hans      (1000)       18 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/en-US/short_description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/en-US/title.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/en-US/video.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     1571 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)      112 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/info.zwanenburg.caffeinetile.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)      137 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/no.min.target.sdk.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)      323 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/obb.main.oldversion.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)      302 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/obb.main.twoversions.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)      316 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/obb.mainpatch.current.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)     8505 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/org.adaway.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)      123 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/org.fdroid.ci.test.app.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)    18495 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/org.fdroid.fdroid.yml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/134/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/134/28969C09.RSA
+-rw-r--r--   0 hans      (1000) hans      (1000)   233459 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/134/28969C09.SF
+-rw-r--r--   0 hans      (1000) hans      (1000)   233338 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/134/MANIFEST.MF
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/135/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1326 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/135/28969C09.RSA
+-rw-r--r--   0 hans      (1000) hans      (1000)   232264 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/135/28969C09.SF
+-rw-r--r--   0 hans      (1000) hans      (1000)   232161 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/135/MANIFEST.MF
+-rw-r--r--   0 hans      (1000) hans      (1000)     4751 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)    23138 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/org.videolan.vlc.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)      102 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/raw.template.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1690 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata/souch.smsbypass.yml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/metadata-rewrite-yml/
+-rw-r--r--   0 hans      (1000) hans      (1000)     2722 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata-rewrite-yml/app.with.special.build.params.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1552 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata-rewrite-yml/fake.ota.update.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)    18466 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata-rewrite-yml/org.fdroid.fdroid.yml
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    95391 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/metadata.TestCase
+-rw-r--r--   0 hans      (1000) hans      (1000)     2294 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/minimal_targetsdk_30_unsigned.apk
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    19446 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/nightly.TestCase
+-rw-r--r--   0 hans      (1000) hans      (1000)     2266 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/no_targetsdk_minsdk1_unsigned.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)     2310 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/no_targetsdk_minsdk30_unsigned.apk
+-rwxr-xr-x   0 hans      (1000) hans      (1000)      919 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/openssl-version-check-test.py
+-rw-r--r--   0 hans      (1000) hans      (1000)     7173 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/org.bitbucket.tickytacky.mirrormirror_1.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)     7084 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/org.bitbucket.tickytacky.mirrormirror_2.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)     7126 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/org.bitbucket.tickytacky.mirrormirror_3.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)     6588 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/org.bitbucket.tickytacky.mirrormirror_4.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)   132453 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/org.dyndns.fules.ck_20.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    49715 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/org.sajeg.fallingblocks_3.apk
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    17133 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/publish.TestCase
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/repo/
+-rw-r--r--   0 hans      (1000) hans      (1000)    14236 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/com.example.test.helloworld_1.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    17552 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/com.politedroid_3.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    18489 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/com.politedroid_4.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    18817 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/com.politedroid_5.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    16578 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/com.politedroid_6.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    27446 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/duplicate.permisssions_9999999.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)      238 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/entry.json
+-rw-r--r--   0 hans      (1000) hans      (1000)      233 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/fake.ota.update_1234.zip
+-rw-r--r--   0 hans      (1000) hans      (1000)    25399 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/index-v1.json
+-rw-r--r--   0 hans      (1000) hans      (1000)    53527 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/index-v2.json
+-rw-r--r--   0 hans      (1000) hans      (1000)    20519 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/index.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)    11740 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/info.zwanenburg.caffeinetile_4.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/main.1101613.obb.main.twoversions.obb
+-rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/main.1101615.obb.main.twoversions.obb
+-rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/main.1434483388.obb.main.oldversion.obb
+-rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/main.1619.obb.mainpatch.current.obb
+-rw-r--r--   0 hans      (1000) hans      (1000)    14102 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/no.min.target.sdk_987.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    14323 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/obb.main.oldversion_1444412523.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    11477 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/obb.main.twoversions_1101613.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    11480 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/obb.main.twoversions_1101615.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    11481 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/obb.main.twoversions_1101617.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)      150 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/obb.main.twoversions_1101617_src.tar.gz
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/repo/obb.mainpatch.current/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/repo/obb.mainpatch.current/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)    24336 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/obb.mainpatch.current/en-US/featureGraphic.png
+-rw-r--r--   0 hans      (1000) hans      (1000)   260113 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/obb.mainpatch.current/en-US/icon.png
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/repo/obb.mainpatch.current/en-US/phoneScreenshots/
+-rw-r--r--   0 hans      (1000) hans      (1000)    44990 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/obb.mainpatch.current/en-US/phoneScreenshots/screenshot-main.png
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/repo/obb.mainpatch.current/en-US/sevenInchScreenshots/
+-rw-r--r--   0 hans      (1000) hans      (1000)    56049 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/obb.mainpatch.current/en-US/sevenInchScreenshots/screenshot-tablet-main.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    11479 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/obb.mainpatch.current_1619.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    10541 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/obb.mainpatch.current_1619_another-release-key.apk
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)    16660 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/icon.png
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.924383 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/
+-rw-r--r--   0 hans      (1000) hans      (1000)     9272 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot10.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    19938 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot12.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    43014 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot15.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    73703 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot18.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    17626 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot20.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    16417 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot22.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    21486 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot4.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    19667 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot7.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    37518 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot9.png
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/
+-rw-r--r--   0 hans      (1000) hans      (1000)    68918 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot0.png
+-rw-r--r--   0 hans      (1000) hans      (1000)   191534 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot1.png
+-rw-r--r--   0 hans      (1000) hans      (1000)   125878 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot11.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    67178 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot13.png
+-rw-r--r--   0 hans      (1000) hans      (1000)   139199 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot14.png
+-rw-r--r--   0 hans      (1000) hans      (1000)   214383 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot16.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    16876 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot17.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    16876 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot19.png
+-rw-r--r--   0 hans      (1000) hans      (1000)   133244 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot2.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    36011 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot21.png
+-rw-r--r--   0 hans      (1000) hans      (1000)   234480 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot23.png
+-rw-r--r--   0 hans      (1000) hans      (1000)   154254 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot3.png
+-rw-r--r--   0 hans      (1000) hans      (1000)   133546 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot5.png
+-rw-r--r--   0 hans      (1000) hans      (1000)   144451 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot6.png
+-rw-r--r--   0 hans      (1000) hans      (1000)    77587 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot8.png
+-rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/patch.1619.obb.mainpatch.current.obb
+-rw-r--r--   0 hans      (1000) hans      (1000)    81295 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/souch.smsbypass_9.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    11471 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/urzip-; Рахма́, [rɐxˈmanʲɪnəf] سيرجي_رخمانينوف 谢·.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    13493 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/repo/v1.v2.sig_1020.apk
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     8850 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/rewritemeta.TestCase
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    51967 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/run-tests
+-rwxr-xr-x   0 hans      (1000) hans      (1000)    32745 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/scanner.TestCase
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     2643 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/signatures.TestCase
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/signindex/
+-rw-r--r--   0 hans      (1000) hans      (1000)    19941 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/signindex/guardianproject-v1.jar
+-rw-r--r--   0 hans      (1000) hans      (1000)    15703 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/signindex/guardianproject.jar
+-rw-r--r--   0 hans      (1000) hans      (1000)    22091 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/signindex/testy.jar
+-rw-r--r--   0 hans      (1000) hans      (1000)    20068 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/signindex/unsigned.jar
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     7828 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/signindex.TestCase
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/Zillode/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/Zillode/syncthing-silk/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1984 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/Zillode/syncthing-silk/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/at.bitfire.davdroid/
+-rw-r--r--   0 hans      (1000) hans      (1000)     3574 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/at.bitfire.davdroid/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/avenginekit/
+-rw-r--r--   0 hans      (1000) hans      (1000)       87 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/avenginekit/build.gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)      971 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/chat/
+-rw-r--r--   0 hans      (1000) hans      (1000)     4055 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/chat/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/client/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1317 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/client/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/client/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/client/src/main/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1303 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/client/src/main/AndroidManifest.xml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/emojilibrary/
+-rwxr-xr-x   0 hans      (1000) hans      (1000)      685 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/emojilibrary/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/gradle/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1138 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/gradle/build_libraries.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/imagepicker/
+-rwxr-xr-x   0 hans      (1000) hans      (1000)      716 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/imagepicker/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/mars-core-release/
+-rw-r--r--   0 hans      (1000) hans      (1000)       93 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/mars-core-release/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/push/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1458 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/push/build.gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)      155 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/settings.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.anpmech.launcher/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.anpmech.launcher/app/
+-rw-r--r--   0 hans      (1000) hans      (1000)     2258 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.anpmech.launcher/app/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.anpmech.launcher/app/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.anpmech.launcher/app/src/main/
+-rw-r--r--   0 hans      (1000) hans      (1000)     2779 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.anpmech.launcher/app/src/main/AndroidManifest.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1203 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.anpmech.launcher/build.gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)      653 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.anpmech.launcher/settings.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.github.jameshnsears.quoteunquote/
+-rw-r--r--   0 hans      (1000) hans      (1000)     7817 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.github.jameshnsears.quoteunquote/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/
+-rw-r--r--   0 hans      (1000) hans      (1000)      358 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/gradle/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/gradle/wrapper/
+-rw-r--r--   0 hans      (1000) hans      (1000)      230 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/gradle/wrapper/gradle-wrapper.properties
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/localeapi/
+-rw-r--r--   0 hans      (1000) hans      (1000)      433 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/localeapi/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/localeapi/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/localeapi/src/main/
+-rw-r--r--   0 hans      (1000) hans      (1000)      273 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/localeapi/src/main/AndroidManifest.xml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/oneSheeld/
+-rw-r--r--   0 hans      (1000) hans      (1000)     4085 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/oneSheeld/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/oneSheeld/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/oneSheeld/src/main/
+-rw-r--r--   0 hans      (1000) hans      (1000)    12491 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/oneSheeld/src/main/AndroidManifest.xml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/pagerIndicator/
+-rw-r--r--   0 hans      (1000) hans      (1000)      432 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/pagerIndicator/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/pagerIndicator/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/pagerIndicator/src/main/
+-rw-r--r--   0 hans      (1000) hans      (1000)      264 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/pagerIndicator/src/main/AndroidManifest.xml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/pullToRefreshlibrary/
+-rw-r--r--   0 hans      (1000) hans      (1000)      378 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/pullToRefreshlibrary/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/pullToRefreshlibrary/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/pullToRefreshlibrary/src/main/
+-rw-r--r--   0 hans      (1000) hans      (1000)      299 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/pullToRefreshlibrary/src/main/AndroidManifest.xml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/quickReturnHeader/
+-rw-r--r--   0 hans      (1000) hans      (1000)      433 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/quickReturnHeader/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/quickReturnHeader/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/quickReturnHeader/src/main/
+-rw-r--r--   0 hans      (1000) hans      (1000)      322 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/quickReturnHeader/src/main/AndroidManifest.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)      129 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/settings.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.jens.automation2/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.jens.automation2/app/
+-rw-r--r--   0 hans      (1000) hans      (1000)     2439 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.jens.automation2/app/build.gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)     2166 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.jens.automation2/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.kunzisoft.testcase/
+-rw-r--r--   0 hans      (1000) hans      (1000)     3053 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.kunzisoft.testcase/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/
+-rw-r--r--   0 hans      (1000) hans      (1000)     8769 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/generic/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/generic/fastlane/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/android/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/android/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1073 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/android/en-US/full_description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       78 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/android/en-US/short_description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        9 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/android/en-US/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/versionDev/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/android/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/android/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)      586 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/android/en-US/full_description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       79 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/android/en-US/short_description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       13 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/android/en-US/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/generic/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/android/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/android/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1073 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/android/en-US/full_description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       78 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/android/en-US/short_description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        9 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/android/en-US/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/versionDev/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/android/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/android/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)      586 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/android/en-US/full_description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       79 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/android/en-US/short_description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       13 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/android/en-US/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.seafile.seadroid2/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.seafile.seadroid2/app/
+-rw-r--r--   0 hans      (1000) hans      (1000)     5178 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.seafile.seadroid2/app/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.ubergeek42.WeechatAndroid/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.ubergeek42.WeechatAndroid/app/
+-rw-r--r--   0 hans      (1000) hans      (1000)    11566 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.ubergeek42.WeechatAndroid/app/build.gradle.kts
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.ubergeek42.WeechatAndroid/app/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.ubergeek42.WeechatAndroid/app/src/main/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/com.ubergeek42.WeechatAndroid/app/src/main/res/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/com.ubergeek42.WeechatAndroid/app/src/main/res/values/
+-rw-r--r--   0 hans      (1000) hans      (1000)    50651 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/com.ubergeek42.WeechatAndroid/app/src/main/res/values/strings.xml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/de.varengold.activeTAN/
+-rw-r--r--   0 hans      (1000) hans      (1000)     3711 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/de.varengold.activeTAN/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/dev.patrickgold.florisboard/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/dev.patrickgold.florisboard/app/
+-rw-r--r--   0 hans      (1000) hans      (1000)     3693 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/dev.patrickgold.florisboard/app/build.gradle.kts
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/eu.siacs.conversations/
+-rw-r--r--   0 hans      (1000) hans      (1000)     3564 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/eu.siacs.conversations/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/eu.siacs.conversations/metadata/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/eu.siacs.conversations/metadata/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)       13 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/eu.siacs.conversations/metadata/en-US/name.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/fdroid/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/fdroid/fdroidclient/
+-rw-r--r--   0 hans      (1000) hans      (1000)    20507 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/fdroid/fdroidclient/AndroidManifest.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)     8314 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/fdroid/fdroidclient/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/firebase-allowlisted/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/firebase-allowlisted/app/
+-rw-r--r--   0 hans      (1000) hans      (1000)      109 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/firebase-allowlisted/app/build.gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)      201 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/firebase-allowlisted/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/firebase-suspect/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/firebase-suspect/app/
+-rw-r--r--   0 hans      (1000) hans      (1000)      108 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/firebase-suspect/app/build.gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)      189 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/firebase-suspect/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/info.guardianproject.ripple/
+-rw-r--r--   0 hans      (1000) hans      (1000)      405 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/info.guardianproject.ripple/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/open-keychain/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/open-keychain/open-keychain/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/open-keychain/open-keychain/OpenKeychain/
+-rw-r--r--   0 hans      (1000) hans      (1000)    11841 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/open-keychain/open-keychain/OpenKeychain/build.gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)     1304 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/open-keychain/open-keychain/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/org.mozilla.rocket/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/org.mozilla.rocket/app/
+-rw-r--r--   0 hans      (1000) hans      (1000)    16741 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/org.mozilla.rocket/app/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/org.noise_planet.noisecapture/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/org.noise_planet.noisecapture/app/
+-rw-r--r--   0 hans      (1000) hans      (1000)     4194 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/org.noise_planet.noisecapture/app/build.gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)       27 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/org.noise_planet.noisecapture/settings.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.928383 fdroidserver-2.3a1/tests/source-files/org.noise_planet.noisecapture/sosfilter/
+-rw-r--r--   0 hans      (1000) hans      (1000)      814 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/org.noise_planet.noisecapture/sosfilter/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/org.tasks/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/org.tasks/app/
+-rw-r--r--   0 hans      (1000) hans      (1000)     8530 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/org.tasks/app/build.gradle.kts
+-rw-r--r--   0 hans      (1000) hans      (1000)      232 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/org.tasks/build.gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)      826 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/org.tasks/build.gradle.kts
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/org.tasks/buildSrc/
+-rw-r--r--   0 hans      (1000) hans      (1000)       60 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/org.tasks/buildSrc/build.gradle.kts
+-rw-r--r--   0 hans      (1000) hans      (1000)       16 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/org.tasks/settings.gradle.kts
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/osmandapp/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/osmandapp/osmand/
+-rw-r--r--   0 hans      (1000) hans      (1000)     8372 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/osmandapp/osmand/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/osmandapp/osmand/gradle/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/osmandapp/osmand/gradle/wrapper/
+-rw-r--r--   0 hans      (1000) hans      (1000)      233 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/osmandapp/osmand/gradle/wrapper/gradle-wrapper.properties
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/realm/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/realm/react-native/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/realm/react-native/android/
+-rw-r--r--   0 hans      (1000) hans      (1000)    13331 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/realm/react-native/android/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/se.manyver/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/se.manyver/android/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/se.manyver/android/app/
+-rw-r--r--   0 hans      (1000) hans      (1000)    10781 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/se.manyver/android/app/build.gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)     2006 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/se.manyver/android/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/se.manyver/android/gradle/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/se.manyver/android/gradle/wrapper/
+-rw-r--r--   0 hans      (1000) hans      (1000)      199 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/se.manyver/android/gradle/wrapper/gradle-wrapper.properties
+-rw-r--r--   0 hans      (1000) hans      (1000)      938 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/se.manyver/android/gradle.properties
+-rw-r--r--   0 hans      (1000) hans      (1000)     3487 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/se.manyver/android/settings.gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)       56 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/se.manyver/app.json
+-rw-r--r--   0 hans      (1000) hans      (1000)      571 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/se.manyver/index.android.js
+-rw-r--r--   0 hans      (1000) hans      (1000)     5237 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/se.manyver/package.json
+-rw-r--r--   0 hans      (1000) hans      (1000)      531 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/se.manyver/react-native.config.js
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/ut.ewh.audiometrytest/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/ut.ewh.audiometrytest/app/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1127 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/ut.ewh.audiometrytest/app/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/ut.ewh.audiometrytest/app/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/ut.ewh.audiometrytest/app/src/main/
+-rw-r--r--   0 hans      (1000) hans      (1000)     5729 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/ut.ewh.audiometrytest/app/src/main/AndroidManifest.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)      548 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/ut.ewh.audiometrytest/build.gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)       15 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/ut.ewh.audiometrytest/settings.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/yuriykulikov/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/yuriykulikov/AlarmClock/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/source-files/yuriykulikov/AlarmClock/gradle/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/source-files/yuriykulikov/AlarmClock/gradle/wrapper/
+-rw-r--r--   0 hans      (1000) hans      (1000)      238 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/source-files/yuriykulikov/AlarmClock/gradle/wrapper/gradle-wrapper.properties
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/stats/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1138 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/stats/known_apks.txt
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     2067 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/test-gradlew-fdroid
+-rw-r--r--   0 hans      (1000) hans      (1000)     2611 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/testcommon.py
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-2/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/triple-t-2/build/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/
+-rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/.gitignore
+-rw-r--r--   0 hans      (1000) hans      (1000)     5496 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/build.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/debug/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/debug/res/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/debug/res/values/
+-rw-r--r--   0 hans      (1000) hans      (1000)      114 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/debug/res/values/constants.xml
+-rw-r--r--   0 hans      (1000) hans      (1000)       96 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/debug/res/values/strings.xml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/java/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/java/org/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/java/org/piwigo/
+-rw-r--r--   0 hans      (1000) hans      (1000)     4061 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/java/org/piwigo/PiwigoApplication.java
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/
+-rw-r--r--   0 hans      (1000) hans      (1000)       19 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/contact-email.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       23 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/contact-website.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        6 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/default-language.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/de-DE/
+-rw-r--r--   0 hans      (1000) hans      (1000)      518 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/de-DE/full-description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       58 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/de-DE/short-description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/de-DE/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)      478 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/full-description.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.880381 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/feature-graphic/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1221 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/feature-graphic/piwigo-full.png
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/icon/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1110 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/icon/piwigo-icon.png
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/
+-rw-r--r--   0 hans      (1000) hans      (1000)      964 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/01_Login.jpg
+-rw-r--r--   0 hans      (1000) hans      (1000)     1108 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/02_Albums.jpg
+-rw-r--r--   0 hans      (1000) hans      (1000)     1131 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/03_Photos.jpg
+-rw-r--r--   0 hans      (1000) hans      (1000)     1052 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/04_Albums_horizontal.jpg
+-rw-r--r--   0 hans      (1000) hans      (1000)      985 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/05_Menu.jpg
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/tablet-screenshots/
+-rw-r--r--   0 hans      (1000) hans      (1000)      748 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/tablet-screenshots/01_Login.png
+-rw-r--r--   0 hans      (1000) hans      (1000)       44 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/short-description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/fr-FR/
+-rw-r--r--   0 hans      (1000) hans      (1000)      646 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/fr-FR/full-description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       57 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/fr-FR/short-description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/fr-FR/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/kn-IN/
+-rw-r--r--   0 hans      (1000) hans      (1000)      478 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/kn-IN/full-description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       44 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/kn-IN/short-description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/kn-IN/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/de-DE/
+-rw-r--r--   0 hans      (1000) hans      (1000)      475 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/de-DE/default.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)      482 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/en-US/default.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/fr-FR/
+-rw-r--r--   0 hans      (1000) hans      (1000)      495 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/fr-FR/default.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/kn-IN/
+-rw-r--r--   0 hans      (1000) hans      (1000)      482 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/release-notes/kn-IN/default.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)      422 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/build.gradle
+-rw-r--r--   0 hans      (1000) hans      (1000)       51 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/settings.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-2/metadata/
+-rw-r--r--   0 hans      (1000) hans      (1000)      673 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-2/metadata/org.piwigo.android.yml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/src/main/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/src/main/play/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/src/main/play/listings/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/src/main/play/listings/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)       26 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/addons/languages/dutch/apk/src/main/play/listings/en-US/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/src/main/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/src/main/play/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/src/main/play/listings/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/src/main/play/listings/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)       16 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/ime/app/src/main/play/listings/en-US/title.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     4549 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/settings.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/src/main/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/src/main/play/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/src/main/play/listings/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/src/main/play/listings/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)       26 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/addons/languages/dutch/apk/src/main/play/listings/en-US/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/src/main/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/src/main/play/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/src/main/play/listings/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/src/main/play/listings/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)       16 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/ime/app/src/main/play/listings/en-US/title.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)     4549 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/settings.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/metadata/
+-rw-r--r--   0 hans      (1000) hans      (1000)     2907 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/metadata/com.anysoftkeyboard.languagepack.dutch.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)    15227 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/metadata/com.menny.android.anysoftkeyboard.yml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-flutter/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-flutter/build/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-flutter/build/fr.emersion.goguma/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-flutter/build/fr.emersion.goguma/android/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/
+-rw-r--r--   0 hans      (1000) hans      (1000)       20 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/contact-website.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/listings/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/listings/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)      577 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/listings/en-US/full-description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)       33 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/listings/en-US/short-description.txt
+-rw-r--r--   0 hans      (1000) hans      (1000)        7 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/listings/en-US/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-flutter/metadata/
+-rw-r--r--   0 hans      (1000) hans      (1000)      868 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-flutter/metadata/fr.emersion.goguma.yml
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/
+-rw-r--r--   0 hans      (1000) hans      (1000)       56 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/settings.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/src/main/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/src/main/play/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/src/main/play/listings/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/src/main/play/listings/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)       23 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/verifier/src/main/play/listings/en-US/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/src/main/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/src/main/play/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/src/main/play/listings/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/src/main/play/listings/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)       17 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.verifier/wallet/src/main/play/listings/en-US/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/
+-rw-r--r--   0 hans      (1000) hans      (1000)       56 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/settings.gradle
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/src/main/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/src/main/play/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/src/main/play/listings/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/src/main/play/listings/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)       23 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/verifier/src/main/play/listings/en-US/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/src/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/src/main/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/src/main/play/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.884381 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/src/main/play/listings/
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/src/main/play/listings/en-US/
+-rw-r--r--   0 hans      (1000) hans      (1000)       17 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-multiple/build/ch.admin.bag.covidcertificate.wallet/wallet/src/main/play/listings/en-US/title.txt
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/triple-t-multiple/metadata/
+-rw-r--r--   0 hans      (1000) hans      (1000)     1761 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-multiple/metadata/ch.admin.bag.covidcertificate.verifier.yml
+-rw-r--r--   0 hans      (1000) hans      (1000)     1741 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/triple-t-multiple/metadata/ch.admin.bag.covidcertificate.wallet.yml
+-rwxr-xr-x   0 hans      (1000) hans      (1000)   102214 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/update.TestCase
+-rw-r--r--   0 hans      (1000) hans      (1000)     9925 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/urzip-badcert.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)     9923 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/urzip-badsig.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)     8471 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/urzip-release-unsigned.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    11406 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/urzip-release.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)     9969 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/urzip.apk
+-rw-r--r--   0 hans      (1000) hans      (1000)    12086 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/v2.only.sig_2.apk
+drwxr-xr-x   0 hans      (1000) hans      (1000)        0 2024-05-13 08:46:29.932383 fdroidserver-2.3a1/tests/valid-package-names/
+-rw-r--r--   0 hans      (1000) hans      (1000)     8815 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/valid-package-names/RandomPackageNames.java
+-rwxr-xr-x   0 hans      (1000) hans      (1000)      196 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/valid-package-names/random-package-names
+-rwxr-xr-x   0 hans      (1000) hans      (1000)      885 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/valid-package-names/test.py
+-rwxr-xr-x   0 hans      (1000) hans      (1000)     3413 2024-05-13 08:43:01.000000 fdroidserver-2.3a1/tests/vcs.TestCase
```

### Comparing `fdroidserver-2.3a0/CHANGELOG.md` & `fdroidserver-2.3a1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 ### Fixed
 
 ### Removed
 
 * The `maven:` field is now always a string, with `yes` as a legacy special
   value.  It is no longer treated like a boolean in any case.
 
+## [2.2.2] - 2024-04-24
+
+### Added
+
+* Include sdkmanager as dep in setup.py for Homebrew package.
+  https://github.com/Homebrew/homebrew-core/pull/164510
+
 ## [2.2.1] - 2023-03-09
 
 ### Added
 
 * `download_repo_index_v2()` and `download_repo_index_v2()` API functions
   https://gitlab.com/fdroid/fdroidserver/-/merge_requests/1323
```

### Comparing `fdroidserver-2.3a0/LICENSE` & `fdroidserver-2.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/MANIFEST.in` & `fdroidserver-2.3a1/MANIFEST.in`

 * *Files 1% similar despite different names*

```diff
@@ -587,14 +587,19 @@
 include tests/gradle-maven-blocks.yaml
 include tests/gradle-release-checksums.py
 include tests/import_subcommand.TestCase
 include tests/index.TestCase
 include tests/init.TestCase
 include tests/install.TestCase
 include tests/IsMD5Disabled.java
+include tests/issue-1128-min-sdk-30-poc.apk
+include tests/issue-1128-poc1.apk
+include tests/issue-1128-poc2.apk
+include tests/issue-1128-poc3a.apk
+include tests/issue-1128-poc3b.apk
 include tests/janus.apk
 include tests/keystore.jks
 include tests/key-tricks.py
 include tests/lint.TestCase
 include tests/main.TestCase
 include tests/metadata/apk/info.guardianproject.urzip.yaml
 include tests/metadata/apk/org.dyndns.fules.ck.yaml
@@ -719,14 +724,16 @@
 include tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot8.png
 include tests/repo/patch.1619.obb.mainpatch.current.obb
 include tests/repo/souch.smsbypass_9.apk
 include tests/repo/urzip-*.apk
 include tests/repo/v1.v2.sig_1020.apk
 include tests/rewritemeta.TestCase
 include tests/run-tests
+include tests/SANAPPSI.RSA
+include tests/SANAPPSI.SF
 include tests/scanner.TestCase
 include tests/signatures.TestCase
 include tests/signindex.TestCase
 include tests/signindex/guardianproject.jar
 include tests/signindex/guardianproject-v1.jar
 include tests/signindex/testy.jar
 include tests/signindex/unsigned.jar
```

### Comparing `fdroidserver-2.3a0/PKG-INFO` & `fdroidserver-2.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdroidserver
-Version: 2.3a0
+Version: 2.3a1
 Summary: F-Droid Server Tools
 Home-page: https://f-droid.org
 Author: The F-Droid Project
 Author-email: team@f-droid.org
 License: AGPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `fdroidserver-2.3a0/README.md` & `fdroidserver-2.3a1/README.md`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/buildserver/Vagrantfile` & `fdroidserver-2.3a1/buildserver/Vagrantfile`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/buildserver/provision-android-ndk` & `fdroidserver-2.3a1/buildserver/provision-android-ndk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/buildserver/provision-android-sdk` & `fdroidserver-2.3a1/buildserver/provision-android-sdk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/buildserver/provision-apt-get-install` & `fdroidserver-2.3a1/buildserver/provision-apt-get-install`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/buildserver/provision-gradle` & `fdroidserver-2.3a1/buildserver/provision-gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/buildserver/setup-env-vars` & `fdroidserver-2.3a1/buildserver/setup-env-vars`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/completion/bash-completion` & `fdroidserver-2.3a1/completion/bash-completion`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/examples/Vagrantfile.yaml` & `fdroidserver-2.3a1/examples/Vagrantfile.yaml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/examples/config.yml` & `fdroidserver-2.3a1/examples/config.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/examples/fdroid_export_keystore_to_nitrokey.py` & `fdroidserver-2.3a1/examples/fdroid_export_keystore_to_nitrokey.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         raise BuildException(error, p.output)
 
 
 def main():
     global config
     parser = ArgumentParser()
     common.setup_global_opts(parser)
-    options = parser.parse_args()
-    config = common.read_config(options)
+    common.parse_args(parser)
+    config = common.read_config()
     destkeystore = config['keystore'].replace('.jks', '.p12').replace('/', '_')
     exportkeystore = config['keystore'].replace('.jks', '.pem').replace('/', '_')
     if os.path.exists(destkeystore) or os.path.exists(exportkeystore):
         raise BuildException('%s exists!' % exportkeystore)
     run([config['keytool'], '-importkeystore',
          '-srckeystore', config['keystore'],
          '-srcalias', config['repo_keyalias'],
```

### Comparing `fdroidserver-2.3a0/examples/fdroid_exportkeystore.py` & `fdroidserver-2.3a1/examples/fdroid_exportkeystore.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 fdroid_summary = 'export the keystore in standard PEM format'
 
 
 def main():
     parser = ArgumentParser()
     common.setup_global_opts(parser)
-    options = parser.parse_args()
-    config = common.read_config(options)
+    common.parse_args(parser)
+    config = common.read_config()
     env_vars = {'LC_ALL': 'C.UTF-8',
                 'FDROID_KEY_STORE_PASS': config['keystorepass'],
                 'FDROID_KEY_PASS': config['keypass']}
     destkeystore = config['keystore'].replace('.jks', '.p12').replace('/', '_')
     exportkeystore = config['keystore'].replace('.jks', '.pem').replace('/', '_')
     if os.path.exists(destkeystore) or os.path.exists(exportkeystore):
         raise BuildException('%s exists!' % exportkeystore)
```

### Comparing `fdroidserver-2.3a0/examples/fdroid_extract_repo_pubkey.py` & `fdroidserver-2.3a1/examples/fdroid_extract_repo_pubkey.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 fdroid_summary = 'export the keystore in standard PEM format'
 
 
 def main():
     parser = ArgumentParser()
     common.setup_global_opts(parser)
-    options = parser.parse_args()
-    common.config = common.read_config(options)
+    common.parse_args(parser)
+    common.read_config()
     pubkey, repo_pubkey_fingerprint = index.extract_pubkey()
     print('repo_pubkey = "%s"' % pubkey.decode())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fdroidserver-2.3a0/examples/fdroid_fetchsrclibs.py` & `fdroidserver-2.3a1/examples/fdroid_fetchsrclibs.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,19 @@
 
 
 def main():
     parser = argparse.ArgumentParser(usage="%(prog)s [options] [APPID[:VERCODE] [APPID[:VERCODE] ...]]")
     common.setup_global_opts(parser)
     parser.add_argument("appid", nargs='*', help=_("applicationId with optional versionCode in the form APPID[:VERCODE]"))
     metadata.add_metadata_arguments(parser)
-    options = parser.parse_args()
-    common.options = options
+    options = common.parse_args(parser)
     pkgs = common.read_pkg_args(options.appid, True)
     allapps = metadata.read_metadata(pkgs)
     apps = common.read_app_args(options.appid, allapps, True)
-    common.read_config(options)
+    common.read_config()
     srclib_dir = os.path.join('build', 'srclib')
     os.makedirs(srclib_dir, exist_ok=True)
     srclibpaths = []
     for appid, app in apps.items():
         vcs, _ignored = common.setup_vcs(app)
         for build in app.get('Builds', []):
             vcs.gotorevision(build.commit, refresh=False)
```

### Comparing `fdroidserver-2.3a0/examples/fdroid_nitrokeyimport.py` & `fdroidserver-2.3a1/examples/fdroid_nitrokeyimport.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 fdroid_summary = 'import the local keystore into a SmartCard HSM'
 
 
 def main():
     parser = ArgumentParser()
     common.setup_global_opts(parser)
-    options = parser.parse_args()
-    config = common.read_config(options)
+    common.parse_args(parser)
+    config = common.read_config()
     env_vars = {
         'LC_ALL': 'C.UTF-8',
         'FDROID_KEY_STORE_PASS': config['keystorepass'],
         'FDROID_KEY_PASS': config['keypass'],
         'SMARTCARD_PIN': str(config['smartcard_pin']),
     }
     p = FDroidPopen([config['keytool'], '-importkeystore',
```

### Comparing `fdroidserver-2.3a0/fdroidserver/__init__.py` & `fdroidserver-2.3a1/fdroidserver/__init__.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/fdroidserver/__main__.py` & `fdroidserver-2.3a1/fdroidserver/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
     logging.basicConfig(format=logformat, level=loglevel)
 
     if verbose and quiet:
         logging.critical(_("Conflicting arguments: '--verbose' and '--quiet' "
                            "can not be specified at the same time."))
         sys.exit(1)
 
-    # Trick optparse into displaying the right usage when --help is used.
+    # Trick argparse into displaying the right usage when --help is used.
     sys.argv[0] += ' ' + command
 
     del sys.argv[1]
     if command in COMMANDS.keys():
         # import is named import_subcommand internally b/c import is reserved by Python
         command = 'import_subcommand' if command == 'import' else command
         mod = __import__('fdroidserver.' + command, None, None, [command])
```

### Comparing `fdroidserver-2.3a0/fdroidserver/apksigcopier.py` & `fdroidserver-2.3a1/fdroidserver/apksigcopier.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/fdroidserver/asynchronousfilereader/__init__.py` & `fdroidserver-2.3a1/fdroidserver/asynchronousfilereader/__init__.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/fdroidserver/btlog.py` & `fdroidserver-2.3a1/fdroidserver/btlog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+"""Update the binary transparency log for a URL."""
 #
 # btlog.py - part of the FDroid server tools
 # Copyright (C) 2017, Hans-Christoph Steiner <hans@eds.org>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -22,46 +23,59 @@
 # HTTP ETag to check if the file has changed.  HEAD requests should
 # not count against the download counts.  This pattern of a HEAD then
 # a GET is what fdroidclient uses to avoid ETags being abused as
 # cookies. This also uses the same HTTP User Agent as the F-Droid
 # client app so its not easy for the server to distinguish this from
 # the F-Droid client.
 
-
 import collections
 import defusedxml.minidom
 import git
 import glob
 import os
 import json
 import logging
 import requests
 import shutil
 import tempfile
 import zipfile
 from argparse import ArgumentParser
+from typing import Optional
 
 from . import _
 from . import common
 from . import deploy
 from .exception import FDroidException
 
 
-options = None
-
-
 def make_binary_transparency_log(
-    repodirs, btrepo='binary_transparency', url=None, commit_title='fdroid update'
+    repodirs: collections.abc.Iterable,
+    btrepo: str = 'binary_transparency',
+    url: Optional[str] = None,
+    commit_title: str = 'fdroid update',
 ):
     """Log the indexes in a standalone git repo to serve as a "binary transparency" log.
 
-    References
+    Parameters
     ----------
-    https://www.eff.org/deeplinks/2014/02/open-letter-to-tech-companies
-
+    repodirs
+        The directories of the F-Droid repository to generate the binary
+        transparency log for.
+    btrepo
+        The path to the Git repository of the binary transparency log.
+    url
+        The URL of the F-Droid repository to generate the binary transparency
+        log for.
+    commit_title
+        The commit title for commits in the binary transparency log Git
+        repository.
+
+    Notes
+    -----
+    Also see https://www.eff.org/deeplinks/2014/02/open-letter-to-tech-companies .
     """
     logging.info('Committing indexes to ' + btrepo)
     if os.path.exists(os.path.join(btrepo, '.git')):
         gitrepo = git.Repo(btrepo)
     else:
         if not os.path.exists(btrepo):
             os.mkdir(btrepo)
@@ -145,16 +159,25 @@
         for f in glob.glob(os.path.join(cpdir, '*.HTTP-headers.json')):
             gitrepo.index.add([os.path.join(repodir, os.path.basename(f))])
 
     gitrepo.index.commit(commit_title)
 
 
 def main():
-    global options
+    """Generate or update a binary transparency log for a F-Droid repository.
 
+    The behaviour of this function is influenced by the configuration file as
+    well as command line parameters.
+
+    Raises
+    ------
+    :exc:`~fdroidserver.exception.FDroidException`
+        If the specified or default Git repository does not exist.
+
+    """
     parser = ArgumentParser()
     common.setup_global_opts(parser)
     parser.add_argument(
         "--git-repo",
         default=os.path.join(os.getcwd(), 'binary_transparency'),
         help=_("Path to the git repo to use as the log"),
     )
@@ -165,15 +188,15 @@
         help=_("The base URL for the repo to log (default: https://f-droid.org)"),
     )
     parser.add_argument(
         "--git-remote",
         default=None,
         help=_("Push the log to this git remote repository"),
     )
-    options = parser.parse_args()
+    options = common.parse_args(parser)
 
     if options.verbose:
         logging.getLogger("requests").setLevel(logging.INFO)
         logging.getLogger("urllib3").setLevel(logging.INFO)
     else:
         logging.getLogger("requests").setLevel(logging.WARNING)
         logging.getLogger("urllib3").setLevel(logging.WARNING)
```

### Comparing `fdroidserver-2.3a0/fdroidserver/build.py` & `fdroidserver-2.3a1/fdroidserver/build.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+"""Build a package from source."""
 #
 # build.py - part of the FDroid server tools
 # Copyright (C) 2010-2014, Ciaran Gultnieks, ciaran@ciarang.com
 # Copyright (C) 2013-2014 Daniel Martí <mvdan@mvdan.cc>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
@@ -55,23 +56,38 @@
 # Note that 'force' here also implies test mode.
 def build_server(app, build, vcs, build_dir, output_dir, log_dir, force):
     """Do a build on the builder vm.
 
     Parameters
     ----------
     app
-        app metadata dict
+        The metadata of the app to build.
     build
+        The build of the app to build.
     vcs
-        version control system controller object
+        The version control system controller object of the app.
     build_dir
-        local source-code checkout of app
+        The local source-code checkout directory of the app.
     output_dir
-        target folder for the build result
+        The target folder for the build result.
+    log_dir
+        The directory in the VM where the build logs are getting stored.
     force
+        Don't refresh the already cloned repository and make the build stop on
+        exceptions.
+
+    Raises
+    ------
+    :exc:`~fdroidserver.exception.BuildException`
+        If Paramiko is not installed, a srclib directory or srclib metadata
+        file is unexpectedly missing, the build process in the VM failed or
+        output files of the build process are missing.
+    :exc:`~fdroidserver.exception.FDroidException`
+        If the Buildserver ID could not be obtained or copying a directory to
+        the server failed.
     """
     global buildserverid, ssh_channel
 
     try:
         paramiko
     except NameError as e:
         raise BuildException("Paramiko is required to use the buildserver") from e
@@ -111,16 +127,16 @@
         # Get an SFTP connection...
         ftp = sshs.open_sftp()
         ftp.get_channel().settimeout(60)
 
         # Put all the necessary files in place...
         ftp.chdir(homedir)
 
-        # Helper to copy the contents of a directory to the server...
         def send_dir(path):
+            """Copy the contents of a directory to the server."""
             logging.debug("rsyncing %s to %s" % (path, ftp.getcwd()))
             # TODO this should move to `vagrant rsync` from >= v1.5
             try:
                 subprocess.check_output(['rsync', '--recursive', '--perms', '--links', '--quiet', '--rsh='
                                          + 'ssh -o StrictHostKeyChecking=no'
                                          + ' -o UserKnownHostsFile=/dev/null'
                                          + ' -o LogLevel=FATAL'
@@ -312,14 +328,23 @@
             common.deploy_build_log_with_rsync(app.id, build.versionCode, output)
         else:
             logging.debug('skip publishing full build logs: '
                           'no output present')
 
 
 def force_gradle_build_tools(build_dir, build_tools):
+    """Manipulate build tools version used in top level gradle file.
+
+    Parameters
+    ----------
+    build_dir
+        The directory to start looking for gradle files.
+    build_tools
+        The build tools version that should be forced to use.
+    """
     for root, dirs, files in os.walk(build_dir):
         for filename in files:
             if not filename.endswith('.gradle'):
                 continue
             path = os.path.join(root, filename)
             if not os.path.isfile(path):
                 continue
@@ -338,14 +363,39 @@
     return method(string[0]) + string[1:]
 
 
 def get_metadata_from_apk(app, build, apkfile):
     """Get the required metadata from the built APK.
 
     VersionName is allowed to be a blank string, i.e. ''
+
+    Parameters
+    ----------
+    app
+        The app metadata used to build the APK.
+    build
+        The build that resulted in the APK.
+    apkfile
+        The path of the APK file.
+
+    Returns
+    -------
+    versionCode
+        The versionCode from the APK or from the metadata is build.novcheck is
+        set.
+    versionName
+        The versionName from the APK or from the metadata is build.novcheck is
+        set.
+
+    Raises
+    ------
+    :exc:`~fdroidserver.exception.BuildException`
+        If native code should have been built but was not packaged, no version
+        information or no package ID could be found or there is a mismatch
+        between the package ID in the metadata and the one found in the APK.
     """
     appid, versionCode, versionName = common.get_apk_id(apkfile)
     native_code = common.get_native_code(apkfile)
 
     if build.buildjni and build.buildjni != ['no'] and not native_code:
         raise BuildException("Native code should have been built but none was packaged")
     if build.novcheck:
@@ -358,15 +408,64 @@
     if appid != app.id:
         raise BuildException("Wrong package ID - build " + appid + " but expected " + app.id)
 
     return versionCode, versionName
 
 
 def build_local(app, build, vcs, build_dir, output_dir, log_dir, srclib_dir, extlib_dir, tmp_dir, force, onserver, refresh):
-    """Do a build locally."""
+    """Do a build locally.
+
+    Parameters
+    ----------
+    app
+        The metadata of the app to build.
+    build
+        The build of the app to build.
+    vcs
+        The version control system controller object of the app.
+    build_dir
+        The local source-code checkout directory of the app.
+    output_dir
+        The target folder for the build result.
+    log_dir
+        The directory in the VM where the build logs are getting stored.
+    srclib_dir
+        The path to the srclibs directory, usually 'build/srclib'.
+    extlib_dir
+        The path to the extlibs directory, usually 'build/extlib'.
+    tmp_dir
+        The temporary directory for building the source tarball.
+    force
+        Don't refresh the already cloned repository and make the build stop on
+        exceptions.
+    onserver
+        Assume the build is happening inside the VM.
+    refresh
+        Enable fetching the latest refs from the VCS remote.
+
+    Raises
+    ------
+    :exc:`~fdroidserver.exception.BuildException`
+        If running a `sudo` command failed, locking the root account failed,
+        `sudo` couldn't be removed, cleaning the build environment failed,
+        skipping the scanning has been requested but `scandelete` is present,
+        errors occurred during scanning, running the `build` commands from the
+        metadata failed, building native code failed, building with the
+        specified build method failed, no output could be found with build
+        method `maven`, more or less than one APK were found with build method
+        `gradle`, less or more than one APKs match the `output` glob specified
+        in the metadata, running a `postbuild` command specified in the
+        metadata failed, the built APK is debuggable, the unsigned APK is not
+        at the expected location, the APK does not contain the expected
+        `versionName` and `versionCode` or undesired package names have been
+        found in the APK.
+    :exc:`~fdroidserver.exception.FDroidException`
+        If no Android NDK version could be found and the build isn't run in a
+        builder VM, the selected Android NDK is not a directory.
+    """
     ndk_path = build.ndk_path()
     if build.ndk or (build.buildjni and build.buildjni != ['no']):
         if not ndk_path:
             logging.warning("Android NDK version '%s' could not be found!" % build.ndk)
             logging.warning("Configured versions:")
             for k, v in config['ndk_paths'].items():
                 if k.endswith("_orig"):
@@ -762,31 +861,55 @@
 def trybuild(app, build, build_dir, output_dir, log_dir, also_check_dir,
              srclib_dir, extlib_dir, tmp_dir, repo_dir, vcs, test,
              server, force, onserver, refresh):
     """Build a particular version of an application, if it needs building.
 
     Parameters
     ----------
+    app
+        The metadata of the app to build.
+    build
+        The build of the app to build.
+    build_dir
+        The local source-code checkout directory of the app.
     output_dir
-        The directory where the build output will go.
-        Usually this is the 'unsigned' directory.
+        The directory where the build output will go.  Usually this is the
+        'unsigned' directory.
+    log_dir
+        The directory in the VM where the build logs are getting stored.
+    also_check_dir
+        An additional location for checking if the build is necessary (usually
+        the archive repo).
+    srclib_dir
+        The path to the srclibs directory, usually 'build/srclib'.
+    extlib_dir
+        The path to the extlibs directory, usually 'build/extlib'.
+    tmp_dir
+        The temporary directory for building the source tarball of the app to
+        build.
     repo_dir
         The repo directory - used for checking if the build is necessary.
-    also_check_dir
-        An additional location for checking if the build
-        is necessary (usually the archive repo)
+    vcs
+        The version control system controller object of the app to build.
     test
-        True if building in test mode, in which case the build will
-        always happen, even if the output already exists. In test mode, the
-        output directory should be a temporary location, not any of the real
-        ones.
+        True if building in test mode, in which case the build will always
+        happen, even if the output already exists.  In test mode, the output
+        directory should be a temporary location, not any of the real ones.
+    server
+        Use buildserver VM for building.
+    force
+        Build app regardless of disabled state or scanner errors.
+    onserver
+        Assume the build is happening inside the VM.
+    refresh
+        Enable fetching the latest refs from the VCS remote.
 
     Returns
     -------
-    Boolean
+    status
         True if the build was done, False if it wasn't necessary.
     """
     dest_file = common.get_release_filename(app, build)
 
     dest = os.path.join(output_dir, dest_file)
     dest_repo = os.path.join(repo_dir, dest_file)
 
@@ -817,15 +940,21 @@
         build_server(app, build, vcs, build_dir, output_dir, log_dir, force)
     else:
         build_local(app, build, vcs, build_dir, output_dir, log_dir, srclib_dir, extlib_dir, tmp_dir, force, onserver, refresh)
     return True
 
 
 def force_halt_build(timeout):
-    """Halt the currently running Vagrant VM, to be called from a Timer."""
+    """Halt the currently running Vagrant VM, to be called from a Timer.
+
+    Parameters
+    ----------
+    timeout
+        The timeout in seconds.
+    """
     logging.error(_('Force halting build after {0} sec timeout!').format(timeout))
     timeout_event.set()
     if ssh_channel:
         ssh_channel.close()
     vm = vmtools.get_build_vm('builder')
     vm.destroy()
 
@@ -841,15 +970,17 @@
 
 def parse_commandline():
     """Parse the command line.
 
     Returns
     -------
     options
+        The resulting options parsed from the command line arguments.
     parser
+        The argument parser.
     """
     parser = argparse.ArgumentParser(usage="%(prog)s [options] [APPID[:VERCODE] [APPID[:VERCODE] ...]]")
     common.setup_global_opts(parser)
     parser.add_argument("appid", nargs='*', help=_("application ID with optional versionCode in the form APPID[:VERCODE]"))
     parser.add_argument("-l", "--latest", action="store_true", default=False,
                         help=_("Build only the latest version of each package"))
     parser.add_argument("-s", "--stop", action="store_true", default=False,
@@ -879,15 +1010,15 @@
     parser.add_argument("-a", "--all", action="store_true", default=False,
                         help=_("Build all applications available"))
     parser.add_argument("--keep-when-not-allowed", default=False, action="store_true",
                         help=argparse.SUPPRESS)
     parser.add_argument("-w", "--wiki", default=False, action="store_true",
                         help=argparse.SUPPRESS)
     metadata.add_metadata_arguments(parser)
-    options = parser.parse_args()
+    options = common.parse_args(parser)
     metadata.warnings_action = options.W
 
     # Force --stop with --on-server to get correct exit code
     if options.onserver:
         options.stop = True
 
     if options.force and not options.test:
@@ -901,14 +1032,30 @@
 fdroidserverid = None
 start_timestamp = time.gmtime()
 status_output = None
 timeout_event = threading.Event()
 
 
 def main():
+    """Build a package from source.
+
+    The behaviour of this function is influenced by the configuration file as
+    well as command line parameters.
+
+    Raises
+    ------
+    :exc:`~fdroidserver.exception.FDroidException`
+        If more than one local metadata file has been found, no app metadata
+        has been found, there are no apps to process, downloading binaries for
+        checking the reproducibility of a built binary failed, the built binary
+        is different from supplied reference binary, the reference binary is
+        signed with a different signing key than expected, a VCS error occured
+        while building an app or a different error occured while building an
+        app.
+    """
     global options, config, buildserverid, fdroidserverid
 
     options, parser = parse_commandline()
 
     # The defaults for .fdroid.* metadata that is included in a git repo are
     # different than for the standard metadata/ layout because expectations
     # are different.  In this case, the most common user will be the app
@@ -925,15 +1072,15 @@
                               + " ".join(local_metadata_files))
     else:
         if not os.path.isdir('metadata') and len(local_metadata_files) == 0:
             raise FDroidException("No app metadata found, nothing to process!")
         if not options.appid and not options.all:
             parser.error("option %s: If you really want to build all the apps, use --all" % "all")
 
-    config = common.read_config(opts=options)
+    config = common.read_config()
 
     if config['build_server_always']:
         options.server = True
     if options.reset_server and not options.server:
         parser.error("option %s: Using --reset-server without --server makes no sense" % "reset-server")
 
     log_dir = 'logs'
```

### Comparing `fdroidserver-2.3a0/fdroidserver/checkupdates.py` & `fdroidserver-2.3a1/fdroidserver/checkupdates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+"""Check for updates to applications."""
 #
 # checkupdates.py - part of the FDroid server tools
 # Copyright (C) 2010-2015, Ciaran Gultnieks, ciaran@ciarang.com
 # Copyright (C) 2013-2014 Daniel Martí <mvdan@mvdan.cc>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
@@ -501,15 +502,15 @@
     oldvercode = vercode
     op = operation.replace("%c", str(oldvercode))
     vercode = common.calculate_math_string(op)
     logging.debug("Applied vercode operation: %d -> %d" % (oldvercode, vercode))
     return vercode
 
 
-def checkupdates_app(app: metadata.App) -> None:
+def checkupdates_app(app: metadata.App, auto: bool, commit: bool = False) -> None:
     """Check for new versions and updated name of a single app.
 
     Also write back changes to the metadata file and create a Git commit if
     requested.
 
     Parameters
     ----------
@@ -577,15 +578,15 @@
 
     if updating:
         name = _getappname(app)
         ver = _getcvname(app)
         logging.info('...updating to version %s' % ver)
         commitmsg = 'Update CurrentVersion of %s to %s' % (name, ver)
 
-    if options.auto:
+    if auto:
         mode = app.AutoUpdateMode
         if not app.CurrentVersionCode:
             raise MetaDataException(
                 _("Can't auto-update app with no CurrentVersionCode")
             )
         elif mode in ('None', 'Static'):
             pass
@@ -660,15 +661,15 @@
         else:
             raise MetaDataException(
                 _('Invalid AutoUpdateMode: {mode}').format(mode=mode)
             )
 
     if commitmsg:
         metadata.write_metadata(app.metadatapath, app)
-        if options.commit:
+        if commit:
             logging.info("Commiting update for " + app.metadatapath)
             gitcmd = ["git", "commit", "-m", commitmsg]
             if 'auto_author' in config:
                 gitcmd.extend(['--author', config['auto_author']])
             gitcmd.extend(["--", app.metadatapath])
             if subprocess.call(gitcmd) != 0:
                 raise FDroidException("Git commit failed")
@@ -690,43 +691,42 @@
         output['processed'] = processed
     if failed:
         output['failed'] = failed
     common.write_status_json(output)
 
 
 config = None
-options = None
 start_timestamp = time.gmtime()
 
 
 def main():
     """Check for updates for one or more apps.
 
     The behaviour of this function is influenced by the configuration file as
     well as command line parameters.
     """
-    global config, options
+    global config
 
     # Parse command line...
     parser = ArgumentParser()
     common.setup_global_opts(parser)
     parser.add_argument("appid", nargs='*', help=_("application ID of file to operate on"))
     parser.add_argument("--auto", action="store_true", default=False,
                         help=_("Process auto-updates"))
     parser.add_argument("--autoonly", action="store_true", default=False,
                         help=_("Only process apps with auto-updates"))
     parser.add_argument("--commit", action="store_true", default=False,
                         help=_("Commit changes"))
     parser.add_argument("--allow-dirty", action="store_true", default=False,
                         help=_("Run on git repo that has uncommitted changes"))
     metadata.add_metadata_arguments(parser)
-    options = parser.parse_args()
+    options = common.parse_args(parser)
     metadata.warnings_action = options.W
 
-    config = common.read_config(options)
+    config = common.read_config()
 
     if not options.allow_dirty:
         status = subprocess.check_output(['git', 'status', '--porcelain'])
         if status:
             logging.error(_('Build metadata git repo has uncommited changes!'))
             sys.exit(1)
 
@@ -744,15 +744,15 @@
             logging.debug(_("Nothing to do for {appid}.").format(appid=appid))
             continue
 
         msg = _("Processing {appid}").format(appid=appid)
         logging.info(msg)
 
         try:
-            checkupdates_app(app)
+            checkupdates_app(app, options.auto, options.commit)
             processed.append(appid)
         except Exception as e:
             msg = _("...checkupdate failed for {appid} : {error}").format(appid=appid, error=e)
             logging.error(msg)
             logging.debug(traceback.format_exc())
             failed[appid] = str(e)
             exit_code = 1
```

### Comparing `fdroidserver-2.3a0/fdroidserver/common.py` & `fdroidserver-2.3a1/fdroidserver/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,24 +50,21 @@
 import zipfile
 import tempfile
 import json
 from pathlib import Path
 
 import defusedxml.ElementTree as XMLElementTree
 
+from asn1crypto import cms
 from base64 import urlsafe_b64encode
 from binascii import hexlify
 from datetime import datetime, timedelta, timezone
 from queue import Queue
 from zipfile import ZipFile
 
-from pyasn1.codec.der import decoder, encoder
-from pyasn1_modules import rfc2315
-from pyasn1.error import PyAsn1Error
-
 import fdroidserver.metadata
 import fdroidserver.lint
 from fdroidserver import _
 from fdroidserver.exception import FDroidException, VCSException, NoSubmodulesException, \
     BuildException, VerificationException, MetaDataException
 from .asynchronousfilereader import AsynchronousFileReader
 from .looseversion import LooseVersion
@@ -190,14 +187,42 @@
     'archive_older': 0,
     'lint_licenses': fdroidserver.lint.APPROVED_LICENSES,  # type: ignore
     'git_mirror_size_limit': 10000000000,
     'scanner_signature_sources': ['suss'],
 }
 
 
+def get_options():
+    """Return options as set up by parse_args().
+
+    This provides an easy way to get the global instance without
+    having to think about very confusing import and submodule
+    visibility.  The code should be probably refactored so it does not
+    need this.  If each individual option value was always passed to
+    functions as args, for example.
+
+    https://docs.python.org/3/reference/import.html#submodules
+
+    """
+    return fdroidserver.common.options
+
+
+def parse_args(parser):
+    """Call parser.parse_args(), store result in module-level variable and return it.
+
+    This is needed to set up the copy of the options instance in the
+    fdroidserver.common module.  A subcommand only needs to call this
+    if it uses functions from fdroidserver.common that expect the
+    "options" variable to be initialized.
+
+    """
+    fdroidserver.common.options = parser.parse_args()
+    return fdroidserver.common.options
+
+
 def setup_global_opts(parser):
     try:  # the buildserver VM might not have PIL installed
         from PIL import PngImagePlugin
         logger = logging.getLogger(PngImagePlugin.__name__)
         logger.setLevel(logging.INFO)  # tame the "STREAM" debug messages
     except ImportError:
         pass
@@ -372,28 +397,46 @@
 
     if 'cachedir_scanner' not in thisconfig:
         thisconfig['cachedir_scanner'] = str(Path(thisconfig['cachedir']) / 'scanner')
     if 'gradle_version_dir' not in thisconfig:
         thisconfig['gradle_version_dir'] = str(Path(thisconfig['cachedir']) / 'gradle')
 
 
-def get_config(opts=None):
-    """Get config instace. This function takes care of initializing config data before returning it."""
-    global config, options
+def get_config():
+    """Get the initalized, singleton config instance.
+
+    config and options are intertwined in read_config(), so they have
+    to be here too.  In the current ugly state of things, there are
+    multiple potential instances of config and options in use:
+
+    * global
+    * module-level in the subcommand module (e.g. fdroidserver/build.py)
+    * module-level in fdroidserver.common
+
+    There are some insane parts of the code that are probably
+    referring to multiple instances of these at different points.
+    This can be super confusing and maddening.
+
+    The current intermediate refactoring step is to move all
+    subcommands to always get/set config and options via this function
+    so that there is no longer a distinction between the global and
+    module-level instances.  Then there can be only one module-level
+    instance in fdroidserver.common.
+
+    """
+    global config
 
     if config is not None:
         return config
 
-    common.read_config(opts=opts)
+    read_config()
 
     # make sure these values are available in common.py even if they didn't
     # declare global in a scope
     common.config = config
-    if opts is not None:
-        common.options = opts
 
     return config
 
 
 def regsub_file(pattern, repl, path):
     with open(path, 'rb') as f:
         text = f.read()
@@ -418,15 +461,15 @@
                 path=path,
                 expected_type=expected_type.__name__,
                 datatype=type(data).__name__,
             )
         )
 
 
-def read_config(opts=None):
+def read_config():
     """Read the repository config.
 
     The config is read from config_file, which is in the current
     directory when any of the repo management commands are used. If
     there is a local metadata file in the git repo, then the config is
     not required, just use defaults.
 
@@ -437,21 +480,19 @@
     config.yml requires ASCII or UTF-8 encoding because this code does
     not auto-detect the file's encoding.  That is left up to the YAML
     library.  YAML allows ASCII, UTF-8, UTF-16, and UTF-32 encodings.
     Since it is a good idea to manage config.yml (WITHOUT PASSWORDS!)
     in git, it makes sense to use a globally standard encoding.
 
     """
-    global config, options
+    global config
 
     if config is not None:
         return config
 
-    options = opts
-
     config = {}
     config_file = 'config.yml'
     old_config_file = 'config.py'
 
     if os.path.exists(config_file) and os.path.exists(old_config_file):
         logging.error(_("""Conflicting config files! Using {newfile}, ignoring {oldfile}!""")
                       .format(oldfile=old_config_file, newfile=config_file))
@@ -476,16 +517,16 @@
                     logging.warning(
                         _("'{field}' will be in random order! Use () or [] brackets if order is important!")
                         .format(field=k))
 
     # smartcardoptions must be a list since its command line args for Popen
     smartcardoptions = config.get('smartcardoptions')
     if isinstance(smartcardoptions, str):
-        options = re.sub(r'\s+', r' ', config['smartcardoptions']).split(' ')
-        config['smartcardoptions'] = [i.strip() for i in options if i]
+        sco_items = re.sub(r'\s+', r' ', config['smartcardoptions']).split(' ')
+        config['smartcardoptions'] = [i.strip() for i in sco_items if i]
     elif not smartcardoptions and 'keystore' in config and config['keystore'] == 'NONE':
         # keystore='NONE' means use smartcard, these are required defaults
         config['smartcardoptions'] = ['-storetype', 'PKCS11', '-providerName',
                                       'SunPKCS11-OpenSC', '-providerClass',
                                       'sun.security.pkcs11.SunPKCS11',
                                       '-providerArg', 'opensc-fdroid.cfg']
 
@@ -569,15 +610,15 @@
     else:
         raise TypeError(_('only accepts strings, lists, and tuples'))
 
 
 def file_entry(filename, hash_value=None):
     meta = {}
     meta["name"] = "/" + Path(filename).as_posix().split("/", 1)[1]
-    meta["sha256"] = hash_value or common.sha256sum(filename)
+    meta["sha256"] = hash_value or sha256sum(filename)
     meta["size"] = os.stat(filename).st_size
     return meta
 
 
 def load_localized_config(name, repodir):
     """Load localized config files and put them into internal dict format.
 
@@ -2350,14 +2391,16 @@
             n = build.target.split('-')[1]
             build_gradle = os.path.join(root_dir, "build.gradle")
             build_gradle_kts = build_gradle + ".kts"
             if os.path.exists(build_gradle):
                 gradlefile = build_gradle
             elif os.path.exists(build_gradle_kts):
                 gradlefile = build_gradle_kts
+            else:
+                raise BuildException("No gradle file found")
             regsub_file(r'compileSdkVersion[ =]+[0-9]+',
                         r'compileSdkVersion %s' % n,
                         gradlefile)
 
     # Remove forced debuggable flags
     remove_debuggable_flags(root_dir)
 
@@ -2625,39 +2668,56 @@
 def get_file_extension(filename):
     """Get the normalized file extension, can be blank string but never None."""
     if isinstance(filename, bytes):
         filename = filename.decode('utf-8')
     return os.path.splitext(filename)[1].lower()[1:]
 
 
-def use_androguard():
-    """Report if androguard is available, and config its debug logging."""
-    try:
-        import androguard
-        if use_androguard.show_path:
-            logging.debug(_('Using androguard from "{path}"').format(path=androguard.__file__))
-            use_androguard.show_path = False
-        if options and options.verbose:
-            logging.getLogger("androguard.axml").setLevel(logging.INFO)
-        logging.getLogger("androguard.core.api_specific_resources").setLevel(logging.ERROR)
-        return True
-    except ImportError:
-        return False
+def _androguard_logging_level(level=logging.ERROR):
+    """Tames androguard's default debug output.
 
+    There should be no debug output when the functions are being used
+    via the API.  Otherwise, the output is controlled by the --verbose
+    flag.
+
+    To get coverage across the full range of androguard >= 3.3.5, this
+    includes all known logger names that are relevant.  So some of
+    these names might not be present in the version of androguard
+    currently in use.
+
+    """
+    if options and options.verbose:
+        level = logging.WARNING
+
+    for name in (
+        'androguard.apk',
+        'androguard.axml',
+        'androguard.core.api_specific_resources',
+        'androguard.core.apk',
+        'androguard.core.axml',
+    ):
+        logging.getLogger(name).setLevel(level)
 
-use_androguard.show_path = True  # type: ignore
+    # some parts of androguard 4.x use loguru instead of logging
+    try:
+        from loguru import logger
+        logger.remove()
+    except ImportError:
+        pass
 
 
-def _get_androguard_APK(apkfile):
+def get_androguard_APK(apkfile, skip_analysis=False):
     try:
+        # these were moved in androguard 4.0
+        from androguard.core.apk import APK
+    except ImportError:
         from androguard.core.bytecodes.apk import APK
-    except ImportError as exc:
-        raise FDroidException("androguard library is not installed") from exc
+    _androguard_logging_level()
 
-    return APK(apkfile)
+    return APK(apkfile, skip_analysis=skip_analysis)
 
 
 def ensure_final_value(packageName, arsc, value):
     """Ensure incoming value is always the value, not the resid.
 
     androguard will sometimes return the Android "resId" aka
     Resource ID instead of the actual value.  This checks whether
@@ -2689,15 +2749,21 @@
     ----------
     apkfile
         full path to the APK to check
 
     """
     if get_file_extension(apkfile) != 'apk':
         return False
-    from androguard.core.bytecodes.axml import AXMLParser, format_value, START_TAG
+    try:
+        # these were moved in androguard 4.0
+        from androguard.core.axml import AXMLParser, format_value, START_TAG
+    except ImportError:
+        from androguard.core.bytecodes.axml import AXMLParser, format_value, START_TAG
+    _androguard_logging_level()
+
     with ZipFile(apkfile) as apk:
         with apk.open('AndroidManifest.xml') as manifest:
             axml = AXMLParser(manifest.read())
             while axml.is_valid():
                 _type = next(axml)
                 if _type == START_TAG and axml.getName() == 'application':
                     for i in range(0, axml.getAttributeCount()):
@@ -2749,20 +2815,28 @@
 
     This first tries to do quick binary XML parsing to just get the
     values that are needed.  It will fallback to full androguard
     parsing, which is slow, if it can't find the versionName value or
     versionName is set to a Android String Resource (e.g. an integer
     hex value that starts with @).
 
+    This function is part of androguard as get_apkid(), so this
+    vendored and modified to return versionCode as an integer.
+
     """
     if not os.path.exists(apkfile):
         raise FDroidException(_("Reading packageName/versionCode/versionName failed, APK invalid: '{apkfilename}'")
                               .format(apkfilename=apkfile))
 
-    from androguard.core.bytecodes.axml import AXMLParser, format_value, START_TAG, END_TAG, TEXT, END_DOCUMENT
+    try:
+        # these were moved in androguard 4.0
+        from androguard.core.axml import AXMLParser, format_value, START_TAG, END_TAG, TEXT, END_DOCUMENT
+    except ImportError:
+        from androguard.core.bytecodes.axml import AXMLParser, format_value, START_TAG, END_TAG, TEXT, END_DOCUMENT
+    _androguard_logging_level()
 
     appid = None
     versionCode = None
     versionName = None
     with zipfile.ZipFile(apkfile) as apk:
         with apk.open('AndroidManifest.xml') as manifest:
             axml = AXMLParser(manifest.read())
@@ -2789,15 +2863,15 @@
                     if axml.getName() == 'manifest':
                         break
                 elif _type in (END_TAG, TEXT, END_DOCUMENT):
                     raise RuntimeError('{path}: <manifest> must be the first element in AndroidManifest.xml'
                                        .format(path=apkfile))
 
     if not versionName or versionName[0] == '@':
-        a = _get_androguard_APK(apkfile)
+        a = get_androguard_APK(apkfile)
         versionName = ensure_final_value(a.package, a.get_android_resources(), a.get_androidversion_name())
     if not versionName:
         versionName = ''  # versionName is expected to always be a str
 
     return appid, versionCode, versionName.strip('\0')
 
 
@@ -3127,95 +3201,158 @@
     -------
     shortened signing-key fingerprint.
     """
     return signer_fingerprint(cert_encoded)[:7]
 
 
 def signer_fingerprint(cert_encoded):
-    """Obtain sha256 signing-key fingerprint for pkcs7 DER certificate.
-
-    Extracts hexadecimal sha256 signing-key fingerprint string
-    for a given pkcs7 signature.
+    """Return SHA-256 signer fingerprint for PKCS#7 DER-encoded signature.
 
     Parameters
     ----------
     Contents of an APK signature.
 
     Returns
     -------
-    shortened signature fingerprint.
+    Standard SHA-256 signer fingerprint.
+
     """
     return hashlib.sha256(cert_encoded).hexdigest()
 
 
 def get_first_signer_certificate(apkpath):
-    """Get the first signing certificate from the APK, DER-encoded."""
-    certs = None
+    """Get the first signing certificate from the APK, DER-encoded.
+
+    JAR and APK Signatures allow for multiple signers, though it is
+    rarely used, and this is poorly documented.  So this method only
+    fetches the first certificate, and errors out if there are more.
+
+    Starting with targetSdkVersion 30, APK v2 Signatures are required.
+    https://developer.android.com/about/versions/11/behavior-changes-11#minimum-signature-scheme
+
+    When a APK v2+ signature is present, the JAR signature is not
+    verified.  The verifier parses the signers from the v2+ signature
+    and does not seem to look at the JAR signature.
+    https://source.android.com/docs/security/features/apksigning/v2#apk-signature-scheme-v2-block
+    https://android.googlesource.com/platform/tools/apksig/+/refs/tags/android-13.0.0_r3/src/main/java/com/android/apksig/ApkVerifier.java#270
+
+    apksigner checks that the signers from all the APK signatures match:
+    https://android.googlesource.com/platform/tools/apksig/+/refs/tags/android-13.0.0_r3/src/main/java/com/android/apksig/ApkVerifier.java#383
+
+    apksigner verifies each signer's signature block file
+    .(RSA|DSA|EC) against the corresponding signature file .SF
+    https://android.googlesource.com/platform/tools/apksig/+/refs/tags/android-13.0.0_r3/src/main/java/com/android/apksig/internal/apk/v1/V1SchemeVerifier.java#280
+
+    NoOverwriteDict is a workaround for:
+    https://github.com/androguard/androguard/issues/1030
+
+    Lots more discusion here:
+    https://gitlab.com/fdroid/fdroidserver/-/issues/1128
+
+    """
+
+    class NoOverwriteDict(dict):
+        def __setitem__(self, k, v):
+            if k not in self:
+                super().__setitem__(k, v)
+
     cert_encoded = None
-    with zipfile.ZipFile(apkpath, 'r') as apk:
-        cert_files = [n for n in apk.namelist() if SIGNATURE_BLOCK_FILE_REGEX.match(n)]
-        if len(cert_files) > 1:
-            logging.error(_("Found multiple JAR Signature Block Files in {path}").format(path=apkpath))
-            return None
-        elif len(cert_files) == 1:
-            cert_encoded = get_certificate(apk.read(cert_files[0]))
+    found_certs = []
+    apkobject = get_androguard_APK(apkpath)
+    apkobject._v2_blocks = NoOverwriteDict()
+    certs_v3 = apkobject.get_certificates_der_v3()
+    if certs_v3:
+        cert_v3 = certs_v3[0]
+        found_certs.append(cert_v3)
+        if not cert_encoded:
+            logging.debug(_('Using APK Signature v3'))
+            cert_encoded = cert_v3
 
-    if not cert_encoded and use_androguard():
-        apkobject = _get_androguard_APK(apkpath)
-        certs = apkobject.get_certificates_der_v2()
-        if len(certs) > 0:
-            logging.debug(_('Using APK Signature v2'))
-            cert_encoded = certs[0]
+    certs_v2 = apkobject.get_certificates_der_v2()
+    if certs_v2:
+        cert_v2 = certs_v2[0]
+        found_certs.append(cert_v2)
         if not cert_encoded:
-            certs = apkobject.get_certificates_der_v3()
-            if len(certs) > 0:
-                logging.debug(_('Using APK Signature v3'))
-                cert_encoded = certs[0]
+            logging.debug(_('Using APK Signature v2'))
+            cert_encoded = cert_v2
+
+    if get_min_sdk_version(apkobject) < 24 or (
+        not (certs_v3 or certs_v2) and get_effective_target_sdk_version(apkobject) < 30
+    ):
+        with zipfile.ZipFile(apkpath, 'r') as apk:
+            cert_files = [
+                n for n in apk.namelist() if SIGNATURE_BLOCK_FILE_REGEX.match(n)
+            ]
+            if len(cert_files) > 1:
+                logging.error(
+                    _("Found multiple JAR Signature Block Files in {path}").format(
+                        path=apkpath
+                    )
+                )
+                return
+            elif len(cert_files) == 1:
+                signature_block_file = cert_files[0]
+                signature_file = (
+                    cert_files[0][: signature_block_file.rindex('.')] + '.SF'
+                )
+                cert_v1 = get_certificate(
+                    apk.read(signature_block_file),
+                    apk.read(signature_file),
+                )
+                found_certs.append(cert_v1)
+                if not cert_encoded:
+                    logging.debug(_('Using JAR Signature'))
+                    cert_encoded = cert_v1
 
     if not cert_encoded:
         logging.error(_("No signing certificates found in {path}").format(path=apkpath))
-        return None
+        return
+
+    if not all(cert == found_certs[0] for cert in found_certs):
+        logging.error(
+            _("APK signatures have different certificates in {path}:").format(
+                path=apkpath
+            )
+        )
+        return
+
     return cert_encoded
 
 
 def apk_signer_fingerprint(apk_path):
-    """Obtain sha256 signing-key fingerprint for APK.
-
-    Extracts hexadecimal sha256 signing-key fingerprint string
-    for a given APK.
+    """Get SHA-256 fingerprint string for the first signer from given APK.
 
     Parameters
     ----------
     apk_path
         path to APK
 
     Returns
     -------
-    signature fingerprint
+    Standard SHA-256 signer fingerprint
+
     """
     cert_encoded = get_first_signer_certificate(apk_path)
     if not cert_encoded:
         return None
     return signer_fingerprint(cert_encoded)
 
 
 def apk_signer_fingerprint_short(apk_path):
-    """Obtain shortened sha256 signing-key fingerprint for APK.
-
-    Extracts the first 7 hexadecimal digits of sha256 signing-key fingerprint
-    for a given pkcs7 APK.
+    """Get 7 hex digit SHA-256 fingerprint string for the first signer from given APK.
 
     Parameters
     ----------
     apk_path
         path to APK
 
     Returns
     -------
-    shortened signing-key fingerprint
+    first 7 chars of the standard SHA-256 signer fingerprint
+
     """
     return apk_signer_fingerprint(apk_path)[:7]
 
 
 def metadata_get_sigdir(appid, vercode=None):
     """Get signature directory for app."""
     if vercode:
@@ -3426,33 +3563,51 @@
     * https://source.android.com/security/apksigning/v3
 
     """
     apksigcopier.do_extract(apkpath, outdir, v1_only=None)
 
 
 def get_min_sdk_version(apk):
-    """Wrap the androguard function to always return and int.
+    """Wrap the androguard function to always return an integer.
 
     Fall back to 1 if we can't get a valid minsdk version.
 
     Parameters
     ----------
     apk
         androguard APK object
 
     Returns
     -------
-    minsdk: int
+    minSdkVersion: int
     """
     try:
         return int(apk.get_min_sdk_version())
     except TypeError:
         return 1
 
 
+def get_effective_target_sdk_version(apk):
+    """Wrap the androguard function to always return an integer.
+
+    Parameters
+    ----------
+    apk
+        androguard APK object
+
+    Returns
+    -------
+    targetSdkVersion: int
+    """
+    try:
+        return int(apk.get_effective_target_sdk_version())
+    except TypeError:
+        return get_min_sdk_version(apk)
+
+
 def get_apksigner_smartcardoptions(smartcardoptions):
     if '-providerName' in smartcardoptions.copy():
         pos = smartcardoptions.index('-providerName')
         # remove -providerName and it's argument
         del smartcardoptions[pos]
         del smartcardoptions[pos]
     replacements = {'-storetype': '--ks-type',
@@ -3856,41 +4011,149 @@
 def get_cert_fingerprint(pubkey):
     """Generate a certificate fingerprint the same way keytool does it (but with slightly different formatting)."""
     digest = hashlib.sha256(pubkey).digest()
     ret = [' '.join("%02X" % b for b in bytearray(digest))]
     return " ".join(ret)
 
 
-def get_certificate(signature_block_file):
-    """Extract a DER certificate from JAR Signature's "Signature Block File".
+def get_certificate(signature_block_file, signature_file=None):
+    """Extract a single DER certificate from JAR Signature's "Signature Block File".
+
+    If there is more than one signer certificate, this exits with an
+    error, unless the signature_file is provided.  If that is set, it
+    will return the certificate that matches the Signature File, for
+    example, if there is a certificate chain, like TLS does.  In the
+    fdroidserver use cases, there should always be a single signer.
+    But rarely, some APKs include certificate chains.
+
+    This could be replaced by androguard's APK.get_certificate_der()
+    provided the cert chain fix was merged there.  Maybe in 4.1.2?
+    https://github.com/androguard/androguard/pull/1038
+
+    https://docs.oracle.com/en/java/javase/21/docs/specs/man/jarsigner.html#the-signed-jar-file
 
     Parameters
     ----------
     signature_block_file
-        file bytes (as string) representing the
-        certificate, as read directly out of the APK/ZIP
+        Bytes representing the PKCS#7 signer certificate and
+        signature, as read directly out of the JAR/APK, e.g. CERT.RSA.
+
+    signature_file
+        Bytes representing the manifest signed by the Signature Block
+        File, e.g. CERT.SF.  If this is not given, the assumption is
+        there will be only a single certificate in
+        signature_block_file, otherwise it is an error.
 
     Returns
     -------
     A binary representation of the certificate's public key,
     or None in case of error
 
     """
-    content = decoder.decode(signature_block_file, asn1Spec=rfc2315.ContentInfo())[0]
-    if content.getComponentByName('contentType') != rfc2315.signedData:
-        return None
-    content = decoder.decode(content.getComponentByName('content'),
-                             asn1Spec=rfc2315.SignedData())[0]
-    try:
-        certificates = content.getComponentByName('certificates')
-        cert = certificates[0].getComponentByName('certificate')
-    except PyAsn1Error:
-        logging.error("Certificates not found.")
-        return None
-    return encoder.encode(cert)
+    pkcs7obj = cms.ContentInfo.load(signature_block_file)
+    certificates = pkcs7obj['content']['certificates']
+    if len(certificates) == 1:
+        return certificates[0].chosen.dump()
+    elif not signature_file:
+        logging.error(_('Found multiple Signer Certificates!'))
+        return
+    certificate = get_jar_signer_certificate(pkcs7obj, signature_file)
+    if certificate:
+        return certificate.chosen.dump()
+
+
+def _find_matching_certificate(signer_info, certificate):
+    """Find the certificates that matches signer_info using issuer and serial number.
+
+    https://android.googlesource.com/platform/tools/apksig/+/refs/tags/android-13.0.0_r3/src/main/java/com/android/apksig/internal/apk/v1/V1SchemeVerifier.java#590
+    https://android.googlesource.com/platform/tools/apksig/+/refs/tags/android-13.0.0_r3/src/main/java/com/android/apksig/internal/x509/Certificate.java#55
+
+    """
+    certificate_serial = certificate.chosen['tbs_certificate']['serial_number']
+    expected_issuer_serial = signer_info['sid'].chosen
+    return (
+        expected_issuer_serial['issuer'] == certificate.chosen.issuer
+        and expected_issuer_serial['serial_number'] == certificate_serial
+    )
+
+
+def get_jar_signer_certificate(pkcs7obj: cms.ContentInfo, signature_file: bytes):
+    """Return the one certificate in a chain that actually signed the manifest.
+
+    PKCS#7-signed data can include certificate chains for use cases
+    where an Certificate Authority (CA) is used.  Android does not
+    validate the certificate chain on APK signatures, so neither does
+    this.
+    https://android.googlesource.com/platform/tools/apksig/+/refs/tags/android-13.0.0_r3/src/main/java/com/android/apksig/internal/apk/v1/V1SchemeVerifier.java#512
+
+    Some useful fodder for understanding all this:
+    https://docs.oracle.com/javase/tutorial/deployment/jar/intro.html
+    https://technotes.shemyak.com/posts/jar-signature-block-file-format/
+    https://docs.oracle.com/en/java/javase/21/docs/specs/man/jarsigner.html#the-signed-jar-file
+    https://qistoph.blogspot.com/2012/01/manual-verify-pkcs7-signed-data-with.html
+
+    """
+    import oscrypto.asymmetric
+    import oscrypto.errors
+
+    # Android attempts to verify all SignerInfos and then picks the first verified SignerInfo.
+    first_verified_signer_info = None
+    first_verified_signer_info_signing_certificate = None
+    for signer_info in pkcs7obj['content']['signer_infos']:
+        signature = signer_info['signature'].contents
+        digest_algorithm = signer_info["digest_algorithm"]["algorithm"].native
+        public_key = None
+        for certificate in pkcs7obj['content']['certificates']:
+            if _find_matching_certificate(signer_info, certificate):
+                public_key = oscrypto.asymmetric.load_public_key(certificate.chosen.public_key)
+                break
+        if public_key is None:
+            logging.info('No certificate found that matches signer info!')
+            continue
+
+        signature_algo = signer_info['signature_algorithm'].signature_algo
+        if signature_algo == 'rsassa_pkcs1v15':
+            # ASN.1 - 1.2.840.113549.1.1.1
+            verify_func = oscrypto.asymmetric.rsa_pkcs1v15_verify
+        elif signature_algo == 'rsassa_pss':
+            # ASN.1 - 1.2.840.113549.1.1.10
+            verify_func = oscrypto.asymmetric.rsa_pss_verify
+        elif signature_algo == 'dsa':
+            # ASN.1 - 1.2.840.10040.4.1
+            verify_func = oscrypto.asymmetric.dsa_verify
+        elif signature_algo == 'ecdsa':
+            # ASN.1 - 1.2.840.10045.4
+            verify_func = oscrypto.asymmetric.ecdsa_verify
+        else:
+            logging.error(
+                'Unknown signature algorithm %s:\n  %s\n  %s'
+                % (
+                    signature_algo,
+                    hexlify(certificate.chosen.sha256).decode(),
+                    certificate.chosen.subject.human_friendly,
+                ),
+            )
+            return
+
+        try:
+            verify_func(public_key, signature, signature_file, digest_algorithm)
+            if not first_verified_signer_info:
+                first_verified_signer_info = signer_info
+                first_verified_signer_info_signing_certificate = certificate
+
+        except oscrypto.errors.SignatureError as e:
+            logging.error(
+                '"%s", skipping:\n  %s\n  %s' % (
+                    e,
+                    hexlify(certificate.chosen.sha256).decode(),
+                    certificate.chosen.subject.human_friendly),
+            )
+
+    if first_verified_signer_info_signing_certificate:
+        return first_verified_signer_info_signing_certificate
 
 
 def load_stats_fdroid_signing_key_fingerprints():
     """Load signing-key fingerprints stored in file generated by fdroid publish.
 
     Returns
     -------
@@ -4161,15 +4424,20 @@
         b'index.html',
         b'index.jar',
         b'index.png',
         b'index.xml',
         b'index_unsigned.jar',
     ]
     if not for_gpg_signing:
-        ignore_files += [b'entry.json', b'index-v1.json', b'index-v2.json']
+        ignore_files += [
+            b'altstore-index.json',
+            b'entry.json',
+            b'index-v1.json',
+            b'index-v2.json',
+        ]
 
     return (
         os.path.isfile(filename)
         and not filename.endswith(b'.asc')
         and not filename.endswith(b'.sig')
         and not filename.endswith(b'.idsig')
         and not filename.endswith(b'.log.gz')
```

### Comparing `fdroidserver-2.3a0/fdroidserver/deploy.py` & `fdroidserver-2.3a1/fdroidserver/deploy.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 from . import _
 from . import common
 from . import index
 from .exception import FDroidException
 
 config = None
-options = None
 start_timestamp = time.gmtime()
 
 GIT_BRANCH = 'master'
 
 BINARY_TRANSPARENCY_DIR = 'binary_transparency'
 
 AUTO_S3CFG = '.fdroid-deploy-s3cfg'
@@ -67,14 +66,15 @@
     The process of pushing all the new packages to the various
     services can take a while.  So the index files should be updated
     last.  That ensures that the package files are available when the
     client learns about them from the new index files.
 
     """
     indexes = [
+        os.path.join(repo_section, 'altstore-index.json'),
         os.path.join(repo_section, 'entry.jar'),
         os.path.join(repo_section, 'entry.json'),
         os.path.join(repo_section, 'entry.json.asc'),
         os.path.join(repo_section, 'index-v1.jar'),
         os.path.join(repo_section, 'index-v1.json'),
         os.path.join(repo_section, 'index-v1.json.asc'),
         os.path.join(repo_section, 'index-v2.json'),
@@ -93,16 +93,17 @@
     """Upload the contents of the directory `repo_section` (including subdirectories) to the AWS S3 "bucket".
 
     The contents of that subdir of the
     bucket will first be deleted.
 
     Requires AWS credentials set in config.yml: awsaccesskeyid, awssecretkey
     """
-    logging.debug('Syncing "' + repo_section + '" to Amazon S3 bucket "'
-                  + config['awsbucket'] + '"')
+    logging.debug(
+        f'''Syncing "{repo_section}" to Amazon S3 bucket "{config['awsbucket']}"'''
+    )
 
     if common.set_command_in_config('s3cmd'):
         update_awsbucket_s3cmd(repo_section)
     else:
         update_awsbucket_libcloud(repo_section)
 
 
@@ -113,43 +114,47 @@
     interfering with an existing client-server interaction.  In the
     first pass, only new files are uploaded.  In the second pass,
     changed files are uploaded, overwriting what is on the server.  On
     the third/last pass, the indexes are uploaded, and any removed
     files are deleted from the server.  The last pass is the only pass
     to use a full MD5 checksum of all files to detect changes.
     """
-    logging.debug(_('Using s3cmd to sync with: {url}')
-                  .format(url=config['awsbucket']))
+    logging.debug(_('Using s3cmd to sync with: {url}').format(url=config['awsbucket']))
 
     if os.path.exists(USER_S3CFG):
         logging.info(_('Using "{path}" for configuring s3cmd.').format(path=USER_S3CFG))
         configfilename = USER_S3CFG
     else:
         fd = os.open(AUTO_S3CFG, os.O_CREAT | os.O_TRUNC | os.O_WRONLY, 0o600)
-        logging.debug(_('Creating "{path}" for configuring s3cmd.').format(path=AUTO_S3CFG))
+        logging.debug(
+            _('Creating "{path}" for configuring s3cmd.').format(path=AUTO_S3CFG)
+        )
         os.write(fd, '[default]\n'.encode('utf-8'))
-        os.write(fd, ('access_key = ' + config['awsaccesskeyid'] + '\n').encode('utf-8'))
+        os.write(
+            fd, ('access_key = ' + config['awsaccesskeyid'] + '\n').encode('utf-8')
+        )
         os.write(fd, ('secret_key = ' + config['awssecretkey'] + '\n').encode('utf-8'))
         os.close(fd)
         configfilename = AUTO_S3CFG
 
     s3bucketurl = 's3://' + config['awsbucket']
     s3cmd = [config['s3cmd'], '--config=' + configfilename]
     if subprocess.call(s3cmd + ['info', s3bucketurl]) != 0:
-        logging.warning(_('Creating new S3 bucket: {url}')
-                        .format(url=s3bucketurl))
+        logging.warning(_('Creating new S3 bucket: {url}').format(url=s3bucketurl))
         if subprocess.call(s3cmd + ['mb', s3bucketurl]) != 0:
-            logging.error(_('Failed to create S3 bucket: {url}')
-                          .format(url=s3bucketurl))
+            logging.error(
+                _('Failed to create S3 bucket: {url}').format(url=s3bucketurl)
+            )
             raise FDroidException()
 
     s3cmd_sync = s3cmd + ['sync', '--acl-public']
-    if options.verbose:
+    options = common.get_options()
+    if options and options.verbose:
         s3cmd_sync += ['--verbose']
-    if options.quiet:
+    if options and options.quiet:
         s3cmd_sync += ['--quiet']
 
     s3url = s3bucketurl + '/fdroid/'
     logging.debug('s3cmd sync new files in ' + repo_section + ' to ' + s3url)
     logging.debug(_('Running first pass with MD5 checking disabled'))
     excludes = _get_index_excludes(repo_section)
     returncode = subprocess.call(
@@ -162,16 +167,19 @@
     logging.debug('s3cmd sync all files in ' + repo_section + ' to ' + s3url)
     returncode = subprocess.call(
         s3cmd_sync + excludes + ['--no-check-md5', repo_section, s3url]
     )
     if returncode != 0:
         raise FDroidException()
 
-    logging.debug(_('s3cmd sync indexes {path} to {url} and delete')
-                  .format(path=repo_section, url=s3url))
+    logging.debug(
+        _('s3cmd sync indexes {path} to {url} and delete').format(
+            path=repo_section, url=s3url
+        )
+    )
     s3cmd_sync.append('--delete-removed')
     s3cmd_sync.append('--delete-after')
     if options.no_checksum:
         s3cmd_sync.append('--no-check-md5')
     else:
         s3cmd_sync.append('--check-md5')
     if subprocess.call(s3cmd_sync + [repo_section, s3url]) != 0:
@@ -185,39 +193,44 @@
     subdirectories) to the AWS S3 "bucket".
 
     The contents of that subdir of the
     bucket will first be deleted.
 
     Requires AWS credentials set in config.yml: awsaccesskeyid, awssecretkey
     """
-    logging.debug(_('using Apache libcloud to sync with {url}')
-                  .format(url=config['awsbucket']))
+    logging.debug(
+        _('using Apache libcloud to sync with {url}').format(url=config['awsbucket'])
+    )
 
     import libcloud.security
+
     libcloud.security.VERIFY_SSL_CERT = True
     from libcloud.storage.types import Provider, ContainerDoesNotExistError
     from libcloud.storage.providers import get_driver
 
     if not config.get('awsaccesskeyid') or not config.get('awssecretkey'):
         raise FDroidException(
-            _('To use awsbucket, awssecretkey and awsaccesskeyid must also be set in config.yml!'))
+            _(
+                'To use awsbucket, awssecretkey and awsaccesskeyid must also be set in config.yml!'
+            )
+        )
     awsbucket = config['awsbucket']
 
     if os.path.exists(USER_S3CFG):
-        raise FDroidException(_('"{path}" exists but s3cmd is not installed!')
-                              .format(path=USER_S3CFG))
+        raise FDroidException(
+            _('"{path}" exists but s3cmd is not installed!').format(path=USER_S3CFG)
+        )
 
     cls = get_driver(Provider.S3)
     driver = cls(config['awsaccesskeyid'], config['awssecretkey'])
     try:
         container = driver.get_container(container_name=awsbucket)
     except ContainerDoesNotExistError:
         container = driver.create_container(container_name=awsbucket)
-        logging.info(_('Created new container "{name}"')
-                     .format(name=container.name))
+        logging.info(_('Created new container "{name}"').format(name=container.name))
 
     upload_dir = 'fdroid/' + repo_section
     objs = dict()
     for obj in container.list_objects():
         if obj.name.startswith(upload_dir + '/'):
             objs[obj.name] = obj
 
@@ -251,21 +264,23 @@
             if upload:
                 logging.debug(' uploading "' + file_to_upload + '"...')
                 extra = {'acl': 'public-read'}
                 if file_to_upload.endswith('.sig'):
                     extra['content_type'] = 'application/pgp-signature'
                 elif file_to_upload.endswith('.asc'):
                     extra['content_type'] = 'application/pgp-signature'
-                logging.info(' uploading ' + os.path.relpath(file_to_upload)
-                             + ' to s3://' + awsbucket + '/' + object_name)
+                path = os.path.relpath(file_to_upload)
+                logging.info(f' uploading {path} to s3://{awsbucket}/{object_name}')
                 with open(file_to_upload, 'rb') as iterator:
-                    obj = driver.upload_object_via_stream(iterator=iterator,
-                                                          container=container,
-                                                          object_name=object_name,
-                                                          extra=extra)
+                    obj = driver.upload_object_via_stream(
+                        iterator=iterator,
+                        container=container,
+                        object_name=object_name,
+                        extra=extra,
+                    )
     # delete the remnants in the bucket, they do not exist locally
     while objs:
         object_name, obj = objs.popitem()
         s3url = 's3://' + awsbucket + '/' + object_name
         if object_name.startswith(upload_dir):
             logging.warning(' deleting ' + s3url)
             driver.delete_object(obj)
@@ -293,36 +308,42 @@
     try:
         subprocess.run(['rsync', '--version'], capture_output=True, check=True)
     except Exception as e:
         raise FDroidException(
             _('rsync is missing or broken: {error}').format(error=e)
         ) from e
     rsyncargs = ['rsync', '--archive', '--delete-after', '--safe-links']
+    options = common.get_options()
     if not options or not options.no_checksum:
         rsyncargs.append('--checksum')
     if options and options.verbose:
         rsyncargs += ['--verbose']
     if options and options.quiet:
         rsyncargs += ['--quiet']
     if options and options.identity_file:
-        rsyncargs += ['-e', 'ssh -oBatchMode=yes -oIdentitiesOnly=yes -i ' + options.identity_file]
+        rsyncargs += [
+            '-e',
+            'ssh -oBatchMode=yes -oIdentitiesOnly=yes -i ' + options.identity_file,
+        ]
     elif config and config.get('identity_file'):
-        rsyncargs += ['-e', 'ssh -oBatchMode=yes -oIdentitiesOnly=yes -i ' + config['identity_file']]
+        rsyncargs += [
+            '-e',
+            'ssh -oBatchMode=yes -oIdentitiesOnly=yes -i ' + config['identity_file'],
+        ]
     url = serverwebroot['url']
     logging.info('rsyncing ' + repo_section + ' to ' + url)
     excludes = _get_index_excludes(repo_section)
     if subprocess.call(rsyncargs + excludes + [repo_section, url]) != 0:
         raise FDroidException()
     if subprocess.call(rsyncargs + [repo_section, url]) != 0:
         raise FDroidException()
     # upload "current version" symlinks if requested
     if config and config.get('make_current_version_link') and repo_section == 'repo':
         links_to_upload = []
-        for f in glob.glob('*.apk') \
-                + glob.glob('*.apk.asc') + glob.glob('*.apk.sig'):
+        for f in glob.glob('*.apk') + glob.glob('*.apk.asc') + glob.glob('*.apk.sig'):
             if os.path.islink(f):
                 links_to_upload.append(f)
         if len(links_to_upload) > 0:
             if subprocess.call(rsyncargs + links_to_upload + [url]) != 0:
                 raise FDroidException()
 
 
@@ -362,17 +383,19 @@
     repo on the local filesystem.  That local repo is then used to
     push to all the servers that are configured.
 
     """
     logging.info('Syncing from local_copy_dir to this repo.')
     # trailing slashes have a meaning in rsync which is not needed here, so
     # make sure both paths have exactly one trailing slash
-    common.local_rsync(options,
-                       os.path.join(local_copy_dir, repo_section).rstrip('/') + '/',
-                       repo_section.rstrip('/') + '/')
+    common.local_rsync(
+        common.get_options(),
+        os.path.join(local_copy_dir, repo_section).rstrip('/') + '/',
+        repo_section.rstrip('/') + '/',
+    )
 
     offline_copy = os.path.join(local_copy_dir, BINARY_TRANSPARENCY_DIR)
     if os.path.exists(os.path.join(offline_copy, '.git')):
         online_copy = os.path.join(os.getcwd(), BINARY_TRANSPARENCY_DIR)
         push_binary_transparency(offline_copy, online_copy)
 
 
@@ -381,15 +404,15 @@
 
     This updates the copy of this repo used to shuttle data from an
     offline signing machine to the online machine, e.g. on a thumb
     drive.
 
     """
     # local_copy_dir is guaranteed to have a trailing slash in main() below
-    common.local_rsync(options, repo_section, local_copy_dir)
+    common.local_rsync(common.get_options(), repo_section, local_copy_dir)
 
     offline_copy = os.path.join(os.getcwd(), BINARY_TRANSPARENCY_DIR)
     if os.path.isdir(os.path.join(offline_copy, '.git')):
         online_copy = os.path.join(local_copy_dir, BINARY_TRANSPARENCY_DIR)
         push_binary_transparency(offline_copy, online_copy)
 
 
@@ -413,46 +436,56 @@
     This git repo is only a git repo for the purpose of being hosted.
     For history, there is the archive section, and there is the binary
     transparency log.
 
     """
     import git
     from clint.textui import progress
-    if config.get('local_copy_dir') \
-       and not config.get('sync_from_local_copy_dir'):
-        logging.debug(_('Offline machine, skipping git mirror generation until `fdroid deploy`'))
+
+    if config.get('local_copy_dir') and not config.get('sync_from_local_copy_dir'):
+        logging.debug(
+            _('Offline machine, skipping git mirror generation until `fdroid deploy`')
+        )
         return
 
+    options = common.get_options()
+
     # right now we support only 'repo' git-mirroring
     if repo_section == 'repo':
         git_mirror_path = 'git-mirror'
         dotgit = os.path.join(git_mirror_path, '.git')
         git_fdroiddir = os.path.join(git_mirror_path, 'fdroid')
         git_repodir = os.path.join(git_fdroiddir, repo_section)
         if not os.path.isdir(git_repodir):
             os.makedirs(git_repodir)
         # github/gitlab use bare git repos, so only count the .git folder
         # test: generate giant APKs by including AndroidManifest.xml and and large
         # file from /dev/urandom, then sign it.  Then add those to the git repo.
         dotgit_size = _get_size(dotgit)
         dotgit_over_limit = dotgit_size > config['git_mirror_size_limit']
         if os.path.isdir(dotgit) and dotgit_over_limit:
-            logging.warning(_('Deleting git-mirror history, repo is too big ({size} max {limit})')
-                            .format(size=dotgit_size, limit=config['git_mirror_size_limit']))
+            logging.warning(
+                _(
+                    'Deleting git-mirror history, repo is too big ({size} max {limit})'
+                ).format(size=dotgit_size, limit=config['git_mirror_size_limit'])
+            )
             shutil.rmtree(dotgit)
         if options.no_keep_git_mirror_archive and dotgit_over_limit:
-            logging.warning(_('Deleting archive, repo is too big ({size} max {limit})')
-                            .format(size=dotgit_size, limit=config['git_mirror_size_limit']))
+            logging.warning(
+                _('Deleting archive, repo is too big ({size} max {limit})').format(
+                    size=dotgit_size, limit=config['git_mirror_size_limit']
+                )
+            )
             archive_path = os.path.join(git_mirror_path, 'fdroid', 'archive')
             shutil.rmtree(archive_path, ignore_errors=True)
 
         # rsync is very particular about trailing slashes
-        common.local_rsync(options,
-                           repo_section.rstrip('/') + '/',
-                           git_repodir.rstrip('/') + '/')
+        common.local_rsync(
+            options, repo_section.rstrip('/') + '/', git_repodir.rstrip('/') + '/'
+        )
 
         # use custom SSH command if identity_file specified
         ssh_cmd = 'ssh -oBatchMode=yes'
         if options.identity_file is not None:
             ssh_cmd += ' -oIdentitiesOnly=yes -i "%s"' % options.identity_file
         elif 'identity_file' in config:
             ssh_cmd += ' -oIdentitiesOnly=yes -i "%s"' % config['identity_file']
@@ -482,14 +515,15 @@
         if options.verbose:
             progressbar = progress.Bar()
 
             class MyProgressPrinter(git.RemoteProgress):
                 def update(self, op_code, current, maximum=None, message=None):
                     if isinstance(maximum, float):
                         progressbar.show(current, maximum)
+
             progress = MyProgressPrinter()
         else:
             progress = None
 
         # only deploy to GitLab Artifacts if too big for GitLab Pages
         if common.get_dir_size(git_fdroiddir) <= common.GITLAB_COM_PAGES_MAX_SIZE:
             gitlab_ci_job_name = 'pages'
@@ -531,36 +565,44 @@
 
             logging.debug(_('Pushing to {url}').format(url=remote.url))
             with repo.git.custom_environment(GIT_SSH_COMMAND=ssh_cmd):
                 pushinfos = remote.push(
                     GIT_BRANCH, force=True, set_upstream=True, progress=progress
                 )
                 for pushinfo in pushinfos:
-                    if pushinfo.flags & (git.remote.PushInfo.ERROR
-                                         | git.remote.PushInfo.REJECTED
-                                         | git.remote.PushInfo.REMOTE_FAILURE
-                                         | git.remote.PushInfo.REMOTE_REJECTED):
+                    if pushinfo.flags & (
+                        git.remote.PushInfo.ERROR
+                        | git.remote.PushInfo.REJECTED
+                        | git.remote.PushInfo.REMOTE_FAILURE
+                        | git.remote.PushInfo.REMOTE_REJECTED
+                    ):
                         # Show potentially useful messages from git remote
                         for line in progress.other_lines:
                             if line.startswith('remote:'):
                                 logging.debug(line)
-                        raise FDroidException(remote.url + ' push failed: ' + str(pushinfo.flags)
-                                              + ' ' + pushinfo.summary)
+                        raise FDroidException(
+                            '{url} push failed: {flags} {summary}'.format(
+                                url=remote.url,
+                                flags=pushinfo.flags,
+                                summary=pushinfo.summary,
+                            )
+                        )
                     else:
                         logging.debug(remote.url + ': ' + pushinfo.summary)
 
         if progress:
             progressbar.done()
 
 
 def upload_to_android_observatory(repo_section):
     import requests
+
     requests  # stop unused import warning
 
-    if options.verbose:
+    if common.get_options().verbose:
         logging.getLogger("requests").setLevel(logging.INFO)
         logging.getLogger("urllib3").setLevel(logging.INFO)
     else:
         logging.getLogger("requests").setLevel(logging.WARNING)
         logging.getLogger("urllib3").setLevel(logging.WARNING)
 
     if repo_section == 'repo':
@@ -571,17 +613,20 @@
 def upload_apk_to_android_observatory(path):
     # depend on requests and lxml only if users enable AO
     import requests
     from . import net
     from lxml.html import fromstring
 
     apkfilename = os.path.basename(path)
-    r = requests.post('https://androidobservatory.org/',
-                      data={'q': common.sha256sum(path), 'searchby': 'hash'},
-                      headers=net.HEADERS, timeout=300)
+    r = requests.post(
+        'https://androidobservatory.org/',
+        data={'q': common.sha256sum(path), 'searchby': 'hash'},
+        headers=net.HEADERS,
+        timeout=300,
+    )
     if r.status_code == 200:
         # from now on XPath will be used to retrieve the message in the HTML
         # androidobservatory doesn't have a nice API to talk with
         # so we must scrape the page content
         tree = fromstring(r.text)
 
         href = None
@@ -590,132 +635,162 @@
             if a:
                 m = re.match(r'^/app/[0-9A-F]{40}$', a)
                 if m:
                     href = m.group()
 
         page = 'https://androidobservatory.org'
         if href:
-            message = (_('Found {apkfilename} at {url}')
-                       .format(apkfilename=apkfilename, url=(page + href)))
+            message = _('Found {apkfilename} at {url}').format(
+                apkfilename=apkfilename, url=(page + href)
+            )
             logging.debug(message)
             return
 
     # upload the file with a post request
-    logging.info(_('Uploading {apkfilename} to androidobservatory.org')
-                 .format(apkfilename=apkfilename))
-    r = requests.post('https://androidobservatory.org/upload',
-                      files={'apk': (apkfilename, open(path, 'rb'))},
-                      headers=net.HEADERS,
-                      allow_redirects=False, timeout=300)
+    logging.info(
+        _('Uploading {apkfilename} to androidobservatory.org').format(
+            apkfilename=apkfilename
+        )
+    )
+    r = requests.post(
+        'https://androidobservatory.org/upload',
+        files={'apk': (apkfilename, open(path, 'rb'))},
+        headers=net.HEADERS,
+        allow_redirects=False,
+        timeout=300,
+    )
 
 
 def upload_to_virustotal(repo_section, virustotal_apikey):
     import requests
+
     requests  # stop unused import warning
 
     if repo_section == 'repo':
         if not os.path.exists('virustotal'):
             os.mkdir('virustotal')
 
         if os.path.exists(os.path.join(repo_section, 'index-v1.json')):
             with open(os.path.join(repo_section, 'index-v1.json')) as fp:
                 data = json.load(fp)
         else:
-            data, _ignored, _ignored = index.get_index_from_jar(os.path.join(repo_section, 'index-v1.jar'))
+            local_jar = os.path.join(repo_section, 'index-v1.jar')
+            data, _ignored, _ignored = index.get_index_from_jar(local_jar)
 
         for packageName, packages in data['packages'].items():
             for package in packages:
                 upload_apk_to_virustotal(virustotal_apikey, **package)
 
 
-def upload_apk_to_virustotal(virustotal_apikey, packageName, apkName, hash,
-                             versionCode, **kwargs):
+def upload_apk_to_virustotal(
+    virustotal_apikey, packageName, apkName, hash, versionCode, **kwargs
+):
     import requests
 
     logging.getLogger("urllib3").setLevel(logging.WARNING)
     logging.getLogger("requests").setLevel(logging.WARNING)
 
-    outputfilename = os.path.join('virustotal',
-                                  packageName + '_' + str(versionCode)
-                                  + '_' + hash + '.json')
+    outputfilename = os.path.join(
+        'virustotal', packageName + '_' + str(versionCode) + '_' + hash + '.json'
+    )
     if os.path.exists(outputfilename):
         logging.debug(apkName + ' results are in ' + outputfilename)
         return outputfilename
     repofilename = os.path.join('repo', apkName)
     logging.info('Checking if ' + repofilename + ' is on virustotal')
 
-    headers = {
-        "User-Agent": "F-Droid"
-    }
+    headers = {"User-Agent": "F-Droid"}
     if 'headers' in kwargs:
         for k, v in kwargs['headers'].items():
             headers[k] = v
 
-    data = {
+    apikey = {
         'apikey': virustotal_apikey,
         'resource': hash,
     }
     needs_file_upload = False
     while True:
-        r = requests.get('https://www.virustotal.com/vtapi/v2/file/report?'
-                         + urllib.parse.urlencode(data), headers=headers, timeout=300)
+        report_url = (
+            'https://www.virustotal.com/vtapi/v2/file/report?'
+            + urllib.parse.urlencode(apikey)
+        )
+        r = requests.get(report_url, headers=headers, timeout=300)
         if r.status_code == 200:
             response = r.json()
             if response['response_code'] == 0:
                 needs_file_upload = True
             else:
                 response['filename'] = apkName
                 response['packageName'] = packageName
                 response['versionCode'] = versionCode
                 if kwargs.get('versionName'):
                     response['versionName'] = kwargs.get('versionName')
                 with open(outputfilename, 'w') as fp:
                     json.dump(response, fp, indent=2, sort_keys=True)
 
             if response.get('positives', 0) > 0:
-                logging.warning(repofilename + ' has been flagged by virustotal '
-                                + str(response['positives']) + ' times:'
-                                + '\n\t' + response['permalink'])
+                logging.warning(
+                    _('{path} has been flagged by virustotal {count} times:').format(
+                        path=repofilename, count=response['positives']
+                    ),
+                    +'\n\t' + response['permalink'],
+                )
             break
         if r.status_code == 204:
             logging.warning(_('virustotal.com is rate limiting, waiting to retry...'))
             time.sleep(30)  # wait for public API rate limiting
 
     upload_url = None
     if needs_file_upload:
         manual_url = 'https://www.virustotal.com/'
         size = os.path.getsize(repofilename)
         if size > 200000000:
             # VirusTotal API 200MB hard limit
-            logging.error(_('{path} more than 200MB, manually upload: {url}')
-                          .format(path=repofilename, url=manual_url))
+            logging.error(
+                _('{path} more than 200MB, manually upload: {url}').format(
+                    path=repofilename, url=manual_url
+                )
+            )
         elif size > 32000000:
             # VirusTotal API requires fetching a URL to upload bigger files
-            r = requests.get('https://www.virustotal.com/vtapi/v2/file/scan/upload_url?'
-                             + urllib.parse.urlencode(data), headers=headers, timeout=300)
+            query_url = (
+                'https://www.virustotal.com/vtapi/v2/file/scan/upload_url?'
+                + urllib.parse.urlencode(apikey)
+            )
+            r = requests.get(query_url, headers=headers, timeout=300)
             if r.status_code == 200:
                 upload_url = r.json().get('upload_url')
             elif r.status_code == 403:
-                logging.error(_('VirusTotal API key cannot upload files larger than 32MB, '
-                                + 'use {url} to upload {path}.')
-                              .format(path=repofilename, url=manual_url))
+                logging.error(
+                    _(
+                        'VirusTotal API key cannot upload files larger than 32MB, '
+                        + 'use {url} to upload {path}.'
+                    ).format(path=repofilename, url=manual_url)
+                )
             else:
                 r.raise_for_status()
         else:
             upload_url = 'https://www.virustotal.com/vtapi/v2/file/scan'
 
     if upload_url:
-        logging.info(_('Uploading {apkfilename} to virustotal')
-                     .format(apkfilename=repofilename))
-        files = {
-            'file': (apkName, open(repofilename, 'rb'))
-        }
-        r = requests.post(upload_url, data=data, headers=headers, files=files, timeout=300)
-        logging.debug(_('If this upload fails, try manually uploading to {url}')
-                      .format(url=manual_url))
+        logging.info(
+            _('Uploading {apkfilename} to virustotal').format(apkfilename=repofilename)
+        )
+        r = requests.post(
+            upload_url,
+            data=apikey,
+            headers=headers,
+            files={'file': (apkName, open(repofilename, 'rb'))},
+            timeout=300,
+        )
+        logging.debug(
+            _('If this upload fails, try manually uploading to {url}').format(
+                url=manual_url
+            )
+        )
         r.raise_for_status()
         response = r.json()
         logging.info(response['verbose_msg'] + " " + response['permalink'])
 
     return outputfilename
 
 
@@ -732,16 +807,15 @@
     data from the offline machine to the online machine.  In that
     case, git_remote is a dir on the local file system, e.g. a thumb
     drive.
 
     """
     import git
 
-    logging.info(_('Pushing binary transparency log to {url}')
-                 .format(url=git_remote))
+    logging.info(_('Pushing binary transparency log to {url}').format(url=git_remote))
 
     if os.path.isdir(os.path.dirname(git_remote)):
         # from offline machine to thumbdrive
         remote_path = os.path.abspath(git_repo_path)
         if not os.path.isdir(os.path.join(git_remote, '.git')):
             os.makedirs(git_remote, exist_ok=True)
             thumbdriverepo = git.Repo.init(git_remote, initial_branch=GIT_BRANCH)
@@ -762,32 +836,55 @@
         origin = git.remote.Remote(gitrepo, 'origin')
         if origin in gitrepo.remotes:
             origin = gitrepo.remote('origin')
             if 'set_url' in dir(origin):  # added in GitPython 2.x
                 origin.set_url(git_remote)
         else:
             origin = gitrepo.create_remote('origin', git_remote)
-        origin.push(GIT_BRANCH)
+        for _i in range(3):
+            try:
+                origin.push(GIT_BRANCH)
+            except git.GitCommandError as e:
+                logging.error(e)
+                continue
+            break
+        else:
+            raise FDroidException(_("Pushing to remote server failed!"))
 
 
 def main():
-    global config, options
+    global config
 
     parser = ArgumentParser()
     common.setup_global_opts(parser)
-    parser.add_argument("-i", "--identity-file", default=None,
-                        help=_("Specify an identity file to provide to SSH for rsyncing"))
-    parser.add_argument("--local-copy-dir", default=None,
-                        help=_("Specify a local folder to sync the repo to"))
-    parser.add_argument("--no-checksum", action="store_true", default=False,
-                        help=_("Don't use rsync checksums"))
-    parser.add_argument("--no-keep-git-mirror-archive", action="store_true", default=False,
-                        help=_("If a git mirror gets to big, allow the archive to be deleted"))
-    options = parser.parse_args()
-    config = common.read_config(options)
+    parser.add_argument(
+        "-i",
+        "--identity-file",
+        default=None,
+        help=_("Specify an identity file to provide to SSH for rsyncing"),
+    )
+    parser.add_argument(
+        "--local-copy-dir",
+        default=None,
+        help=_("Specify a local folder to sync the repo to"),
+    )
+    parser.add_argument(
+        "--no-checksum",
+        action="store_true",
+        default=False,
+        help=_("Don't use rsync checksums"),
+    )
+    parser.add_argument(
+        "--no-keep-git-mirror-archive",
+        action="store_true",
+        default=False,
+        help=_("If a git mirror gets to big, allow the archive to be deleted"),
+    )
+    options = common.parse_args(parser)
+    config = common.read_config()
 
     if config.get('nonstandardwebroot') is True:
         standardwebroot = False
     else:
         standardwebroot = True
 
     if options.local_copy_dir is not None:
@@ -798,54 +895,66 @@
         local_copy_dir = None
     if local_copy_dir is not None:
         fdroiddir = local_copy_dir.rstrip('/')
         if os.path.exists(fdroiddir) and not os.path.isdir(fdroiddir):
             logging.error(_('local_copy_dir must be directory, not a file!'))
             sys.exit(1)
         if not os.path.exists(os.path.dirname(fdroiddir)):
-            logging.error(_('The root dir for local_copy_dir "{path}" does not exist!')
-                          .format(path=os.path.dirname(fdroiddir)))
+            logging.error(
+                _('The root dir for local_copy_dir "{path}" does not exist!').format(
+                    path=os.path.dirname(fdroiddir)
+                )
+            )
             sys.exit(1)
         if not os.path.isabs(fdroiddir):
             logging.error(_('local_copy_dir must be an absolute path!'))
             sys.exit(1)
         repobase = os.path.basename(fdroiddir)
         if standardwebroot and repobase != 'fdroid':
-            logging.error(_('local_copy_dir does not end with "fdroid", '
-                            + 'perhaps you meant: "{path}"')
-                          .format(path=fdroiddir + '/fdroid'))
+            logging.error(
+                _(
+                    'local_copy_dir does not end with "fdroid", '
+                    + 'perhaps you meant: "{path}"'
+                ).format(path=fdroiddir + '/fdroid')
+            )
             sys.exit(1)
         if local_copy_dir[-1] != '/':
             local_copy_dir += '/'
         local_copy_dir = local_copy_dir.replace('//', '/')
         if not os.path.exists(fdroiddir):
             os.mkdir(fdroiddir)
 
-    if not config.get('awsbucket') \
-            and not config.get('serverwebroot') \
-            and not config.get('servergitmirrors') \
-            and not config.get('androidobservatory') \
-            and not config.get('binary_transparency_remote') \
-            and not config.get('virustotal_apikey') \
-            and local_copy_dir is None:
-        logging.warning(_('No option set! Edit your config.yml to set at least one of these:')
-                        + '\nserverwebroot, servergitmirrors, local_copy_dir, awsbucket, '
-                        + 'virustotal_apikey, androidobservatory, or binary_transparency_remote')
+    if (
+        not config.get('awsbucket')
+        and not config.get('serverwebroot')
+        and not config.get('servergitmirrors')
+        and not config.get('androidobservatory')
+        and not config.get('binary_transparency_remote')
+        and not config.get('virustotal_apikey')
+        and local_copy_dir is None
+    ):
+        logging.warning(
+            _('No option set! Edit your config.yml to set at least one of these:')
+            + '\nserverwebroot, servergitmirrors, local_copy_dir, awsbucket, '
+            + 'virustotal_apikey, androidobservatory, or binary_transparency_remote'
+        )
         sys.exit(1)
 
     repo_sections = ['repo']
     if config['archive_older'] != 0:
         repo_sections.append('archive')
         if not os.path.exists('archive'):
             os.mkdir('archive')
     if config['per_app_repos']:
         repo_sections += common.get_per_app_repos()
 
-    if os.path.isdir('unsigned') or (local_copy_dir is not None
-                                     and os.path.isdir(os.path.join(local_copy_dir, 'unsigned'))):
+    if os.path.isdir('unsigned') or (
+        local_copy_dir is not None
+        and os.path.isdir(os.path.join(local_copy_dir, 'unsigned'))
+    ):
         repo_sections.append('unsigned')
 
     for repo_section in repo_sections:
         if local_copy_dir is not None:
             if config['sync_from_local_copy_dir']:
                 sync_from_localcopy(repo_section, local_copy_dir)
             else:
@@ -862,16 +971,15 @@
         if config.get('androidobservatory'):
             upload_to_android_observatory(repo_section)
         if config.get('virustotal_apikey'):
             upload_to_virustotal(repo_section, config.get('virustotal_apikey'))
 
     binary_transparency_remote = config.get('binary_transparency_remote')
     if binary_transparency_remote:
-        push_binary_transparency(BINARY_TRANSPARENCY_DIR,
-                                 binary_transparency_remote)
+        push_binary_transparency(BINARY_TRANSPARENCY_DIR, binary_transparency_remote)
 
     common.write_status_json(common.setup_status_output(start_timestamp))
     sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fdroidserver-2.3a0/fdroidserver/exception.py` & `fdroidserver-2.3a1/fdroidserver/exception.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/fdroidserver/gpgsign.py` & `fdroidserver-2.3a1/fdroidserver/gpgsign.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,36 +24,35 @@
 
 from . import _
 from . import common
 from .common import FDroidPopen
 from .exception import FDroidException
 
 config = None
-options = None
 start_timestamp = time.gmtime()
 
 
 def status_update_json(signed):
     """Output a JSON file with metadata about this run."""
     logging.debug(_('Outputting JSON'))
     output = common.setup_status_output(start_timestamp)
     if signed:
         output['signed'] = signed
     common.write_status_json(output)
 
 
 def main():
-    global config, options
+    global config
 
     # Parse command line...
     parser = ArgumentParser()
     common.setup_global_opts(parser)
-    options = parser.parse_args()
+    common.parse_args(parser)
 
-    config = common.read_config(options)
+    config = common.read_config()
 
     repodirs = ['repo']
     if config['archive_older'] != 0:
         repodirs.append('archive')
 
     signed = []
     for output_dir in repodirs:
```

### Comparing `fdroidserver-2.3a0/fdroidserver/import_subcommand.py` & `fdroidserver-2.3a1/fdroidserver/import_subcommand.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+"""Extract application metadata from a source repository."""
 #
 # import_subcommand.py - part of the FDroid server tools
 # Copyright (C) 2010-13, Ciaran Gultnieks, ciaran@ciarang.com
 # Copyright (C) 2013-2014 Daniel Martí <mvdan@mvdan.cc>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
@@ -26,59 +27,83 @@
 import json
 import shutil
 import sys
 import yaml
 from argparse import ArgumentParser
 import logging
 from pathlib import Path
+from typing import Optional
 
 try:
     from yaml import CSafeLoader as SafeLoader
 except ImportError:
     from yaml import SafeLoader
 
 from . import _
 from . import common
 from . import metadata
 from .exception import FDroidException
 
 
 config = None
-options = None
 
 
 def handle_retree_error_on_windows(function, path, excinfo):
     """Python can't remove a readonly file on Windows so chmod first."""
     if function in (os.unlink, os.rmdir, os.remove) and excinfo[0] == PermissionError:
         os.chmod(path, stat.S_IWRITE)
         function(path)
 
 
-def clone_to_tmp_dir(app):
+def clone_to_tmp_dir(app: metadata.App, rev=None) -> Path:
+    """Clone the source repository of an app to a temporary directory for further processing.
+
+    Parameters
+    ----------
+    app
+        The App instance to clone the source of.
+
+    Returns
+    -------
+    tmp_dir
+        The (temporary) directory the apps source has been cloned into.
+
+    """
     tmp_dir = Path('tmp')
     tmp_dir.mkdir(exist_ok=True)
 
     tmp_dir = tmp_dir / 'importer'
 
     if tmp_dir.exists():
         shutil.rmtree(str(tmp_dir), onerror=handle_retree_error_on_windows)
     vcs = common.getvcs(app.RepoType, app.Repo, tmp_dir)
-    vcs.gotorevision(options.rev)
+    vcs.gotorevision(rev)
 
     return tmp_dir
 
 
-def getrepofrompage(url):
+def getrepofrompage(url: str) -> tuple[Optional[str], str]:
     """Get the repo type and address from the given web page.
 
     The page is scanned in a rather naive manner for 'git clone xxxx',
     'hg clone xxxx', etc, and when one of these is found it's assumed
     that's the information we want.  Returns repotype, address, or
     None, reason
 
+    Parameters
+    ----------
+    url
+        The url to look for repository information at.
+
+    Returns
+    -------
+    repotype_or_none
+        The found repository type or None if an error occured.
+    address_or_reason
+        The address to the found repository or the reason if an error occured.
     """
     if not url.startswith('http'):
         return (None, _('{url} does not start with "http"!'.format(url=url)))
     req = urllib.request.urlopen(url)  # nosec B310 non-http URLs are filtered out
     if req.getcode() != 200:
         return (None, 'Unable to get ' + url + ' - return code ' + str(req.getcode()))
     page = req.read().decode(req.headers.get_content_charset())
@@ -116,21 +141,37 @@
         repo = repo[:index]
         repo = repo.split('"')[0]
         return (repotype, repo)
 
     return (None, _("No information found.") + page)
 
 
-def get_app_from_url(url):
+def get_app_from_url(url: str) -> metadata.App:
     """Guess basic app metadata from the URL.
 
     The URL must include a network hostname, unless it is an lp:,
     file:, or git/ssh URL.  This throws ValueError on bad URLs to
     match urlparse().
 
+    Parameters
+    ----------
+    url
+        The URL to look to look for app metadata at.
+
+    Returns
+    -------
+    app
+        App instance with the found metadata.
+
+    Raises
+    ------
+    :exc:`~fdroidserver.exception.FDroidException`
+        If the VCS type could not be determined.
+    :exc:`ValueError`
+        If the URL is invalid.
     """
     parsed = urllib.parse.urlparse(url)
     invalid_url = False
     if not parsed.scheme or not parsed.path:
         invalid_url = True
 
     app = metadata.App()
@@ -179,15 +220,29 @@
     if not app.RepoType:
         raise FDroidException("Unable to determine vcs type. " + app.Repo)
 
     return app
 
 
 def main():
-    global config, options
+    """Extract app metadata and write it to a file.
+
+    The behaviour of this function is influenced by the configuration file as
+    well as command line parameters.
+
+    Raises
+    ------
+    :exc:`~fdroidserver.exception.FDroidException`
+        If the repository already has local metadata, no URL is specified and
+        the current directory is not a Git repository, no application ID could
+        be found, no Gradle project could be found or there is already metadata
+        for the found application ID.
+
+    """
+    global config
 
     # Parse command line...
     parser = ArgumentParser()
     common.setup_global_opts(parser)
     parser.add_argument("-u", "--url", default=None,
                         help=_("Project URL to import from."))
     parser.add_argument("-s", "--subdir", default=None,
@@ -197,18 +252,18 @@
     parser.add_argument("-l", "--license", default=None,
                         help=_("Overall license of the project."))
     parser.add_argument("--omit-disable", action="store_true", default=False,
                         help=_("Do not add 'disable:' to the generated build entries"))
     parser.add_argument("--rev", default=None,
                         help=_("Allows a different revision (or git branch) to be specified for the initial import"))
     metadata.add_metadata_arguments(parser)
-    options = parser.parse_args()
+    options = common.parse_args(parser)
     metadata.warnings_action = options.W
 
-    config = common.read_config(options)
+    config = common.read_config()
 
     apps = metadata.read_metadata()
     app = None
 
     tmp_importer_dir = None
 
     local_metadata_files = common.get_local_metadata_files()
@@ -231,15 +286,15 @@
                 if url.startswith('https://git'):  # github, gitlab
                     app.SourceCode = url.rstrip('.git')
                 app.Repo = url
                 break
         write_local_file = True
     elif options.url:
         app = get_app_from_url(options.url)
-        tmp_importer_dir = clone_to_tmp_dir(app)
+        tmp_importer_dir = clone_to_tmp_dir(app, options.rev)
         git_repo = git.Repo(tmp_importer_dir)
 
         if not options.omit_disable:
             build.disable = 'Generated by `fdroid import` - check version fields and commitid'
         write_local_file = False
     else:
         raise FDroidException("Specify project url.")
```

### Comparing `fdroidserver-2.3a0/fdroidserver/index.py` & `fdroidserver-2.3a1/fdroidserver/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,14 +121,21 @@
     make_v0(sortedapps, apks, repodir, repodict, requestsdict,
             fdroid_signing_key_fingerprints)
     make_v1(sortedapps, apks, repodir, repodict, requestsdict,
             fdroid_signing_key_fingerprints)
     make_v2(sortedapps, apks, repodir, repodict, requestsdict,
             fdroid_signing_key_fingerprints, archive)
     make_website(sortedapps, repodir, repodict)
+    make_altstore(
+        sortedapps,
+        apks,
+        common.config,
+        repodir,
+        pretty=common.options.pretty,
+    )
 
 
 def _should_file_be_generated(path, magic_string):
     if os.path.exists(path):
         with open(path) as f:
             # if the magic_string is not in the first line the file should be overwritten
             if magic_string not in f.readline():
@@ -1746,7 +1753,104 @@
         raise VerificationException(_("Found multiple signing certificates for repository."))
 
     # extract public key from certificate
     public_key = common.get_certificate(jar.read(certs[0]))
     public_key_fingerprint = common.get_cert_fingerprint(public_key).replace(' ', '')
 
     return public_key, public_key_fingerprint
+
+
+def make_altstore(apps, apks, config, repodir, pretty=False):
+    """Assemble altstore-index.json for iOS (.ipa) apps.
+
+    builds index files based on:
+    https://faq.altstore.io/distribute-your-apps/make-a-source
+    https://faq.altstore.io/distribute-your-apps/updating-apps
+    """
+    if not any(Path(repodir).glob('*.ipa')):
+        # no IPA files present in repo, nothing to do here, exiting early
+        return
+
+    indent = 2 if pretty else None
+    # for now alt-store support is english only
+    for lang in ['en']:
+
+        # prepare minimal altstore index
+        idx = {
+            'name': config['repo_name'],
+            "apps": [],
+            "news": [],
+        }
+
+        # add optional values if available
+        # idx["subtitle"] F-Droid doesn't have a corresponding value
+        if config.get("repo_description"):
+            idx['description'] = config['repo_description']
+        if (Path(repodir) / 'icons' / config['repo_icon']).exists():
+            idx['iconURL'] = f"{config['repo_url']}/icons/{config['repo_icon']}"
+        # idx["headerURL"] F-Droid doesn't have a corresponding value
+        # idx["website"] F-Droid doesn't have a corresponding value
+        # idx["patreonURL"] F-Droid doesn't have a corresponding value
+        # idx["tintColor"] F-Droid doesn't have a corresponding value
+        # idx["featuredApps"] = [] maybe mappable to F-Droids what's new?
+
+        # assemble "apps"
+        for packageName, app in apps.items():
+            app_name = app.get("Name") or app.get("AutoName")
+            icon_url = "{}{}".format(
+                config['repo_url'],
+                app.get('iconv2', {}).get(DEFAULT_LOCALE, {}).get('name', ''),
+            )
+            screenshot_urls = [
+                "{}{}".format(config["repo_url"], s["name"])
+                for s in app.get("screenshots", {})
+                .get("phone", {})
+                .get(DEFAULT_LOCALE, {})
+            ]
+
+            a = {
+                "name": app_name,
+                'bundleIdentifier': packageName,
+                'developerName': app.get("AuthorName") or f"{app_name} team",
+                'iconURL': icon_url,
+                "localizedDescription": "",
+                'appPermissions': {
+                    "entitlements": set(),
+                    "privacy": {},
+                },
+                'versions': [],
+            }
+
+            if app.get('summary'):
+                a['subtitle'] = app['summary']
+            # a["tintColor"] F-Droid doesn't have a corresponding value
+            # a["category"] F-Droid doesn't have a corresponding value
+            # a['patreon'] F-Droid doesn't have a corresponding value
+            a["screenshots"] = screenshot_urls
+
+            # populate 'versions'
+            for apk in apks:
+                last4 = apk.get('apkName', '').lower()[-4:]
+                if apk['packageName'] == packageName and last4 == '.ipa':
+                    v = {
+                        "version": apk["versionName"],
+                        "date": apk["added"].isoformat(),
+                        "downloadURL": f"{config['repo_url']}/{apk['apkName']}",
+                        "size": apk['size'],
+                    }
+
+                    # v['localizedDescription'] maybe what's new text?
+                    v["minOSVersion"] = apk["ipa_MinimumOSVersion"]
+                    v["maxOSVersion"] = apk["ipa_DTPlatformVersion"]
+
+                    # writing this spot here has the effect that always the
+                    # permissions of the latest processed permissions list used
+                    a['appPermissions']['privacy'] = apk['ipa_permissions']
+                    a['appPermissions']['entitlements'] = list(apk['ipa_entitlements'])
+
+                    a['versions'].append(v)
+
+            if len(a['versions']) > 0:
+                idx['apps'].append(a)
+
+        with open(Path(repodir) / 'altstore-index.json', "w", encoding="utf-8") as f:
+            json.dump(idx, f, indent=indent)
```

### Comparing `fdroidserver-2.3a0/fdroidserver/init.py` & `fdroidserver-2.3a1/fdroidserver/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 import logging
 
 from . import _
 from . import common
 from .exception import FDroidException
 
 config = {}
-options = None
 
 
 def disable_in_config(key, value):
     """Write a key/value to the local config.yml, then comment it out."""
     import yaml
 
     with open('config.yml') as f:
@@ -45,15 +44,15 @@
     repl = '\n#' + yaml.dump({key: value}, default_flow_style=False)
     data = re.sub(pattern, repl, data)
     with open('config.yml', 'w') as f:
         f.writelines(data)
 
 
 def main():
-    global options, config
+    global config
 
     # Parse command line...
     parser = ArgumentParser()
     common.setup_global_opts(parser)
     parser.add_argument(
         "-d",
         "--distinguished-name",
@@ -77,15 +76,15 @@
     )
     parser.add_argument(
         "--no-prompt",
         action="store_true",
         default=False,
         help=_("Do not prompt for Android SDK path, just fail"),
     )
-    options = parser.parse_args()
+    options = common.parse_args(parser)
 
     common.set_console_logging(options.verbose)
 
     fdroiddir = os.getcwd()
     test_config = dict()
     examplesdir = common.get_examples_dir()
     common.fill_config_defaults(test_config)
@@ -167,15 +166,15 @@
         logging.warning(
             'Looks like this is already an F-Droid repo, cowardly refusing to overwrite it...'
         )
         logging.info('Try running `fdroid init` in an empty directory.')
         raise FDroidException('Repository already exists.')
 
     # now that we have a local config.yml, read configuration...
-    config = common.read_config(options)
+    config = common.read_config()
 
     # the NDK is optional and there may be multiple versions of it, so it's
     # left for the user to configure
 
     # find or generate the keystore for the repo signing key. First try the
     # path written in the default config.yml.  Then check if the user has
     # specified a path from the command line, which will trump all others.
@@ -278,21 +277,21 @@
     msg += '\n\n  Android SDK:\t\t\t' + config['sdk_path']
     msg += '\n  ' + _('Keystore for signing key:\t') + keystore
     if repo_keyalias is not None:
         msg += '\n  Alias for key in store:\t' + repo_keyalias
     msg += '\n\n'
     msg += (
         _(
-            '''To complete the setup, add your APKs to "%s"
+            """To complete the setup, add your APKs to "%s"
 then run "fdroid update -c; fdroid update".  You might also want to edit
 "config.yml" to set the URL, repo name, and more.  You should also set up
 a signing key (a temporary one might have been automatically generated).
 
 For more info: https://f-droid.org/docs/Setup_an_F-Droid_App_Repo
-and https://f-droid.org/docs/Signing_Process'''
+and https://f-droid.org/docs/Signing_Process"""
         )
         % os.path.join(fdroiddir, 'repo')
     )
     if not options.quiet:
         # normally, INFO is only shown with --verbose, but show this unless --quiet
         logger = logging.getLogger()
         logger.setLevel(logging.INFO)
```

### Comparing `fdroidserver-2.3a0/fdroidserver/install.py` & `fdroidserver-2.3a1/fdroidserver/install.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 import logging
 
 from . import _
 from . import common
 from .common import SdkToolsPopen
 from .exception import FDroidException
 
-options = None
 config = None
 
 
 def devices():
     p = SdkToolsPopen(['adb', "devices"])
     if p.returncode != 0:
         raise FDroidException("An error occured when finding devices: %s" % p.output)
@@ -40,15 +39,15 @@
     if len(lines) < 3:
         return []
     lines = lines[1:-1]
     return [line.split()[0] for line in lines]
 
 
 def main():
-    global options, config
+    global config
 
     # Parse command line...
     parser = ArgumentParser(
         usage="%(prog)s [options] [APPID[:VERCODE] [APPID[:VERCODE] ...]]"
     )
     common.setup_global_opts(parser)
     parser.add_argument(
@@ -59,25 +58,25 @@
     parser.add_argument(
         "-a",
         "--all",
         action="store_true",
         default=False,
         help=_("Install all signed applications available"),
     )
-    options = parser.parse_args()
+    options = common.parse_args(parser)
 
     common.set_console_logging(options.verbose)
 
     if not options.appid and not options.all:
         parser.error(
             _("option %s: If you really want to install all the signed apps, use --all")
             % "all"
         )
 
-    config = common.read_config(options)
+    config = common.read_config()
 
     output_dir = 'repo'
     if not os.path.isdir(output_dir):
         logging.info(_("No signed output directory - nothing to do"))
         sys.exit(0)
 
     if options.appid:
```

### Comparing `fdroidserver-2.3a0/fdroidserver/lint.py` & `fdroidserver-2.3a1/fdroidserver/lint.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 from . import _
 from . import common
 from . import metadata
 from . import rewritemeta
 
 config = None
-options = None
 
 
 def enforce_https(domain):
     return (
         re.compile(
             r'^http://([^/]*\.)?' + re.escape(domain) + r'(/.*)?', re.IGNORECASE
         ),
@@ -210,15 +209,15 @@
             re.compile(
                 r'.*<(applet|base|body|button|embed|form|head|html|iframe|img|input|link|object|picture|script|source|style|svg|video).*',
                 re.IGNORECASE,
             ),
             _("Forbidden HTML tags"),
         ),
         (
-            re.compile(r'''.*\s+src=["']javascript:.*'''),
+            re.compile(r""".*\s+src=["']javascript:.*"""),
             _("Javascript in HTML src attributes"),
         ),
     ],
 }
 
 locale_pattern = re.compile(r"[a-z]{2,3}(-([A-Z][a-zA-Z]+|\d+|[a-z]+))*")
 
@@ -455,17 +454,20 @@
                 if '@' in srclib:
                     ref = srclib.split('@')[1].split('/')[0]
                     if ref.startswith(s):
                         yield _(
                             "Branch '{branch}' used as commit in srclib '{srclib}'"
                         ).format(branch=s, srclib=srclib)
                 else:
-                    yield _(
-                        'srclibs missing name and/or @'
-                    ) + ' (srclibs: ' + srclib + ')'
+                    yield (
+                        _('srclibs missing name and/or @')
+                        + ' (srclibs: '
+                        + srclib
+                        + ')'
+                    )
         for key in build.keys():
             if key not in supported_flags:
                 yield _('%s is not an accepted build field') % key
 
 
 def check_files_dir(app):
     dir_path = Path('metadata') / app.id
@@ -496,15 +498,15 @@
     for name in files.difference(used):
         if locale_pattern.fullmatch(name):
             continue
         yield _("Unused file at %s") % (dir_path / name)
 
 
 def check_format(app):
-    if options.format and not rewritemeta.proper_format(app):
+    if common.options.format and not rewritemeta.proper_format(app):
         yield _("Run rewritemeta to fix formatting")
 
 
 def check_license_tag(app):
     """Ensure all license tags contain only valid/approved values."""
     if config['lint_licenses'] is None:
         return
@@ -718,15 +720,21 @@
 def check_updates_ucm_http_aum_pattern(app):  # noqa: D403
     """AutoUpdateMode with UpdateCheckMode: HTTP must have a pattern."""
     if app.UpdateCheckMode == "HTTP" and app.AutoUpdateMode == "Version":
         yield _("AutoUpdateMode with UpdateCheckMode: HTTP must have a pattern.")
 
 
 def check_certificate_pinned_binaries(app):
-    if len(app.get('AllowedAPKSigningKeys')) > 0:
+    keys = app.get('AllowedAPKSigningKeys')
+    known_keys = common.config.get('apk_signing_key_block_list', [])
+    if keys:
+        if known_keys:
+            for key in keys:
+                if key in known_keys:
+                    yield _('Known debug key is used in AllowedAPKSigningKeys: ') + key
         return
     if app.get('Binaries') is not None:
         yield _(
             'App has Binaries but does not have corresponding AllowedAPKSigningKeys to pin certificate.'
         )
         return
     builds = app.get('Builds')
@@ -774,15 +782,15 @@
                     msg += _('Did you mean {code}?').format(code=', '.join(sorted(m)))
                 print(msg)
 
     return passed
 
 
 def main():
-    global config, options
+    global config
 
     # Parse command line...
     parser = ArgumentParser()
     common.setup_global_opts(parser)
     parser.add_argument(
         "-f",
         "--format",
@@ -799,18 +807,18 @@
             "This option forces yamllint regardless."
         ),
     )
     parser.add_argument(
         "appid", nargs='*', help=_("application ID of file to operate on")
     )
     metadata.add_metadata_arguments(parser)
-    options = parser.parse_args()
+    options = common.parse_args(parser)
     metadata.warnings_action = options.W
 
-    config = common.read_config(options)
+    config = common.read_config()
     load_antiFeatures_config()
     load_categories_config()
 
     if options.force_yamllint:
         import yamllint  # throw error if it is not installed
 
         yamllint  # make pyflakes ignore this
```

### Comparing `fdroidserver-2.3a0/fdroidserver/looseversion.py` & `fdroidserver-2.3a1/fdroidserver/looseversion.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/fdroidserver/metadata.py` & `fdroidserver-2.3a1/fdroidserver/metadata.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/fdroidserver/mirror.py` & `fdroidserver-2.3a1/fdroidserver/mirror.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,17 @@
 import urllib.parse
 
 from . import _
 from . import common
 from . import index
 from . import update
 
-options = None
 
-
-def _run_wget(path, urls):
-    if options.verbose:
+def _run_wget(path, urls, verbose=False):
+    if verbose:
         verbose = '--verbose'
     else:
         verbose = '--no-verbose'
 
     if not urls:
         return
     logging.debug(_('Running wget in {path}').format(path=path))
@@ -44,16 +42,14 @@
         ]
     )
     os.remove(urls_file)
     os.chdir(cwd)  # leave the working env the way we found it
 
 
 def main():
-    global options
-
     parser = ArgumentParser()
     common.setup_global_opts(parser)
     parser.add_argument(
         "url",
         nargs='?',
         help=_(
             'Base URL to mirror, can include the index signing key '
@@ -89,15 +85,15 @@
         action='store_true',
         default=False,
         help=_("Include the source tarballs in the mirror"),
     )
     parser.add_argument(
         "--output-dir", default=None, help=_("The directory to write the mirror to")
     )
-    options = parser.parse_args()
+    options = common.parse_args(parser)
 
     common.set_console_logging(options.verbose)
 
     if options.all:
         options.archive = True
         options.build_logs = True
         options.pgp_signatures = True
@@ -115,15 +111,15 @@
         """Append the list of path components to URL, keeping the rest the same."""
         newpath = posixpath.join(path, *args)
         return urllib.parse.urlunparse(
             (scheme, hostname, newpath, params, query, fragment)
         )
 
     if fingerprint:
-        config = common.read_config(options)
+        config = common.read_config()
         if not ('jarsigner' in config or 'apksigner' in config):
             logging.error(
                 _('Java JDK not found! Install in standard location or set java_paths!')
             )
             sys.exit(1)
 
         def _get_index(section, etag=None):
@@ -225,37 +221,41 @@
                         if options.pgp_signatures:
                             urls.append(_append_to_url_path(section, f + '.asc'))
                         if options.build_logs and f.endswith('.apk'):
                             urls.append(
                                 _append_to_url_path(section, f[:-4] + '.log.gz')
                             )
 
-        _run_wget(sectiondir, urls)
+        _run_wget(sectiondir, urls, options.verbose)
 
         for app in data['apps']:
             localized = app.get('localized')
             if localized:
                 for locale, d in localized.items():
                     urls = []
                     components = (section, app['packageName'], locale)
                     for k in update.GRAPHIC_NAMES:
                         f = d.get(k)
                         if f:
                             filepath_tuple = components + (f,)
                             urls.append(_append_to_url_path(*filepath_tuple))
-                    _run_wget(os.path.join(basedir, *components), urls)
+                    _run_wget(os.path.join(basedir, *components), urls, options.verbose)
                     for k in update.SCREENSHOT_DIRS:
                         urls = []
                         filelist = d.get(k)
                         if filelist:
                             components = (section, app['packageName'], locale, k)
                             for f in filelist:
                                 filepath_tuple = components + (f,)
                                 urls.append(_append_to_url_path(*filepath_tuple))
-                            _run_wget(os.path.join(basedir, *components), urls)
+                            _run_wget(
+                                os.path.join(basedir, *components),
+                                urls,
+                                options.verbose,
+                            )
 
         urls = dict()
         for app in data['apps']:
             if 'icon' not in app:
                 logging.error(
                     _('no "icon" in {appid}').format(appid=app['packageName'])
                 )
@@ -264,12 +264,17 @@
             for icondir in icondirs:
                 url = _append_to_url_path(section, icondir, icon)
                 if icondir not in urls:
                     urls[icondir] = []
                 urls[icondir].append(url)
 
         for icondir in icondirs:
-            _run_wget(os.path.join(basedir, section, icondir), urls[icondir])
+            if icondir in urls:
+                _run_wget(
+                    os.path.join(basedir, section, icondir),
+                    urls[icondir],
+                    options.verbose,
+                )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fdroidserver-2.3a0/fdroidserver/net.py` & `fdroidserver-2.3a1/fdroidserver/net.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/fdroidserver/nightly.py` & `fdroidserver-2.3a1/fdroidserver/nightly.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+"""Set up an app build for a nightly build repo."""
 #
 # nightly.py - part of the FDroid server tools
 # Copyright (C) 2017 Hans-Christoph Steiner <hans@eds.org>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -28,14 +29,15 @@
 import ssl
 import subprocess
 import sys
 import tempfile
 import yaml
 from urllib.parse import urlparse
 from argparse import ArgumentParser
+from typing import Optional
 
 from . import _
 from . import common
 from .exception import VCSException
 
 # hard coded defaults for Android ~/.android/debug.keystore files
 # https://developers.google.com/android/guides/client-auth
@@ -44,20 +46,46 @@
 KEY_ALIAS = 'androiddebugkey'
 DISTINGUISHED_NAME = 'CN=Android Debug,O=Android,C=US'
 
 # standard suffix for naming fdroid git repos
 NIGHTLY = '-nightly'
 
 
-def _get_keystore_secret_var(keystore):
+def _get_keystore_secret_var(keystore: str) -> str:
+    """Get keystore secret as base64.
+
+    Parameters
+    ----------
+    keystore
+        The path of the keystore.
+
+    Returns
+    -------
+    base64_secret
+        The keystore secret as base64 string.
+    """
     with open(keystore, 'rb') as fp:
         return base64.standard_b64encode(fp.read()).decode('ascii')
 
 
-def _ssh_key_from_debug_keystore(keystore=None):
+def _ssh_key_from_debug_keystore(keystore: Optional[str] = None) -> str:
+    """Convert a debug keystore to an SSH private key.
+
+    This leaves the original keystore file in place.
+
+    Parameters
+    ----------
+    keystore
+        The keystore to convert to a SSH private key.
+
+    Returns
+    -------
+    key_path
+        The SSH private key file path in the temporary directory.
+    """
     if keystore is None:
         # set this here so it can be overridden in the tests
         # TODO convert this to a class to get rid of this nonsense
         keystore = KEYSTORE_FILE
     tmp_dir = tempfile.mkdtemp(prefix='.')
     privkey = os.path.join(tmp_dir, '.privkey')
     key_pem = os.path.join(tmp_dir, '.key.pem')
@@ -144,26 +172,53 @@
         fp.write(pub)
 
     logging.info(_('\nSSH public key to be used as deploy key:') + '\n' + pub)
 
     return ssh_private_key_file
 
 
-def get_repo_base_url(clone_url, repo_git_base, force_type=None):
+def get_repo_base_url(clone_url: str, repo_git_base: str, force_type: Optional[str] = None) -> str:
+    """Generate the base URL for the F-Droid repository.
+
+    Parameters
+    ----------
+    clone_url
+        The URL to clone the Git repository.
+    repo_git_base
+        The project path of the Git repository at the Git forge.
+    force_type
+        The Git forge of the project.
+
+    Returns
+    -------
+    repo_base_url
+        The base URL of the F-Droid repository.
+    """
     if force_type is None:
         force_type = urlparse(clone_url).netloc
     if force_type == 'gitlab.com':
         return clone_url + '/-/raw/master/fdroid'
     if force_type == 'github.com':
         return 'https://raw.githubusercontent.com/%s/master/fdroid' % repo_git_base
     print(_('ERROR: unsupported git host "%s", patches welcome!') % force_type)
     sys.exit(1)
 
 
 def main():
+    """Deploy to F-Droid repository or generate SSH private key from keystore.
+
+    The behaviour of this function is influenced by the configuration file as
+    well as command line parameters.
+
+    Raises
+    ------
+    :exc:`~fdroidserver.exception.VCSException`
+        If the nightly Git repository could not be cloned during an attempt to
+        deploy.
+    """
     parser = ArgumentParser()
     common.setup_global_opts(parser)
     parser.add_argument(
         "--keystore",
         default=KEYSTORE_FILE,
         help=_("Specify which debug keystore file to use."),
     )
@@ -200,16 +255,15 @@
     parser.add_argument(
         "--archive-older",
         type=int,
         default=archive_older_unset,
         help=_("Set maximum releases in repo before older ones are archived"),
     )
     # TODO add --with-btlog
-    options = parser.parse_args()
-    common.options = options
+    options = common.parse_args(parser)
 
     # force a tighter umask since this writes private key material
     umask = os.umask(0o077)
 
     if 'CI' in os.environ:
         v = os.getenv('DEBUG_KEYSTORE')
         debug_keystore = None
@@ -369,15 +423,15 @@
             'keydname': DISTINGUISHED_NAME,
             'make_current_version_link': False,
             'update_stats': True,
         }
         with open('config.yml', 'w') as fp:
             yaml.dump(config, fp, default_flow_style=False)
         os.chmod('config.yml', 0o600)
-        config = common.read_config(options)
+        config = common.read_config()
         common.assert_config_keystore(config)
 
         for root, dirs, files in os.walk(cibase):
             for d in dirs:
                 if d == '.git' or d == '.gradle' or (d == 'fdroid' and root == cibase):
                     dirs.remove(d)
             for f in files:
```

### Comparing `fdroidserver-2.3a0/fdroidserver/publish.py` & `fdroidserver-2.3a1/fdroidserver/publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 from . import _
 from . import common
 from . import metadata
 from .common import FDroidPopen
 from .exception import BuildException, FDroidException
 
 config = None
-options = None
 start_timestamp = time.gmtime()
 
 
 def publish_source_tarball(apkfilename, unsigned_dir, output_dir):
     """Move the source tarball into the output directory..."""
     tarfilename = apkfilename[:-4] + '_src.tar.gz'
     tarfile = os.path.join(unsigned_dir, tarfilename)
@@ -265,15 +264,15 @@
             raise BuildException("Failed to generate key", p.output)
         return True
     else:
         return False
 
 
 def main():
-    global config, options
+    global config
 
     # Parse command line...
     parser = ArgumentParser(
         usage="%(prog)s [options] " "[APPID[:VERCODE] [APPID[:VERCODE] ...]]"
     )
     common.setup_global_opts(parser)
     parser.add_argument(
@@ -285,18 +284,18 @@
     )
     parser.add_argument(
         "appid",
         nargs='*',
         help=_("application ID with optional versionCode in the form APPID[:VERCODE]"),
     )
     metadata.add_metadata_arguments(parser)
-    options = parser.parse_args()
+    options = common.parse_args(parser)
     metadata.warnings_action = options.W
 
-    config = common.read_config(options)
+    config = common.read_config()
 
     if not ('jarsigner' in config and 'keytool' in config):
         logging.critical(
             _('Java JDK not found! Install in standard location or set java_paths!')
         )
         sys.exit(1)
```

### Comparing `fdroidserver-2.3a0/fdroidserver/readmeta.py` & `fdroidserver-2.3a1/fdroidserver/readmeta.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,23 +16,21 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from argparse import ArgumentParser
 from . import common
 from . import metadata
 
-options = None
-
 
 def main():
     parser = ArgumentParser()
     common.setup_global_opts(parser)
     metadata.add_metadata_arguments(parser)
     options = parser.parse_args()
     metadata.warnings_action = options.W
-    common.read_config(None)
+    common.read_config()
 
     metadata.read_metadata()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fdroidserver-2.3a0/fdroidserver/rewritemeta.py` & `fdroidserver-2.3a1/fdroidserver/rewritemeta.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from pathlib import Path
 
 from . import _
 from . import common
 from . import metadata
 
 config = None
-options = None
 
 
 def proper_format(app):
     s = io.StringIO()
     # TODO: currently reading entire file again, should reuse first
     # read in metadata.py
     cur_content = Path(app.metadatapath).read_text(encoding='utf-8')
@@ -58,33 +57,33 @@
                 continue
             new[k] = v
         newbuilds.append(new)
     return newbuilds
 
 
 def main():
-    global config, options
+    global config
 
     parser = ArgumentParser()
     common.setup_global_opts(parser)
     parser.add_argument(
         "-l",
         "--list",
         action="store_true",
         default=False,
         help=_("List files that would be reformatted (dry run)"),
     )
     parser.add_argument(
         "appid", nargs='*', help=_("application ID of file to operate on")
     )
     metadata.add_metadata_arguments(parser)
-    options = parser.parse_args()
+    options = common.parse_args(parser)
     metadata.warnings_action = options.W
 
-    config = common.read_config(options)
+    config = common.read_config()
 
     # Get all apps...
     allapps = metadata.read_metadata(options.appid)
     apps = common.read_app_args(options.appid, allapps, False)
 
     for appid, app in apps.items():
         path = Path(app.metadatapath)
```

### Comparing `fdroidserver-2.3a0/fdroidserver/scanner.py` & `fdroidserver-2.3a1/fdroidserver/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,14 @@
 
 from . import _
 from . import common
 from . import metadata
 from .exception import BuildException, VCSException, ConfigurationException
 from . import scanner
 
-options = None
-
 
 @dataclass
 class MessageStore:
     infos: list = field(default_factory=list)
     warnings: list = field(default_factory=list)
     errors: list = field(default_factory=list)
 
@@ -328,16 +326,17 @@
 class ScannerTool:
     def __init__(self):
         # we could add support for loading additional signature source
         # definitions from config.yml here
 
         self.scanner_data_lookup()
 
-        config = common.get_config()
-        if (options and options.refresh_scanner) or config.get('refresh_scanner'):
+        options = common.get_options()
+        options_refresh_scanner = options and options.refresh_scanner
+        if options_refresh_scanner or common.get_config().get('refresh_scanner'):
             self.refresh()
 
         self.load()
         self.compile_regexes()
 
     def scanner_data_lookup(self):
         sigsources = common.get_config().get('scanner_signature_sources', [])
@@ -585,14 +584,15 @@
         filepath
           Path (relative to our current path) to the file
 
         Returns
         -------
         0 if the problem was ignored/deleted/is only a warning, 1 otherwise
         """
+        options = common.get_options()
         if toignore(path_in_build_dir):
             return ignoreproblem(what, path_in_build_dir, json_per_build)
         if todelete(path_in_build_dir):
             return removeproblem(what, path_in_build_dir, filepath, json_per_build)
         if 'src/test' in path_in_build_dir or '/test/' in path_in_build_dir:
             return warnproblem(what, path_in_build_dir, json_per_build)
         if options and 'json' in vars(options) and options.json:
@@ -772,43 +772,40 @@
             logging.error(_('Unused scandelete path: %s') % p)
             count += 1
 
     return count
 
 
 def main():
-    global options
-
-    # Parse command line...
     parser = ArgumentParser(
         usage="%(prog)s [options] [(APPID[:VERCODE] | path/to.apk) ...]"
     )
     common.setup_global_opts(parser)
     parser.add_argument("appid", nargs='*', help=_("application ID with optional versionCode in the form APPID[:VERCODE]"))
     parser.add_argument("-f", "--force", action="store_true", default=False,
                         help=_("Force scan of disabled apps and builds."))
     parser.add_argument("--json", action="store_true", default=False,
                         help=_("Output JSON to stdout."))
     parser.add_argument("-r", "--refresh", dest="refresh_scanner", action="store_true", default=False,
                         help=_("fetch the latest version of signatures from the web"))
     parser.add_argument("-e", "--exit-code", action="store_true", default=False,
                         help=_("Exit with a non-zero code if problems were found"))
     metadata.add_metadata_arguments(parser)
-    options = parser.parse_args()
+    options = common.parse_args(parser)
     metadata.warnings_action = options.W
 
     json_output = dict()
     if options.json:
         if options.verbose:
             logging.basicConfig(stream=sys.stderr, level=logging.DEBUG)
         else:
             logging.getLogger().setLevel(logging.ERROR)
 
     # initialize/load configuration values
-    common.get_config(opts=options)
+    common.get_config()
 
     probcount = 0
 
     appids = []
     for apk in options.appid:
         if os.path.isfile(apk):
             count = scanner.scan_binary(apk)
```

### Comparing `fdroidserver-2.3a0/fdroidserver/signatures.py` & `fdroidserver-2.3a1/fdroidserver/signatures.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,12 @@
 def main():
     parser = ArgumentParser()
     common.setup_global_opts(parser)
     parser.add_argument(
         "APK", nargs='*', help=_("signed APK, either a file-path or HTTPS URL.")
     )
     parser.add_argument("--no-check-https", action="store_true", default=False)
-    options = parser.parse_args()
-
+    options = common.parse_args(parser)
     common.set_console_logging(options.verbose)
-
-    # Read config.py...
-    common.read_config(options)
+    common.read_config()
 
     extract(options)
```

### Comparing `fdroidserver-2.3a0/fdroidserver/signindex.py` & `fdroidserver-2.3a1/fdroidserver/signindex.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 from . import _
 from . import common
 from . import metadata
 from .exception import FDroidException
 
 config = None
-options = None
 start_timestamp = time.gmtime()
 
 
 def sign_jar(jar, use_old_algs=False):
     """Sign a JAR file with the best available algorithm.
 
     The current signing method uses apksigner to sign the JAR so that
@@ -171,21 +170,21 @@
     output = common.setup_status_output(start_timestamp)
     if signed:
         output['signed'] = signed
     common.write_status_json(output)
 
 
 def main():
-    global config, options
+    global config
 
     parser = ArgumentParser()
     common.setup_global_opts(parser)
-    options = parser.parse_args()
+    common.parse_args(parser)
 
-    config = common.read_config(options)
+    config = common.read_config()
 
     if 'jarsigner' not in config:
         raise FDroidException(
             _(
                 'Java jarsigner not found! Install in standard location or set java_paths!'
             )
         )
```

### Comparing `fdroidserver-2.3a0/fdroidserver/tail.py` & `fdroidserver-2.3a1/fdroidserver/tail.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/fdroidserver/update.py` & `fdroidserver-2.3a1/fdroidserver/update.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 import warnings
 import zipfile
 import hashlib
 import json
 import time
 import yaml
 import copy
+import asn1crypto.cms
 import defusedxml.ElementTree as ElementTree
 from datetime import datetime, timezone
 from argparse import ArgumentParser
 from pathlib import Path
 
 try:
     from yaml import CSafeLoader as SafeLoader
@@ -540,33 +541,113 @@
         raise ValueError(f"invalid version string '{version}'")
     major = int(m.group(1))
     minor = int(m.group(2))
     patch = int(m.group(3))
     return major * 10**12 + minor * 10**6 + patch
 
 
+# iOS app permissions, source:
+# https://developer.apple.com/documentation/bundleresources/information_property_list/protected_resources
+IPA_PERMISSIONS = [
+    "NSBluetoothAlwaysUsageDescription",
+    "NSBluetoothPeripheralUsageDescription",
+    "NSCalendarsFullAccessUsageDescription",
+    "NSCalendarsWriteOnlyAccessUsageDescription",
+    "NSRemindersFullAccessUsageDescription",
+    "NSCameraUsageDescription",
+    "NSMicrophoneUsageDescription",
+    "NSContactsUsageDescription",
+    "NSFaceIDUsageDescription",
+    "NSDesktopFolderUsageDescription",
+    "NSDocumentsFolderUsageDescription",
+    "NSDownloadsFolderUsageDescription",
+    "NSNetworkVolumesUsageDescription",
+    "NSNetworkVolumesUsageDescription",
+    "NSRemovableVolumesUsageDescription",
+    "NSRemovableVolumesUsageDescription",
+    "NSFileProviderDomainUsageDescription",
+    "NSGKFriendListUsageDescription",
+    "NSHealthClinicalHealthRecordsShareUsageDescription",
+    "NSHealthShareUsageDescription",
+    "NSHealthUpdateUsageDescription",
+    "NSHomeKitUsageDescription",
+    "NSLocationAlwaysAndWhenInUseUsageDescription",
+    "NSLocationUsageDescription",
+    "NSLocationWhenInUseUsageDescription",
+    "NSLocationAlwaysUsageDescription",
+    "NSAppleMusicUsageDescription",
+    "NSMotionUsageDescription",
+    "NSFallDetectionUsageDescription",
+    "NSLocalNetworkUsageDescription",
+    "NSNearbyInteractionUsageDescription",
+    "NSNearbyInteractionAllowOnceUsageDescription",
+    "NFCReaderUsageDescription",
+    "NSPhotoLibraryAddUsageDescription",
+    "NSPhotoLibraryUsageDescription",
+    "NSAppDataUsageDescription",
+    "NSUserTrackingUsageDescription",
+    "NSAppleEventsUsageDescription",
+    "NSSystemAdministrationUsageDescription",
+    "NSSensorKitUsageDescription",
+    "NSSiriUsageDescription",
+    "NSSpeechRecognitionUsageDescription",
+    "NSVideoSubscriberAccountUsageDescription",
+    "NSWorldSensingUsageDescription",
+    "NSHandsTrackingUsageDescription",
+    "NSIdentityUsageDescription",
+    "NSCalendarsUsageDescription",
+    "NSRemindersUsageDescription",
+]
+
+
 def parse_ipa(ipa_path, file_size, sha256):
-    from biplist import readPlist
+    import biplist
 
     ipa = {
         "apkName": os.path.basename(ipa_path),
         "hash": sha256,
         "hashType": "sha256",
         "size": file_size,
+        "ipa_entitlements": set(),
+        "ipa_permissions": {},
     }
 
     with zipfile.ZipFile(ipa_path) as ipa_zip:
         for info in ipa_zip.infolist():
             if re.match("Payload/[^/]*.app/Info.plist", info.filename):
                 with ipa_zip.open(info) as plist_file:
-                    plist = readPlist(plist_file)
+                    plist = biplist.readPlist(plist_file)
+                    ipa["name"] = plist['CFBundleName']
                     ipa["packageName"] = plist["CFBundleIdentifier"]
                     # https://developer.apple.com/documentation/bundleresources/information_property_list/cfbundleshortversionstring
                     ipa["versionCode"] = version_string_to_int(plist["CFBundleShortVersionString"])
                     ipa["versionName"] = plist["CFBundleShortVersionString"]
+                    ipa["ipa_MinimumOSVersion"] = plist['MinimumOSVersion']
+                    ipa["ipa_DTPlatformVersion"] = plist['DTPlatformVersion']
+                    for ipap in IPA_PERMISSIONS:
+                        if ipap in plist:
+                            ipa["ipa_permissions"][ipap] = str(plist[ipap])
+            if info.filename.endswith("/embedded.mobileprovision"):
+                print("parsing", info.filename)
+                with ipa_zip.open(info) as mopro_file:
+                    mopro_content_info = asn1crypto.cms.ContentInfo.load(
+                        mopro_file.read()
+                    )
+                    mopro_payload_info = mopro_content_info['content']
+                    mopro_payload = mopro_payload_info['encap_content_info'][
+                        'content'
+                    ].native
+                    mopro = biplist.readPlistFromString(mopro_payload)
+                    # https://faq.altstore.io/distribute-your-apps/make-a-source#entitlements-array-of-strings
+                    for entitlement in mopro.get('Entitlements', {}).keys():
+                        if entitlement not in [
+                            "com.app.developer.team-identifier",
+                            'application-identifier'
+                        ]:
+                            ipa["ipa_entitlements"].add(entitlement)
     return ipa
 
 
 def scan_repo_for_ipas(apkcache, repodir, knownapks):
     """Scan for IPA files in a given repo directory.
 
     Parameters
@@ -588,16 +669,15 @@
     cachechanged = False
     ipas = []
     for ipa_path in glob.glob(os.path.join(repodir, '*.ipa')):
         ipa_name = os.path.basename(ipa_path)
 
         file_size = os.stat(ipa_path).st_size
         if file_size == 0:
-            raise FDroidException(_('{path} is zero size!')
-                                  .format(path=ipa_path))
+            raise FDroidException(_('{path} is zero size!').format(path=ipa_path))
 
         sha256 = common.sha256sum(ipa_path)
         ipa = apkcache.get(ipa_name, {})
 
         if ipa.get('hash') != sha256:
             ipa = fdroidserver.update.parse_ipa(ipa_path, file_size, sha256)
             apkcache[ipa_name] = ipa
@@ -1342,19 +1422,36 @@
             for lang_dir in fastlane_meta_dir.iterdir():
                 locale = lang_dir.name
                 m = LANG_CODE.match(locale)
                 if m:
                     for metadata_file in (lang_dir).iterdir():
                         key = FASTLANE_IOS_MAP.get(metadata_file.name)
                         if key:
-                            fdroidserver.update._set_localized_text_entry(app, locale, key, metadata_file)
+                            fdroidserver.update._set_localized_text_entry(
+                                app, locale, key, metadata_file
+                            )
 
         screenshots = fdroidserver.update.discover_ios_screenshots(fastlane_dir)
         fdroidserver.update.copy_ios_screenshots_to_repo(screenshots, package_name)
 
+        # lookup icons, copy them and put them into app
+        icon_path = _get_ipa_icon(Path('build') / package_name)
+        icon_dest = Path('repo') / package_name / 'icon.png'  # for now just assume png
+        icon_stat = os.stat(icon_path)
+        app['iconv2'] = {
+            DEFAULT_LOCALE: {
+                'name': str(icon_dest).lstrip('repo'),
+                'sha256': common.sha256sum(icon_dest),
+                'size': icon_stat.st_size,
+            }
+        }
+        if not icon_dest.exists():
+            icon_dest.parent.mkdir(parents=True, exist_ok=True)
+            shutil.copy(icon_path, icon_dest)
+
 
 def scan_repo_files(apkcache, repodir, knownapks, use_date_from_file=False):
     """Scan a repo for all files with an extension except APK/OBB/IPA.
 
     This allows putting all kinds of files into repostories. E.g. Media Files,
     Zip archives, ...
 
@@ -1544,14 +1641,68 @@
                     density = '160'
                 icons_src[density] = m.group(0)
     if icons_src.get('-1') is None and '160' in icons_src:
         icons_src['-1'] = icons_src['160']
     return icons_src
 
 
+def _get_ipa_icon(src_dir):
+    """Search source directory of an IPA project for the app icon."""
+    # parse app icon name from project config file
+    src_dir = Path(src_dir)
+    prj = next(src_dir.glob("**/project.pbxproj"), None)
+    if not prj or not prj.exists():
+        return
+
+    icon_name = _parse_from_pbxproj(prj, 'ASSETCATALOG_COMPILER_APPICON_NAME')
+    if not icon_name:
+        return
+
+    icon_dir = next(src_dir.glob(f'**/{icon_name}.appiconset'), None)
+    if not icon_dir:
+        return
+
+    with open(icon_dir / "Contents.json") as f:
+        cntnt = json.load(f)
+
+    fname = None
+    fsize = 0
+    for image in cntnt['images']:
+        s = float(image.get("size", "0x0").split("x")[0])
+        if image.get('scale') == "1x" and s > fsize and s <= 128:
+            fname = image['filename']
+            fsize = s
+
+    return str(icon_dir / fname)
+
+
+def _parse_from_pbxproj(pbxproj_path, key):
+    """Parse values from apple project files.
+
+    This is a naive regex based parser. Should this proofe to unreliable we
+    might want to consider using a dedicated pbxproj parser:
+    https://pypi.org/project/pbxproj/
+
+    e.g. when looking for key 'ASSETCATALOG_COMPILER_APPICON_NAME'
+    This function will extract 'MyIcon' from if the provided file
+    contains this line:
+
+        ASSETCATALOG_COMPILER_APPICON_NAME = MyIcon;
+
+    returns None if parsing for that value didn't yield anything
+    """
+    r = re.compile(f"\\s*{key}\\s*=\\s*(?P<value>[a-zA-Z0-9-_]+)\\s*;\\s*")
+    with open(pbxproj_path, 'r', encoding='utf-8') as f:
+        for line in f.readlines():
+            m = r.match(line)
+            if m:
+                return m.group("value")
+    return None
+
+
 def _sanitize_sdk_version(value):
     """Sanitize the raw values from androguard to handle bad values.
 
     minSdkVersion/targetSdkVersion/maxSdkVersion must be integers, but
     that doesn't stop devs from doing strange things like setting them
     using Android XML strings. This method makes the Androguard output
     match the output from `aapt dump badging`: bad values are ignored.
@@ -1567,16 +1718,15 @@
     except (TypeError, ValueError):
         pass
     return None
 
 
 def scan_apk_androguard(apk, apkfile):
     try:
-        from androguard.core.bytecodes.apk import APK
-        apkobject = APK(apkfile)
+        apkobject = common.get_androguard_APK(apkfile)
         if apkobject.is_valid_APK():
             arsc = apkobject.get_android_resources()
         else:
             if options.delete_unknown:
                 if os.path.exists(apkfile):
                     logging.error(_("Failed to get APK information, deleting {path}")
                                   .format(path=apkfile))
@@ -1584,15 +1734,15 @@
                 else:
                     logging.error(_("Could not find {path} to remove it")
                                   .format(path=apkfile))
             else:
                 logging.error(_("Failed to get APK information, skipping {path}")
                               .format(path=apkfile))
             raise BuildException(_("Invalid APK"))
-    except (FileNotFoundError, zipfile.BadZipFile) as e:
+    except (FileNotFoundError, ValueError, zipfile.BadZipFile) as e:
         logging.error(_("Could not open APK {path} for analysis: ").format(path=apkfile)
                       + str(e))
         raise BuildException(_("Invalid APK")) from e
 
     apk['packageName'] = apkobject.get_package()
 
     xml = apkobject.get_android_manifest_xml()
@@ -1624,15 +1774,15 @@
     if targetSdkVersion is not None:
         apk['targetSdkVersion'] = targetSdkVersion
 
     maxSdkVersion = _sanitize_sdk_version(apkobject.get_max_sdk_version())
     if maxSdkVersion is not None:
         apk['maxSdkVersion'] = maxSdkVersion
 
-    icon_id_str = apkobject.get_element("application", "icon")
+    icon_id_str = apkobject.get_attribute_value("application", "icon")
     if icon_id_str:
         try:
             icon_id = int(icon_id_str.replace("@", "0x"), 16)
             resource_id = arsc.get_id(apk['packageName'], icon_id)
             if resource_id:
                 icon_name = arsc.get_id(apk['packageName'], icon_id)[1]
             else:
@@ -2420,21 +2570,20 @@
     parser.add_argument("--use-date-from-apk", action="store_true", default=False,
                         help=_("Use date from APK instead of current time for newly added APKs"))
     parser.add_argument("--rename-apks", action="store_true", default=False,
                         help=_("Rename APK files that do not match package.name_123.apk"))
     parser.add_argument("--allow-disabled-algorithms", action="store_true", default=False,
                         help=_("Include APKs that are signed with disabled algorithms like MD5"))
     metadata.add_metadata_arguments(parser)
-    options = parser.parse_args()
+    options = common.parse_args(parser)
     metadata.warnings_action = options.W
 
-    config = common.read_config(options)
+    config = common.read_config()
     common.setup_status_output(start_timestamp)
 
-    common.use_androguard()
     if not (('jarsigner' in config or 'apksigner' in config)
             and 'keytool' in config):
         raise FDroidException(_('Java JDK not found! Install in standard location or set java_paths!'))
 
     repodirs = ['repo']
     if config['archive_older'] != 0:
         repodirs.append('archive')
```

### Comparing `fdroidserver-2.3a0/fdroidserver/verify.py` & `fdroidserver-2.3a1/fdroidserver/verify.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from collections import OrderedDict
 
 from . import _
 from . import common
 from . import net
 from .exception import FDroidException
 
-options = None
 config = None
 
 
 def _add_diffoscope_info(d):
     """Add diffoscope setup metadata to provided dict under 'diffoscope' key.
 
     The imports are broken out at stages since various versions of
@@ -142,15 +141,15 @@
         if not found:
             data['packages'][packageName].insert(0, json.loads(output_dump))
         with open(jsonfile, 'w') as fp:
             json.dump(data, fp, cls=common.Encoder, sort_keys=True)
 
 
 def main():
-    global options, config
+    global config
 
     # Parse command line...
     parser = ArgumentParser(
         usage="%(prog)s [options] [APPID[:VERCODE] [APPID[:VERCODE] ...]]"
     )
     common.setup_global_opts(parser)
     parser.add_argument(
@@ -166,17 +165,17 @@
     )
     parser.add_argument(
         "--output-json",
         action="store_true",
         default=False,
         help=_("Output JSON report to file named after APK."),
     )
-    options = parser.parse_args()
+    options = common.parse_args(parser)
 
-    config = common.read_config(options)
+    config = common.read_config()
 
     tmp_dir = 'tmp'
     if not os.path.isdir(tmp_dir):
         logging.info(_("Creating temporary directory"))
         os.makedirs(tmp_dir)
 
     unsigned_dir = 'unsigned'
```

### Comparing `fdroidserver-2.3a0/fdroidserver/vmtools.py` & `fdroidserver-2.3a1/fdroidserver/vmtools.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/fdroidserver.egg-info/PKG-INFO` & `fdroidserver-2.3a1/fdroidserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdroidserver
-Version: 2.3a0
+Version: 2.3a1
 Summary: F-Droid Server Tools
 Home-page: https://f-droid.org
 Author: The F-Droid Project
 Author-email: team@f-droid.org
 License: AGPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `fdroidserver-2.3a0/fdroidserver.egg-info/SOURCES.txt` & `fdroidserver-2.3a1/fdroidserver.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,16 @@
 locale/sq/LC_MESSAGES/fdroidserver.po
 locale/tr/LC_MESSAGES/fdroidserver.po
 locale/uk/LC_MESSAGES/fdroidserver.po
 locale/zh_Hans/LC_MESSAGES/fdroidserver.po
 locale/zh_Hant/LC_MESSAGES/fdroidserver.po
 tests/IsMD5Disabled.java
 tests/Norway_bouvet_europe_2.obf.zip
+tests/SANAPPSI.RSA
+tests/SANAPPSI.SF
 tests/SpeedoMeterApp.main_1.apk
 tests/aosp_testkey_debug.keystore
 tests/apk.embedded_1.apk
 tests/bad-unicode-πÇÇ现代通用字-български-عربي1.apk
 tests/build.TestCase
 tests/check-fdroid-apk
 tests/checkupdates.TestCase
@@ -103,14 +105,19 @@
 tests/funding-usernames.yaml
 tests/gradle-maven-blocks.yaml
 tests/gradle-release-checksums.py
 tests/import_subcommand.TestCase
 tests/index.TestCase
 tests/init.TestCase
 tests/install.TestCase
+tests/issue-1128-min-sdk-30-poc.apk
+tests/issue-1128-poc1.apk
+tests/issue-1128-poc2.apk
+tests/issue-1128-poc3a.apk
+tests/issue-1128-poc3b.apk
 tests/janus.apk
 tests/key-tricks.py
 tests/keystore.jks
 tests/lint.TestCase
 tests/main.TestCase
 tests/metadata.TestCase
 tests/minimal_targetsdk_30_unsigned.apk
```

### Comparing `fdroidserver-2.3a0/gradlew-fdroid` & `fdroidserver-2.3a1/gradlew-fdroid`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/bo/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/bo/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/cs/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/cs/LC_MESSAGES/fdroidserver.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 # This file is put in the public domain.
 # mondstern <mondstern@snopyta.org>, 2021.
 # Petr Novák <nit.monkey@gmail.com>, 2021.
 # Fjuro <fjuro@seznam.cz>, 2022.
 # Filip Klopec <filipklopec@gmail.com>, 2022.
 # Fjuro <ifjuro@proton.me>, 2022, 2023.
 # Daniel Hejduk <jellymail@protonmail.com>, 2023.
+# Fjuro <fjuro@alius.cz>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: fdroidserver 1.0.0-95-gd7af22b\n"
 "Report-Msgid-Bugs-To: https://gitlab.com/fdroid/fdroidserver/issues\n"
 "POT-Creation-Date: 2023-05-24 22:18+0200\n"
-"PO-Revision-Date: 2023-10-20 14:22+0000\n"
-"Last-Translator: Daniel Hejduk <jellymail@protonmail.com>\n"
+"PO-Revision-Date: 2024-04-23 10:07+0000\n"
+"Last-Translator: Fjuro <fjuro@alius.cz>\n"
 "Language-Team: Czech <https://hosted.weblate.org/projects/f-droid/fdroidserver/cs/>\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
-"X-Generator: Weblate 5.1\n"
+"Plural-Forms: nplurals=3; plural=((n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2);\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: ../fdroidserver/nightly.py
 msgid ""
 "\n"
 "SSH public key to be used as deploy key:"
 msgstr ""
 "\n"
@@ -1809,15 +1810,15 @@
 #, python-brace-format
 msgid "UpdateCheckData not a valid URL: {url}"
 msgstr "UpdateCheckData není platná URL: {url}"
 
 #. Translators: https://developer.android.com/studio/build/application-id
 #: ../fdroidserver/lint.py
 msgid "UpdateCheckMode is set but it looks like checkupdates hasn't been run yet."
-msgstr "UpdateCheckMode je nastaven, ale vypadá to, že checkupdates ještě nebylo spuštěno"
+msgstr "UpdateCheckMode je nastaven, ale vypadá to, že akce checkupdates ještě nebyla spuštěna."
 
 #: ../fdroidserver/lint.py
 msgid "UpdateCheckName is set to the known application ID, it can be removed"
 msgstr "UpdateCheckName je nastaveno na známé ID aplikace, lze jej odstranit"
 
 #: ../fdroidserver/deploy.py
 #, python-brace-format
```

### Comparing `fdroidserver-2.3a0/locale/de/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/de/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/es/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/es/LC_MESSAGES/fdroidserver.po`

 * *Files 1% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 # Fioddor Superconcentrado <fioddor@gmail.com>, 2021.
 # Adolfo Jayme Barrientos <fitojb@ubuntu.com>, 2021.
 # mondstern <mondstern@snopyta.org>, 2021.
 # Germe the fur star <FOSSgerme.deb@tuta.io>, 2021.
 # Iago <iagrivmoa@gmail.com>, 2022.
 # Iago <translate@delthia.com>, 2022.
 # Jaime Marquínez Ferrándiz <weblate@jregistros.fastmail.net>, 2022.
-# gallegonovato <fran-carro@hotmail.es>, 2022, 2023.
+# gallegonovato <fran-carro@hotmail.es>, 2022, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: fdroidserver 0.9\n"
 "Report-Msgid-Bugs-To: https://gitlab.com/fdroid/fdroidserver/issues\n"
 "POT-Creation-Date: 2023-05-24 22:18+0200\n"
-"PO-Revision-Date: 2023-08-01 21:07+0000\n"
+"PO-Revision-Date: 2024-04-10 18:44+0000\n"
 "Last-Translator: gallegonovato <fran-carro@hotmail.es>\n"
 "Language-Team: Spanish <https://hosted.weblate.org/projects/f-droid/fdroidserver/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: ../fdroidserver/nightly.py
 msgid ""
 "\n"
 "SSH public key to be used as deploy key:"
 msgstr ""
 "\n"
@@ -1813,19 +1813,19 @@
 #, python-brace-format
 msgid "UpdateCheckData not a valid URL: {url}"
 msgstr "UpdateCheckData tiene una URL no válida: {url}"
 
 #. Translators: https://developer.android.com/studio/build/application-id
 #: ../fdroidserver/lint.py
 msgid "UpdateCheckMode is set but it looks like checkupdates hasn't been run yet."
-msgstr "UpdateCheckMode está configurado pero parece que checkupdates aún no se ha ejecutado"
+msgstr "UpdateCheckMode está configurado pero parece que aún no se han ejecutado las actualizaciones."
 
 #: ../fdroidserver/lint.py
 msgid "UpdateCheckName is set to the known application ID, it can be removed"
-msgstr "El nombre de verificación de actualización (UpdateCheckName) es el identificador (ID) conocido de la aplicación. Se puede borrar"
+msgstr "UpdateCheckName está configurado con el ID de la aplicación conocida, se puede eliminar"
 
 #: ../fdroidserver/deploy.py
 #, python-brace-format
 msgid "Uploading {apkfilename} to androidobservatory.org"
 msgstr "Subiendo {apkfilename} a androidobservatory.org"
 
 #: ../fdroidserver/deploy.py
```

### Comparing `fdroidserver-2.3a0/locale/fr/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/fr/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/hu/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/hu/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/it/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/it/LC_MESSAGES/fdroidserver.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 # mondstern <mondstern@snopyta.org>, 2021.
 # Frankie McEyes <mceyes@protonmail.com>, 2022.
 # Antonello Pirina <fardeledge@tutanota.com>, 2022.
 # Pixel-Tux <luis.pardus@gmail.com>, 2023.
 # Davide Neri <davnerix@gmail.com>, 2023.
 # Mirko Di <mirko@mirkodi.eu>, 2023.
 # coronabond <coronabond@airmail.cc>, 2023.
-# Random <random-r@users.noreply.hosted.weblate.org>, 2023.
+# Random <random-r@users.noreply.hosted.weblate.org>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: fdroidserver 0.9\n"
 "Report-Msgid-Bugs-To: https://gitlab.com/fdroid/fdroidserver/issues\n"
 "POT-Creation-Date: 2023-05-24 22:18+0200\n"
-"PO-Revision-Date: 2023-09-06 17:31+0000\n"
+"PO-Revision-Date: 2024-04-13 17:01+0000\n"
 "Last-Translator: Random <random-r@users.noreply.hosted.weblate.org>\n"
 "Language-Team: Italian <https://hosted.weblate.org/projects/f-droid/fdroidserver/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.1-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: ../fdroidserver/nightly.py
 msgid ""
 "\n"
 "SSH public key to be used as deploy key:"
 msgstr ""
 "\n"
@@ -1817,15 +1817,15 @@
 #, python-brace-format
 msgid "UpdateCheckData not a valid URL: {url}"
 msgstr "UpdateCheckData non è un URL valido: {url}"
 
 #. Translators: https://developer.android.com/studio/build/application-id
 #: ../fdroidserver/lint.py
 msgid "UpdateCheckMode is set but it looks like checkupdates hasn't been run yet."
-msgstr "UpdateCheckMode impostato ma sembra che checkupdates non sia ancora stato eseguito"
+msgstr "UpdateCheckMode impostato ma sembra che checkupdates non sia ancora stato eseguito."
 
 #: ../fdroidserver/lint.py
 msgid "UpdateCheckName is set to the known application ID, it can be removed"
 msgstr "UpdateCheckName è impostato sull'ID dell'applicazione nota, può essere rimosso"
 
 #: ../fdroidserver/deploy.py
 #, python-brace-format
```

### Comparing `fdroidserver-2.3a0/locale/ko/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/ko/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/nb_NO/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/nb_NO/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/pl/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/pl/LC_MESSAGES/fdroidserver.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # This file is put in the public domain.
 # WaldiS <sto@tutanota.de>, 2020, 2021.
 # Michal L <michalrmsmi@wp.pl>, 2020, 2021.
 # mondstern <mondstern@snopyta.org>, 2021.
 # Hans-Christoph Steiner <hans@guardianproject.info>, 2021.
-# Agnieszka C <aga_04@o2.pl>, 2021, 2022, 2023.
+# Agnieszka C <aga_04@o2.pl>, 2021, 2022, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: fdroidserver 1.0.0-95-gd7af22b\n"
 "Report-Msgid-Bugs-To: https://gitlab.com/fdroid/fdroidserver/issues\n"
 "POT-Creation-Date: 2023-05-24 22:18+0200\n"
-"PO-Revision-Date: 2023-05-26 19:39+0000\n"
+"PO-Revision-Date: 2024-04-10 18:44+0000\n"
 "Last-Translator: Agnieszka C <aga_04@o2.pl>\n"
 "Language-Team: Polish <https://hosted.weblate.org/projects/f-droid/fdroidserver/pl/>\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.18-dev\n"
+"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: ../fdroidserver/nightly.py
 msgid ""
 "\n"
 "SSH public key to be used as deploy key:"
 msgstr ""
 "\n"
```

### Comparing `fdroidserver-2.3a0/locale/pt/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/pt/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/pt_BR/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/pt_BR/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/pt_PT/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/pt_PT/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/ro/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/ro/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/ru/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/ru/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/sq/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/sq/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/tr/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/tr/LC_MESSAGES/fdroidserver.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR Free Software Foundation, Inc.
 # Oğuz Ersen <oguzersen@protonmail.com>, 2020, 2021, 2022.
 # Orhan <orya@pm.me>, 2021.
-# Oğuz Ersen <oguz@ersen.moe>, 2022, 2023.
+# Oğuz Ersen <oguz@ersen.moe>, 2022, 2023, 2024.
 # Bai <batuhanakkurt000@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: fdroidserver 0.9\n"
 "Report-Msgid-Bugs-To: https://gitlab.com/fdroid/fdroidserver/issues\n"
 "POT-Creation-Date: 2023-05-24 22:18+0200\n"
-"PO-Revision-Date: 2023-09-09 10:53+0000\n"
-"Last-Translator: Bai <batuhanakkurt000@gmail.com>\n"
+"PO-Revision-Date: 2024-04-11 20:02+0000\n"
+"Last-Translator: Oğuz Ersen <oguz@ersen.moe>\n"
 "Language-Team: Turkish <https://hosted.weblate.org/projects/f-droid/fdroidserver/tr/>\n"
 "Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.1-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: ../fdroidserver/nightly.py
 msgid ""
 "\n"
 "SSH public key to be used as deploy key:"
 msgstr ""
 "\n"
@@ -1804,15 +1804,15 @@
 #, python-brace-format
 msgid "UpdateCheckData not a valid URL: {url}"
 msgstr "UpdateCheckData geçerli bir URL değil: {url}"
 
 #. Translators: https://developer.android.com/studio/build/application-id
 #: ../fdroidserver/lint.py
 msgid "UpdateCheckMode is set but it looks like checkupdates hasn't been run yet."
-msgstr "UpdateCheckMode ayarlı ancak checkupdates henüz çalıştırılmamış gibi görünüyor"
+msgstr "UpdateCheckMode ayarlı ancak checkupdates henüz çalıştırılmamış gibi görünüyor."
 
 #: ../fdroidserver/lint.py
 msgid "UpdateCheckName is set to the known application ID, it can be removed"
 msgstr "UpdateCheckName bilinen uygulama kimliğine ayarlı - kaldırılabilir"
 
 #: ../fdroidserver/deploy.py
 #, python-brace-format
```

### Comparing `fdroidserver-2.3a0/locale/uk/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/uk/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/locale/zh_Hans/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/zh_Hans/LC_MESSAGES/fdroidserver.po`

 * *Files 1% similar despite different names*

```diff
@@ -25,29 +25,29 @@
 # Xiang Heng Wei <yylteam@hotmail.com>, 2022, 2023.
 # RainSlide <RainSlide@outlook.com>, 2023.
 # Eric <hamburger2048@users.noreply.hosted.weblate.org>, 2023.
 # Max Xie <monyxie@gmail.com>, 2023.
 # Kingo Bingo <bingokingosoft@gmail.com>, 2023.
 # zhiqi <lzqlzq21@gmail.com>, 2023.
 # David Jiang <david.jiang2024@gmail.com>, 2023.
+# ALoLo_527 <ALoLo@users.noreply.hosted.weblate.org>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: fdroidserver 0.9\n"
 "Report-Msgid-Bugs-To: https://gitlab.com/fdroid/fdroidserver/issues\n"
 "POT-Creation-Date: 2023-05-24 22:18+0200\n"
-"PO-Revision-Date: 2023-11-05 08:05+0000\n"
-"Last-Translator: David Jiang <david.jiang2024@gmail.com>\n"
-"Language-Team: Chinese (Simplified) <https://hosted.weblate.org/projects/f-"
-"droid/fdroidserver/zh_Hans/>\n"
+"PO-Revision-Date: 2024-04-13 17:01+0000\n"
+"Last-Translator: ALoLo_527 <ALoLo@users.noreply.hosted.weblate.org>\n"
+"Language-Team: Chinese (Simplified) <https://hosted.weblate.org/projects/f-droid/fdroidserver/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.2-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: ../fdroidserver/nightly.py
 msgid ""
 "\n"
 "SSH public key to be used as deploy key:"
 msgstr ""
 "\n"
@@ -2635,30 +2635,30 @@
 #, python-brace-format
 msgid "{appid} does not have a name! Using application ID instead."
 msgstr ""
 
 #: ../fdroidserver/update.py
 #, python-brace-format
 msgid "{appid} from {path} is not a valid Android application ID!"
-msgstr ""
+msgstr "{appid}来自{path}不是一个有效的Android应用ID！"
 
 #: ../fdroidserver/metadata.py ../fdroidserver/update.py
 #, python-brace-format
 msgid "{appid} from {path} is not a valid Java Package Name!"
-msgstr ""
+msgstr "{appid}来自{path}不是一个有效的Java安装包名称！"
 
 #: ../fdroidserver/update.py
 #, python-brace-format
 msgid "{appid} has both APKs and files: {files}"
 msgstr ""
 
 #: ../fdroidserver/mirror.py
 #, python-brace-format
 msgid "{appid} is missing {name}"
-msgstr ""
+msgstr "{appid}缺失了{name}"
 
 #. Translators: https://developer.android.com/guide/topics/manifest/manifest-element.html#vname
 #: ../fdroidserver/lint.py
 #, python-brace-format
 msgid "{appid}: Unknown extlib {path} in build '{versionName}'"
 msgstr ""
 
@@ -2666,20 +2666,20 @@
 #, python-brace-format
 msgid "{appid}: no builds specified, running on current source state"
 msgstr ""
 
 #: ../fdroidserver/lint.py
 #, python-brace-format
 msgid "{appid}: {field} must be a '{type}', but it is a '{fieldtype}!'"
-msgstr ""
+msgstr "{appid}：{field}必须为‘{type}’，但它是‘{fieldtype}！’"
 
 #: ../fdroidserver/lint.py
 #, python-brace-format
 msgid "{appid}: {field} must be a '{type}', but it is a '{fieldtype}'!"
-msgstr ""
+msgstr "{appid}：{field}必须为‘{type}’，但它是‘{fieldtype}’！"
 
 #: ../fdroidserver/metadata.py
 #, python-brace-format
 msgid "{build_flag} must be an integer, found: {value}"
 msgstr ""
 
 #: ../fdroidserver/metadata.py
@@ -2716,35 +2716,35 @@
 #, python-brace-format
 msgid "{path} has bad file signature \"{pattern}\", possible Janus exploit!"
 msgstr ""
 
 #: ../fdroidserver/update.py
 #, python-brace-format
 msgid "{path} is zero size!"
-msgstr ""
+msgstr "{path}的大小为零！"
 
 #: ../fdroidserver/deploy.py
 #, python-brace-format
 msgid "{path} more than 200MB, manually upload: {url}"
-msgstr ""
+msgstr "{path}的大小超过200MB，请手动上传：{url}"
 
 #: ../fdroidserver/update.py
 #, python-brace-format
 msgid "{path}: {error}"
 msgstr "{path}：{error}"
 
 #: ../fdroidserver/mirror.py
 #, python-brace-format
 msgid "{url} does not end with \"fdroid\", check the URL path!"
-msgstr ""
+msgstr "{url}不是以“fdroid”结尾的，请检查链接路径！"
 
 #: ../fdroidserver/import_subcommand.py
 #, python-brace-format
 msgid "{url} does not start with \"http\"!"
-msgstr ""
+msgstr "{url}不是以“http”为开头！"
 
 #: ../fdroidserver/build.py
 msgid "{} build failed"
 msgid_plural "{} builds failed"
 msgstr[0] ""
 
 #: ../fdroidserver/build.py
```

### Comparing `fdroidserver-2.3a0/locale/zh_Hant/LC_MESSAGES/fdroidserver.po` & `fdroidserver-2.3a1/locale/zh_Hant/LC_MESSAGES/fdroidserver.po`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/makebuildserver` & `fdroidserver-2.3a1/makebuildserver`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/pyproject.toml` & `fdroidserver-2.3a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
   | fdroidserver/__init__\.py
   | fdroidserver/__main__\.py
   | fdroidserver/apksigcopier\.py
   | fdroidserver/looseversion\.py
   | fdroidserver/build\.py
   | fdroidserver/checkupdates\.py
   | fdroidserver/common\.py
-  | fdroidserver/deploy\.py
   | fdroidserver/import_subcommand\.py
   | fdroidserver/index\.py
   | fdroidserver/metadata\.py
   | fdroidserver/nightly\.py
   | fdroidserver/publish\.py
   | fdroidserver/scanner\.py
   | fdroidserver/update\.py
```

### Comparing `fdroidserver-2.3a0/setup.cfg` & `fdroidserver-2.3a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/setup.py` & `fdroidserver-2.3a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='fdroidserver',
-    version='2.3a0',
+    version='2.3a1',
     description='F-Droid Server Tools',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='The F-Droid Project',
     author_email='team@f-droid.org',
     url='https://f-droid.org',
     license='AGPL-3.0',
@@ -88,23 +88,23 @@
         'install': InstallWithCompile,
     },
     setup_requires=[
         'babel',
     ],
     install_requires=[
         'appdirs',
-        'androguard >= 3.1.0, != 3.3.0, != 3.3.1, != 3.3.2, <4',
+        'androguard >= 3.3.5',
+        'asn1crypto',
         'clint',
         'defusedxml',
         'GitPython',
+        'oscrypto',
         'paramiko',
         'Pillow',
         'apache-libcloud >= 0.14.1',
-        'pyasn1 >=0.4.1',
-        'pyasn1-modules >= 0.2.1',
         'python-vagrant',
         'PyYAML',
         'qrcode',
         'ruamel.yaml >= 0.15, < 0.17.22',
         'requests >= 2.5.2, != 2.11.0, != 2.12.2, != 2.18.0',
         'sdkmanager >= 0.6.4',
         'yamllint',
```

### Comparing `fdroidserver-2.3a0/tests/IsMD5Disabled.java` & `fdroidserver-2.3a1/tests/IsMD5Disabled.java`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/Norway_bouvet_europe_2.obf.zip` & `fdroidserver-2.3a1/tests/Norway_bouvet_europe_2.obf.zip`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/SpeedoMeterApp.main_1.apk` & `fdroidserver-2.3a1/tests/SpeedoMeterApp.main_1.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/aosp_testkey_debug.keystore` & `fdroidserver-2.3a1/tests/aosp_testkey_debug.keystore`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/apk.embedded_1.apk` & `fdroidserver-2.3a1/tests/apk.embedded_1.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/bad-unicode-πÇÇ现代通用字-български-عربي1.apk` & `fdroidserver-2.3a1/tests/bad-unicode-πÇÇ现代通用字-български-عربي1.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/17.0.0/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/17.0.0/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/18.1.1/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/18.1.1/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.0.0/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/19.0.0/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/19.1.0/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/19.1.0/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/20.0.0/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/20.0.0/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.1/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.1/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/21.1.2/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/21.1.2/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.0/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.0/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/22.0.1/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/22.0.1/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.0/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.0/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.1/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.1/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.2/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.2/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/23.0.3/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/23.0.3/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.0/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.0/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.1/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.1/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.2/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.2/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/24.0.3/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/24.0.3/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.0/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.0/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.1/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.1/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.2/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.2/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/25.0.3/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/25.0.3/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.0/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.0/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.1/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.1/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.2/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.2/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/26.0.3/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/26.0.3/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.0/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.0/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.1/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.1/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.2/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.2/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/27.0.3/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/27.0.3/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.0/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.0/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-com.moez.QKSMS_182.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-com.moez.QKSMS_182.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.1/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.1/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-org.droidtr.keyboard_34.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-org.droidtr.keyboard_34.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.2/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.2/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-com.example.test.helloworld_1.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-com.example.test.helloworld_1.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-com.politedroid_3.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-com.politedroid_3.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-com.politedroid_4.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-com.politedroid_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-com.politedroid_5.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-com.politedroid_5.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-com.politedroid_6.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-com.politedroid_6.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-duplicate.permisssions_9999999.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-duplicate.permisssions_9999999.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-info.guardianproject.urzip_100.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-info.guardianproject.urzip_100.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-info.zwanenburg.caffeinetile_4.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-no.min.target.sdk_987.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-no.min.target.sdk_987.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-obb.main.oldversion_1444412523.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-obb.main.oldversion_1444412523.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-obb.main.twoversions_1101613.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-obb.main.twoversions_1101613.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-obb.main.twoversions_1101615.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-obb.main.twoversions_1101615.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-obb.main.twoversions_1101617.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-obb.main.twoversions_1101617.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-obb.mainpatch.current_1619.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-obb.mainpatch.current_1619.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/28.0.3/aapt-output-souch.smsbypass_9.txt` & `fdroidserver-2.3a1/tests/build-tools/28.0.3/aapt-output-souch.smsbypass_9.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build-tools/generate.sh` & `fdroidserver-2.3a1/tests/build-tools/generate.sh`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/build.TestCase` & `fdroidserver-2.3a1/tests/build.TestCase`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 
 # http://www.drdobbs.com/testing/unit-testing-with-python/240165163
 
 import inspect
 import logging
-import optparse
 import os
 import shutil
 import sys
 import tempfile
 import textwrap
 import unittest
 import yaml
@@ -25,15 +24,15 @@
 from testcommon import TmpCwd
 
 import fdroidserver.build
 import fdroidserver.common
 import fdroidserver.metadata
 import fdroidserver.scanner
 import fdroidserver.vmtools
-from testcommon import mkdtemp
+from testcommon import mkdtemp, parse_args_for_test
 
 
 class FakeProcess:
     output = 'fake output'
     returncode = 0
 
     def __init__(self, args, **kwargs):
@@ -45,16 +44,14 @@
 
 
 class BuildTest(unittest.TestCase):
     '''fdroidserver/build.py'''
 
     def setUp(self):
         logging.basicConfig(level=logging.DEBUG)
-        logger = logging.getLogger('androguard.axml')
-        logger.setLevel(logging.INFO)  # tame the axml debug messages
         self.basedir = os.path.join(localmodule, 'tests')
         os.chdir(self.basedir)
         fdroidserver.common.config = None
         fdroidserver.build.config = None
         fdroidserver.build.options = None
         self._td = mkdtemp()
         self.testdir = self._td.name
@@ -560,15 +557,15 @@
         self.assertFalse(os.path.exists('gen'))
         self.assertFalse(os.path.exists('gradle-wrapper.jar'))
 
     def test_scan_with_extlib(self):
         os.chdir(self.testdir)
         os.mkdir("build")
 
-        config = fdroidserver.common.get_config()
+        config = fdroidserver.common.read_config()
         config['sdk_path'] = os.getenv('ANDROID_HOME')
         config['ndk_paths'] = {'r10d': os.getenv('ANDROID_NDK_HOME')}
         fdroidserver.common.config = config
         app = fdroidserver.metadata.App()
         app.id = 'com.gpl.rpg.AndorsTrail'
         build = fdroidserver.metadata.Build()
         build.commit = 'master'
@@ -1102,20 +1099,22 @@
         fdroidserver.build.config = {'keep_when_not_allowed': False}
         self.assertFalse(fdroidserver.build.keep_when_not_allowed())
 
 
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (fdroidserver.common.options, args) = parser.parse_args(['--verbose'])
+    parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(BuildTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/check-fdroid-apk` & `fdroidserver-2.3a1/tests/check-fdroid-apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/checkupdates.TestCase` & `fdroidserver-2.3a1/tests/checkupdates.TestCase`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 
 # http://www.drdobbs.com/testing/unit-testing-with-python/240165163
 
 import logging
-import optparse
 import os
 import sys
 import unittest
 from unittest import mock
 from pathlib import Path
 
 
@@ -26,16 +25,14 @@
 
     def setUp(self):
         logging.basicConfig(level=logging.DEBUG)
         self.basedir = localmodule / 'tests'
         os.chdir(self.basedir)
 
     def test_autoupdatemode_no_suffix(self):
-        fdroidserver.checkupdates.options = mock.Mock()
-        fdroidserver.checkupdates.options.auto = 'bleh'
         fdroidserver.checkupdates.config = {}
 
         app = fdroidserver.metadata.App()
         app.id = 'loop.starts.shooting'
         app.metadatapath = 'metadata/' + app.id + '.yml'
         app.CurrentVersion = '1.1.8-fdroid'
         app.CurrentVersionCode = 10108
@@ -48,35 +45,33 @@
         app['Builds'].append(build)
 
         with mock.patch(
             'fdroidserver.checkupdates.check_http', lambda app: ('1.1.9', 10109)
         ):
             with mock.patch('fdroidserver.metadata.write_metadata', mock.Mock()):
                 with mock.patch('subprocess.call', lambda cmd: 0):
-                    fdroidserver.checkupdates.checkupdates_app(app)
+                    fdroidserver.checkupdates.checkupdates_app(app, auto=True)
 
         build = app['Builds'][-1]
         self.assertEqual(build.versionName, '1.1.9')
         self.assertEqual(build.commit, '1.1.9')
 
         with mock.patch(
             'fdroidserver.checkupdates.check_http', lambda app: ('1.7.9', 10107)
         ):
             with mock.patch('fdroidserver.metadata.write_metadata', mock.Mock()):
                 with mock.patch('subprocess.call', lambda cmd: 0):
                     with self.assertRaises(FDroidException):
-                        fdroidserver.checkupdates.checkupdates_app(app)
+                        fdroidserver.checkupdates.checkupdates_app(app, auto=True)
 
         build = app['Builds'][-1]
         self.assertEqual(build.versionName, '1.1.9')
         self.assertEqual(build.commit, '1.1.9')
 
     def test_autoupdatemode_suffix(self):
-        fdroidserver.checkupdates.options = mock.Mock()
-        fdroidserver.checkupdates.options.auto = 'bleh'
         fdroidserver.checkupdates.config = {}
 
         app = fdroidserver.metadata.App()
         app.id = 'loop.starts.shooting'
         app.metadatapath = 'metadata/' + app.id + '.yml'
         app.CurrentVersion = '1.1.8-fdroid'
         app.CurrentVersionCode = 10108
@@ -89,23 +84,21 @@
         app['Builds'].append(build)
 
         with mock.patch(
             'fdroidserver.checkupdates.check_http', lambda app: ('1.1.9', 10109)
         ):
             with mock.patch('fdroidserver.metadata.write_metadata', mock.Mock()):
                 with mock.patch('subprocess.call', lambda cmd: 0):
-                    fdroidserver.checkupdates.checkupdates_app(app)
+                    fdroidserver.checkupdates.checkupdates_app(app, auto=True)
 
         build = app['Builds'][-1]
         self.assertEqual(build.versionName, '1.1.9.10109-fdroid')
         self.assertEqual(build.commit, 'v1.1.9_10109')
 
     def test_autoupdate_multi_variants(self):
-        fdroidserver.checkupdates.options = mock.Mock()
-        fdroidserver.checkupdates.options.auto = 'bleh'
         fdroidserver.checkupdates.config = {}
 
         app = fdroidserver.metadata.App()
         app.id = 'loop.starts.shooting'
         app.metadatapath = 'metadata/' + app.id + '.yml'
         app.CurrentVersion = '1.1.8'
         app.CurrentVersionCode = 101083
@@ -130,15 +123,15 @@
 
         with mock.patch(
             'fdroidserver.checkupdates.check_tags',
             lambda app, pattern: ('1.1.9', 10109, 'v1.1.9'),
         ):
             with mock.patch('fdroidserver.metadata.write_metadata', mock.Mock()):
                 with mock.patch('subprocess.call', lambda cmd: 0):
-                    fdroidserver.checkupdates.checkupdates_app(app)
+                    fdroidserver.checkupdates.checkupdates_app(app, auto=True)
 
         build = app['Builds'][-2]
         self.assertEqual(build.versionName, '1.1.9')
         self.assertEqual(build.versionCode, 101091)
         self.assertEqual(build.gradle, ["arm"])
 
         build = app['Builds'][-1]
@@ -146,44 +139,40 @@
         self.assertEqual(build.versionCode, 101093)
         self.assertEqual(build.gradle, ["x86"])
 
         self.assertEqual(app.CurrentVersion, '1.1.9')
         self.assertEqual(app.CurrentVersionCode, 101093)
 
     def test_checkupdates_app_http(self):
-        fdroidserver.checkupdates.options = mock.Mock()
-        fdroidserver.checkupdates.options.auto = 'bleh'
         fdroidserver.checkupdates.config = {}
 
         app = fdroidserver.metadata.App()
         app.id = 'loop.starts.shooting'
         app.metadatapath = 'metadata/' + app.id + '.yml'
         app.CurrentVersionCode = 10108
         app.UpdateCheckMode = 'HTTP'
         app.UpdateCheckData = 'mock'
 
         with mock.patch(
             'fdroidserver.checkupdates.check_http', lambda app: (None, 'bla')
         ):
             with self.assertRaises(FDroidException):
-                fdroidserver.checkupdates.checkupdates_app(app)
+                fdroidserver.checkupdates.checkupdates_app(app, auto=True)
 
         with mock.patch(
             'fdroidserver.checkupdates.check_http', lambda app: ('1.1.9', 10109)
         ):
             with mock.patch(
                 'fdroidserver.metadata.write_metadata', mock.Mock()
             ) as wrmock:
                 with mock.patch('subprocess.call', lambda cmd: 0):
-                    fdroidserver.checkupdates.checkupdates_app(app)
+                    fdroidserver.checkupdates.checkupdates_app(app, auto=True)
                 wrmock.assert_called_with(app.metadatapath, app)
 
     def test_checkupdates_app_tags(self):
-        fdroidserver.checkupdates.options = mock.Mock()
-        fdroidserver.checkupdates.options.auto = 'bleh'
         fdroidserver.checkupdates.config = {}
 
         app = fdroidserver.metadata.App()
         app.id = 'loop.starts.shooting'
         app.metadatapath = 'metadata/' + app.id + '.yml'
         app.CurrentVersion = '1.1.8'
         app.CurrentVersionCode = 10108
@@ -196,31 +185,29 @@
         app['Builds'].append(build)
 
         with mock.patch(
             'fdroidserver.checkupdates.check_tags',
             lambda app, pattern: (None, 'bla', None),
         ):
             with self.assertRaises(FDroidException):
-                fdroidserver.checkupdates.checkupdates_app(app)
+                fdroidserver.checkupdates.checkupdates_app(app, auto=True)
 
         with mock.patch(
             'fdroidserver.checkupdates.check_tags',
             lambda app, pattern: ('1.1.9', 10109, 'v1.1.9'),
         ):
             with mock.patch('fdroidserver.metadata.write_metadata', mock.Mock()):
                 with mock.patch('subprocess.call', lambda cmd: 0):
-                    fdroidserver.checkupdates.checkupdates_app(app)
+                    fdroidserver.checkupdates.checkupdates_app(app, auto=True)
 
         build = app['Builds'][-1]
         self.assertEqual(build.versionName, '1.1.9')
         self.assertEqual(build.commit, 'v1.1.9')
 
     def test_check_http(self):
-        fdroidserver.checkupdates.options = mock.Mock()
-
         app = fdroidserver.metadata.App()
         app.id = 'loop.starts.shooting'
         app.metadatapath = 'metadata/' + app.id + '.yml'
         app.CurrentVersionCode = 10108
         app.UpdateCheckMode = 'HTTP'
         app.UpdateCheckData = r'https://a.net/b.txt|c(.*)|https://d.net/e.txt|v(.*)'
         app.UpdateCheckIgnore = 'beta'
@@ -239,16 +226,14 @@
             faked = scheme + '://fake.url/for/testing/scheme'
             app.UpdateCheckData = faked + '|ignored|' + faked + '|ignored'
             app.metadatapath = 'metadata/' + app.id + '.yml'
             with self.assertRaises(FDroidException):
                 fdroidserver.checkupdates.check_http(app)
 
     def test_check_http_ignore(self):
-        fdroidserver.checkupdates.options = mock.Mock()
-
         app = fdroidserver.metadata.App()
         app.id = 'loop.starts.shooting'
         app.metadatapath = 'metadata/' + app.id + '.yml'
         app.CurrentVersionCode = 10108
         app.UpdateCheckMode = 'HTTP'
         app.UpdateCheckData = r'https://a.net/b.txt|c(.*)|https://d.net/e.txt|v(.*)'
         app.UpdateCheckIgnore = 'beta'
@@ -256,16 +241,14 @@
         respmock = mock.Mock()
         respmock.read = lambda: 'v1.1.9-beta\nc10109'.encode('utf-8')
         with mock.patch('urllib.request.urlopen', lambda a, b, c: respmock):
             vername, vercode = fdroidserver.checkupdates.check_http(app)
         self.assertEqual(vername, None)
 
     def test_check_tags_data(self):
-        fdroidserver.checkupdates.options = mock.Mock()
-
         app = fdroidserver.metadata.App()
         app.id = 'loop.starts.shooting'
         app.metadatapath = 'metadata/' + app.id + '.yml'
         app.RepoType = 'git'
         app.CurrentVersionCode = 10108
         app.UpdateCheckMode = 'Tags'
         app.UpdateCheckData = r'b.txt|c(.*)|e.txt|v(.*)'
@@ -332,20 +315,23 @@
         with mock.patch('fdroidserver.common.getvcs', return_value=vcs):
             vername, vercode, _tag = fdroidserver.checkupdates.check_tags(app, None)
         self.assertEqual(vername, '2')
         self.assertEqual(vercode, 2)
 
 
 if __name__ == "__main__":
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+    from testcommon import parse_args_for_test
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (fdroidserver.common.options, args) = parser.parse_args(['--verbose'])
+    parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(CheckupdatesTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/com.fake.IpaApp_1000000000001.ipa` & `fdroidserver-2.3a1/tests/com.fake.IpaApp_1000000000001.ipa`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/common.TestCase` & `fdroidserver-2.3a1/tests/common.TestCase`

 * *Files 8% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 import difflib
 import git
 import glob
 import importlib
 import inspect
 import json
 import logging
-import optparse
 import os
 import re
 import ruamel.yaml
 import shutil
 import subprocess
 import sys
 import tempfile
 import time
 import unittest
 import textwrap
 import yaml
 import gzip
+from argparse import ArgumentParser
 from zipfile import BadZipFile, ZipFile
 from unittest import mock
 from pathlib import Path
 
 
 localmodule = os.path.realpath(
     os.path.join(os.path.dirname(inspect.getfile(inspect.currentframe())), '..')
@@ -34,44 +34,55 @@
 if localmodule not in sys.path:
     sys.path.insert(0, localmodule)
 
 import fdroidserver.index
 import fdroidserver.signindex
 import fdroidserver.common
 import fdroidserver.metadata
-from testcommon import TmpCwd, mkdtemp
+from testcommon import TmpCwd, mkdtemp, parse_args_for_test
 from fdroidserver.common import ANTIFEATURES_CONFIG_NAME, CATEGORIES_CONFIG_NAME
 from fdroidserver.exception import FDroidException, VCSException,\
     MetaDataException, VerificationException
 from fdroidserver.looseversion import LooseVersion
 
 
+def _mock_common_module_options_instance():
+    """Helper method to deal with difficult visibility of the module-level options."""
+    fdroidserver.common.options = mock.Mock()
+    fdroidserver.common.options.verbose = False
+
+
 class CommonTest(unittest.TestCase):
     '''fdroidserver/common.py'''
 
     def setUp(self):
         logging.basicConfig(level=logging.DEBUG)
         logger = logging.getLogger('androguard.axml')
         logger.setLevel(logging.INFO)  # tame the axml debug messages
         self.basedir = os.path.join(localmodule, 'tests')
         self.tmpdir = os.path.abspath(os.path.join(self.basedir, '..', '.testfiles'))
         if not os.path.exists(self.tmpdir):
             os.makedirs(self.tmpdir)
         os.chdir(self.basedir)
+
+        # these are declared as None at the top of the module file
         fdroidserver.common.config = None
-        fdroidserver.common.options = mock.Mock()
-        fdroidserver.common.options.verbose = False
+        fdroidserver.common.options = None
         fdroidserver.metadata.srclibs = None
+
         self._td = mkdtemp()
         self.testdir = self._td.name
 
     def tearDown(self):
+        fdroidserver.common.config = None
+        fdroidserver.common.options = None
         os.chdir(self.basedir)
         self._td.cleanup()
-        shutil.rmtree(self.tmpdir)
+        if os.path.exists(self.tmpdir):
+            shutil.rmtree(self.tmpdir)
 
     def test_parse_human_readable_size(self):
         for k, v in (
             (9827, 9827),
             (123.456, 123),
             ('123b', 123),
             ('1.2', 1),
@@ -352,14 +363,15 @@
         subdir_path.mkdir(parents=True, exist_ok=True)
         build_gradle = subdir_path / 'build.gradle'
         build_gradle.write_text('// just a test placeholder', encoding='utf-8')
 
         config = dict()
         fdroidserver.common.fill_config_defaults(config)
         fdroidserver.common.config = config
+        _mock_common_module_options_instance()
 
         srclibname = 'FakeSrcLib'
         srclib_testdir = os.path.join(self.testdir, 'build', 'srclib')
         os.makedirs(os.path.join(srclib_testdir, srclibname, 'testdirshouldexist'))
         fdroidserver.metadata.srclibs = {
             srclibname: {
                 'RepoType': 'git',
@@ -393,14 +405,15 @@
                 pass
 
         fdroidserver.common.prepare_source(FakeVcs(), app, build,
                                            app_build_dir, srclib_testdir, app_build_dir,
                                            onserver=True, refresh=False)  # do not clone in this test
 
     def test_prepare_sources_refresh(self):
+        _mock_common_module_options_instance()
         packageName = 'org.fdroid.ci.test.app'
         os.chdir(self.tmpdir)
         os.mkdir('build')
         os.mkdir('metadata')
 
         # use a local copy if available to avoid hitting the network
         tmprepo = os.path.join(self.basedir, 'tmp', 'importer')
@@ -463,25 +476,27 @@
         with self.assertRaises(VCSException):
             fdroidserver.common.getvcs(vcstype, Path(remote), Path('bad'))
 
     def test_fdroid_popen_stderr_redirect(self):
         config = dict()
         fdroidserver.common.fill_config_defaults(config)
         fdroidserver.common.config = config
+        _mock_common_module_options_instance()
 
         commands = ['sh', '-c', 'echo stdout message && echo stderr message 1>&2']
 
         p = fdroidserver.common.FDroidPopen(commands)
         self.assertEqual(p.output, 'stdout message\nstderr message\n')
 
         p = fdroidserver.common.FDroidPopen(commands, stderr_to_stdout=False)
         self.assertEqual(p.output, 'stdout message\n')
 
     def test_signjar(self):
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        _mock_common_module_options_instance()
+        config = fdroidserver.common.read_config()
         config['jarsigner'] = fdroidserver.common.find_sdk_tools_cmd('jarsigner')
         fdroidserver.common.config = config
         fdroidserver.signindex.config = config
 
         sourcedir = os.path.join(self.basedir, 'signindex')
         with tempfile.TemporaryDirectory(
             prefix=inspect.currentframe().f_code.co_name, dir=self.tmpdir
@@ -493,15 +508,16 @@
                 fdroidserver.signindex.sign_jar(testfile, use_old_algs=True)
                 # these should be resigned, and therefore different
                 self.assertNotEqual(
                     open(sourcefile, 'rb').read(), open(testfile, 'rb').read()
                 )
 
     def test_verify_apk_signature(self):
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        _mock_common_module_options_instance()
+        config = fdroidserver.common.read_config()
         fdroidserver.common.config = config
 
         self.assertTrue(fdroidserver.common.verify_apk_signature('bad-unicode-πÇÇ现代通用字-български-عربي1.apk'))
         if 'apksigner' in fdroidserver.common.config:  # apksigner considers MD5 signatures valid
             self.assertTrue(fdroidserver.common.verify_apk_signature('org.bitbucket.tickytacky.mirrormirror_1.apk'))
             self.assertTrue(fdroidserver.common.verify_apk_signature('org.bitbucket.tickytacky.mirrormirror_2.apk'))
             self.assertTrue(fdroidserver.common.verify_apk_signature('org.bitbucket.tickytacky.mirrormirror_3.apk'))
@@ -515,15 +531,16 @@
         self.assertTrue(fdroidserver.common.verify_apk_signature('urzip.apk'))
         self.assertFalse(fdroidserver.common.verify_apk_signature('urzip-badcert.apk'))
         self.assertFalse(fdroidserver.common.verify_apk_signature('urzip-badsig.apk'))
         self.assertTrue(fdroidserver.common.verify_apk_signature('urzip-release.apk'))
         self.assertFalse(fdroidserver.common.verify_apk_signature('urzip-release-unsigned.apk'))
 
     def test_verify_old_apk_signature(self):
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        _mock_common_module_options_instance()
+        config = fdroidserver.common.read_config()
         config['jarsigner'] = fdroidserver.common.find_sdk_tools_cmd('jarsigner')
         fdroidserver.common.config = config
 
         try:
             fdroidserver.common.verify_deprecated_jar_signature('bad-unicode-πÇÇ现代通用字-български-عربي1.apk')
             fdroidserver.common.verify_deprecated_jar_signature('org.bitbucket.tickytacky.mirrormirror_1.apk')
             fdroidserver.common.verify_deprecated_jar_signature('org.bitbucket.tickytacky.mirrormirror_2.apk')
@@ -536,15 +553,15 @@
             self.fail("failed to jarsigner failed to verify an old apk")
         self.assertRaises(VerificationException, fdroidserver.common.verify_deprecated_jar_signature, 'urzip-badcert.apk')
         self.assertRaises(VerificationException, fdroidserver.common.verify_deprecated_jar_signature, 'urzip-badsig.apk')
         self.assertRaises(VerificationException, fdroidserver.common.verify_deprecated_jar_signature, 'urzip-release-unsigned.apk')
 
     def test_verify_jar_signature(self):
         """Sign entry.jar and make sure it validates"""
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         config['jarsigner'] = fdroidserver.common.find_sdk_tools_cmd('jarsigner')
         config['keystore'] = os.path.join(self.basedir, 'keystore.jks')
         config['repo_keyalias'] = 'sova'
         config['keystorepass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keypass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         fdroidserver.common.config = config
         fdroidserver.signindex.config = config
@@ -554,39 +571,40 @@
         shutil.copy('repo/index-v2.json', repo_dir)
         os.chdir(self.testdir)
         fdroidserver.signindex.sign_index('repo', 'entry.json')
         fdroidserver.common.verify_jar_signature('repo/entry.jar')
 
     def test_verify_jar_signature_fails(self):
         """Test verify_jar_signature fails on unsigned and deprecated algorithms"""
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         config['jarsigner'] = fdroidserver.common.find_sdk_tools_cmd('jarsigner')
         fdroidserver.common.config = config
         source_dir = os.path.join(self.basedir, 'signindex')
         for f in ('unsigned.jar', 'testy.jar', 'guardianproject.jar', 'guardianproject-v1.jar'):
             testfile = os.path.join(source_dir, f)
             with self.assertRaises(fdroidserver.index.VerificationException):
                 fdroidserver.common.verify_jar_signature(testfile)
 
     def test_verify_deprecated_jar_signature(self):
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         config['jarsigner'] = fdroidserver.common.find_sdk_tools_cmd('jarsigner')
         fdroidserver.common.config = config
         source_dir = os.path.join(self.basedir, 'signindex')
         for f in ('testy.jar', 'guardianproject.jar'):
             testfile = os.path.join(source_dir, f)
             fdroidserver.common.verify_deprecated_jar_signature(testfile)
 
         testfile = os.path.join(source_dir, 'unsigned.jar')
         with self.assertRaises(fdroidserver.index.VerificationException):
             fdroidserver.common.verify_deprecated_jar_signature(testfile)
 
     def test_verify_apks(self):
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         fdroidserver.common.config = config
+        _mock_common_module_options_instance()
 
         sourceapk = os.path.join(self.basedir, 'urzip.apk')
 
         copyapk = os.path.join(self.testdir, 'urzip-copy.apk')
         shutil.copy(sourceapk, copyapk)
         self.assertTrue(fdroidserver.common.verify_apk_signature(copyapk))
         self.assertIsNone(
@@ -611,14 +629,35 @@
                     testapk.writestr(info, apk.read(info.filename))
                     if info.filename.startswith('META-INF/'):
                         testapk.writestr(info.filename, otherapk.read(info.filename))
         otherapk.close()
         self.assertFalse(fdroidserver.common.verify_apk_signature(twosigapk))
         self.assertIsNone(fdroidserver.common.verify_apks(sourceapk, twosigapk, self.tmpdir))
 
+    def test_get_certificate_with_chain_sandisk(self):
+        """Test that APK signatures with a cert chain are parsed like apksigner.
+
+        SanDisk signs their APKs with a X.509 certificate chain of
+        trust, so there are actually three certificates
+        included. apksigner only cares about the certificate in the
+        chain that actually signs the manifest.
+
+        The correct value comes from:
+        apksigner verify --print-certs 883cbdae7aeb2e4b122e8ee8d89966c7062d0d49107a130235fa220a5b994a79.apk
+
+        """
+        cert = fdroidserver.common.get_certificate(
+            signature_block_file=Path('SANAPPSI.RSA').read_bytes(),
+            signature_file=Path('SANAPPSI.SF').read_bytes(),
+        )
+        self.assertEqual(
+            'ea0abbf2a142e4b167405d516b2cc408c4af4b29cd50ba281aa4470d4aab3e53',
+            fdroidserver.common.signer_fingerprint(cert),
+        )
+
     def test_write_to_config(self):
         with tempfile.TemporaryDirectory() as tmpPath:
             cfgPath = os.path.join(tmpPath, 'config.py')
             with open(cfgPath, 'w') as f:
                 f.write(
                     textwrap.dedent(
                         """\
@@ -864,15 +903,16 @@
             fdroidserver.common.find_apksigner(config)
             self.assertEqual(
                 os.path.join(android_home, 'build-tools'),
                 os.path.dirname(os.path.dirname(config.get('apksigner'))),
             )
 
     def test_sign_apk(self):
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        _mock_common_module_options_instance()
+        config = fdroidserver.common.read_config()
         if 'apksigner' not in config:
             self.skipTest('SKIPPING test_sign_apk, apksigner not installed!')
 
         config['keyalias'] = 'sova'
         config['keystorepass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keypass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keystore'] = os.path.join(self.basedir, 'keystore.jks')
@@ -898,51 +938,52 @@
             os.path.join(unsigned),
         )
         fdroidserver.common.apk_strip_v1_signatures(unsigned, strip_manifest=True)
         fdroidserver.common.sign_apk(unsigned, signed, config['keyalias'])
         self.assertTrue(os.path.isfile(signed))
         self.assertFalse(os.path.isfile(unsigned))
         self.assertTrue(fdroidserver.common.verify_apk_signature(signed))
-        self.assertEqual('18', fdroidserver.common._get_androguard_APK(signed).get_min_sdk_version())
+        self.assertEqual('18', fdroidserver.common.get_androguard_APK(signed).get_min_sdk_version())
 
         shutil.copy(os.path.join(self.basedir, 'minimal_targetsdk_30_unsigned.apk'), self.testdir)
         unsigned = os.path.join(self.testdir, 'minimal_targetsdk_30_unsigned.apk')
         signed = os.path.join(self.testdir, 'minimal_targetsdk_30.apk')
 
         self.assertFalse(fdroidserver.common.verify_apk_signature(unsigned))
         fdroidserver.common.sign_apk(unsigned, signed, config['keyalias'])
 
         self.assertTrue(os.path.isfile(signed))
         self.assertFalse(os.path.isfile(unsigned))
         self.assertTrue(fdroidserver.common.verify_apk_signature(signed))
         # verify it has a v2 signature
-        self.assertTrue(fdroidserver.common._get_androguard_APK(signed).is_signed_v2())
+        self.assertTrue(fdroidserver.common.get_androguard_APK(signed).is_signed_v2())
 
         shutil.copy(os.path.join(self.basedir, 'no_targetsdk_minsdk30_unsigned.apk'), self.testdir)
         unsigned = os.path.join(self.testdir, 'no_targetsdk_minsdk30_unsigned.apk')
         signed = os.path.join(self.testdir, 'no_targetsdk_minsdk30_signed.apk')
 
         fdroidserver.common.sign_apk(unsigned, signed, config['keyalias'])
         self.assertTrue(fdroidserver.common.verify_apk_signature(signed))
-        self.assertTrue(fdroidserver.common._get_androguard_APK(signed).is_signed_v2())
+        self.assertTrue(fdroidserver.common.get_androguard_APK(signed).is_signed_v2())
 
         shutil.copy(os.path.join(self.basedir, 'no_targetsdk_minsdk1_unsigned.apk'), self.testdir)
         unsigned = os.path.join(self.testdir, 'no_targetsdk_minsdk1_unsigned.apk')
         signed = os.path.join(self.testdir, 'no_targetsdk_minsdk1_signed.apk')
 
         self.assertFalse(fdroidserver.common.verify_apk_signature(unsigned))
         fdroidserver.common.sign_apk(unsigned, signed, config['keyalias'])
 
         self.assertTrue(os.path.isfile(signed))
         self.assertFalse(os.path.isfile(unsigned))
         self.assertTrue(fdroidserver.common.verify_apk_signature(signed))
 
     @unittest.skipIf(os.getuid() == 0, 'This is meaningless when run as root')
     def test_sign_apk_fail(self):
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        _mock_common_module_options_instance()
+        config = fdroidserver.common.read_config()
         if 'apksigner' not in config:
             self.skipTest('SKIPPING test_sign_apk_fail, apksigner not installed!')
 
         config['keyalias'] = 'sova'
         config['keystorepass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keypass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keystore'] = os.path.join(self.basedir, 'keystore.jks')
@@ -957,15 +998,16 @@
         with self.assertRaises(fdroidserver.exception.BuildException):
             fdroidserver.common.sign_apk(unsigned, signed, config['keyalias'])
         os.chmod(unsigned, 0o777)
         self.assertTrue(os.path.isfile(unsigned))
         self.assertFalse(os.path.isfile(signed))
 
     def test_sign_apk_corrupt(self):
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        _mock_common_module_options_instance()
+        config = fdroidserver.common.read_config()
         if 'apksigner' not in config:
             self.skipTest('SKIPPING test_sign_apk_corrupt, apksigner not installed!')
 
         config['keyalias'] = 'sova'
         config['keystorepass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keypass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keystore'] = os.path.join(self.basedir, 'keystore.jks')
@@ -983,15 +1025,16 @@
         self.assertFalse(os.path.isfile(signed))
 
     @unittest.skipUnless(
         os.path.exists('tests/SystemWebView-repack.apk'), "file too big for sdist"
     )
     def test_resign_apk(self):
         """When using apksigner, it should resign signed APKs"""
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        _mock_common_module_options_instance()
+        config = fdroidserver.common.read_config()
         if 'apksigner' not in config:
             self.skipTest('SKIPPING test_resign_apk, apksigner not installed!')
 
         config['keyalias'] = 'sova'
         config['keystorepass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keypass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keystore'] = os.path.join(self.basedir, 'keystore.jks')
@@ -1035,14 +1078,19 @@
         testcases = [
             ('repo/obb.main.twoversions_1101613.apk', 'obb.main.twoversions', 1101613, '0.1'),
             ('org.bitbucket.tickytacky.mirrormirror_1.apk', 'org.bitbucket.tickytacky.mirrormirror', 1, '1.0'),
             ('org.bitbucket.tickytacky.mirrormirror_2.apk', 'org.bitbucket.tickytacky.mirrormirror', 2, '1.0.1'),
             ('org.bitbucket.tickytacky.mirrormirror_3.apk', 'org.bitbucket.tickytacky.mirrormirror', 3, '1.0.2'),
             ('org.bitbucket.tickytacky.mirrormirror_4.apk', 'org.bitbucket.tickytacky.mirrormirror', 4, '1.0.3'),
             ('org.dyndns.fules.ck_20.apk', 'org.dyndns.fules.ck', 20, 'v1.6pre2'),
+            ('issue-1128-min-sdk-30-poc.apk', 'org.fdroid.ci', 1, '1.0'),
+            ('issue-1128-poc1.apk', 'android.appsecurity.cts.tinyapp', 10, '1.0'),
+            ('issue-1128-poc2.apk', 'android.appsecurity.cts.tinyapp', 10, '1.0'),
+            ('issue-1128-poc3a.apk', 'android.appsecurity.cts.tinyapp', 10, '1.0'),
+            ('issue-1128-poc3b.apk', 'android.appsecurity.cts.tinyapp', 10, '1.0'),
             ('urzip.apk', 'info.guardianproject.urzip', 100, '0.1'),
             ('urzip-badcert.apk', 'info.guardianproject.urzip', 100, '0.1'),
             ('urzip-badsig.apk', 'info.guardianproject.urzip', 100, '0.1'),
             ('urzip-release.apk', 'info.guardianproject.urzip', 100, '0.1'),
             ('urzip-release-unsigned.apk', 'info.guardianproject.urzip', 100, '0.1'),
             ('repo/com.politedroid_3.apk', 'com.politedroid', 3, '1.2'),
             ('repo/com.politedroid_4.apk', 'com.politedroid', 4, '1.3'),
@@ -1142,32 +1190,38 @@
             nc = fdroidserver.common.get_native_code(apkfilename)
             self.assertEqual(native_code, nc)
 
     def test_get_sdkversions_androguard(self):
         """This is a sanity test that androguard isn't broken"""
 
         def get_minSdkVersion(apkfile):
-            apk = fdroidserver.common._get_androguard_APK(apkfile)
+            apk = fdroidserver.common.get_androguard_APK(apkfile)
             return fdroidserver.common.get_min_sdk_version(apk)
 
         def get_targetSdkVersion(apkfile):
-            apk = fdroidserver.common._get_androguard_APK(apkfile)
+            apk = fdroidserver.common.get_androguard_APK(apkfile)
             return apk.get_effective_target_sdk_version()
 
         self.assertEqual(4, get_minSdkVersion('bad-unicode-πÇÇ现代通用字-български-عربي1.apk'))
+        self.assertEqual(30, get_minSdkVersion('issue-1128-min-sdk-30-poc.apk'))
+        self.assertEqual(29, get_minSdkVersion('issue-1128-poc1.apk'))
+        self.assertEqual(29, get_minSdkVersion('issue-1128-poc2.apk'))
+        self.assertEqual(23, get_minSdkVersion('issue-1128-poc3a.apk'))
+        self.assertEqual(23, get_minSdkVersion('issue-1128-poc3b.apk'))
         self.assertEqual(14, get_minSdkVersion('org.bitbucket.tickytacky.mirrormirror_1.apk'))
         self.assertEqual(14, get_minSdkVersion('org.bitbucket.tickytacky.mirrormirror_2.apk'))
         self.assertEqual(14, get_minSdkVersion('org.bitbucket.tickytacky.mirrormirror_3.apk'))
         self.assertEqual(14, get_minSdkVersion('org.bitbucket.tickytacky.mirrormirror_4.apk'))
         self.assertEqual(7, get_minSdkVersion('org.dyndns.fules.ck_20.apk'))
         self.assertEqual(4, get_minSdkVersion('urzip.apk'))
         self.assertEqual(4, get_minSdkVersion('urzip-badcert.apk'))
         self.assertEqual(4, get_minSdkVersion('urzip-badsig.apk'))
         self.assertEqual(4, get_minSdkVersion('urzip-release.apk'))
         self.assertEqual(4, get_minSdkVersion('urzip-release-unsigned.apk'))
+        self.assertEqual(27, get_minSdkVersion('v2.only.sig_2.apk'))
         self.assertEqual(3, get_minSdkVersion('repo/com.politedroid_3.apk'))
         self.assertEqual(3, get_minSdkVersion('repo/com.politedroid_4.apk'))
         self.assertEqual(3, get_minSdkVersion('repo/com.politedroid_5.apk'))
         self.assertEqual(14, get_minSdkVersion('repo/com.politedroid_6.apk'))
         self.assertEqual(4, get_minSdkVersion('repo/obb.main.oldversion_1444412523.apk'))
         self.assertEqual(4, get_minSdkVersion('repo/obb.mainpatch.current_1619_another-release-key.apk'))
         self.assertEqual(4, get_minSdkVersion('repo/obb.mainpatch.current_1619.apk'))
@@ -1878,121 +1932,121 @@
             self.assertNotEqual(result, '')
 
     def test_with_no_config(self):
         """It should set defaults if no config file is found"""
         os.chdir(self.tmpdir)
         self.assertFalse(os.path.exists('config.yml'))
         self.assertFalse(os.path.exists('config.py'))
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertFalse(config.get('update_stats'))
         self.assertIsNotNone(config.get('char_limits'))
 
     def test_with_zero_size_config(self):
         """It should set defaults if config file has nothing in it"""
         os.chdir(self.tmpdir)
         open('config.yml', 'w').close()
         self.assertTrue(os.path.exists('config.yml'))
         self.assertFalse(os.path.exists('config.py'))
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertFalse(config.get('update_stats'))
         self.assertIsNotNone(config.get('char_limits'))
 
     def test_with_config_yml(self):
         """Make sure it is possible to use config.yml alone."""
         os.chdir(self.tmpdir)
         with open('config.yml', 'w') as fp:
             fp.write('apksigner: yml')
         self.assertTrue(os.path.exists('config.yml'))
         self.assertFalse(os.path.exists('config.py'))
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertEqual('yml', config.get('apksigner'))
 
     def test_with_config_yml_utf8(self):
         """Make sure it is possible to use config.yml in UTF-8 encoding."""
         os.chdir(self.tmpdir)
         teststr = '/πÇÇ现代通用字-български-عربي1/ö/yml'
         with open('config.yml', 'w', encoding='utf-8') as fp:
             fp.write('apksigner: ' + teststr)
         self.assertTrue(os.path.exists('config.yml'))
         self.assertFalse(os.path.exists('config.py'))
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertEqual(teststr, config.get('apksigner'))
 
     def test_with_config_yml_utf8_as_ascii(self):
         """Make sure it is possible to use config.yml Unicode encoded as ASCII."""
         os.chdir(self.tmpdir)
         teststr = '/πÇÇ现代通用字-български-عربي1/ö/yml'
         with open('config.yml', 'w') as fp:
             yaml.dump({'apksigner': teststr}, fp)
         self.assertTrue(os.path.exists('config.yml'))
         self.assertFalse(os.path.exists('config.py'))
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertEqual(teststr, config.get('apksigner'))
 
     def test_with_config_yml_with_env_var(self):
         """Make sure it is possible to use config.yml alone."""
         os.chdir(self.tmpdir)
         with mock.patch.dict(os.environ):
             os.environ['SECRET'] = 'mysecretpassword'
             with open('config.yml', 'w') as fp:
                 fp.write("""keypass: {'env': 'SECRET'}""")
             self.assertTrue(os.path.exists('config.yml'))
             self.assertFalse(os.path.exists('config.py'))
-            config = fdroidserver.common.read_config(fdroidserver.common.options)
+            config = fdroidserver.common.read_config()
             self.assertEqual(os.getenv('SECRET', 'fail'), config.get('keypass'))
 
     def test_with_config_yml_is_dict(self):
         os.chdir(self.tmpdir)
         Path('config.yml').write_text('apksigner = /placeholder/path')
         with self.assertRaises(TypeError):
-            fdroidserver.common.read_config(fdroidserver.common.options)
+            fdroidserver.common.read_config()
 
     def test_with_config_yml_is_not_mixed_type(self):
         os.chdir(self.tmpdir)
         Path('config.yml').write_text('k: v\napksigner = /placeholder/path')
         with self.assertRaises(yaml.scanner.ScannerError):
-            fdroidserver.common.read_config(fdroidserver.common.options)
+            fdroidserver.common.read_config()
 
     def test_with_config_py(self):
         """Make sure it is still possible to use config.py alone."""
         os.chdir(self.tmpdir)
         with open('config.py', 'w') as fp:
             fp.write('apksigner = "py"')
         self.assertFalse(os.path.exists('config.yml'))
         self.assertTrue(os.path.exists('config.py'))
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertEqual("py", config.get('apksigner'))
 
     def test_config_perm_warning(self):
         """Exercise the code path that issues a warning about unsafe permissions."""
         os.chdir(self.tmpdir)
         with open('config.yml', 'w') as fp:
             fp.write('keystore: foo.jks')
         self.assertTrue(os.path.exists(fp.name))
         os.chmod(fp.name, 0o666)
-        fdroidserver.common.read_config(fdroidserver.common.options)
+        fdroidserver.common.read_config()
         os.remove(fp.name)
         fdroidserver.common.config = None
 
         with open('config.py', 'w') as fp:
             fp.write('keystore = "foo.jks"')
         self.assertTrue(os.path.exists(fp.name))
         os.chmod(fp.name, 0o666)
-        fdroidserver.common.read_config(fdroidserver.common.options)
+        fdroidserver.common.read_config()
 
     def test_with_both_config_yml_py(self):
         """If config.yml and config.py are present, config.py should be ignored."""
         os.chdir(self.tmpdir)
         with open('config.yml', 'w') as fp:
             fp.write('apksigner: yml')
         with open('config.py', 'w') as fp:
             fp.write('apksigner = "py"')
         self.assertTrue(os.path.exists('config.yml'))
         self.assertTrue(os.path.exists('config.py'))
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertEqual('yml', config.get('apksigner'))
 
     def test_config_repo_url(self):
         """repo_url ends in /repo, archive_url ends in /archive."""
         os.chdir(self.tmpdir)
         with open('config.yml', 'w') as fp:
             fp.write('repo_url: https://MyFirstFDroidRepo.org/fdroid/repo\n')
@@ -2035,45 +2089,45 @@
 
     def test_write_to_config_yml(self):
         os.chdir(self.tmpdir)
         with open('config.yml', 'w') as fp:
             fp.write('apksigner: yml')
         self.assertTrue(os.path.exists(fp.name))
         self.assertFalse(os.path.exists('config.py'))
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertFalse('keypass' in config)
         self.assertEqual('yml', config.get('apksigner'))
         fdroidserver.common.write_to_config(config, 'keypass', 'mysecretpassword')
         with open(fp.name) as fp:
             print(fp.read())
         fdroidserver.common.config = None
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertEqual('mysecretpassword', config['keypass'])
 
     def test_write_to_config_py(self):
         os.chdir(self.tmpdir)
         with open('config.py', 'w') as fp:
             fp.write('apksigner = "py"')
         self.assertTrue(os.path.exists(fp.name))
         self.assertFalse(os.path.exists('config.yml'))
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertFalse('keypass' in config)
         self.assertEqual('py', config.get('apksigner'))
         fdroidserver.common.write_to_config(config, 'keypass', 'mysecretpassword')
         fdroidserver.common.config = None
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertEqual('mysecretpassword', config['keypass'])
 
     def test_config_dict_with_int_keys(self):
         os.chdir(self.tmpdir)
         with open('config.yml', 'w') as fp:
             fp.write('java_paths:\n  8: /usr/lib/jvm/java-8-openjdk\n')
         self.assertTrue(os.path.exists(fp.name))
         self.assertFalse(os.path.exists('config.py'))
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertEqual('/usr/lib/jvm/java-8-openjdk', config.get('java_paths', {}).get('8'))
 
     @mock.patch.dict(os.environ, {'PATH': os.getenv('PATH')}, clear=True)
     def test_test_sdk_exists_fails_on_bad_sdk_path(self):
         config = {'sdk_path': 'nothinghere'}
         self.assertFalse(fdroidserver.common.test_sdk_exists(config))
 
@@ -2143,15 +2197,15 @@
 
     def test_loading_config_buildserver_yml(self):
         """Smoke check to make sure this file is properly parsed"""
         os.chdir(self.tmpdir)
         shutil.copy(os.path.join(self.basedir, '..', 'buildserver', 'config.buildserver.yml'),
                     'config.yml')
         self.assertFalse(os.path.exists('config.py'))
-        fdroidserver.common.read_config(fdroidserver.common.options)
+        fdroidserver.common.read_config()
 
     def test_setup_status_output(self):
         os.chdir(self.tmpdir)
         start_timestamp = time.gmtime()
         subcommand = 'test'
 
         fakecmd = ['fdroid ' + subcommand, '--option']
@@ -2496,14 +2550,15 @@
         build.ndk = 'r21d'
         os.environ['PATH'] = '/usr/bin:/usr/sbin'
         with self.assertRaises(TypeError):
             fdroidserver.common.set_FDroidPopen_env(build)
 
     @mock.patch.dict(os.environ, clear=True)
     def test_FDroidPopen_envs_paths_can_be_pathlib(self):
+        _mock_common_module_options_instance()
         os.environ['PATH'] = '/usr/bin:/usr/sbin'
         envs = {'PATHLIB': Path('/pathlib/path'), 'STRING': '/string/path'}
         p = fdroidserver.common.FDroidPopen(['/bin/sh', '-c', 'export'], envs=envs)
         self.assertIn('/string/path', p.output)
         self.assertIn('/pathlib/path', p.output)
 
     def test_vcs_git_latesttags(self):
@@ -2911,23 +2966,377 @@
         s = 'foo@example.com:/var/www'
         mirrors = ruamel.yaml.YAML(typ='safe').load("""- url: '%s'""" % s)
         self.assertEqual(
             [{'url': s}], fdroidserver.common.parse_mirrors_config(mirrors)
         )
 
 
+APKS_WITH_JAR_SIGNATURES = (
+    (
+        'SpeedoMeterApp.main_1.apk',
+        '2e6b3126fb7e0db6a9d4c2a06df690620655454d6e152cf244cc9efe9787a77d',
+    ),
+    (
+        'apk.embedded_1.apk',
+        '764f0eaac0cdcde35023658eea865c4383ab580f9827c62fdd3daf9e654199ee',
+    ),
+    (
+        'bad-unicode-πÇÇ现代通用字-български-عربي1.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+    (
+        'issue-1128-poc3a.apk',
+        '1dbb8be012293e988a0820f7d455b07abd267d2c0b500fc793fcfd80141cb5ce',
+    ),
+    (
+        'issue-1128-poc3b.apk',
+        '1dbb8be012293e988a0820f7d455b07abd267d2c0b500fc793fcfd80141cb5ce',
+    ),
+    (
+        'janus.apk',
+        'ebb0fedf1942a099b287c3db00ff732162152481abb2b6c7cbcdb2ba5894a768',
+    ),
+    (
+        'org.bitbucket.tickytacky.mirrormirror_1.apk',
+        'feaa63df35b4635cf091513dfcd6d11209632555efdfc47e33b70d4e4eb5ba28',
+    ),
+    (
+        'org.bitbucket.tickytacky.mirrormirror_2.apk',
+        'feaa63df35b4635cf091513dfcd6d11209632555efdfc47e33b70d4e4eb5ba28',
+    ),
+    (
+        'org.bitbucket.tickytacky.mirrormirror_3.apk',
+        'feaa63df35b4635cf091513dfcd6d11209632555efdfc47e33b70d4e4eb5ba28',
+    ),
+    (
+        'org.bitbucket.tickytacky.mirrormirror_4.apk',
+        'feaa63df35b4635cf091513dfcd6d11209632555efdfc47e33b70d4e4eb5ba28',
+    ),
+    (
+        'org.dyndns.fules.ck_20.apk',
+        '9326a2cc1a2f148202bc7837a0af3b81200bd37fd359c9e13a2296a71d342056',
+    ),
+    (
+        'org.sajeg.fallingblocks_3.apk',
+        '033389681f4288fdb3e72a28058c8506233ca50de75452ab6c9c76ea1ca2d70f',
+    ),
+    (
+        'repo/com.example.test.helloworld_1.apk',
+        'c3a5ca5465a7585a1bda30218ae4017083605e3576867aa897d724208d99696c',
+    ),
+    (
+        'repo/com.politedroid_3.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+    (
+        'repo/com.politedroid_4.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+    (
+        'repo/com.politedroid_5.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+    (
+        'repo/com.politedroid_6.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+    (
+        'repo/duplicate.permisssions_9999999.apk',
+        '659e1fd284549f70d13fb02c620100e27eeea3420558cce62b0f5d4cf2b77d84',
+    ),
+    (
+        'repo/info.zwanenburg.caffeinetile_4.apk',
+        '51cfa5c8a743833ad89acf81cb755936876a5c8b8eca54d1ffdcec0cdca25d0e',
+    ),
+    (
+        'repo/no.min.target.sdk_987.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+    (
+        'repo/obb.main.oldversion_1444412523.apk',
+        '818e469465f96b704e27be2fee4c63ab9f83ddf30e7a34c7371a4728d83b0bc1',
+    ),
+    (
+        'repo/obb.main.twoversions_1101613.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+    (
+        'repo/obb.main.twoversions_1101615.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+    (
+        'repo/obb.main.twoversions_1101617.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+    (
+        'repo/obb.mainpatch.current_1619.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+    (
+        'repo/obb.mainpatch.current_1619_another-release-key.apk',
+        'ce9e200667f02d96d49891a2e08a3c178870e91853d61bdd33ef5f0b54701aa5',
+    ),
+    (
+        'repo/souch.smsbypass_9.apk',
+        'd3aec784b1fd71549fc22c999789122e3639895db6bd585da5835fbe3db6985c',
+    ),
+    (
+        'repo/urzip-; Рахма́, [rɐxˈmanʲɪnəf] سيرجي_رخمانينوف 谢·.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+    (
+        'repo/v1.v2.sig_1020.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+    (
+        'urzip-release.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+    (
+        'urzip.apk',
+        '7eabd8c15de883d1e82b5df2fd4f7f769e498078e9ad6dc901f0e96db77ceac3',
+    ),
+)
+APKS_WITHOUT_JAR_SIGNATURES = (
+    (
+        'issue-1128-poc1.apk',  # APK v3 Signature only
+        '1dbb8be012293e988a0820f7d455b07abd267d2c0b500fc793fcfd80141cb5ce',
+    ),
+    (
+        'issue-1128-poc2.apk',  # APK v3 Signature only
+        '1dbb8be012293e988a0820f7d455b07abd267d2c0b500fc793fcfd80141cb5ce',
+    ),
+    (
+        'issue-1128-min-sdk-30-poc.apk',  # APK v3 Signature only
+        '09350d5f3460a8a0ea5cf6b68ccd296a58754f7e683ba6aa08c19be8353504f3',
+    ),
+    (
+        'v2.only.sig_2.apk',
+        '32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6',
+    ),
+)
+
+
+class SignerExtractionTest(unittest.TestCase):
+    """Test extraction of the signer certificate from JARs and APKs
+
+    These fingerprints can be confirmed with:
+    apksigner verify --print-certs foo.apk | grep SHA-256
+    keytool -printcert -file ____.RSA
+    """
+
+    def setUp(self):
+        os.chdir(os.path.join(localmodule, 'tests'))
+        self._td = mkdtemp()
+        self.testdir = self._td.name
+
+        self.apksigner = shutil.which('apksigner')
+        self.keytool = shutil.which('keytool')
+
+    def tearDown(self):
+        self._td.cleanup()
+
+    def test_get_first_signer_certificate_with_jars(self):
+        for jar in (
+            'signindex/guardianproject-v1.jar',
+            'signindex/guardianproject.jar',
+            'signindex/testy.jar',
+        ):
+            outdir = os.path.join(self.testdir, jar[:-4].replace('/', '_'))
+            os.mkdir(outdir)
+            fdroidserver.common.apk_extract_signatures(jar, outdir)
+            certs = glob.glob(os.path.join(outdir, '*.RSA'))
+            with open(certs[0], 'rb') as fp:
+                self.assertEqual(
+                    fdroidserver.common.get_certificate(fp.read()),
+                    fdroidserver.common.get_first_signer_certificate(jar),
+                )
+
+    @unittest.skip("slow and only needed when adding to APKS_WITH_JAR_SIGNATURES")
+    def test_vs_keytool(self):
+        unittest.skipUnless(self.keytool, 'requires keytool to run')
+        pat = re.compile(r'[0-9A-F:]{95}')
+        cmd = [self.keytool, '-printcert', '-jarfile']
+        for apk, fingerprint in APKS_WITH_JAR_SIGNATURES:
+            o = subprocess.check_output(cmd + [apk], text=True)
+            try:
+                self.assertEqual(
+                    fingerprint,
+                    pat.search(o).group().replace(':', '').lower(),
+                )
+            except AttributeError as e:
+                print(e, o)
+
+    @unittest.skip("slow and only needed when adding to APKS_WITH_JAR_SIGNATURES")
+    def test_vs_apksigner(self):
+        unittest.skipUnless(self.apksigner, 'requires apksigner to run')
+        pat = re.compile(r'\s[0-9a-f]{64}\s')
+        cmd = [self.apksigner, 'verify', '--print-certs']
+        for apk, fingerprint in APKS_WITH_JAR_SIGNATURES + APKS_WITHOUT_JAR_SIGNATURES:
+            output = subprocess.check_output(cmd + [apk], text=True)
+            self.assertEqual(
+                fingerprint,
+                pat.search(output).group().strip(),
+                apk + " should have matching signer fingerprints",
+            )
+
+    def test_apk_signer_fingerprint_with_v1_apks(self):
+        for apk, fingerprint in APKS_WITH_JAR_SIGNATURES:
+            self.assertEqual(
+                fingerprint,
+                fdroidserver.common.apk_signer_fingerprint(apk),
+                f'apk_signer_fingerprint should match stored fingerprint for {apk}',
+            )
+
+    def test_apk_signer_fingerprint_without_v1_apks(self):
+        for apk, fingerprint in APKS_WITHOUT_JAR_SIGNATURES:
+            self.assertEqual(
+                fingerprint,
+                fdroidserver.common.apk_signer_fingerprint(apk),
+                f'apk_signer_fingerprint should match stored fingerprint for {apk}',
+            )
+
+    def test_get_first_signer_certificate_with_unsigned_jar(self):
+        self.assertIsNone(
+            fdroidserver.common.get_first_signer_certificate('signindex/unsigned.jar')
+        )
+
+    def test_apk_extract_fingerprint(self):
+        """Test extraction of JAR signatures (does not cover APK v2+ extraction)."""
+        for apk, fingerprint in APKS_WITH_JAR_SIGNATURES:
+            outdir = os.path.join(self.testdir, apk[:-4].replace('/', '_'))
+            os.mkdir(outdir)
+            try:
+                fdroidserver.common.apk_extract_signatures(apk, outdir)
+            except fdroidserver.apksigcopier.APKSigCopierError:
+                # nothing to test here when this error is thrown
+                continue
+            v1_certs = [str(cert) for cert in Path(outdir).glob('*.[DR]SA')]
+            cert = fdroidserver.common.get_certificate(
+                signature_block_file=Path(v1_certs[0]).read_bytes(),
+                signature_file=Path(v1_certs[0][:-4] + '.SF').read_bytes(),
+            )
+            self.assertEqual(
+                fingerprint,
+                fdroidserver.common.signer_fingerprint(cert),
+            )
+            apkobject = fdroidserver.common.get_androguard_APK(apk, skip_analysis=True)
+            v2_certs = apkobject.get_certificates_der_v2()
+            if v2_certs:
+                if v1_certs:
+                    self.assertEqual(len(v1_certs), len(v2_certs))
+                self.assertEqual(
+                    fingerprint,
+                    fdroidserver.common.signer_fingerprint(v2_certs[0]),
+                )
+            v3_certs = apkobject.get_certificates_der_v3()
+            if v3_certs:
+                if v2_certs:
+                    self.assertEqual(len(v2_certs), len(v3_certs))
+                self.assertEqual(
+                    fingerprint,
+                    fdroidserver.common.signer_fingerprint(v3_certs[0]),
+                )
+
+
+class ConfigOptionsScopeTest(unittest.TestCase):
+    """Test assumptions about variable scope for "config" and "options".
+
+    The ancient architecture of config and options in fdroidserver has
+    weird issues around unexpected scope, like there are cases where
+    the global config is not the same as the module-level config, and
+    more.
+
+    This is about describing what is happening, it is not about
+    documenting behaviors that are good design. The config and options
+    handling should really be refactored into a well-known, workable
+    Pythonic pattern.
+
+    """
+
+    def setUp(self):
+        # these are declared as None at the top of the module file
+        fdroidserver.common.config = None
+        fdroidserver.common.options = None
+
+    def tearDown(self):
+        fdroidserver.common.config = None
+        fdroidserver.common.options = None
+        if 'config' in globals():
+            global config
+            del config
+        if 'options' in globals():
+            global options
+            del options
+
+    def test_parse_args(self):
+        """Test that options is properly set up at the module-level and not global."""
+        self.assertFalse('options' in globals())
+        self.assertIsNone(fdroidserver.common.options)
+        parser = ArgumentParser()
+        fdroidserver.common.setup_global_opts(parser)
+        with mock.patch('sys.argv', ['$0']):
+            o = fdroidserver.common.parse_args(parser)
+        self.assertEqual(o, fdroidserver.common.options)
+
+        # No function should set options as a global, and the global
+        # keyword does not create the variable.
+        global options
+        with self.assertRaises(NameError):
+            options
+        self.assertFalse('options' in globals())
+
+    def test_parse_args_without_args(self):
+        """Test that the parsing function works fine when there are no args."""
+        parser = ArgumentParser()
+        fdroidserver.common.setup_global_opts(parser)
+        with mock.patch('sys.argv', ['$0']):
+            o = fdroidserver.common.parse_args(parser)
+        self.assertFalse(o.verbose)
+
+    def test_parse_args_with_args(self):
+        parser = ArgumentParser()
+        fdroidserver.common.setup_global_opts(parser)
+        with mock.patch('sys.argv', ['$0', '-v']):
+            o = fdroidserver.common.parse_args(parser)
+        self.assertTrue(o.verbose)
+
+    def test_get_config(self):
+        """Show how the module-level variables are initialized."""
+        self.assertTrue('config' not in vars() and 'config' not in globals())
+        self.assertIsNone(fdroidserver.common.config)
+        config = fdroidserver.common.read_config()
+        self.assertIsNotNone(fdroidserver.common.config)
+        self.assertEqual(dict, type(config))
+        self.assertEqual(config, fdroidserver.common.config)
+
+    def test_get_config_global(self):
+        """Test assumptions about variable scope using global keyword."""
+        global config
+        self.assertTrue('config' not in vars() and 'config' not in globals())
+        self.assertIsNone(fdroidserver.common.config)
+        c = fdroidserver.common.read_config()
+        self.assertIsNotNone(fdroidserver.common.config)
+        self.assertEqual(dict, type(c))
+        self.assertEqual(c, fdroidserver.common.config)
+        self.assertTrue(
+            'config' not in vars() and 'config' not in globals(),
+            "The config should not be set in the global context, only module-level.",
+        )
+
+
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    parser = ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (fdroidserver.common.options, args) = parser.parse_args(['--verbose'])
+    parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(CommonTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/config/antiFeatures.yml` & `fdroidserver-2.3a1/tests/config/antiFeatures.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/de/antiFeatures.yml` & `fdroidserver-2.3a1/tests/config/de/antiFeatures.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/fa/antiFeatures.yml` & `fdroidserver-2.3a1/tests/config/fa/antiFeatures.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/ic_antifeature_ads.xml` & `fdroidserver-2.3a1/tests/config/ic_antifeature_ads.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/ic_antifeature_disabledalgorithm.xml` & `fdroidserver-2.3a1/tests/config/ic_antifeature_disabledalgorithm.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/ic_antifeature_knownvuln.xml` & `fdroidserver-2.3a1/tests/config/ic_antifeature_knownvuln.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/ic_antifeature_nonfreeadd.xml` & `fdroidserver-2.3a1/tests/config/ic_antifeature_nonfreeadd.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/ic_antifeature_nonfreeassets.xml` & `fdroidserver-2.3a1/tests/config/ic_antifeature_nonfreeassets.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/ic_antifeature_nonfreedep.xml` & `fdroidserver-2.3a1/tests/config/ic_antifeature_nonfreedep.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/ic_antifeature_nonfreenet.xml` & `fdroidserver-2.3a1/tests/config/ic_antifeature_nonfreenet.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/ic_antifeature_nosourcesince.xml` & `fdroidserver-2.3a1/tests/config/ic_antifeature_nosourcesince.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/ic_antifeature_nsfw.xml` & `fdroidserver-2.3a1/tests/config/ic_antifeature_nsfw.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/ic_antifeature_tracking.xml` & `fdroidserver-2.3a1/tests/config/ic_antifeature_tracking.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/ic_antifeature_upstreamnonfree.xml` & `fdroidserver-2.3a1/tests/config/ic_antifeature_upstreamnonfree.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/ro/antiFeatures.yml` & `fdroidserver-2.3a1/tests/config/ro/antiFeatures.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config/zh-rCN/antiFeatures.yml` & `fdroidserver-2.3a1/tests/config/zh-rCN/antiFeatures.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/config.py` & `fdroidserver-2.3a1/tests/config.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/corrupt-featureGraphic.png` & `fdroidserver-2.3a1/tests/corrupt-featureGraphic.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/deploy.TestCase` & `fdroidserver-2.3a1/tests/deploy.TestCase`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python3
 
 import inspect
 import logging
-import optparse
 import os
 import sys
 import tempfile
 import unittest
 from pathlib import Path
 from unittest import mock
 
@@ -15,15 +14,15 @@
 )
 if localmodule not in sys.path:
     sys.path.insert(0, localmodule)
 
 import fdroidserver.common
 import fdroidserver.deploy
 from fdroidserver.exception import FDroidException
-from testcommon import TmpCwd, mkdtemp
+from testcommon import TmpCwd, mkdtemp, parse_args_for_test
 
 
 class DeployTest(unittest.TestCase):
     '''fdroidserver/deploy.py'''
 
     def setUp(self):
         logging.basicConfig(level=logging.DEBUG)
@@ -108,20 +107,22 @@
     def test_update_serverwebroot_no_rsync_error(self):
         os.environ['PATH'] = self.testdir
         os.chdir(self.testdir)
         with self.assertRaises(FDroidException):
             fdroidserver.deploy.update_serverwebroot('serverwebroot', 'repo')
 
     def test_update_serverwebroot_make_cur_version_link(self):
+        self.maxDiff = None
+
         # setup parameters for this test run
-        fdroidserver.deploy.options = mock.Mock()
-        fdroidserver.deploy.options.no_checksum = True
-        fdroidserver.deploy.options.identity_file = None
-        fdroidserver.deploy.options.verbose = False
-        fdroidserver.deploy.options.quiet = True
+        fdroidserver.common.options = mock.Mock()
+        fdroidserver.common.options.no_checksum = True
+        fdroidserver.common.options.identity_file = None
+        fdroidserver.common.options.verbose = False
+        fdroidserver.common.options.quiet = True
         fdroidserver.deploy.config = {'make_current_version_link': True}
         url = "example.com:/var/www/fdroid"
         repo_section = 'repo'
 
         # setup function for asserting subprocess.call invocations
         call_iteration = 0
 
@@ -133,14 +134,16 @@
                     [
                         'rsync',
                         '--archive',
                         '--delete-after',
                         '--safe-links',
                         '--quiet',
                         '--exclude',
+                        'repo/altstore-index.json',
+                        '--exclude',
                         'repo/entry.jar',
                         '--exclude',
                         'repo/entry.json',
                         '--exclude',
                         'repo/entry.json.asc',
                         '--exclude',
                         'repo/index-v1.jar',
@@ -200,20 +203,20 @@
             os.symlink('repo/com.example.sym.apk.sig', 'Sym.apk.sig')
             with mock.patch('subprocess.call', side_effect=update_server_webroot_call):
                 fdroidserver.deploy.update_serverwebroot({'url': url}, repo_section)
         self.assertEqual(call_iteration, 3, 'expected 3 invocations of subprocess.call')
 
     def test_update_serverwebroot_with_id_file(self):
         # setup parameters for this test run
-        fdroidserver.deploy.options = mock.Mock()
-        fdroidserver.deploy.options.identity_file = None
-        fdroidserver.deploy.options.no_checksum = True
-        fdroidserver.deploy.options.verbose = True
-        fdroidserver.deploy.options.quiet = False
-        fdroidserver.deploy.options.identity_file = None
+        fdroidserver.common.options = mock.Mock()
+        fdroidserver.common.options.identity_file = None
+        fdroidserver.common.options.no_checksum = True
+        fdroidserver.common.options.verbose = True
+        fdroidserver.common.options.quiet = False
+        fdroidserver.common.options.identity_file = None
         fdroidserver.deploy.config = {'identity_file': './id_rsa'}
         url = "example.com:/var/www/fdroid"
         repo_section = 'archive'
 
         # setup function for asserting subprocess.call invocations
         call_iteration = 0
 
@@ -228,14 +231,16 @@
                         '--delete-after',
                         '--safe-links',
                         '--verbose',
                         '-e',
                         'ssh -oBatchMode=yes -oIdentitiesOnly=yes -i '
                         + fdroidserver.deploy.config['identity_file'],
                         '--exclude',
+                        'archive/altstore-index.json',
+                        '--exclude',
                         'archive/entry.jar',
                         '--exclude',
                         'archive/entry.json',
                         '--exclude',
                         'archive/entry.json.asc',
                         '--exclude',
                         'archive/index-v1.jar',
@@ -280,15 +285,15 @@
             fdroidserver.deploy.update_serverwebroot({'url': url}, repo_section)
         self.assertEqual(call_iteration, 2, 'expected 2 invocations of subprocess.call')
 
     @unittest.skipIf(
         not os.getenv('VIRUSTOTAL_API_KEY'), 'VIRUSTOTAL_API_KEY is not set'
     )
     def test_upload_to_virustotal(self):
-        fdroidserver.deploy.options.verbose = True
+        fdroidserver.common.options.verbose = True
         virustotal_apikey = os.getenv('VIRUSTOTAL_API_KEY')
         fdroidserver.deploy.upload_to_virustotal('repo', virustotal_apikey)
 
     def test_remote_hostname_regex(self):
         for remote_url, name in (
             ('git@github.com:guardianproject/fdroid-repo', 'github'),
             ('git@gitlab.com:guardianproject/fdroid-repo', 'gitlab'),
@@ -298,20 +303,20 @@
         ):
             self.assertEqual(
                 name, fdroidserver.deploy.REMOTE_HOSTNAME_REGEX.sub(r'\1', remote_url)
             )
 
     def test_update_servergitmirrors(self):
         # setup parameters for this test run
-        fdroidserver.deploy.options = mock.Mock()
-        fdroidserver.deploy.options.identity_file = None
-        fdroidserver.deploy.options.no_keep_git_mirror_archive = False
-        fdroidserver.deploy.options.verbose = False
-        fdroidserver.deploy.options.quiet = True
-        fdroidserver.deploy.options.index_only = False
+        fdroidserver.common.options = mock.Mock()
+        fdroidserver.common.options.identity_file = None
+        fdroidserver.common.options.no_keep_git_mirror_archive = False
+        fdroidserver.common.options.verbose = False
+        fdroidserver.common.options.quiet = True
+        fdroidserver.common.options.index_only = False
 
         config = {}
         fdroidserver.common.fill_config_defaults(config)
         fdroidserver.deploy.config = config
         fdroidserver.deploy.config["servergitmirrors"] = []
 
         repo_section = 'repo'
@@ -380,20 +385,22 @@
             remote_push_call_iteration, 1, 'expected 1 invocations of git.Remote.push'
         )
 
 
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (fdroidserver.common.options, args) = parser.parse_args(['--verbose'])
+    parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(DeployTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/dummy-keystore.jks` & `fdroidserver-2.3a1/tests/dummy-keystore.jks`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/dump_internal_metadata_format.py` & `fdroidserver-2.3a1/tests/dump_internal_metadata_format.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 
     return dumper.represent_dict(output)
 
 
 parser = ArgumentParser()
 fdroidserver.common.setup_global_opts(parser)
 fdroidserver.metadata.add_metadata_arguments(parser)
-options = parser.parse_args()
+options = fdroidserver.common.parse_args(parser)
 fdroidserver.metadata.warnings_action = options.W
-fdroidserver.common.read_config(None)
+fdroidserver.common.read_config()
 
 if not os.path.isdir('metadata'):
     print("This script must be run in an F-Droid data folder with a 'metadata' subdir!")
     sys.exit(1)
 
 repo = git.Repo(localmodule)
 savedir = os.path.join('metadata', 'dump_' + repo.git.rev_parse('HEAD'))
```

### Comparing `fdroidserver-2.3a0/tests/exception.TestCase` & `fdroidserver-2.3a1/tests/exception.TestCase`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 
 # http://www.drdobbs.com/testing/unit-testing-with-python/240165163
 
 import inspect
-import optparse
 import os
 import sys
 import unittest
 
 localmodule = os.path.realpath(
     os.path.join(os.path.dirname(inspect.getfile(inspect.currentframe())), '..')
 )
@@ -53,21 +52,23 @@
         except fdroidserver.exception.FDroidException as e:
             str(e)
 
 
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+    from testcommon import parse_args_for_test
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (fdroidserver.exception.options, args) = parser.parse_args(['--verbose'])
-    fdroidserver.common.options = fdroidserver.exception.options
+    parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(ExceptionTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/extra/manual-vmtools-test.py` & `fdroidserver-2.3a1/tests/extra/manual-vmtools-test.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/funding-usernames.yaml` & `fdroidserver-2.3a1/tests/funding-usernames.yaml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/ndk-bundle/package.xml` & `fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/ndk-bundle/package.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/get_android_tools_versions/android-sdk/patcher/v4/source.properties` & `fdroidserver-2.3a1/tests/get_android_tools_versions/android-sdk/patcher/v4/source.properties`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/gnupghome/pubring.gpg` & `fdroidserver-2.3a1/tests/gnupghome/pubring.gpg`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/gnupghome/random_seed` & `fdroidserver-2.3a1/tests/gnupghome/random_seed`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/gnupghome/secring.gpg` & `fdroidserver-2.3a1/tests/gnupghome/secring.gpg`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/gnupghome/trustdb.gpg` & `fdroidserver-2.3a1/tests/gnupghome/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/gradle-maven-blocks.yaml` & `fdroidserver-2.3a1/tests/gradle-maven-blocks.yaml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/gradle-release-checksums.py` & `fdroidserver-2.3a1/tests/gradle-release-checksums.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/import_subcommand.TestCase` & `fdroidserver-2.3a1/tests/import_subcommand.TestCase`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 #!/usr/bin/env python3
 
 # http://www.drdobbs.com/testing/unit-testing-with-python/240165163
 
 import git
 import logging
-import optparse
 import os
 import shutil
 import sys
 import tempfile
 import unittest
 import yaml
 from unittest import mock
 from pathlib import Path
 
 import requests
-from testcommon import TmpCwd, mkdtemp
 
 localmodule = Path(__file__).resolve().parent.parent
 print('localmodule: ' + str(localmodule))
 if localmodule not in sys.path:
     sys.path.insert(0, str(localmodule))
 
 import fdroidserver.common
 import fdroidserver.import_subcommand
 import fdroidserver.metadata
 from fdroidserver.exception import FDroidException
+from testcommon import TmpCwd, mkdtemp, parse_args_for_test
 
 
 class ImportTest(unittest.TestCase):
     '''fdroid import'''
 
     def setUp(self):
         logging.basicConfig(level=logging.DEBUG)
         self.basedir = localmodule / 'tests'
-        fdroidserver.import_subcommand.options = mock.Mock()
-        fdroidserver.import_subcommand.options.rev = None
         os.chdir(self.basedir)
         self._td = mkdtemp()
         self.testdir = self._td.name
 
     def tearDown(self):
         os.chdir(self.basedir)
         self._td.cleanup()
@@ -142,35 +139,39 @@
         the network, if it gets past the code that throws the error.
 
         """
         with self.assertRaises(FDroidException):
             fdroidserver.import_subcommand.main()
 
     @mock.patch('sys.argv', ['fdroid import', '-u', 'https://fake/git/url.git'])
-    @mock.patch('fdroidserver.import_subcommand.clone_to_tmp_dir', lambda a: Path('td'))
+    @mock.patch(
+        'fdroidserver.import_subcommand.clone_to_tmp_dir', lambda a, r: Path('td')
+    )
     def test_main_local_git(self):
         os.chdir(self.testdir)
         git.Repo.init('td')
         with Path('td/build.gradle').open('w') as fp:
             fp.write('android { defaultConfig { applicationId "com.example" } }')
         fdroidserver.import_subcommand.main()
         with open('metadata/com.example.yml') as fp:
             data = yaml.safe_load(fp)
         self.assertEqual(data['Repo'], sys.argv[2])
         self.assertEqual(data['RepoType'], 'git')
         self.assertEqual(1, len(data['Builds']))
 
 
 if __name__ == "__main__":
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (fdroidserver.common.options, args) = parser.parse_args(['--verbose'])
+    parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(ImportTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/index.TestCase` & `fdroidserver-2.3a1/tests/index.TestCase`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 import copy
 import datetime
+import glob
 import inspect
 import logging
-import optparse
 import os
 import sys
 import unittest
 import yaml
 import zipfile
 from unittest.mock import patch
 import requests
@@ -21,15 +21,15 @@
 )
 print('localmodule: ' + localmodule)
 if localmodule not in sys.path:
     sys.path.insert(0, localmodule)
 
 import fdroidserver
 from fdroidserver import common, index, publish, signindex, update
-from testcommon import TmpCwd, mkdtemp
+from testcommon import TmpCwd, mkdtemp, parse_args_for_test
 from pathlib import Path
 
 
 GP_FINGERPRINT = 'B7C2EEFD8DAC7806AF67DFCD92EB18126BC08312A7F2D6F3862E46013C7A6135'
 
 
 class Options:
@@ -51,15 +51,15 @@
     def setUp(self):
         logging.basicConfig(level=logging.ERROR)
         os.chmod(os.path.join(self.basedir, 'config.py'), 0o600)
         os.chdir(self.basedir)  # so read_config() can find config.py
 
         common.config = None
         common.options = Options
-        config = common.read_config(common.options)
+        config = common.read_config()
         config['jarsigner'] = common.find_sdk_tools_cmd('jarsigner')
         common.config = config
         signindex.config = config
         update.config = config
 
         self._td = mkdtemp()
         self.testdir = self._td.name
@@ -414,14 +414,25 @@
 
             index.v1_sort_packages(
                 i, common.load_stats_fdroid_signing_key_fingerprints()
             )
             self.maxDiff = None
             self.assertEqual(json.dumps(i, indent=2), json.dumps(o, indent=2))
 
+            # and test it still works with get_first_signer_certificate
+            outdir = os.path.join(self.testdir, 'publishsigkeys')
+            os.mkdir(outdir)
+            common.apk_extract_signatures(jarfile, outdir)
+            certs = glob.glob(os.path.join(outdir, '*.RSA'))
+            with open(certs[0], 'rb') as fp:
+                self.assertEqual(
+                    common.get_certificate(fp.read()),
+                    common.get_first_signer_certificate(jarfile),
+                )
+
     def test_make_v0_repo_only(self):
         os.chdir(self.testdir)
         os.mkdir('repo')
         repo_icons_dir = os.path.join('repo', 'icons')
         self.assertFalse(os.path.isdir(repo_icons_dir))
         repodict = {
             'address': 'https://example.com/fdroid/repo',
@@ -697,16 +708,22 @@
                     self.assertTrue(isinstance(metadata[_kn(k)], str))
 
         # make sure these known values were properly parsed and included
         appid = 'info.guardianproject.urzip'
         app = apps[appid]
         metadata = index.package_metadata(app, 'repo')
         # files
-        self.assertEqual(36027, metadata['featureGraphic']['en-US']['size'])
-        self.assertEqual(1413, metadata['icon']['en-US']['size'])
+        self.assertEqual(
+            os.path.getsize(f'repo/{appid}/en-US/featureGraphic.png'),
+            metadata['featureGraphic']['en-US']['size'],
+        )
+        self.assertEqual(
+            os.path.getsize(f'repo/{appid}/en-US/icon.png'),
+            metadata['icon']['en-US']['size'],
+        )
         # localized strings
         self.assertEqual({'en-US': 'title'}, metadata['name'])
         self.assertEqual({'en-US': 'video'}, metadata['video'])
         # strings
         self.assertEqual(
             'https://dev.guardianproject.info/projects/urzip',
             metadata['webSite'],
@@ -730,15 +747,15 @@
         os.chdir(self.testdir)
         repo_url = 'https://example.com/fdroid/repo'
         c = {'repo_url': repo_url, 'mirrors': ['http://one/fdroid']}
         with open('config.yml', 'w') as fp:
             yaml.dump(c, fp)
         os.system('cat config.yml')
         common.config = None
-        common.read_config(Options)
+        common.read_config()
         repodict = {'address': common.config['repo_url']}
         index.add_mirrors_to_repodict('repo', repodict)
         self.assertEqual(
             repodict['mirrors'],
             [
                 {'url': 'https://example.com/fdroid/repo', 'isPrimary': True},
                 {'url': 'http://one/fdroid/repo'},
@@ -825,24 +842,118 @@
             'address': 'https://foo.com',
             'mirrors': {'url': 'http://two/fdroid/repo'},
         }
         with self.assertRaises(fdroidserver.exception.FDroidException):
             index.add_mirrors_to_repodict('repo', repodict)
 
 
+class AltstoreIndexTest(unittest.TestCase):
+    def test_make_altstore(self):
+        self.maxDiff = None
+
+        apps = {
+            "app.fake": {
+                "AutoName": "Fake App",
+                "AuthorName": "Fake Author",
+                "iconv2": {"en_US": "fake_icon.png"},
+            }
+        }
+        apks = [
+            {
+                "packageName": "app.fake",
+                "apkName": "app.fake_123.ipa",
+                "versionName": "v123",
+                "added": datetime.datetime(2000, 2, 2, 2, 2, 2),
+                "size": 123,
+                "ipa_MinimumOSVersion": "10.0",
+                "ipa_DTPlatformVersion": "12.0",
+                "ipa_permissions": [
+                    "NSCameraUsageDescription",
+                    "NSDocumentsFolderUsageDescription",
+                ],
+                "ipa_entitlements": [
+                    "com.apple.developer.team-identifier",
+                    "com.apple.developer.web-browser",
+                    "keychain-access-groups",
+                ],
+            },
+        ]
+        config = {
+            "repo_icon": "fake_repo_icon.png",
+            "repo_name": "fake_repo",
+            "repo_url": "gopher://fake-repo.com/fdroid/repo",
+        }
+
+        with tempfile.TemporaryDirectory() as tmpdir, TmpCwd(tmpdir):
+            repodir = Path(tmpdir) / 'repo'
+            repodir.mkdir()
+            with open(repodir / "fake.ipa", "w") as f:
+                f.write("")
+
+            fdroidserver.index.make_altstore(
+                apps,
+                apks,
+                config,
+                repodir,
+                True,
+            )
+
+            with open(repodir / "altstore-index.json", 'r') as f:
+                self.assertDictEqual(
+                    {
+                        "apps": [
+                            {
+                                "appPermissions": {
+                                    "entitlements": [
+                                        'com.apple.developer.team-identifier',
+                                        'com.apple.developer.web-browser',
+                                        'keychain-access-groups',
+                                    ],
+                                    'privacy': [
+                                        'NSCameraUsageDescription',
+                                        'NSDocumentsFolderUsageDescription',
+                                    ],
+                                },
+                                'bundleIdentifier': 'app.fake',
+                                'developerName': 'Fake Author',
+                                'iconURL': 'gopher://fake-repo.com/fdroid/repo',
+                                'localizedDescription': '',
+                                'name': 'Fake App',
+                                'screenshots': [],
+                                'versions': [
+                                    {
+                                        'date': '2000-02-02T02:02:02',
+                                        'downloadURL': 'gopher://fake-repo.com/fdroid/repo/app.fake_123.ipa',
+                                        'maxOSVersion': '12.0',
+                                        'minOSVersion': '10.0',
+                                        'size': 123,
+                                        'version': 'v123',
+                                    }
+                                ],
+                            },
+                        ],
+                        'name': 'fake_repo',
+                        'news': [],
+                    },
+                    json.load(f),
+                )
+
+
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (options, args) = parser.parse_args(["--verbose"])
-    Options.verbose = options.verbose
+    parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(IndexTest))
+    newSuite.addTest(unittest.makeSuite(AltstoreIndexTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/init.TestCase` & `fdroidserver-2.3a1/tests/init.TestCase`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 #!/usr/bin/env python3
 
 # http://www.drdobbs.com/testing/unit-testing-with-python/240165163
 
 import inspect
 import logging
 import os
-import optparse
 import shutil
 import sys
 import unittest
 
 
 localmodule = os.path.realpath(
     os.path.join(os.path.dirname(inspect.getfile(inspect.currentframe())), '..')
 )
 print('localmodule: ' + localmodule)
 if localmodule not in sys.path:
     sys.path.insert(0, localmodule)
 
 import fdroidserver.init
-from testcommon import mkdtemp
+from testcommon import mkdtemp, parse_args_for_test
 
 
 class InitTest(unittest.TestCase):
     '''fdroidserver/init.py'''
 
     def setUp(self):
         logging.basicConfig(level=logging.DEBUG)
@@ -39,22 +38,22 @@
 
     def test_disable_in_config(self):
         os.chdir(self.testdir)
         with open('config.yml', 'w') as fp:
             fp.write('keystore: NONE\n')
             fp.write('keypass: mysupersecrets\n')
         os.chmod('config.yml', 0o600)
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertEqual('NONE', config['keystore'])
         self.assertEqual('mysupersecrets', config['keypass'])
         fdroidserver.init.disable_in_config('keypass', 'comment')
         with open(fp.name) as fp:
             self.assertTrue('#keypass:' in fp.read())
         fdroidserver.common.config = None
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         self.assertIsNone(config.get('keypass'))
 
     @unittest.skipIf(os.name == 'nt', "calling main() like this hangs on Windows")
     def test_main_in_empty_dir(self):
         """Test that `fdroid init` will find apksigner and add it to the config"""
         os.chdir(self.testdir)
 
@@ -71,20 +70,22 @@
         fdroidserver.init.main()
         self.assertEqual(apksigner, fdroidserver.init.config.get('apksigner'))
 
 
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (fdroidserver.init.options, args) = parser.parse_args(['--verbose'])
+    fdroidserver.init.options = parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(InitTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/install.TestCase` & `fdroidserver-2.3a1/tests/install.TestCase`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 
 # http://www.drdobbs.com/testing/unit-testing-with-python/240165163
 
 import inspect
-import optparse
 import os
 import sys
 import unittest
 
 localmodule = os.path.realpath(
     os.path.join(os.path.dirname(inspect.getfile(inspect.currentframe())), '..')
 )
@@ -34,21 +33,23 @@
         for device in devices:
             self.assertIsInstance(device, str)
 
 
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+    from testcommon import parse_args_for_test
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (fdroidserver.install.options, args) = parser.parse_args(['--verbose'])
-    fdroidserver.common.options = fdroidserver.install.options
+    fdroidserver.install.options = parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(InstallTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/janus.apk` & `fdroidserver-2.3a1/tests/janus.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/key-tricks.py` & `fdroidserver-2.3a1/tests/key-tricks.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from fdroidserver import common, nightly
 
 if os.getenv('CI') is None:
     print('ERROR: This can overwrite SSH keys, so it should only be run in CI')
     sys.exit(1)
 
 os.chdir(os.path.dirname(__file__))
-config = fdroidserver.common.read_config(common.options)
+config = fdroidserver.common.read_config()
 nightly.PASSWORD = config['keystorepass']
 nightly.KEY_ALIAS = config['repo_keyalias']
 
 privkey = nightly._ssh_key_from_debug_keystore('keystore.jks')
 print('privkey', privkey)
 ssh_private_key_file = os.path.join(os.getenv('HOME'), '.ssh', 'id_rsa')
 if os.path.exists(ssh_private_key_file):
```

### Comparing `fdroidserver-2.3a0/tests/keystore.jks` & `fdroidserver-2.3a1/tests/keystore.jks`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/lint.TestCase` & `fdroidserver-2.3a1/tests/lint.TestCase`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 #!/usr/bin/env python3
 
 # http://www.drdobbs.com/testing/unit-testing-with-python/240165163
 
 import logging
-import optparse
 import os
 import ruamel.yaml
 import shutil
 import sys
 import tempfile
 import unittest
 from pathlib import Path
-from testcommon import mkdtemp
 
 localmodule = Path(__file__).resolve().parent.parent
 print('localmodule: ' + str(localmodule))
 if localmodule not in sys.path:
     sys.path.insert(0, str(localmodule))
 
 import fdroidserver.common
 import fdroidserver.lint
 import fdroidserver.metadata
 from fdroidserver.common import CATEGORIES_CONFIG_NAME
+from testcommon import mkdtemp, parse_args_for_test
 
 
 class LintTest(unittest.TestCase):
     '''fdroidserver/lint.py'''
 
     def setUp(self):
         logging.basicConfig(level=logging.DEBUG)
@@ -434,14 +433,53 @@
 
     def test_lint_config_bad_mirrors_yml_str(self):
         os.chdir(self.testdir)
         Path('mirrors.yml').write_text('foo\n')
         with self.assertRaises(TypeError):
             fdroidserver.lint.lint_config('mirrors.yml')
 
+    def test_check_certificate_pinned_binaries_empty(self):
+        fdroidserver.common.config = {}
+        app = fdroidserver.metadata.App()
+        app.AllowedAPKSigningKeys = [
+            'a40da80a59d170caa950cf15c18c454d47a39b26989d8b640ecd745ba71bf5dc'
+        ]
+        self.assertEqual(
+            [],
+            list(fdroidserver.lint.check_certificate_pinned_binaries(app)),
+            "when the config is empty, any signing key should be allowed",
+        )
+
+    def test_lint_known_debug_keys_no_match(self):
+        fdroidserver.common.config = {
+            "apk_signing_key_block_list": "a40da80a59d170caa950cf15c18c454d47a39b26989d8b640ecd745ba71bf5dc"
+        }
+        app = fdroidserver.metadata.App()
+        app.AllowedAPKSigningKeys = [
+            '2fd4fd5f54babba4bcb21237809bb653361d0d2583c80964ec89b28a26e9539e'
+        ]
+        self.assertEqual(
+            [],
+            list(fdroidserver.lint.check_certificate_pinned_binaries(app)),
+            "A signing key that does not match one in the config should be allowed",
+        )
+
+    def test_lint_known_debug_keys(self):
+        fdroidserver.common.config = {
+            'apk_signing_key_block_list': 'a40da80a59d170caa950cf15c18c454d47a39b26989d8b640ecd745ba71bf5dc'
+        }
+        app = fdroidserver.metadata.App()
+        app.AllowedAPKSigningKeys = [
+            'a40da80a59d170caa950cf15c18c454d47a39b26989d8b640ecd745ba71bf5dc'
+        ]
+        for warn in fdroidserver.lint.check_certificate_pinned_binaries(app):
+            anywarns = True
+            logging.debug(warn)
+        self.assertTrue(anywarns)
+
 
 class LintAntiFeaturesTest(unittest.TestCase):
     def setUp(self):
         self.basedir = localmodule / 'tests'
         os.chdir(self.basedir)
         fdroidserver.common.config = dict()
         fdroidserver.lint.ANTIFEATURES_KEYS = None
@@ -484,21 +522,22 @@
     def test_check_antiFeatures_build_fail(self):
         app = fdroidserver.metadata.App()
         app['Builds'] = [{'antifeatures': ['Ads', 'Tracker']}]
         self.assertEqual(1, len(list(fdroidserver.lint.check_antiFeatures(app))))
 
 
 if __name__ == "__main__":
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (fdroidserver.lint.options, args) = parser.parse_args(['--verbose'])
-    fdroidserver.common.options = fdroidserver.lint.options
+    fdroidserver.lint.options = parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(LintTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/main.TestCase` & `fdroidserver-2.3a1/tests/main.TestCase`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 #!/usr/bin/env python3
 
 import inspect
-import optparse
 import os
 import sys
 import pkgutil
 import textwrap
 import unittest
 import tempfile
 from unittest import mock
-from testcommon import TmpCwd, TmpPyPath
 
 localmodule = os.path.realpath(
     os.path.join(os.path.dirname(inspect.getfile(inspect.currentframe())), '..')
 )
 print('localmodule: ' + localmodule)
 if localmodule not in sys.path:
     sys.path.insert(0, localmodule)
 
 from fdroidserver import common
 import fdroidserver.__main__
+from testcommon import TmpCwd, TmpPyPath
 
 
 class MainTest(unittest.TestCase):
     '''this tests fdroid.py'''
 
     def test_COMMANDS_check(self):
         """make sure the built in sub-command defs didn't change unintentionally"""
@@ -261,20 +260,22 @@
                 d = fdroidserver.__main__.preparse_plugin(module_name, module_path)
             self.assertDictEqual(d, {'name': 'fdroid_testy8', 'summary': 'ttt'})
 
 
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (common.options, args) = parser.parse_args(['--verbose'])
+    common.options = common.parse_args(parser)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(MainTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/metadata/apk/info.guardianproject.urzip.yaml` & `fdroidserver-2.3a1/tests/metadata/apk/info.guardianproject.urzip.yaml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/apk/org.dyndns.fules.ck.yaml` & `fdroidserver-2.3a1/tests/metadata/apk/org.dyndns.fules.ck.yaml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/app.with.special.build.params.yml` & `fdroidserver-2.3a1/tests/metadata/app.with.special.build.params.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/com.politedroid.yml` & `fdroidserver-2.3a1/tests/metadata/com.politedroid.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/dump/app.with.special.build.params.yaml` & `fdroidserver-2.3a1/tests/metadata/dump/app.with.special.build.params.yaml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/dump/com.politedroid.yaml` & `fdroidserver-2.3a1/tests/metadata/dump/com.politedroid.yaml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/dump/org.adaway.yaml` & `fdroidserver-2.3a1/tests/metadata/dump/org.adaway.yaml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/dump/org.smssecure.smssecure.yaml` & `fdroidserver-2.3a1/tests/metadata/dump/org.smssecure.smssecure.yaml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/dump/org.videolan.vlc.yaml` & `fdroidserver-2.3a1/tests/metadata/dump/org.videolan.vlc.yaml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/fake.ota.update.yml` & `fdroidserver-2.3a1/tests/metadata/fake.ota.update.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/info.guardianproject.checkey/en-US/phoneScreenshots/checkey-phone.png` & `fdroidserver-2.3a1/tests/metadata/info.guardianproject.checkey/en-US/phoneScreenshots/checkey-phone.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/info.guardianproject.checkey/en-US/phoneScreenshots/checkey.png` & `fdroidserver-2.3a1/tests/metadata/info.guardianproject.checkey/en-US/phoneScreenshots/checkey.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/en-US/images/featureGraphic.png` & `fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/en-US/images/featureGraphic.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip/en-US/images/icon.png` & `fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip/en-US/images/icon.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/info.guardianproject.urzip.yml` & `fdroidserver-2.3a1/tests/metadata/info.guardianproject.urzip.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/org.adaway.yml` & `fdroidserver-2.3a1/tests/metadata/org.adaway.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/org.fdroid.fdroid.yml` & `fdroidserver-2.3a1/tests/metadata/org.fdroid.fdroid.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/134/28969C09.RSA` & `fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/134/28969C09.RSA`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/134/28969C09.SF` & `fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/134/28969C09.SF`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/134/MANIFEST.MF` & `fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/134/MANIFEST.MF`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/135/28969C09.RSA` & `fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/135/28969C09.RSA`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/135/28969C09.SF` & `fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/135/28969C09.SF`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure/signatures/135/MANIFEST.MF` & `fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure/signatures/135/MANIFEST.MF`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/org.smssecure.smssecure.yml` & `fdroidserver-2.3a1/tests/metadata/org.smssecure.smssecure.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/org.videolan.vlc.yml` & `fdroidserver-2.3a1/tests/metadata/org.videolan.vlc.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata/souch.smsbypass.yml` & `fdroidserver-2.3a1/tests/metadata/souch.smsbypass.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata-rewrite-yml/app.with.special.build.params.yml` & `fdroidserver-2.3a1/tests/metadata-rewrite-yml/app.with.special.build.params.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata-rewrite-yml/fake.ota.update.yml` & `fdroidserver-2.3a1/tests/metadata-rewrite-yml/fake.ota.update.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata-rewrite-yml/org.fdroid.fdroid.yml` & `fdroidserver-2.3a1/tests/metadata-rewrite-yml/org.fdroid.fdroid.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/metadata.TestCase` & `fdroidserver-2.3a1/tests/metadata.TestCase`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 #!/usr/bin/env python3
 
 import copy
 import io
 import logging
-import optparse
 import os
 import random
 import ruamel.yaml
 import shutil
 import sys
 import unittest
 import tempfile
 import textwrap
 from collections import OrderedDict
 from pathlib import Path
 from unittest import mock
 
-from testcommon import TmpCwd, mkdtemp
-
 localmodule = Path(__file__).resolve().parent.parent
 print('localmodule: ' + str(localmodule))
 if localmodule not in sys.path:
     sys.path.insert(0, str(localmodule))
 
 import fdroidserver
 from fdroidserver import metadata
 from fdroidserver.exception import MetaDataException
 from fdroidserver.common import DEFAULT_LOCALE
+from testcommon import TmpCwd, mkdtemp, parse_args_for_test
 
 
 def _get_mock_mf(s):
     mf = io.StringIO(s)
     mf.name = 'mock_filename.yaml'
     return mf
 
@@ -2443,20 +2441,22 @@
             self._post_metadata_parse_build_int(True, MetaDataException)
         self.assertEqual(*self._post_metadata_parse_build_list(True, ['true']))
         self.assertEqual(*self._post_metadata_parse_build_script(True, ['true']))
         self.assertEqual(*self._post_metadata_parse_build_string(True, 'true'))
 
 
 if __name__ == "__main__":
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (fdroidserver.common.options, args) = parser.parse_args(['--verbose'])
+    parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(MetadataTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/minimal_targetsdk_30_unsigned.apk` & `fdroidserver-2.3a1/tests/minimal_targetsdk_30_unsigned.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/nightly.TestCase` & `fdroidserver-2.3a1/tests/nightly.TestCase`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python3
 
 import inspect
 import logging
-import optparse
 import os
 import requests
 import shutil
 import subprocess
 import sys
 import tempfile
 import time
@@ -66,15 +65,18 @@
         self.home = self.testdir / 'home'
         self.home.mkdir()
         self.dot_android = self.home / '.android'
         nightly.KEYSTORE_FILE = str(self.dot_android / 'debug.keystore')
 
     def tearDown(self):
         self.tempdir.cleanup()
-        os.rmdir(self.testroot)
+        try:
+            os.rmdir(self.testroot)
+        except OSError:  # other test modules might have left stuff around
+            pass
 
     def _copy_test_debug_keystore(self):
         self.dot_android.mkdir()
         shutil.copy(
             self.basedir / 'aosp_testkey_debug.keystore',
             self.dot_android / 'debug.keystore',
         )
@@ -357,20 +359,22 @@
             del config['identity_file']
             self.assertEqual(expected, config)
 
 
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (common.options, args) = parser.parse_args(['--verbose'])
+    common.options = common.parse_args(parser)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(NightlyTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/no_targetsdk_minsdk1_unsigned.apk` & `fdroidserver-2.3a1/tests/no_targetsdk_minsdk1_unsigned.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/no_targetsdk_minsdk30_unsigned.apk` & `fdroidserver-2.3a1/tests/no_targetsdk_minsdk30_unsigned.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/openssl-version-check-test.py` & `fdroidserver-2.3a1/tests/openssl-version-check-test.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/org.bitbucket.tickytacky.mirrormirror_1.apk` & `fdroidserver-2.3a1/tests/org.bitbucket.tickytacky.mirrormirror_1.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/org.bitbucket.tickytacky.mirrormirror_2.apk` & `fdroidserver-2.3a1/tests/org.bitbucket.tickytacky.mirrormirror_2.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/org.bitbucket.tickytacky.mirrormirror_3.apk` & `fdroidserver-2.3a1/tests/org.bitbucket.tickytacky.mirrormirror_3.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/org.bitbucket.tickytacky.mirrormirror_4.apk` & `fdroidserver-2.3a1/tests/org.bitbucket.tickytacky.mirrormirror_4.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/org.dyndns.fules.ck_20.apk` & `fdroidserver-2.3a1/tests/org.dyndns.fules.ck_20.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/org.sajeg.fallingblocks_3.apk` & `fdroidserver-2.3a1/tests/org.sajeg.fallingblocks_3.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/publish.TestCase` & `fdroidserver-2.3a1/tests/publish.TestCase`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #        -validity '10000' -storepass 123456 -storetype jks \
 #        -keypass 123456 -dname 'CN=test, OU=F-Droid'; done
 #
 
 import inspect
 import json
 import logging
-import optparse
 import os
 import shutil
 import sys
 import unittest
 import tempfile
 import textwrap
 from unittest import mock
@@ -30,15 +29,15 @@
     sys.path.insert(0, localmodule)
 
 from fdroidserver import publish
 from fdroidserver import common
 from fdroidserver import metadata
 from fdroidserver import signatures
 from fdroidserver.exception import FDroidException
-from testcommon import mkdtemp
+from testcommon import mkdtemp, parse_args_for_test
 
 
 class PublishTest(unittest.TestCase):
     '''fdroidserver/publish.py'''
 
     def setUp(self):
         logging.basicConfig(level=logging.DEBUG)
@@ -263,15 +262,16 @@
 
     def test_sign_then_implant_signature(self):
         class Options:
             verbose = False
 
         os.chdir(self.testdir)
 
-        config = common.read_config(Options)
+        common.options = Options
+        config = common.read_config()
         if 'apksigner' not in config:
             self.skipTest('SKIPPING test_sign_then_implant_signature, apksigner not installed!')
         config['repo_keyalias'] = 'sova'
         config['keystorepass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keypass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         shutil.copy(os.path.join(self.basedir, 'keystore.jks'), self.testdir)
         config['keystore'] = 'keystore.jks'
@@ -337,15 +337,16 @@
 
         class Options:
             error_on_failed = True
             verbose = False
 
         os.chdir(self.testdir)
 
-        config = common.read_config(Options)
+        common.options = Options
+        config = common.read_config()
         if 'apksigner' not in config:
             self.skipTest('SKIPPING test_error_on_failed, apksigner not installed!')
         config['repo_keyalias'] = 'sova'
         config['keystorepass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keypass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         shutil.copy(os.path.join(self.basedir, 'keystore.jks'), self.testdir)
         config['keystore'] = 'keystore.jks'
@@ -409,20 +410,22 @@
                 publish.main()
             self.assertEqual(e.exception.code, 1)
 
 
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (common.options, args) = parser.parse_args(['--verbose'])
+    parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(PublishTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/repo/com.example.test.helloworld_1.apk` & `fdroidserver-2.3a1/tests/repo/com.example.test.helloworld_1.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/com.politedroid_3.apk` & `fdroidserver-2.3a1/tests/repo/com.politedroid_3.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/com.politedroid_4.apk` & `fdroidserver-2.3a1/tests/repo/com.politedroid_4.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/com.politedroid_5.apk` & `fdroidserver-2.3a1/tests/repo/com.politedroid_5.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/com.politedroid_6.apk` & `fdroidserver-2.3a1/tests/repo/com.politedroid_6.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/duplicate.permisssions_9999999.apk` & `fdroidserver-2.3a1/tests/repo/duplicate.permisssions_9999999.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/index-v1.json` & `fdroidserver-2.3a1/tests/repo/index-v1.json`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/index-v2.json` & `fdroidserver-2.3a1/tests/repo/index-v2.json`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/index.xml` & `fdroidserver-2.3a1/tests/repo/index.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/info.zwanenburg.caffeinetile_4.apk` & `fdroidserver-2.3a1/tests/repo/info.zwanenburg.caffeinetile_4.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/no.min.target.sdk_987.apk` & `fdroidserver-2.3a1/tests/repo/no.min.target.sdk_987.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/obb.main.oldversion_1444412523.apk` & `fdroidserver-2.3a1/tests/repo/obb.main.oldversion_1444412523.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/obb.main.twoversions_1101613.apk` & `fdroidserver-2.3a1/tests/repo/obb.main.twoversions_1101613.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/obb.main.twoversions_1101615.apk` & `fdroidserver-2.3a1/tests/repo/obb.main.twoversions_1101615.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/obb.main.twoversions_1101617.apk` & `fdroidserver-2.3a1/tests/repo/obb.main.twoversions_1101617.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/obb.mainpatch.current/en-US/featureGraphic.png` & `fdroidserver-2.3a1/tests/repo/obb.mainpatch.current/en-US/featureGraphic.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/obb.mainpatch.current/en-US/icon.png` & `fdroidserver-2.3a1/tests/repo/obb.mainpatch.current/en-US/icon.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/obb.mainpatch.current/en-US/phoneScreenshots/screenshot-main.png` & `fdroidserver-2.3a1/tests/repo/obb.mainpatch.current/en-US/phoneScreenshots/screenshot-main.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/obb.mainpatch.current/en-US/sevenInchScreenshots/screenshot-tablet-main.png` & `fdroidserver-2.3a1/tests/repo/obb.mainpatch.current/en-US/sevenInchScreenshots/screenshot-tablet-main.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/obb.mainpatch.current_1619.apk` & `fdroidserver-2.3a1/tests/repo/obb.mainpatch.current_1619.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/obb.mainpatch.current_1619_another-release-key.apk` & `fdroidserver-2.3a1/tests/repo/obb.mainpatch.current_1619_another-release-key.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/icon.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/icon.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot10.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot10.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot12.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot12.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot15.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot15.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot18.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot18.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot20.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot20.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot22.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot22.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot4.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot4.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot7.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot7.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot9.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/phoneScreenshots/screenshot9.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot0.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot0.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot1.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot1.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot11.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot11.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot13.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot13.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot14.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot14.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot16.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot16.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot17.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot17.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot19.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot19.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot2.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot2.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot21.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot21.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot23.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot23.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot3.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot3.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot5.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot5.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot6.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot6.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot8.png` & `fdroidserver-2.3a1/tests/repo/org.videolan.vlc/en-US/sevenInchScreenshots/screenshot8.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/souch.smsbypass_9.apk` & `fdroidserver-2.3a1/tests/repo/souch.smsbypass_9.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/urzip-; Рахма́, [rɐxˈmanʲɪnəf] سيرجي_رخمانينوف 谢·.apk` & `fdroidserver-2.3a1/tests/repo/urzip-; Рахма́, [rɐxˈmanʲɪnəf] سيرجي_رخمانينوف 谢·.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/repo/v1.v2.sig_1020.apk` & `fdroidserver-2.3a1/tests/repo/v1.v2.sig_1020.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/rewritemeta.TestCase` & `fdroidserver-2.3a1/tests/rewritemeta.TestCase`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 #!/usr/bin/env python3
 
 import logging
-import optparse
 import os
 import sys
 import unittest
 import tempfile
 import textwrap
 from pathlib import Path
 
-from testcommon import TmpCwd, mkdtemp
-
 localmodule = Path(__file__).resolve().parent.parent
 print('localmodule: ' + str(localmodule))
 if localmodule not in sys.path:
     sys.path.insert(0, str(localmodule))
 
 from fdroidserver import common, metadata, rewritemeta
+from testcommon import TmpCwd, mkdtemp
 
 
 class RewriteMetaTest(unittest.TestCase):
     '''fdroidserver/publish.py'''
 
     def setUp(self):
         logging.basicConfig(level=logging.DEBUG)
@@ -261,20 +259,22 @@
                     UpdateCheckMode: None
                     '''
                 ),
             )
 
 
 if __name__ == "__main__":
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (common.options, args) = parser.parse_args(['--verbose'])
+    common.options = common.parse_args(parser)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(RewriteMetaTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/run-tests` & `fdroidserver-2.3a1/tests/run-tests`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 echo_header() {
     { echo -e "==============================================================================\n$1"; } 2>/dev/null
 }
 
 get_fdroid_apk_filename() {
     if [ -z $aapt ]; then
-        python3 -c "from androguard.core.bytecodes.apk import APK; a=APK('$1'); print(a.package+'_'+a.get_androidversion_code()+'.apk')"
+        appid=$(androguard apkid "$1" | sed -En 's/ +"([a-z][^"]+)",$/\1/ip')
+        versionCode=$(androguard apkid "$1" | sed -En 's/ +"([0-9]+)",$/\1/p')
+        echo "${appid}_${versionCode}.apk"
     else
         $aapt dump badging "$1" | sed -n "s,^package: name='\(.*\)' versionCode='\([0-9][0-9]*\)' .*,\1_\2.apk,p"
     fi
 }
 
 copy_apks_into_repo() {
     set +x
```

### Comparing `fdroidserver-2.3a0/tests/scanner.TestCase` & `fdroidserver-2.3a1/tests/scanner.TestCase`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 
 import glob
 import inspect
 import logging
-import optparse
 import os
 import re
 import shutil
 import sys
 import tempfile
 import textwrap
 import unittest
@@ -27,15 +26,15 @@
 if localmodule not in sys.path:
     sys.path.insert(0, localmodule)
 
 import fdroidserver.build
 import fdroidserver.common
 import fdroidserver.metadata
 import fdroidserver.scanner
-from testcommon import TmpCwd, mkdtemp, mock_open_to_str
+from testcommon import TmpCwd, mkdtemp, mock_open_to_str, parse_args_for_test
 
 
 class ScannerTest(unittest.TestCase):
     def setUp(self):
         logging.basicConfig(level=logging.INFO)
         self.basedir = os.path.join(localmodule, 'tests')
         os.chdir(self.basedir)
@@ -43,16 +42,16 @@
         self.testdir = self._td.name
 
     def tearDown(self):
         os.chdir(self.basedir)
         self._td.cleanup()
 
     def test_scan_source_files(self):
-        fdroidserver.scanner.options = mock.Mock()
-        fdroidserver.scanner.options.json = False
+        fdroidserver.common.options = mock.Mock()
+        fdroidserver.common.options.json = False
         source_files = os.path.join(self.basedir, 'source-files')
         projects = {
             'OtakuWorld': 2,
             'Zillode': 1,
             'cn.wildfirechat.chat': 4,
             'com.github.shadowsocks': 7,
             'com.integreight.onesheeld': 16,
@@ -99,16 +98,16 @@
                             i += 1
             self.assertEqual(count, i)
 
     def test_scan_source_files_sneaky_maven(self):
         """Check for sneaking in banned maven repos"""
         os.chdir(self.testdir)
         fdroidserver.scanner.config = None
-        fdroidserver.scanner.options = mock.Mock()
-        fdroidserver.scanner.options.json = True
+        fdroidserver.common.options = mock.Mock()
+        fdroidserver.common.options.json = True
         with open('build.gradle', 'w', encoding='utf-8') as fp:
             fp.write(
                 textwrap.dedent(
                     """
                  maven {
                     "https://jitpack.io"
                     url 'https://maven.fabric.io/public'
@@ -132,16 +131,16 @@
         """
         build_dir = os.path.join('build', 'fake.app')
         abs_build_dir = os.path.join(self.testdir, build_dir)
         os.makedirs(abs_build_dir, exist_ok=True)
         os.chdir(abs_build_dir)
 
         fdroidserver.scanner.config = None
-        fdroidserver.scanner.options = mock.Mock()
-        fdroidserver.scanner.options.json = True
+        fdroidserver.common.options = mock.Mock()
+        fdroidserver.common.options.json = True
 
         keep = [
             'arg.jar',
             'ascii.out',
             'baz.so',
             'classes.dex',
             'sqlcipher.aar',
@@ -232,15 +231,15 @@
         fdroidserver.common.config = config
         fdroidserver.build.config = config
         fdroidserver.build.options = mock.Mock()
         fdroidserver.build.options.json = False
         fdroidserver.build.options.scan_binary = False
         fdroidserver.build.options.notarball = True
         fdroidserver.build.options.skipscan = False
-        fdroidserver.scanner.options = fdroidserver.build.options
+        fdroidserver.common.options = fdroidserver.build.options
 
         app = fdroidserver.metadata.App()
         app.id = 'mocked.app.id'
         build = fdroidserver.metadata.Build()
         build.commit = '1.0'
         build.output = app.id + '.apk'
         build.scanignore = ['baz.so', 'foo.aar']
@@ -311,15 +310,15 @@
             self.assertTrue(found, 'this block should produce a URL:\n' + entry)
         self.assertEqual(len(data), len(urls), 'each data example should produce a URL')
 
     def test_scan_gradle_file_with_multiple_problems(self):
         """Check that the scanner can handle scandelete with gradle files with multiple problems"""
         os.chdir(self.testdir)
         fdroidserver.scanner.config = None
-        fdroidserver.scanner.options = mock.Mock()
+        fdroidserver.common.options = mock.Mock()
         build = fdroidserver.metadata.Build()
         build.scandelete = ['build.gradle']
         with open('build.gradle', 'w', encoding='utf-8') as fp:
             fp.write(
                 textwrap.dedent(
                     """
                  maven {
@@ -729,37 +728,37 @@
     def test_refresh_no_options_or_config(self):
         """This simulates what happens when running something like scan_source()"""
         with mock.patch('fdroidserver.scanner.ScannerTool.refresh') as refresh:
             fdroidserver.scanner.ScannerTool()
             refresh.assert_not_called()
 
     def test_refresh_true(self):
-        fdroidserver.scanner.options = mock.Mock()
-        fdroidserver.scanner.options.refresh_scanner = True
+        fdroidserver.common.options = mock.Mock()
+        fdroidserver.common.options.refresh_scanner = True
         with mock.patch('fdroidserver.scanner.ScannerTool.refresh') as refresh:
             fdroidserver.scanner.ScannerTool()
             refresh.assert_called_once()
 
     def test_refresh_false(self):
-        fdroidserver.scanner.options = mock.Mock()
-        fdroidserver.scanner.options.refresh_scanner = False
+        fdroidserver.common.options = mock.Mock()
+        fdroidserver.common.options.refresh_scanner = False
         with mock.patch('fdroidserver.scanner.ScannerTool.refresh') as refresh:
             fdroidserver.scanner.ScannerTool()
             refresh.assert_not_called()
 
     def test_refresh_from_config(self):
         os.chdir(self.testdir)
         pathlib.Path('config.yml').write_text('refresh_scanner: true')
         with mock.patch('fdroidserver.scanner.ScannerTool.refresh') as refresh:
             fdroidserver.scanner.ScannerTool()
             refresh.assert_called_once()
 
     def test_refresh_options_overrides_config(self):
-        fdroidserver.scanner.options = mock.Mock()
-        fdroidserver.scanner.options.refresh_scanner = True
+        fdroidserver.common.options = mock.Mock()
+        fdroidserver.common.options.refresh_scanner = True
         os.chdir(self.testdir)
         pathlib.Path('config.yml').write_text('refresh_scanner: false')
         with mock.patch('fdroidserver.scanner.ScannerTool.refresh') as refresh:
             fdroidserver.scanner.ScannerTool()
             refresh.assert_called_once()
 
 
@@ -811,23 +810,25 @@
             self.read_app_args_func.assert_not_called()
             self.scan_binary_func.assert_called_once_with('local.application.apk')
 
 
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (fdroidserver.common.options, args) = parser.parse_args(['--verbose'])
+    parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTests(
         [
             unittest.makeSuite(ScannerTest),
             unittest.makeSuite(Test_scan_binary),
             unittest.makeSuite(Test_SignatureDataController),
```

### Comparing `fdroidserver-2.3a0/tests/signatures.TestCase` & `fdroidserver-2.3a1/tests/signatures.TestCase`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 
 import inspect
-import optparse
 import os
 import sys
 import unittest
 import hashlib
 import logging
 from tempfile import TemporaryDirectory
 
@@ -20,15 +19,15 @@
 from fdroidserver import common, signatures
 
 
 class SignaturesTest(unittest.TestCase):
     def setUp(self):
         logging.basicConfig(level=logging.DEBUG)
         common.config = None
-        config = common.read_config(common.options)
+        config = common.read_config()
         config['jarsigner'] = common.find_sdk_tools_cmd('jarsigner')
         config['verbose'] = True
         common.config = config
 
     def test_main(self):
 
         # option fixture class:
@@ -55,20 +54,22 @@
                 with open(path, 'rb') as f:
                     self.assertEqual(hashlib.sha256(f.read()).hexdigest(), checksum)
 
 
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (common.options, args) = parser.parse_args(['--verbose'])
+    common.options = common.parse_args(parser)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(SignaturesTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/signindex/guardianproject-v1.jar` & `fdroidserver-2.3a1/tests/signindex/guardianproject-v1.jar`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/signindex/guardianproject.jar` & `fdroidserver-2.3a1/tests/signindex/guardianproject.jar`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/signindex/testy.jar` & `fdroidserver-2.3a1/tests/signindex/testy.jar`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/signindex/unsigned.jar` & `fdroidserver-2.3a1/tests/signindex/unsigned.jar`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/signindex.TestCase` & `fdroidserver-2.3a1/tests/signindex.TestCase`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 
 import inspect
 import json
 import logging
-import optparse
 import os
 import shutil
 import subprocess
 import sys
 import tempfile
 import unittest
 
@@ -34,15 +33,15 @@
 
 
 class SignindexTest(unittest.TestCase):
     basedir = Path(__file__).resolve().parent
 
     def setUp(self):
         signindex.config = None
-        config = common.read_config(common.options)
+        config = common.read_config()
         config['jarsigner'] = common.find_sdk_tools_cmd('jarsigner')
         config['verbose'] = True
         config['keystore'] = str(self.basedir / 'keystore.jks')
         config['repo_keyalias'] = 'sova'
         config['keystorepass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keypass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         signindex.config = config
@@ -189,20 +188,22 @@
         )
         self.assertFalse(b'SHA1withRSA' in cp.stdout)
 
 
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (common.options, args) = parser.parse_args(['--verbose'])
+    common.options = common.parse_args(parser)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(SignindexTest))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/source-files/Zillode/syncthing-silk/build.gradle` & `fdroidserver-2.3a1/tests/source-files/Zillode/syncthing-silk/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/at.bitfire.davdroid/build.gradle` & `fdroidserver-2.3a1/tests/source-files/at.bitfire.davdroid/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/build.gradle` & `fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/chat/build.gradle` & `fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/chat/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/client/build.gradle` & `fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/client/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/client/src/main/AndroidManifest.xml` & `fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/client/src/main/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/emojilibrary/build.gradle` & `fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/emojilibrary/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/gradle/build_libraries.gradle` & `fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/gradle/build_libraries.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/imagepicker/build.gradle` & `fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/imagepicker/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/cn.wildfirechat.chat/push/build.gradle` & `fdroidserver-2.3a1/tests/source-files/cn.wildfirechat.chat/push/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.anpmech.launcher/app/build.gradle` & `fdroidserver-2.3a1/tests/source-files/com.anpmech.launcher/app/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.anpmech.launcher/app/src/main/AndroidManifest.xml` & `fdroidserver-2.3a1/tests/source-files/com.anpmech.launcher/app/src/main/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.anpmech.launcher/build.gradle` & `fdroidserver-2.3a1/tests/source-files/com.anpmech.launcher/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.anpmech.launcher/settings.gradle` & `fdroidserver-2.3a1/tests/source-files/com.anpmech.launcher/settings.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.github.jameshnsears.quoteunquote/build.gradle` & `fdroidserver-2.3a1/tests/source-files/com.github.jameshnsears.quoteunquote/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/oneSheeld/build.gradle` & `fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/oneSheeld/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.integreight.onesheeld/oneSheeld/src/main/AndroidManifest.xml` & `fdroidserver-2.3a1/tests/source-files/com.integreight.onesheeld/oneSheeld/src/main/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.jens.automation2/app/build.gradle` & `fdroidserver-2.3a1/tests/source-files/com.jens.automation2/app/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.jens.automation2/build.gradle` & `fdroidserver-2.3a1/tests/source-files/com.jens.automation2/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.kunzisoft.testcase/build.gradle` & `fdroidserver-2.3a1/tests/source-files/com.kunzisoft.testcase/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/build.gradle` & `fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/android/en-US/full_description.txt` & `fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/generic/fastlane/metadata/android/en-US/full_description.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/android/en-US/full_description.txt` & `fdroidserver-2.3a1/tests/source-files/com.nextcloud.client/src/versionDev/fastlane/metadata/android/en-US/full_description.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/android/en-US/full_description.txt` & `fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/generic/fastlane/metadata/android/en-US/full_description.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/android/en-US/full_description.txt` & `fdroidserver-2.3a1/tests/source-files/com.nextcloud.client.dev/src/versionDev/fastlane/metadata/android/en-US/full_description.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.seafile.seadroid2/app/build.gradle` & `fdroidserver-2.3a1/tests/source-files/com.seafile.seadroid2/app/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.ubergeek42.WeechatAndroid/app/build.gradle.kts` & `fdroidserver-2.3a1/tests/source-files/com.ubergeek42.WeechatAndroid/app/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/com.ubergeek42.WeechatAndroid/app/src/main/res/values/strings.xml` & `fdroidserver-2.3a1/tests/source-files/com.ubergeek42.WeechatAndroid/app/src/main/res/values/strings.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/de.varengold.activeTAN/build.gradle` & `fdroidserver-2.3a1/tests/source-files/de.varengold.activeTAN/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/dev.patrickgold.florisboard/app/build.gradle.kts` & `fdroidserver-2.3a1/tests/source-files/dev.patrickgold.florisboard/app/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/eu.siacs.conversations/build.gradle` & `fdroidserver-2.3a1/tests/source-files/eu.siacs.conversations/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/fdroid/fdroidclient/AndroidManifest.xml` & `fdroidserver-2.3a1/tests/source-files/fdroid/fdroidclient/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/fdroid/fdroidclient/build.gradle` & `fdroidserver-2.3a1/tests/source-files/fdroid/fdroidclient/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/open-keychain/open-keychain/OpenKeychain/build.gradle` & `fdroidserver-2.3a1/tests/source-files/open-keychain/open-keychain/OpenKeychain/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/open-keychain/open-keychain/build.gradle` & `fdroidserver-2.3a1/tests/source-files/open-keychain/open-keychain/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/org.mozilla.rocket/app/build.gradle` & `fdroidserver-2.3a1/tests/source-files/org.mozilla.rocket/app/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/org.noise_planet.noisecapture/app/build.gradle` & `fdroidserver-2.3a1/tests/source-files/org.noise_planet.noisecapture/app/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/org.noise_planet.noisecapture/sosfilter/build.gradle` & `fdroidserver-2.3a1/tests/source-files/org.noise_planet.noisecapture/sosfilter/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/org.tasks/app/build.gradle.kts` & `fdroidserver-2.3a1/tests/source-files/org.tasks/app/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/org.tasks/build.gradle.kts` & `fdroidserver-2.3a1/tests/source-files/org.tasks/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/osmandapp/osmand/build.gradle` & `fdroidserver-2.3a1/tests/source-files/osmandapp/osmand/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/realm/react-native/android/build.gradle` & `fdroidserver-2.3a1/tests/source-files/realm/react-native/android/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/se.manyver/android/app/build.gradle` & `fdroidserver-2.3a1/tests/source-files/se.manyver/android/app/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/se.manyver/android/build.gradle` & `fdroidserver-2.3a1/tests/source-files/se.manyver/android/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/se.manyver/android/gradle.properties` & `fdroidserver-2.3a1/tests/source-files/se.manyver/android/gradle.properties`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/se.manyver/android/settings.gradle` & `fdroidserver-2.3a1/tests/source-files/se.manyver/android/settings.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/se.manyver/index.android.js` & `fdroidserver-2.3a1/tests/source-files/se.manyver/index.android.js`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/se.manyver/package.json` & `fdroidserver-2.3a1/tests/source-files/se.manyver/package.json`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/se.manyver/react-native.config.js` & `fdroidserver-2.3a1/tests/source-files/se.manyver/react-native.config.js`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/ut.ewh.audiometrytest/app/build.gradle` & `fdroidserver-2.3a1/tests/source-files/ut.ewh.audiometrytest/app/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/ut.ewh.audiometrytest/app/src/main/AndroidManifest.xml` & `fdroidserver-2.3a1/tests/source-files/ut.ewh.audiometrytest/app/src/main/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/source-files/ut.ewh.audiometrytest/build.gradle` & `fdroidserver-2.3a1/tests/source-files/ut.ewh.audiometrytest/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/stats/known_apks.txt` & `fdroidserver-2.3a1/tests/stats/known_apks.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/test-gradlew-fdroid` & `fdroidserver-2.3a1/tests/test-gradlew-fdroid`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/testcommon.py` & `fdroidserver-2.3a1/tests/testcommon.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
 import sys
 import tempfile
+import unittest
+
+from pathlib import Path
+from unittest import mock
 
 
 class TmpCwd:
     """Context-manager for temporarily changing the current working directory."""
 
     def __init__(self, new_cwd):
         self.new_cwd = new_cwd
@@ -56,7 +60,29 @@
 
 
 def mkdtemp():
     if sys.version_info < (3, 10):  # ignore_cleanup_errors was added in 3.10
         return tempfile.TemporaryDirectory()
     else:
         return tempfile.TemporaryDirectory(ignore_cleanup_errors=True)
+
+
+def mkdir_testfiles(localmodule, test):
+    """Keep the test files in a labeled test dir for easy reference"""
+    testroot = Path(localmodule) / '.testfiles'
+    testroot.mkdir(exist_ok=True)
+    testdir = testroot / unittest.TestCase.id(test)
+    testdir.mkdir(exist_ok=True)
+    return tempfile.mkdtemp(dir=testdir)
+
+
+def parse_args_for_test(parser, args):
+    """Only send --flags to the ArgumentParser, not test classes, etc."""
+
+    from fdroidserver.common import parse_args
+
+    flags = []
+    for arg in args:
+        if arg[0] == '-':
+            flags.append(flags)
+    with mock.patch('sys.argv', flags):
+        parse_args(parser)
```

### Comparing `fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/build.gradle` & `fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/build.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/java/org/piwigo/PiwigoApplication.java` & `fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/java/org/piwigo/PiwigoApplication.java`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/de-DE/full-description.txt` & `fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/de-DE/full-description.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/feature-graphic/piwigo-full.png` & `fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/feature-graphic/piwigo-full.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/icon/piwigo-icon.png` & `fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/icon/piwigo-icon.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/01_Login.jpg` & `fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/01_Login.jpg`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/02_Albums.jpg` & `fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/02_Albums.jpg`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/03_Photos.jpg` & `fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/03_Photos.jpg`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/04_Albums_horizontal.jpg` & `fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/04_Albums_horizontal.jpg`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/05_Menu.jpg` & `fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/phone-screenshots/05_Menu.jpg`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/tablet-screenshots/01_Login.png` & `fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/en-US/graphics/tablet-screenshots/01_Login.png`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/fr-FR/full-description.txt` & `fdroidserver-2.3a1/tests/triple-t-2/build/org.piwigo.android/app/src/main/play/listings/fr-FR/full-description.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-2/metadata/org.piwigo.android.yml` & `fdroidserver-2.3a1/tests/triple-t-2/metadata/org.piwigo.android.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/settings.gradle` & `fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.anysoftkeyboard.languagepack.dutch/settings.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/settings.gradle` & `fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/build/com.menny.android.anysoftkeyboard/settings.gradle`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/metadata/com.anysoftkeyboard.languagepack.dutch.yml` & `fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/metadata/com.anysoftkeyboard.languagepack.dutch.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-anysoftkeyboard/metadata/com.menny.android.anysoftkeyboard.yml` & `fdroidserver-2.3a1/tests/triple-t-anysoftkeyboard/metadata/com.menny.android.anysoftkeyboard.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/listings/en-US/full-description.txt` & `fdroidserver-2.3a1/tests/triple-t-flutter/build/fr.emersion.goguma/android/app/src/main/play/listings/en-US/full-description.txt`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-flutter/metadata/fr.emersion.goguma.yml` & `fdroidserver-2.3a1/tests/triple-t-flutter/metadata/fr.emersion.goguma.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-multiple/metadata/ch.admin.bag.covidcertificate.verifier.yml` & `fdroidserver-2.3a1/tests/triple-t-multiple/metadata/ch.admin.bag.covidcertificate.verifier.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/triple-t-multiple/metadata/ch.admin.bag.covidcertificate.wallet.yml` & `fdroidserver-2.3a1/tests/triple-t-multiple/metadata/ch.admin.bag.covidcertificate.wallet.yml`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/update.TestCase` & `fdroidserver-2.3a1/tests/update.TestCase`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 #!/usr/bin/env python3
 
 # http://www.drdobbs.com/testing/unit-testing-with-python/240165163
 
 import copy
 import git
 import glob
+import hashlib
 import inspect
 import json
 import logging
-import optparse
 import os
 import random
 import shutil
 import string
 import subprocess
 import sys
 import tempfile
 import unittest
 import yaml
 import zipfile
 import textwrap
+from binascii import hexlify
 from datetime import datetime
 from pathlib import Path
-from testcommon import TmpCwd, mkdtemp
 from unittest import mock
 
 try:
+    # these were moved in androguard 4.0
+    from androguard.core.apk import APK
+except ImportError:
+    from androguard.core.bytecodes.apk import APK
+
+try:
     from yaml import CSafeLoader as SafeLoader
 except ImportError:
     from yaml import SafeLoader
 
 try:
     from yaml import CFullLoader as FullLoader
 except ImportError:
@@ -50,14 +56,15 @@
 
 import fdroidserver.common
 import fdroidserver.exception
 import fdroidserver.metadata
 import fdroidserver.update
 from fdroidserver.common import CATEGORIES_CONFIG_NAME
 from fdroidserver.looseversion import LooseVersion
+from testcommon import TmpCwd, mkdtemp, parse_args_for_test
 
 
 DONATION_FIELDS = ('Donate', 'Liberapay', 'OpenCollective')
 
 
 class Options:
     allow_disabled_algorithms = False
@@ -70,17 +77,14 @@
 
 
 class UpdateTest(unittest.TestCase):
     '''fdroid update'''
 
     def setUp(self):
         logging.basicConfig(level=logging.INFO)
-        logging.getLogger('androguard.apk').setLevel(logging.WARNING)
-        logging.getLogger('androguard.axml').setLevel(logging.INFO)
-        logging.getLogger('androguard.core.api_specific_resources').setLevel(logging.INFO)
         from PIL import PngImagePlugin
 
         logging.getLogger(PngImagePlugin.__name__).setLevel(logging.INFO)
         self.basedir = os.path.join(localmodule, 'tests')
         os.chdir(self.basedir)
         self._td = mkdtemp()
         self.testdir = self._td.name
@@ -577,21 +581,14 @@
                          'python sig was: ' + str(sig))
 
         apkpath = 'repo/v1.v2.sig_1020.apk'
         sig = fdroidserver.update.getsig(apkpath)
         self.assertEqual(good_fingerprint, sig,
                          'python sig was: ' + str(sig))
         # check that v1 and v2 have the same certificate
-        try:
-            import hashlib
-            from binascii import hexlify
-            from androguard.core.bytecodes.apk import APK
-        except ImportError:
-            print('WARNING: skipping rest of test since androguard is missing!')
-            return
         apkobject = APK(apkpath)
         cert_encoded = apkobject.get_certificates_der_v2()[0]
         self.assertEqual(good_fingerprint, sig,
                          hashlib.md5(hexlify(cert_encoded)).hexdigest())  # nosec just used as ID for signing key
 
         filename = 'v2.only.sig_2.apk'
         with zipfile.ZipFile(filename) as z:
@@ -1206,15 +1203,15 @@
         with open(metadatafile, 'a') as fp:
             fp.write(
                 '\n\nAllowedAPKSigningKeys: 32a23624c201b949f085996ba5ed53d40f703aca4989476949cae891022e0ed6\n'
             )
 
         # Set up options
         fdroidserver.common.options = Options
-        config = fdroidserver.common.read_config(fdroidserver.common.options)
+        config = fdroidserver.common.read_config()
         if 'apksigner' not in config:  # TODO remove me for buildserver-bullseye
             self.skipTest('SKIPPING test_update_with_AllowedAPKSigningKeys, apksigner not installed!')
         config['repo_keyalias'] = 'sova'
         config['keystorepass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keypass'] = 'r9aquRHYoI8+dYz6jKrLntQ5/NJNASFBacJh7Jv2BlI='
         config['keystore'] = os.path.join(self.basedir, 'keystore.jks')
 
@@ -1932,15 +1929,18 @@
         with open('repo/index-v2.json') as fp:
             index = json.load(fp)
         self.assertEqual(
             {'Time': {'name': {'en-US': 'T'}}},
             index['repo'][CATEGORIES_CONFIG_NAME],
         )
 
+
+class TestParseIpa(unittest.TestCase):
     def test_parse_ipa(self):
+        self.maxDiff = None
         try:
             import biplist  # Fedora does not have a biplist package
 
             biplist  # silence the linters
         except ImportError as e:
             self.skipTest(str(e))
         ipa_path = os.path.join(
@@ -1955,14 +1955,35 @@
                 'apkName': 'com.fake.IpaApp_1000000000001.ipa',
                 'hash': 'fake_sha',
                 'hashType': 'sha256',
                 'packageName': 'org.onionshare.OnionShare',
                 'size': 'fake_size',
                 'versionCode': 1000000000001,
                 'versionName': '1.0.1',
+                'ipa_DTPlatformVersion': '16.4',
+                'ipa_MinimumOSVersion': '15.0',
+                'ipa_entitlements': set(),
+                'ipa_permissions': {
+                    'NSCameraUsageDescription':
+                        'Please allow access to your '
+                        'camera, if you want to '
+                        'create photos or videos for '
+                        'direct sharing.',
+                    'NSMicrophoneUsageDescription':
+                        'Please allow access to '
+                        'your microphone, if you '
+                        'want to create videos '
+                        'for direct sharing.',
+                    'NSPhotoLibraryUsageDescription':
+                        'Please allow access to '
+                        'your photo library, if '
+                        'you want to share '
+                        'photos.',
+                },
+                'name': 'OnionShare',
             },
         )
 
 
 class TestUpdateVersionStringToInt(unittest.TestCase):
     def test_version_string_to_int(self):
         self.assertEqual(
@@ -2197,28 +2218,76 @@
                     'build/org.fake/fastlane/screenshots/de-DE/1_ipadPro129_1.1.png',
                     'repo/org.fake/de-DE/tenInchScreenshots/1_ipadPro129_1.1.png',
                 ),
             ],
         )
 
 
+class TestGetIpaIcon(unittest.TestCase):
+    def test_get_ipa_icon(self):
+        self.maxDiff = None
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            tmpdir = Path(tmpdir)
+            (tmpdir / 'OnionBrowser.xcodeproj').mkdir()
+            with open(tmpdir / 'OnionBrowser.xcodeproj/project.pbxproj', "w") as f:
+                f.write("")
+            icondir = tmpdir / "fake_icon.appiconset"
+            icondir.mkdir()
+            with open(icondir / "Contents.json", "w", encoding="utf-8") as f:
+                f.write("""
+                    {"images": [
+                        {"scale": "2x", "size": "128x128", "filename": "nope"},
+                        {"scale": "1x", "size": "512x512", "filename": "nope"},
+                        {"scale": "1x", "size": "16x16", "filename": "nope"},
+                        {"scale": "1x", "size": "32x32", "filename": "yep"}
+                    ]}
+                """)
+
+            pfp = mock.Mock(return_value="fake_icon")
+            with mock.patch("fdroidserver.update._parse_from_pbxproj", pfp):
+                p = fdroidserver.update._get_ipa_icon(tmpdir)
+                self.assertEqual(str(icondir / "yep"), p)
+
+
+class TestParseFromPbxproj(unittest.TestCase):
+    def test_parse_from_pbxproj(self):
+        self.maxDiff = None
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            with open(Path(tmpdir) / "asdf.pbxproj", 'w', encoding="utf-8") as f:
+                f.write("""
+                    230jfaod=flc'
+                    ASSETCATALOG_COMPILER_APPICON_NAME = MyIcon;
+                    cm opa1c p[m
+                """)
+            v = fdroidserver.update._parse_from_pbxproj(
+                Path(tmpdir) / "asdf.pbxproj",
+                "ASSETCATALOG_COMPILER_APPICON_NAME"
+            )
+            self.assertEqual(v, "MyIcon")
+
+
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (fdroidserver.common.options, args) = parser.parse_args(['--verbose'])
+    parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(UpdateTest))
     newSuite.addTest(unittest.makeSuite(TestUpdateVersionStringToInt))
     newSuite.addTest(unittest.makeSuite(TestScanRepoForIpas))
     newSuite.addTest(unittest.makeSuite(TestParseIosScreenShotName))
     newSuite.addTest(unittest.makeSuite(TestInsertLocalizedIosAppMetadata))
     newSuite.addTest(unittest.makeSuite(TestDiscoverIosScreenshots))
+    newSuite.addTest(unittest.makeSuite(TestGetIpaIcon))
     unittest.main(failfast=False)
```

### Comparing `fdroidserver-2.3a0/tests/urzip-badcert.apk` & `fdroidserver-2.3a1/tests/urzip-badcert.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/urzip-badsig.apk` & `fdroidserver-2.3a1/tests/urzip-badsig.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/urzip-release-unsigned.apk` & `fdroidserver-2.3a1/tests/urzip-release-unsigned.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/urzip-release.apk` & `fdroidserver-2.3a1/tests/urzip-release.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/urzip.apk` & `fdroidserver-2.3a1/tests/urzip.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/v2.only.sig_2.apk` & `fdroidserver-2.3a1/tests/v2.only.sig_2.apk`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/valid-package-names/RandomPackageNames.java` & `fdroidserver-2.3a1/tests/valid-package-names/RandomPackageNames.java`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/valid-package-names/test.py` & `fdroidserver-2.3a1/tests/valid-package-names/test.py`

 * *Files identical despite different names*

### Comparing `fdroidserver-2.3a0/tests/vcs.TestCase` & `fdroidserver-2.3a1/tests/vcs.TestCase`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 
 # http://www.drdobbs.com/testing/unit-testing-with-python/240165163
 
 import inspect
 import logging
-import optparse
 import os
 import sys
 import unittest
 
 from git import Repo
 
 localmodule = os.path.realpath(
@@ -18,15 +17,15 @@
 if localmodule not in sys.path:
     sys.path.insert(0, localmodule)
 
 import fdroidserver.build
 import fdroidserver.common
 import fdroidserver.metadata
 import fdroidserver.scanner
-from testcommon import mkdtemp
+from testcommon import mkdtemp, parse_args_for_test
 
 
 class VCSTest(unittest.TestCase):
     """For some reason the VCS classes are in fdroidserver/common.py"""
 
     def setUp(self):
         logging.basicConfig(level=logging.DEBUG)
@@ -84,20 +83,22 @@
         )
         self.assertTrue(os.path.isfile("build/com.gpl.rpg.AndorsTrail/file"))
 
 
 if __name__ == "__main__":
     os.chdir(os.path.dirname(__file__))
 
-    parser = optparse.OptionParser()
-    parser.add_option(
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Spew out even more information than normal",
     )
-    (fdroidserver.common.options, args) = parser.parse_args(['--verbose'])
+    parse_args_for_test(parser, sys.argv)
 
     newSuite = unittest.TestSuite()
     newSuite.addTest(unittest.makeSuite(VCSTest))
     unittest.main(failfast=False)
```

