# Comparing `tmp/perun.proxygui-5.2.1.tar.gz` & `tmp/perun.proxygui-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun.proxygui-5.2.1.tar", last modified: Fri May 10 21:40:04 2024, max compression
+gzip compressed data, was "perun.proxygui-6.0.0.tar", last modified: Mon May 13 06:58:24 2024, max compression
```

## Comparing `perun.proxygui-5.2.1.tar` & `perun.proxygui-6.0.0.tar`

### file list

```diff
@@ -1,292 +1,292 @@
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.558942 perun.proxygui-5.2.1/
--rw-rw-rw-   0     1001 root         (0)     1560 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/LICENSE
--rw-rw-rw-   0     1001 root         (0)       46 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/MANIFEST.in
--rw-r--r--   0     1001 root         (0)     9351 2024-05-10 21:40:04.558942 perun.proxygui-5.2.1/PKG-INFO
--rw-rw-rw-   0     1001 root         (0)     8072 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/README.md
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.502942 perun.proxygui-5.2.1/perun/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.502942 perun.proxygui-5.2.1/perun/proxygui/
--rw-rw-rw-   0     1001 root         (0)        0 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/__init__.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.506942 perun.proxygui-5.2.1/perun/proxygui/api/
--rw-rw-rw-   0     1001 root         (0)        0 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/api/__init__.py
--rw-rw-rw-   0     1001 root         (0)     2478 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/api/backchannel_logout_api.py
--rw-rw-rw-   0     1001 root         (0)     6368 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/api/ban_api.py
--rw-rw-rw-   0     1001 root         (0)     4900 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/api/consent_api.py
--rw-rw-rw-   0     1001 root         (0)    10747 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/api/heuristic_api.py
--rw-rw-rw-   0     1001 root         (0)     3089 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/api/kerberos_auth_api.py
--rw-rw-rw-   0     1001 root         (0)     6919 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/app.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.506942 perun.proxygui-5.2.1/perun/proxygui/gui/
--rw-rw-rw-   0     1001 root         (0)        0 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/__init__.py
--rw-rw-rw-   0     1001 root         (0)    21954 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/gui.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.506942 perun.proxygui-5.2.1/perun/proxygui/gui/static/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.498942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.498942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.506942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.506942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/
--rw-rw-rw-   0     1001 root         (0)   141520 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map
--rw-rw-rw-   0     1001 root         (0)       99 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_atoms.scss
--rw-rw-rw-   0     1001 root         (0)      612 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss
--rw-rw-rw-   0     1001 root         (0)       67 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_organisms.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.506942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/
--rw-rw-rw-   0     1001 root         (0)      688 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss
--rw-rw-rw-   0     1001 root         (0)       19 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_calendar.scss
--rw-rw-rw-   0     1001 root         (0)      949 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss
--rw-rw-rw-   0     1001 root         (0)     1663 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.506942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/
--rw-rw-rw-   0     1001 root         (0)      477 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/_icons.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.498942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.506942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/
--rw-rw-rw-   0     1001 root         (0)      631 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss
--rw-rw-rw-   0     1001 root         (0)     1451 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss
--rw-rw-rw-   0     1001 root         (0)     3089 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss
--rw-rw-rw-   0     1001 root         (0)     1617 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss
--rw-rw-rw-   0     1001 root         (0)     1776 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss
--rw-rw-rw-   0     1001 root         (0)      437 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_food-menu.scss
--rw-rw-rw-   0     1001 root         (0)      387 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_images.scss
--rw-rw-rw-   0     1001 root         (0)     2945 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss
--rw-rw-rw-   0     1001 root         (0)     2624 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss
--rw-rw-rw-   0     1001 root         (0)      713 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss
--rw-rw-rw-   0     1001 root         (0)     1899 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.506942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/
--rw-rw-rw-   0     1001 root         (0)      815 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss
--rw-rw-rw-   0     1001 root         (0)      571 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.514942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/
--rw-rw-rw-   0     1001 root         (0)      421 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_mega.scss
--rw-rw-rw-   0     1001 root         (0)      403 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_primary.scss
--rw-rw-rw-   0     1001 root         (0)     2758 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.514942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/
--rw-rw-rw-   0     1001 root         (0)      198 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_footer.scss
--rw-rw-rw-   0     1001 root         (0)      684 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss
--rw-rw-rw-   0     1001 root         (0)    29997 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css
--rw-rw-rw-   0     1001 root         (0)      244 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/style.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.498942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.518942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/
--rw-rw-rw-   0     1001 root         (0)    22637 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg
--rw-rw-rw-   0     1001 root         (0)    21057 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg
--rw-rw-rw-   0     1001 root         (0)    22481 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg
--rw-rw-rw-   0     1001 root         (0)    35533 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg
--rw-rw-rw-   0     1001 root         (0)    34805 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg
--rw-rw-rw-   0     1001 root         (0)    28733 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg
--rw-rw-rw-   0     1001 root         (0)    20267 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg
--rw-rw-rw-   0     1001 root         (0)    28025 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg
--rw-rw-rw-   0     1001 root         (0)    25884 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg
--rw-rw-rw-   0     1001 root         (0)   363233 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg
--rw-rw-rw-   0     1001 root         (0)    27013 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg
--rw-rw-rw-   0     1001 root         (0)    33321 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg
--rw-rw-rw-   0     1001 root         (0)    31511 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg
--rw-rw-rw-   0     1001 root         (0)    34010 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg
--rw-rw-rw-   0     1001 root         (0)    28152 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg
--rw-rw-rw-   0     1001 root         (0)    36726 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg
--rw-rw-rw-   0     1001 root         (0)    28663 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg
--rw-rw-rw-   0     1001 root         (0)    22030 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.522942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.534942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/
--rw-rw-rw-   0     1001 root         (0)   125046 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map
--rw-rw-rw-   0     1001 root         (0)   252563 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map
--rw-rw-rw-   0     1001 root         (0)  1052500 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map
--rw-rw-rw-   0     1001 root         (0)  1125125 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map
--rw-rw-rw-   0     1001 root         (0)  1125144 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map
--rw-rw-rw-   0     1001 root         (0)  1125123 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map
--rw-rw-rw-   0     1001 root         (0)  1125121 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map
--rw-rw-rw-   0     1001 root         (0)  1125119 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map
--rw-rw-rw-   0     1001 root         (0)  1125120 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map
--rw-rw-rw-   0     1001 root         (0)  1125147 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map
--rw-rw-rw-   0     1001 root         (0)  1125545 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map
--rw-rw-rw-   0     1001 root         (0)  1125121 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map
--rw-rw-rw-   0     1001 root         (0)  1126098 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map
--rw-rw-rw-   0     1001 root         (0)   139176 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map
--rw-rw-rw-   0     1001 root         (0)     2596 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/documentation.css
--rw-rw-rw-   0     1001 root         (0)    48080 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/print.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.538942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/
--rw-rw-rw-   0     1001 root         (0)     2596 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css
--rw-rw-rw-   0     1001 root         (0)    46987 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css
--rw-rw-rw-   0     1001 root         (0)   303728 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css
--rw-rw-rw-   0     1001 root         (0)   332353 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css
--rw-rw-rw-   0     1001 root         (0)   332557 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css
--rw-rw-rw-   0     1001 root         (0)     5778 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css
--rw-rw-rw-   0     1001 root         (0)   312236 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-custom.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-econ.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-fi.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-fss.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-law.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-med.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-ped.css
--rw-rw-rw-   0     1001 root         (0)   341456 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-phil.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-sci.css
--rw-rw-rw-   0     1001 root         (0)   341664 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style.css
--rw-rw-rw-   0     1001 root         (0)     5772 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.542942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/
--rw-rw-rw-   0     1001 root         (0)    87048 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff
--rw-rw-rw-   0     1001 root         (0)    74284 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2
--rw-rw-rw-   0     1001 root         (0)   208892 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff
--rw-rw-rw-   0     1001 root         (0)   159376 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2
--rw-rw-rw-   0     1001 root         (0)     1632 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot
--rw-rw-rw-   0     1001 root         (0)     1837 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg
--rw-rw-rw-   0     1001 root         (0)     1484 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf
--rw-rw-rw-   0     1001 root         (0)      988 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff
--rw-rw-rw-   0     1001 root         (0)    12252 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff
--rw-rw-rw-   0     1001 root         (0)     9596 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.542942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.542942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/
--rw-rw-rw-   0     1001 root         (0)    70841 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg
--rw-rw-rw-   0     1001 root         (0)     4348 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif
--rw-rw-rw-   0     1001 root         (0)      151 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/ico-external.png
--rw-rw-rw-   0     1001 root         (0)      279 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-ciisb.png
--rw-rw-rw-   0     1001 root         (0)      279 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-crc.png
--rw-rw-rw-   0     1001 root         (0)      280 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-econ.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-fi.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-fsps.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-fss.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-law.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-med.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-ped.png
--rw-rw-rw-   0     1001 root         (0)      281 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-phil.png
--rw-rw-rw-   0     1001 root         (0)      280 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-sci.png
--rw-rw-rw-   0     1001 root         (0)      149 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-small.png
--rw-rw-rw-   0     1001 root         (0)      304 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/select.png
--rw-rw-rw-   0     1001 root         (0)     7406 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/favicon.ico
--rw-rw-rw-   0     1001 root         (0)     4426 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png
--rw-rw-rw-   0     1001 root         (0)      443 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/logo.svg
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.546942 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/
--rw-rw-rw-   0     1001 root         (0)   218591 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/app.js
--rw-rw-rw-   0     1001 root         (0)   659454 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/app.js.map
--rw-rw-rw-   0     1001 root         (0)   337945 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/d3.js
--rw-rw-rw-   0     1001 root         (0)     2707 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/documentation.js
--rw-rw-rw-   0     1001 root         (0)     8806 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/graphs.js
--rw-rw-rw-   0     1001 root         (0)    26171 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js
--rw-rw-rw-   0     1001 root         (0)     4075 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js
--rw-rw-rw-   0     1001 root         (0)   284394 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/jquery.js
--rw-rw-rw-   0     1001 root         (0)   610160 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.498942 perun.proxygui-5.2.1/perun/proxygui/gui/static/bootstrap/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.546942 perun.proxygui-5.2.1/perun/proxygui/gui/static/bootstrap/css/
--rw-rw-rw-   0     1001 root         (0)   155845 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css
--rw-rw-rw-   0     1001 root         (0)   431289 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.546942 perun.proxygui-5.2.1/perun/proxygui/gui/static/bootstrap/js/
--rw-rw-rw-   0     1001 root         (0)    78743 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0     1001 root         (0)   325834 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0     1001 root         (0)       78 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/campus-idp-muni.js
--rw-rw-rw-   0     1001 root         (0)     7365 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/campus-idp.css
--rw-rw-rw-   0     1001 root         (0)     4859 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/campus-idp.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.498942 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.546942 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/css/
--rw-rw-rw-   0     1001 root         (0)    73577 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/css/all.css
--rw-rw-rw-   0     1001 root         (0)    59305 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/css/all.min.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.550942 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/
--rw-rw-rw-   0     1001 root         (0)   134294 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot
--rw-rw-rw-   0     1001 root         (0)   747927 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg
--rw-rw-rw-   0     1001 root         (0)   133988 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0     1001 root         (0)    89988 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff
--rw-rw-rw-   0     1001 root         (0)    76736 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0     1001 root         (0)    34034 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot
--rw-rw-rw-   0     1001 root         (0)   144714 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg
--rw-rw-rw-   0     1001 root         (0)    33736 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0     1001 root         (0)    16276 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff
--rw-rw-rw-   0     1001 root         (0)    13224 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0     1001 root         (0)   203030 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot
--rw-rw-rw-   0     1001 root         (0)   918991 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg
--rw-rw-rw-   0     1001 root         (0)   202744 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0     1001 root         (0)   101648 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff
--rw-rw-rw-   0     1001 root         (0)    78268 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.550942 perun.proxygui-5.2.1/perun/proxygui/gui/static/images/
--rw-rw-rw-   0     1001 root         (0)      490 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/images/check.svg
--rw-rw-rw-   0     1001 root         (0)      536 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/images/circle-check-regular.svg
--rw-rw-rw-   0     1001 root         (0)      483 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/images/circle-exclamation-solid.svg
--rw-rw-rw-   0     1001 root         (0)      730 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/images/questionmark.svg
--rw-rw-rw-   0     1001 root         (0)      625 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/images/spinner.svg
--rw-rw-rw-   0     1001 root         (0)    89501 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/jquery-3.6.0.min.js
--rw-rw-rw-   0     1001 root         (0)      627 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/proxygui.css
--rw-rw-rw-   0     1001 root         (0)     1427 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/proxygui.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.498942 perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.550942 perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/
--rw-rw-rw-   0     1001 root         (0)    15836 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css
--rw-rw-rw-   0     1001 root         (0)     8266 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css
--rw-rw-rw-   0     1001 root         (0)     8862 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css
--rw-rw-rw-   0     1001 root         (0)     8873 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css
--rw-rw-rw-   0     1001 root         (0)     7692 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.css
--rw-rw-rw-   0     1001 root         (0)     8344 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.default.css
--rw-rw-rw-   0     1001 root         (0)    11438 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.legacy.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.498942 perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/js/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.550942 perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/js/standalone/
--rw-rw-rw-   0     1001 root         (0)    64906 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.554942 perun.proxygui-5.2.1/perun/proxygui/gui/templates/
--rw-rw-rw-   0     1001 root         (0)    15205 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/ConsentRegistration.html
--rw-rw-rw-   0     1001 root         (0)     9192 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/HeuristicData.html
--rw-rw-rw-   0     1001 root         (0)      747 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/IsTestingSP.html
--rw-rw-rw-   0     1001 root         (0)     3101 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/Logout.html
--rw-rw-rw-   0     1001 root         (0)     1131 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/MfaResetEmailSent.html
--rw-rw-rw-   0     1001 root         (0)     1942 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/MfaResetInitiated.html
--rw-rw-rw-   0     1001 root         (0)     1133 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html
--rw-rw-rw-   0     1001 root         (0)     1021 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/MfaResult.html
--rw-rw-rw-   0     1001 root         (0)      795 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/MissingAuth.html
--rw-rw-rw-   0     1001 root         (0)     1019 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/OidcError.html
--rw-rw-rw-   0     1001 root         (0)     1223 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/Post-logout.html
--rw-rw-rw-   0     1001 root         (0)      907 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/SPAuthorization.html
--rw-rw-rw-   0     1001 root         (0)     2490 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/_footer.html
--rw-rw-rw-   0     1001 root         (0)     8119 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/_header.html
--rw-rw-rw-   0     1001 root         (0)     1175 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/authorization.html
--rw-rw-rw-   0     1001 root         (0)     3477 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/base.html
--rw-rw-rw-   0     1001 root         (0)      734 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/logout-canceled.html
--rw-rw-rw-   0     1001 root         (0)      561 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/logout-iframe.html
--rw-rw-rw-   0     1001 root         (0)     3769 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/templates/logout-state.html
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.498942 perun.proxygui-5.2.1/perun/proxygui/gui/translations/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.498942 perun.proxygui-5.2.1/perun/proxygui/gui/translations/cs/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.554942 perun.proxygui-5.2.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/
--rw-rw-rw-   0     1001 root         (0)     2973 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo
--rw-rw-rw-   0     1001 root         (0)     8108 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po
--rw-rw-rw-   0     1001 root         (0)     5807 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/jwt.py
--rw-rw-rw-   0     1001 root         (0)    20231 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/logout_manager.py
--rw-rw-rw-   0     1001 root         (0)     2480 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/oauth.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.554942 perun.proxygui-5.2.1/perun/proxygui/openapi/
--rw-rw-rw-   0     1001 root         (0)     6107 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/openapi/openapi.py
--rw-rw-rw-   0     1001 root         (0)    12933 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/openapi/openapi_data.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.554942 perun.proxygui-5.2.1/perun/proxygui/openapi/schemas/
--rw-rw-rw-   0     1001 root         (0)      997 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/openapi/schemas/arguments_schemas.py
--rw-rw-rw-   0     1001 root         (0)     1446 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/openapi/schemas/response_schemas.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.554942 perun.proxygui-5.2.1/perun/proxygui/tests/
--rw-rw-rw-   0     1001 root         (0)        0 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/tests/__init__.py
--rw-rw-rw-   0     1001 root         (0)     1816 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/tests/shared_test_data.py
--rw-rw-rw-   0     1001 root         (0)     9237 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/tests/test_ban_api.py
--rw-rw-rw-   0     1001 root         (0)     6635 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/tests/test_consent_api.py
--rw-rw-rw-   0     1001 root         (0)     4713 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/tests/test_consent_db.py
--rw-rw-rw-   0     1001 root         (0)     2160 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/tests/test_consent_request_db.py
--rw-rw-rw-   0     1001 root         (0)     6850 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/tests/test_gui.py
--rw-rw-rw-   0     1001 root         (0)     1111 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/tests/test_kerberos_auth_api.py
--rw-rw-rw-   0     1001 root         (0)    23012 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/proxygui/user_manager.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.558942 perun.proxygui-5.2.1/perun/utils/
--rw-rw-rw-   0     1001 root         (0)     2496 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/ConfigStore.py
--rw-rw-rw-   0     1001 root         (0)       43 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/CustomExceptions.py
--rw-rw-rw-   0     1001 root         (0)     2555 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/CustomRPHandler.py
--rw-rw-rw-   0     1001 root         (0)     1545 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/DatabaseService.py
--rw-rw-rw-   0     1001 root         (0)     4414 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/EmailService.py
--rw-rw-rw-   0     1001 root         (0)       96 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/Notification.py
--rw-rw-rw-   0     1001 root         (0)      816 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/Utils.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.558942 perun.proxygui-5.2.1/perun/utils/auth_event_loggig/
--rw-rw-rw-   0     1001 root         (0)     2100 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/auth_event_loggig/AuthEventLoggingDbModels.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.558942 perun.proxygui-5.2.1/perun/utils/consent_framework/
--rw-rw-rw-   0     1001 root         (0)     1241 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/consent_framework/consent.py
--rw-rw-rw-   0     1001 root         (0)     2226 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/consent_framework/consent_db.py
--rw-rw-rw-   0     1001 root         (0)     2274 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/consent_framework/consent_manager.py
--rw-rw-rw-   0     1001 root         (0)      730 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/consent_framework/consent_request.py
--rw-rw-rw-   0     1001 root         (0)     1371 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/consent_framework/consent_request_db.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.558942 perun.proxygui-5.2.1/perun/utils/logout_requests/
--rw-rw-rw-   0     1001 root         (0)     2001 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/logout_requests/BackchannelLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)      832 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/logout_requests/FrontchannelLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     3841 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/logout_requests/GraphLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     1361 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/logout_requests/LogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     2204 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/perun/utils/logout_requests/SamlLogoutRequest.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-10 21:40:04.502942 perun.proxygui-5.2.1/perun.proxygui.egg-info/
--rw-r--r--   0     1001 root         (0)     9351 2024-05-10 21:40:04.000000 perun.proxygui-5.2.1/perun.proxygui.egg-info/PKG-INFO
--rw-r--r--   0     1001 root         (0)    12892 2024-05-10 21:40:04.000000 perun.proxygui-5.2.1/perun.proxygui.egg-info/SOURCES.txt
--rw-r--r--   0     1001 root         (0)        1 2024-05-10 21:40:04.000000 perun.proxygui-5.2.1/perun.proxygui.egg-info/dependency_links.txt
--rw-r--r--   0     1001 root         (0)      557 2024-05-10 21:40:04.000000 perun.proxygui-5.2.1/perun.proxygui.egg-info/requires.txt
--rw-r--r--   0     1001 root         (0)        6 2024-05-10 21:40:04.000000 perun.proxygui-5.2.1/perun.proxygui.egg-info/top_level.txt
--rw-rw-rw-   0     1001 root         (0)       90 2024-05-10 21:40:04.558942 perun.proxygui-5.2.1/setup.cfg
--rw-rw-rw-   0     1001 root         (0)     1485 2024-05-10 21:39:22.000000 perun.proxygui-5.2.1/setup.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.281787 perun.proxygui-6.0.0/
+-rw-rw-rw-   0     1001 root         (0)     1560 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/LICENSE
+-rw-rw-rw-   0     1001 root         (0)       46 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/MANIFEST.in
+-rw-r--r--   0     1001 root         (0)     9346 2024-05-13 06:58:24.281787 perun.proxygui-6.0.0/PKG-INFO
+-rw-rw-rw-   0     1001 root         (0)     8067 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/README.md
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.217787 perun.proxygui-6.0.0/perun/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.221787 perun.proxygui-6.0.0/perun/proxygui/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/__init__.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.221787 perun.proxygui-6.0.0/perun/proxygui/api/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/api/__init__.py
+-rw-rw-rw-   0     1001 root         (0)     2478 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/api/backchannel_logout_api.py
+-rw-rw-rw-   0     1001 root         (0)     6353 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/api/ban_api.py
+-rw-rw-rw-   0     1001 root         (0)     4900 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/api/consent_api.py
+-rw-rw-rw-   0     1001 root         (0)    10747 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/api/heuristic_api.py
+-rw-rw-rw-   0     1001 root         (0)     3084 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/api/kerberos_auth_api.py
+-rw-rw-rw-   0     1001 root         (0)     6919 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/app.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.221787 perun.proxygui-6.0.0/perun/proxygui/gui/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/__init__.py
+-rw-rw-rw-   0     1001 root         (0)    21745 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/gui.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.221787 perun.proxygui-6.0.0/perun/proxygui/gui/static/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.217787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.217787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.225787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.225787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/
+-rw-rw-rw-   0     1001 root         (0)   141520 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map
+-rw-rw-rw-   0     1001 root         (0)       99 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_atoms.scss
+-rw-rw-rw-   0     1001 root         (0)      612 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss
+-rw-rw-rw-   0     1001 root         (0)       67 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_organisms.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.225787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/
+-rw-rw-rw-   0     1001 root         (0)      688 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss
+-rw-rw-rw-   0     1001 root         (0)       19 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_calendar.scss
+-rw-rw-rw-   0     1001 root         (0)      949 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss
+-rw-rw-rw-   0     1001 root         (0)     1663 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.225787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/
+-rw-rw-rw-   0     1001 root         (0)      477 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/_icons.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.217787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.225787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/
+-rw-rw-rw-   0     1001 root         (0)      631 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss
+-rw-rw-rw-   0     1001 root         (0)     1451 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss
+-rw-rw-rw-   0     1001 root         (0)     3089 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss
+-rw-rw-rw-   0     1001 root         (0)     1617 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss
+-rw-rw-rw-   0     1001 root         (0)     1776 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss
+-rw-rw-rw-   0     1001 root         (0)      437 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_food-menu.scss
+-rw-rw-rw-   0     1001 root         (0)      387 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_images.scss
+-rw-rw-rw-   0     1001 root         (0)     2945 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss
+-rw-rw-rw-   0     1001 root         (0)     2624 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss
+-rw-rw-rw-   0     1001 root         (0)      713 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss
+-rw-rw-rw-   0     1001 root         (0)     1899 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.225787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/
+-rw-rw-rw-   0     1001 root         (0)      815 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss
+-rw-rw-rw-   0     1001 root         (0)      571 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.225787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/
+-rw-rw-rw-   0     1001 root         (0)      421 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_mega.scss
+-rw-rw-rw-   0     1001 root         (0)      403 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_primary.scss
+-rw-rw-rw-   0     1001 root         (0)     2758 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.225787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/
+-rw-rw-rw-   0     1001 root         (0)      198 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_footer.scss
+-rw-rw-rw-   0     1001 root         (0)      684 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss
+-rw-rw-rw-   0     1001 root         (0)    29997 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css
+-rw-rw-rw-   0     1001 root         (0)      244 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.217787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.229787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/
+-rw-rw-rw-   0     1001 root         (0)    22637 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    21057 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    22481 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg
+-rw-rw-rw-   0     1001 root         (0)    35533 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    34805 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    28733 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg
+-rw-rw-rw-   0     1001 root         (0)    20267 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg
+-rw-rw-rw-   0     1001 root         (0)    28025 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg
+-rw-rw-rw-   0     1001 root         (0)    25884 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg
+-rw-rw-rw-   0     1001 root         (0)   363233 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg
+-rw-rw-rw-   0     1001 root         (0)    27013 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    33321 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    31511 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg
+-rw-rw-rw-   0     1001 root         (0)    34010 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg
+-rw-rw-rw-   0     1001 root         (0)    28152 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg
+-rw-rw-rw-   0     1001 root         (0)    36726 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg
+-rw-rw-rw-   0     1001 root         (0)    28663 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg
+-rw-rw-rw-   0     1001 root         (0)    22030 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.241787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.253787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/
+-rw-rw-rw-   0     1001 root         (0)   125046 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map
+-rw-rw-rw-   0     1001 root         (0)   252563 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map
+-rw-rw-rw-   0     1001 root         (0)  1052500 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125125 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125144 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125123 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125121 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125119 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125120 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125147 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125545 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125121 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map
+-rw-rw-rw-   0     1001 root         (0)  1126098 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map
+-rw-rw-rw-   0     1001 root         (0)   139176 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map
+-rw-rw-rw-   0     1001 root         (0)     2596 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/documentation.css
+-rw-rw-rw-   0     1001 root         (0)    48080 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/print.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.257787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/
+-rw-rw-rw-   0     1001 root         (0)     2596 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css
+-rw-rw-rw-   0     1001 root         (0)    46987 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css
+-rw-rw-rw-   0     1001 root         (0)   303728 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css
+-rw-rw-rw-   0     1001 root         (0)   332353 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css
+-rw-rw-rw-   0     1001 root         (0)   332557 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css
+-rw-rw-rw-   0     1001 root         (0)     5778 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css
+-rw-rw-rw-   0     1001 root         (0)   312236 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-custom.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-econ.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fi.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fss.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-law.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-med.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-ped.css
+-rw-rw-rw-   0     1001 root         (0)   341456 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-phil.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-sci.css
+-rw-rw-rw-   0     1001 root         (0)   341664 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style.css
+-rw-rw-rw-   0     1001 root         (0)     5772 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.261787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/
+-rw-rw-rw-   0     1001 root         (0)    87048 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff
+-rw-rw-rw-   0     1001 root         (0)    74284 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2
+-rw-rw-rw-   0     1001 root         (0)   208892 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff
+-rw-rw-rw-   0     1001 root         (0)   159376 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2
+-rw-rw-rw-   0     1001 root         (0)     1632 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot
+-rw-rw-rw-   0     1001 root         (0)     1837 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg
+-rw-rw-rw-   0     1001 root         (0)     1484 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf
+-rw-rw-rw-   0     1001 root         (0)      988 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff
+-rw-rw-rw-   0     1001 root         (0)    12252 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff
+-rw-rw-rw-   0     1001 root         (0)     9596 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.261787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.261787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/
+-rw-rw-rw-   0     1001 root         (0)    70841 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg
+-rw-rw-rw-   0     1001 root         (0)     4348 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif
+-rw-rw-rw-   0     1001 root         (0)      151 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/ico-external.png
+-rw-rw-rw-   0     1001 root         (0)      279 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-ciisb.png
+-rw-rw-rw-   0     1001 root         (0)      279 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-crc.png
+-rw-rw-rw-   0     1001 root         (0)      280 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-econ.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fi.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fsps.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fss.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-law.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-med.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-ped.png
+-rw-rw-rw-   0     1001 root         (0)      281 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-phil.png
+-rw-rw-rw-   0     1001 root         (0)      280 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-sci.png
+-rw-rw-rw-   0     1001 root         (0)      149 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-small.png
+-rw-rw-rw-   0     1001 root         (0)      304 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select.png
+-rw-rw-rw-   0     1001 root         (0)     7406 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/favicon.ico
+-rw-rw-rw-   0     1001 root         (0)     4426 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png
+-rw-rw-rw-   0     1001 root         (0)      443 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/logo.svg
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.265787 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/
+-rw-rw-rw-   0     1001 root         (0)   218591 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js
+-rw-rw-rw-   0     1001 root         (0)   659454 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js.map
+-rw-rw-rw-   0     1001 root         (0)   337945 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/d3.js
+-rw-rw-rw-   0     1001 root         (0)     2707 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/documentation.js
+-rw-rw-rw-   0     1001 root         (0)     8806 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/graphs.js
+-rw-rw-rw-   0     1001 root         (0)    26171 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js
+-rw-rw-rw-   0     1001 root         (0)     4075 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js
+-rw-rw-rw-   0     1001 root         (0)   284394 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.js
+-rw-rw-rw-   0     1001 root         (0)   610160 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.217787 perun.proxygui-6.0.0/perun/proxygui/gui/static/bootstrap/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.265787 perun.proxygui-6.0.0/perun/proxygui/gui/static/bootstrap/css/
+-rw-rw-rw-   0     1001 root         (0)   155845 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css
+-rw-rw-rw-   0     1001 root         (0)   431289 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.269787 perun.proxygui-6.0.0/perun/proxygui/gui/static/bootstrap/js/
+-rw-rw-rw-   0     1001 root         (0)    78743 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0     1001 root         (0)   325834 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0     1001 root         (0)       78 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/campus-idp-muni.js
+-rw-rw-rw-   0     1001 root         (0)     7365 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/campus-idp.css
+-rw-rw-rw-   0     1001 root         (0)     4859 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/campus-idp.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.217787 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.269787 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/css/
+-rw-rw-rw-   0     1001 root         (0)    73577 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/css/all.css
+-rw-rw-rw-   0     1001 root         (0)    59305 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/css/all.min.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.273787 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/
+-rw-rw-rw-   0     1001 root         (0)   134294 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0     1001 root         (0)   747927 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg
+-rw-rw-rw-   0     1001 root         (0)   133988 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0     1001 root         (0)    89988 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0     1001 root         (0)    76736 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0     1001 root         (0)    34034 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0     1001 root         (0)   144714 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg
+-rw-rw-rw-   0     1001 root         (0)    33736 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0     1001 root         (0)    16276 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0     1001 root         (0)    13224 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0     1001 root         (0)   203030 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0     1001 root         (0)   918991 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg
+-rw-rw-rw-   0     1001 root         (0)   202744 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0     1001 root         (0)   101648 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0     1001 root         (0)    78268 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.273787 perun.proxygui-6.0.0/perun/proxygui/gui/static/images/
+-rw-rw-rw-   0     1001 root         (0)      490 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/images/check.svg
+-rw-rw-rw-   0     1001 root         (0)      536 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/images/circle-check-regular.svg
+-rw-rw-rw-   0     1001 root         (0)      483 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/images/circle-exclamation-solid.svg
+-rw-rw-rw-   0     1001 root         (0)      730 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/images/questionmark.svg
+-rw-rw-rw-   0     1001 root         (0)      625 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/images/spinner.svg
+-rw-rw-rw-   0     1001 root         (0)    89501 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/jquery-3.6.0.min.js
+-rw-rw-rw-   0     1001 root         (0)      627 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/proxygui.css
+-rw-rw-rw-   0     1001 root         (0)     1427 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/proxygui.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.217787 perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.273787 perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/
+-rw-rw-rw-   0     1001 root         (0)    15836 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css
+-rw-rw-rw-   0     1001 root         (0)     8266 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css
+-rw-rw-rw-   0     1001 root         (0)     8862 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css
+-rw-rw-rw-   0     1001 root         (0)     8873 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css
+-rw-rw-rw-   0     1001 root         (0)     7692 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.css
+-rw-rw-rw-   0     1001 root         (0)     8344 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.default.css
+-rw-rw-rw-   0     1001 root         (0)    11438 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.legacy.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.217787 perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/js/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.273787 perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/js/standalone/
+-rw-rw-rw-   0     1001 root         (0)    64906 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.277787 perun.proxygui-6.0.0/perun/proxygui/gui/templates/
+-rw-rw-rw-   0     1001 root         (0)    15205 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/ConsentRegistration.html
+-rw-rw-rw-   0     1001 root         (0)     9168 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/HeuristicData.html
+-rw-rw-rw-   0     1001 root         (0)      747 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/IsTestingSP.html
+-rw-rw-rw-   0     1001 root         (0)     3101 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/Logout.html
+-rw-rw-rw-   0     1001 root         (0)     1131 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/MfaResetEmailSent.html
+-rw-rw-rw-   0     1001 root         (0)     1942 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/MfaResetInitiated.html
+-rw-rw-rw-   0     1001 root         (0)     1133 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html
+-rw-rw-rw-   0     1001 root         (0)     1021 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/MfaResult.html
+-rw-rw-rw-   0     1001 root         (0)      795 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/MissingAuth.html
+-rw-rw-rw-   0     1001 root         (0)     1019 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/OidcError.html
+-rw-rw-rw-   0     1001 root         (0)     1223 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/Post-logout.html
+-rw-rw-rw-   0     1001 root         (0)      907 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/SPAuthorization.html
+-rw-rw-rw-   0     1001 root         (0)     2490 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/_footer.html
+-rw-rw-rw-   0     1001 root         (0)     8119 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/_header.html
+-rw-rw-rw-   0     1001 root         (0)     1175 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/authorization.html
+-rw-rw-rw-   0     1001 root         (0)     3477 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/base.html
+-rw-rw-rw-   0     1001 root         (0)      734 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/logout-canceled.html
+-rw-rw-rw-   0     1001 root         (0)      561 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/logout-iframe.html
+-rw-rw-rw-   0     1001 root         (0)     3769 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/templates/logout-state.html
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.217787 perun.proxygui-6.0.0/perun/proxygui/gui/translations/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.217787 perun.proxygui-6.0.0/perun/proxygui/gui/translations/cs/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.277787 perun.proxygui-6.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/
+-rw-rw-rw-   0     1001 root         (0)     2973 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo
+-rw-rw-rw-   0     1001 root         (0)     8108 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po
+-rw-rw-rw-   0     1001 root         (0)     5807 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/jwt.py
+-rw-rw-rw-   0     1001 root         (0)    20231 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/logout_manager.py
+-rw-rw-rw-   0     1001 root         (0)     2480 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/oauth.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.277787 perun.proxygui-6.0.0/perun/proxygui/openapi/
+-rw-rw-rw-   0     1001 root         (0)     6107 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/openapi/openapi.py
+-rw-rw-rw-   0     1001 root         (0)    12925 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/openapi/openapi_data.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.277787 perun.proxygui-6.0.0/perun/proxygui/openapi/schemas/
+-rw-rw-rw-   0     1001 root         (0)      982 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/openapi/schemas/arguments_schemas.py
+-rw-rw-rw-   0     1001 root         (0)     1426 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/openapi/schemas/response_schemas.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.277787 perun.proxygui-6.0.0/perun/proxygui/tests/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/tests/__init__.py
+-rw-rw-rw-   0     1001 root         (0)     1816 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/tests/shared_test_data.py
+-rw-rw-rw-   0     1001 root         (0)     9207 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/tests/test_ban_api.py
+-rw-rw-rw-   0     1001 root         (0)     6635 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/tests/test_consent_api.py
+-rw-rw-rw-   0     1001 root         (0)     4713 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/tests/test_consent_db.py
+-rw-rw-rw-   0     1001 root         (0)     2160 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/tests/test_consent_request_db.py
+-rw-rw-rw-   0     1001 root         (0)     6877 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/tests/test_gui.py
+-rw-rw-rw-   0     1001 root         (0)     1101 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/tests/test_kerberos_auth_api.py
+-rw-rw-rw-   0     1001 root         (0)    23012 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/proxygui/user_manager.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.281787 perun.proxygui-6.0.0/perun/utils/
+-rw-rw-rw-   0     1001 root         (0)     2496 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/ConfigStore.py
+-rw-rw-rw-   0     1001 root         (0)       43 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/CustomExceptions.py
+-rw-rw-rw-   0     1001 root         (0)     2555 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/CustomRPHandler.py
+-rw-rw-rw-   0     1001 root         (0)     1545 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/DatabaseService.py
+-rw-rw-rw-   0     1001 root         (0)     4414 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/EmailService.py
+-rw-rw-rw-   0     1001 root         (0)       96 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/Notification.py
+-rw-rw-rw-   0     1001 root         (0)      816 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/Utils.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.281787 perun.proxygui-6.0.0/perun/utils/auth_event_loggig/
+-rw-rw-rw-   0     1001 root         (0)     2100 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/auth_event_loggig/AuthEventLoggingDbModels.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.281787 perun.proxygui-6.0.0/perun/utils/consent_framework/
+-rw-rw-rw-   0     1001 root         (0)     1241 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/consent_framework/consent.py
+-rw-rw-rw-   0     1001 root         (0)     2226 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/consent_framework/consent_db.py
+-rw-rw-rw-   0     1001 root         (0)     2274 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/consent_framework/consent_manager.py
+-rw-rw-rw-   0     1001 root         (0)      730 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/consent_framework/consent_request.py
+-rw-rw-rw-   0     1001 root         (0)     1371 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/consent_framework/consent_request_db.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.281787 perun.proxygui-6.0.0/perun/utils/logout_requests/
+-rw-rw-rw-   0     1001 root         (0)     2001 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/logout_requests/BackchannelLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)      832 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/logout_requests/FrontchannelLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     3841 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/logout_requests/GraphLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     1361 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/logout_requests/LogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     2204 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/perun/utils/logout_requests/SamlLogoutRequest.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-13 06:58:24.221787 perun.proxygui-6.0.0/perun.proxygui.egg-info/
+-rw-r--r--   0     1001 root         (0)     9346 2024-05-13 06:58:24.000000 perun.proxygui-6.0.0/perun.proxygui.egg-info/PKG-INFO
+-rw-r--r--   0     1001 root         (0)    12892 2024-05-13 06:58:24.000000 perun.proxygui-6.0.0/perun.proxygui.egg-info/SOURCES.txt
+-rw-r--r--   0     1001 root         (0)        1 2024-05-13 06:58:24.000000 perun.proxygui-6.0.0/perun.proxygui.egg-info/dependency_links.txt
+-rw-r--r--   0     1001 root         (0)      557 2024-05-13 06:58:24.000000 perun.proxygui-6.0.0/perun.proxygui.egg-info/requires.txt
+-rw-r--r--   0     1001 root         (0)        6 2024-05-13 06:58:24.000000 perun.proxygui-6.0.0/perun.proxygui.egg-info/top_level.txt
+-rw-rw-rw-   0     1001 root         (0)       90 2024-05-13 06:58:24.281787 perun.proxygui-6.0.0/setup.cfg
+-rw-rw-rw-   0     1001 root         (0)     1485 2024-05-13 06:57:39.000000 perun.proxygui-6.0.0/setup.py
```

### Comparing `perun.proxygui-5.2.1/LICENSE` & `perun.proxygui-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/PKG-INFO` & `perun.proxygui-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxygui
-Version: 5.2.1
+Version: 6.0.0
 Summary: Module with GUI and API for Perun ProxyIdP
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/proxyidp-gui.git
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Authlib==1.3.0
 Requires-Dist: setuptools
@@ -122,15 +122,15 @@
 
 ### local development
 
 ```sh
 python3 perun/proxygui/app.py
 ```
 
-Now the app is available at `http://localhost:5000/` (e.g. `http://localhost:5000/banned-users/`).
+Now the app is available at `http://localhost:5000/` (e.g. `http://localhost:5000/bans`).
 
 ### local OpenAPI development
 
 To create local, temporal OpenAPI scheme from current version run following command:
 
 ```sh
 flask --app perun.proxygui.app:get_openapi openapi write --format=yaml "temp_out_file.yaml"
@@ -156,23 +156,23 @@
 
 In `openapi.yaml` is OpenAPI specification openable in editors (e.g. [Swagger Editor](https://editor.swagger.io/))
 
 ### Heuristic page
 
 Provides information about user authentication events gathered by the AuthEventLogging microservice, to confirm their identity e.g. during a MFA reset.
 
-**Endpoint:** `/HeuristicGetID`
+**Endpoint:** `/heuristics`
 
 **Description:** Used to gather ID of searched user
 
 **Result:**
 
 - `HTTP OK [200]` indicating successfull load of search page
 
-**Endpoint:** `/GetHeuristic`
+**Endpoint:** `/heuristics/<user_id>`
 
 **Method:** `GET`
 
 **Description:** Used for showing gathered information about past athentications of user, and showing statistics based on that data.
 
 **Performed MFA:** Gathered logs are checked if MFA was performed while handeling original logging event. Upstream ACRs values are compared to two hardcoded values: `https://refeds.org/profile/mfa` and `http://schemas.microsoft.com/claims/multipleauthn`
```

### Comparing `perun.proxygui-5.2.1/README.md` & `perun.proxygui-6.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 ### local development
 
 ```sh
 python3 perun/proxygui/app.py
 ```
 
-Now the app is available at `http://localhost:5000/` (e.g. `http://localhost:5000/banned-users/`).
+Now the app is available at `http://localhost:5000/` (e.g. `http://localhost:5000/bans`).
 
 ### local OpenAPI development
 
 To create local, temporal OpenAPI scheme from current version run following command:
 
 ```sh
 flask --app perun.proxygui.app:get_openapi openapi write --format=yaml "temp_out_file.yaml"
@@ -120,23 +120,23 @@
 
 In `openapi.yaml` is OpenAPI specification openable in editors (e.g. [Swagger Editor](https://editor.swagger.io/))
 
 ### Heuristic page
 
 Provides information about user authentication events gathered by the AuthEventLogging microservice, to confirm their identity e.g. during a MFA reset.
 
-**Endpoint:** `/HeuristicGetID`
+**Endpoint:** `/heuristics`
 
 **Description:** Used to gather ID of searched user
 
 **Result:**
 
 - `HTTP OK [200]` indicating successfull load of search page
 
-**Endpoint:** `/GetHeuristic`
+**Endpoint:** `/heuristics/<user_id>`
 
 **Method:** `GET`
 
 **Description:** Used for showing gathered information about past athentications of user, and showing statistics based on that data.
 
 **Performed MFA:** Gathered logs are checked if MFA was performed while handeling original logging event. Upstream ACRs values are compared to two hardcoded values: `https://refeds.org/profile/mfa` and `http://schemas.microsoft.com/claims/multipleauthn`
```

### Comparing `perun.proxygui-5.2.1/perun/proxygui/api/backchannel_logout_api.py` & `perun.proxygui-6.0.0/perun/proxygui/api/backchannel_logout_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/api/ban_api.py` & `perun.proxygui-6.0.0/perun/proxygui/api/ban_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,25 +96,25 @@
     )
     BAN_CFG = cfg.get("ban_api")
 
     USER_MANAGER = UserManager(BAN_CFG)
     UPLOAD_FILE_MAX_SIZE = int(BAN_CFG.get("max_ban_upload_filesize"))
 
     # Endpoints
-    @openapi_route("/banned-users/", ban_openapi_api)
+    @openapi_route("/bans", ban_openapi_api)
     def update_banned_users() -> Response:
         process_update(request.get_json())
 
         response = flask.Response()
         response.headers["Cache-Control"] = "public, max-age=0"
         response.status_code = HTTPStatus.NO_CONTENT
 
         return response
 
-    @openapi_route("/banned-users-generic/", ban_openapi_api)
+    @openapi_route("/bans/perun-idm", ban_openapi_api)
     def update_banned_users_generic() -> Response:
         if request.content_length > UPLOAD_FILE_MAX_SIZE:
             logger.warn(
                 f"Request too large: "
                 f"{str((request.content_length // 1024) // 1024)} MB"
             )
             response = flask.make_response(
@@ -172,15 +172,15 @@
 
             for user_id, ban in banned_users.items():
                 print(user_id)
                 if not is_ban_in_db(int(ban["id"]), cnxn, ban_table):
                     USER_MANAGER.logout(user_id=user_id, include_refresh_tokens=True)
                 replace_one_in_db(int(ban["id"]), cnxn, ban_table, ban)
 
-    @openapi_route("/ban/<string:ban_id>", ban_openapi_api)
+    @openapi_route("/bans/<string:ban_id>", ban_openapi_api)
     def find_ban(ban_id: str) -> str:
         engine = get_ban_engine(USER_MANAGER)
         response = get_ban_from_db(engine, USER_MANAGER, ban_id, BAN_CFG)
 
         from pprint import pprint
 
         pprint(response)
```

### Comparing `perun.proxygui-5.2.1/perun/proxygui/api/consent_api.py` & `perun.proxygui-6.0.0/perun/proxygui/api/consent_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/api/heuristic_api.py` & `perun.proxygui-6.0.0/perun/proxygui/api/heuristic_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/api/kerberos_auth_api.py` & `perun.proxygui-6.0.0/perun/proxygui/api/kerberos_auth_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         "Kerberos API",
         __name__,
         url_prefix="/proxygui",
         description=apis_desc.get("kerberos", ""),
     )
     KERBEROS_CFG = cfg.get("kerberos_api")
 
-    @openapi_route("/AuthenticateKerberosTicket", kerberos_openapi_auth_api)
+    @openapi_route("/kerberos/authenticate", kerberos_openapi_auth_api)
     def authenticate_kerberos_ticket():
         """
         Import done here to prevent other endpoints from being dependent on
         the kerberos
         module. Flask blueprints are assembled in one file and this process
         would automatically start
         importing kerberos modules regardless of their uselessnes for other
```

### Comparing `perun.proxygui-5.2.1/perun/proxygui/app.py` & `perun.proxygui-6.0.0/perun/proxygui/app.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/gui.py` & `perun.proxygui-6.0.0/perun/proxygui/gui/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,18 +84,18 @@
     consent_db_manager = ConsentManager(GUI_CFG)
     user_manager = UserManager(GUI_CFG)
 
     jwt_service = SingletonJWTServiceProvider.get_provider().get_service()
     logout_manager = LogoutManager(GUI_CFG)
     auth_event = AuthEventLoggingQueries(GUI_CFG)
 
-    @gui.route("/authorization/<token>")
-    def authorization(token):
+    @gui.route("/authorization/<request_jwt>", methods=["POST"])
+    def authorization(request_jwt):
         try:
-            message = jwt_service.verify_jwt(token)
+            message = jwt_service.verify_jwt(request_jwt)
         except InvalidJWTError as e:
             return make_response(
                 jsonify({gettext("fail"): f"JWT validation failed with error: '{e}'"}),
                 400,
             )
         email = message.get("email")
         service = message.get("service")
@@ -108,18 +108,18 @@
         return render_template(
             "authorization.html",
             email=email,
             service=service,
             registration_url=registration_url,
         )
 
-    @gui.route("/SPAuthorization/<token>")
-    def sp_authorization(token):
+    @gui.route("/sp-authorization/<request_jwt>", methods=["POST"])
+    def sp_authorization(request_jwt):
         try:
-            message = jwt_service.verify_jwt(token)
+            message = jwt_service.verify_jwt(request_jwt)
         except InvalidJWTError as e:
             return make_response(
                 jsonify({gettext("fail"): f"JWT validation failed with error: '{e}'"}),
                 400,
             )
         email = message.get("email")
         service = message.get("service")
@@ -130,15 +130,15 @@
             service=service,
             registration_url=registration_url,
         )
 
     # Logout ==================================================================================
     if GUI_CFG.get("logout", None):
 
-        @gui.route("/logout", methods=["POST", "GET"])
+        @gui.route("/logout-system", methods=["POST", "GET"])
         def logout():
             ssp_session_id = request.cookies.get("SimpleSAMLSessionID")
 
             logger.debug(f"Logout call for SimpleSAMLSessionID: {ssp_session_id}")
             # todo - dbs will contain user_id and won't need to be converted in the future
             sub = user_manager.get_user_id_by_ssp_session_id(ssp_session_id)
 
@@ -191,21 +191,21 @@
                     logged_out_service=logged_out_service,
                     session_services=session_services,
                     device_services=device_services,
                 )
             )
             return resp
 
-        @gui.route("/logout_canceled")
+        @gui.route("/logout-canceled")
         def logout_canceled():
             return render_template(
                 "logout-canceled.html",
             )
 
-        @gui.route("/logout_state", methods=["GET"])
+        @gui.route("/logout-state")
         def logout_state():
             if session.get("logout_params") is None:
                 # at least empty dict should be set, or logout endpoint was not visited
                 return redirect(url_for("gui.logout", _external=True))
 
             ssp_session_id = request.cookies.get("SimpleSAMLSessionID")
             # todo - dbs will contain user_id and won't need to be converted in the future
@@ -290,15 +290,15 @@
                     session_services=logout_requests if not include_all_devices else [],
                     device_services=logout_requests if include_all_devices else [],
                 )
             )
             resp.delete_cookie("SimpleSAMLSessionID")
             return resp
 
-        @gui.route("/post_logout")
+        @gui.route("/logout-post")
         def post_logout():
             logout_params = session.get("logout_params")
             init_logged_out_service = session.get("init_logged_out_service")
             session.clear()
 
             if (
                 logout_params is None or init_logged_out_service is None
@@ -313,15 +313,15 @@
                 return redirect(url)
 
             return render_template(
                 "Post-logout.html",
                 init_logged_out_service=init_logged_out_service,
             )
 
-        @gui.route("/logout_iframe_callback", methods=["GET"])
+        @gui.route("/logout-iframe-callback")
         def logout_iframe_callback():
             request_id = request.args.get("request_id")
             logout_requests = session["logout_requests"]
 
             current_request = next(
                 (r for r in logout_requests if str(r["id"]) == request_id), None
             )
@@ -332,40 +332,40 @@
                 req = logout_manager.deserialize_request(current_request)
                 response = req.logout()
             return render_template(
                 "logout-iframe.html",
                 result="success" if response else response,
             )
 
-        @gui.route("/logout_saml_callback/<issuer_id>", methods=["GET"])
+        @gui.route("/logout-saml-callback/<issuer_id>")
         def logout_saml_callback(issuer_id):
             request_ok = logout_manager.check_saml_callback(request, issuer_id)
 
             return render_template(
                 "logout-iframe.html",
                 result="success" if request_ok else "request invalid",
             )
 
     # Testing ==================================================================================
     if GUI_CFG.get("is_testing_sp", None):
 
-        @gui.route("/IsTestingSP")
+        @gui.route("/is-testing-sp")
         def is_testing_sp():
             return render_template(
                 "IsTestingSP.html",
                 redirect_url=REDIRECT_URL,
             )
 
     # Consent ==================================================================================
     if GUI_CFG.get("consent", None):
 
-        @gui.route("/consent/<token>")
-        def consent(token):
+        @gui.route("/consent-requests/<request_jwt>")
+        def consent(request_jwt):
             try:
-                ticket = jwt_service.verify_jwt(token)
+                ticket = jwt_service.verify_jwt(request_jwt)
             except InvalidJWTError as e:
                 return make_response(
                     jsonify(
                         {gettext("fail"): f"JWT validation failed with error: '{e}'"}
                     ),
                     400,
                 )
@@ -407,34 +407,34 @@
                 data_protection_redirect=data["data_protection_redirect"],
                 warning=warning,
             )
 
     # MFA ==================================================================================
     if GUI_CFG.get("mfa_reset", None):
 
-        @gui.route("/mfa-reset-verify/<token>")
+        @gui.route("/mfa/reset/assisted/verify/<mfa_reset_jwt>")
         @auth.oidc_auth(OIDC_CFG["provider_name"])
-        def mfa_reset_verify(token):
+        def mfa_reset_verify(mfa_reset_jwt):
             try:
-                reset_request = jwt_service.verify_jwt(token)
+                reset_request = jwt_service.verify_jwt(mfa_reset_jwt)
             except InvalidJWTError:
                 return render_template(
                     "MfaResult.html",
                     title="request_fail_title",
                     info="request_fail_info",
                 )
             requester_email = reset_request.get("requester_email")
             user_manager.forward_mfa_reset_request(requester_email)
             return render_template(
                 "MfaResult.html",
                 title="request_success_title",
                 info="request_success_info",
             )
 
-        @gui.route("/send-mfa-reset-emails")
+        @gui.route("/mfa/reset/assisted/confirm", methods=["POST"])
         @auth.oidc_auth(OIDC_CFG["provider_name"])
         def send_mfa_reset_emails():
             user_session = UserSession(flask.session, OIDC_CFG["provider_name"])
             sub = user_session.userinfo.get("sub")
             issuer = OIDC_CFG["issuer"]
             user_id = user_manager.sub_to_user_id(sub, issuer)
             if not user_id:
@@ -451,25 +451,25 @@
                 NotificationType.VERIFICATION,
             )
             return render_template(
                 "MfaResetEmailSent.html",
                 email=preferred_email,
             )
 
-        @gui.route("/mfa-reset")
+        @gui.route("/mfa/reset/assisted")
         @auth.oidc_auth(OIDC_CFG["provider_name"])
-        def mfa_reset():
+        def mfa_reset_init():
             return render_template(
                 "MfaResetInitiated.html",
                 redirect_url=REDIRECT_URL,
                 referrer=request.referrer or "/",
                 next_action=url_for("gui.send_mfa_reset_emails"),
             )
 
-        @gui.route("/mfa-perform-delegated-reset")
+        @gui.route("/mfa/reset/delegated/confirm", methods=["POST"])
         @auth.oidc_auth(MFA_CFG["provider_name"])
         def mfa_perform_delegated_reset():
             if not session.get("mfa_reset_visited"):
                 # force user to confirm this action
                 return redirect(url_for("gui.mfa_delegated_reset"))
             user_session = UserSession(flask.session, MFA_CFG["provider_name"])
             username = user_session.id_token.get("sub")
@@ -494,49 +494,41 @@
                 session["mfa_reset_success"] = True
                 return render_template(
                     "MfaResult.html",
                     title="delegated_failed_title",
                     info="delegated_failed_info",
                 )
 
-        @gui.route("/mfa-delegated-reset")
+        @gui.route("/mfa/reset/delegated")
         @auth.oidc_auth(MFA_CFG["provider_name"])
-        def mfa_delegated_reset():
+        def mfa_delegated_reset_init():
             session["mfa_reset_visited"] = True
             return render_template(
                 "MfaResetInitiated.html",
                 redirect_url=REDIRECT_URL,
                 referrer=request.referrer or "/",
                 next_action=url_for("gui.mfa_perform_delegated_reset"),
             )
 
     # Heuristic ==================================================================================
     if GUI_CFG.get("heuristic_page", None):
 
-        @gui.route("/HeuristicGetID")
+        @gui.route("/heuristics")
         @auth.oidc_auth(OIDC_CFG["provider_name"])
-        def heuristic_get_id():
+        def heuristics():
             if not check_scope_claim("heuristic_pages", OIDC_CFG):
                 return "User does not have access to this page", HTTPStatus.FORBIDDEN
 
-            return render_template(
-                "HeuristicData.html",
-                redirect_url=REDIRECT_URL,
-                selected=False,
-            )
-
-        @gui.route("/GetHeuristic", methods=["GET"])
-        @auth.oidc_auth(OIDC_CFG["provider_name"])
-        def get_heuristic():
-            user_id = request.args.get("user")
+            user_id = request.args.get("user_id")
             if not user_id:
-                return "User ID not provided in the request", HTTPStatus.BAD_REQUEST
-
-            if not check_scope_claim("heuristic_pages", OIDC_CFG):
-                return "User does not have access to this page", HTTPStatus.FORBIDDEN
+                return render_template(
+                    "HeuristicData.html",
+                    redirect_url=REDIRECT_URL,
+                    selected=False,
+                )
 
             try:
                 user_id = int(user_id)
             except ValueError:
                 return (
                     f"Provided user ID: '{user_id}' could not be converted to an "
                     f"integer"
```

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/documentation.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/documentation.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/print.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/print.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-custom.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-custom.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-econ.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-econ.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-fi.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fi.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-fss.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fss.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-law.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-law.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-med.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-med.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-ped.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-ped.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-phil.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-phil.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style-sci.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style-sci.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/style.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/favicon.ico` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/app.js` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/app.js.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/d3.js` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/d3.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/documentation.js` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/documentation.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/graphs.js` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/graphs.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/jquery.js` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/campus-idp.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/campus-idp.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/campus-idp.js` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/campus-idp.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/css/all.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/css/all.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/css/all.min.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/images/circle-check-regular.svg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/images/circle-check-regular.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/images/questionmark.svg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/images/questionmark.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/images/spinner.svg` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/images/spinner.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/jquery-3.6.0.min.js` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/proxygui.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/proxygui.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/proxygui.js` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/proxygui.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.default.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.default.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/css/selectize.legacy.css` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/css/selectize.legacy.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js` & `perun.proxygui-6.0.0/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/ConsentRegistration.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/ConsentRegistration.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/HeuristicData.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/HeuristicData.html`

 * *Files 1% similar despite different names*

```diff
@@ -122,19 +122,18 @@
                             </div>
                         </div>
                     {% else %}
                         <div class="content">
                             <br/>
                             <h3><span>{{ _("Specify a Perun user ID to gather data:") }}</span></h3>
                             <form action="{{ url_for('gui.get_heuristic') }}" method="get">
-                                <input type="number" id="userID"
-                                name="user" min="1" required placeholder="User ID">
+                                <input type="number" id="user_id" name="user_id" min="1" required placeholder="User ID">
                                 <p class="btn-wrap">
                                     <button class="btn btn-primary btn-s btn-accept"
-                                        type="submit" name="submit">
+                                            type="submit" name="submit">
                                         <span>Submit</span>
                                     </button>
                                 </p>
                             </form>
                         </div>
                     {% endif %}
                 {% endblock %}
```

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/IsTestingSP.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/IsTestingSP.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/Logout.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/Logout.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/MfaResetEmailSent.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/MfaResetEmailSent.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/MfaResetInitiated.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/MfaResetInitiated.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/MfaResult.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/MfaResult.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/MissingAuth.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/MissingAuth.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/OidcError.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/OidcError.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/Post-logout.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/Post-logout.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/SPAuthorization.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/SPAuthorization.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/_footer.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/_footer.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/_header.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/_header.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/authorization.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/authorization.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/base.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/base.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/logout-canceled.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/logout-canceled.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/logout-iframe.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/logout-iframe.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/templates/logout-state.html` & `perun.proxygui-6.0.0/perun/proxygui/gui/templates/logout-state.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo` & `perun.proxygui-6.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po` & `perun.proxygui-6.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/jwt.py` & `perun.proxygui-6.0.0/perun/proxygui/jwt.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/logout_manager.py` & `perun.proxygui-6.0.0/perun/proxygui/logout_manager.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/oauth.py` & `perun.proxygui-6.0.0/perun/proxygui/oauth.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/openapi/openapi.py` & `perun.proxygui-6.0.0/perun/proxygui/openapi/openapi.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/openapi/openapi_data.py` & `perun.proxygui-6.0.0/perun/proxygui/openapi/openapi_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,17 +136,18 @@
 Performs [OIDC Back-Channel Logout 1.0](https://openid.net/specs/openid-connect-backchannel-1_0.html) in the role of RP.
 """,
 }
 
 
 data = {
     # ------------- Kerberos --------------------------------------------------
-    "/AuthenticateKerberosTicket": {
-        "desc": "AuthenticateKerberosTicket description",
-        "sum": "AuthenticateKerberosTicket summary",
+    "/kerberos/authenticate": {
+        "methods": ["GET"],
+        "desc": "/kerberos/authenticate description",
+        "sum": "/kerberos/authenticate summary",
         "security": [{"NegotiateAuth": []}],
         "response": {
             "status": HTTPStatus.UNAUTHORIZED,
             "example": {"_text": "Kerberos authentication successful"},
             "schema": string_schema,
             "description": TODO_DESCRIPTION,
         },
@@ -273,15 +274,15 @@
         "response": {
             "status": HTTPStatus.OK,
             "schema": delete_consent_schema,
         },
         "arguments": [{"location": "path", "schema": consent_id_argument_schema}],
     },
     # ------------ Ban API ----------------------------------------------------
-    "/banned-users/": {
+    "/bans": {
         "methods": ["PUT"],
         "desc": """
 This endpoint adds all user bans provided in the request input data to the database. This effectively
 bans the Perun users from logging in to the system. If the user is already banned, their ban is replaced with the latest
 one (the one currently provided in the request).
 
 Calling this endpoint revokes user's SSP sessions, Mitre tokens, SATOSA sessions and
@@ -313,18 +314,18 @@
                 "location": "files",
                 "schema": file_input_schema,
                 "description": "List of users bans in JSON format.",
             }
         ],
     },
     # ----------------------------------------
-    "/banned-users-generic/": {
+    "/bans/perun-idm": {
         "methods": ["PUT"],
         "desc": """
-Generalized endpoint behaving in the same way as the `/banned-users` endpoint. The only difference is
+Generalized endpoint behaving in the same way as the `/bans` endpoint. The only difference is
 that the input data is passed in binary form as `.tar` file in the request.
 """,
         "sum": "update_banned_users_generic",
         "response": {
             "status": HTTPStatus.NO_CONTENT,
             "schema": response_schema,
             "description": "`HTTP No Content` - indicating successful banning",
@@ -347,15 +348,15 @@
                 "location": "files",
                 "schema": file_input_schema,
                 "description": "List of users to ban in `.tar` format in request data.",
             }
         ],
     },
     # ----------------------------------------
-    "/ban/<string:ban_id>": {
+    "/bans/<string:ban_id>": {
         "methods": ["GET"],
         "desc": "Used for checking whether a ban with given `ban_id` exists. ",
         "sum": "find_ban",
         "response": {
             "status": HTTPStatus.OK,
             "example": {"_text": "Found ban dictionary"},
             "schema": string_schema,
```

### Comparing `perun.proxygui-5.2.1/perun/proxygui/openapi/schemas/arguments_schemas.py` & `perun.proxygui-6.0.0/perun/proxygui/openapi/schemas/arguments_schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from marshmallow import fields, Schema
 from flask_smorest.fields import Upload
 
 
 # -------------------------- Input schemas ----------------------------------
-# /banned-users/
-# /banned-users-generic/
+# /bans
+# /bans/perun-idm
 class file_input_schema(Schema):
     data = Upload()
 
 
-# /ban/<string:ban_id>
+# /bans/<string:ban_id>
 class ban_id_argument_schema(Schema):
     ban_id = fields.String(
         metadata={"description": "ID of a potential ban in the URL parameter"}
     )
 
 
 # /backchannel-logout
```

### Comparing `perun.proxygui-5.2.1/perun/proxygui/openapi/schemas/response_schemas.py` & `perun.proxygui-6.0.0/perun/proxygui/openapi/schemas/response_schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # /verify/<string:consent_id>
 class consent_attrs_schema(Schema):
     # consent.attributes fields
     # TODO add exact fromat of consent attributes
     pass
 
 
-# /ban/<string:ba_id>
-# /AuthenticateKerberosTicket
+# /bans/<string:ba_id>
+# /kerberos/authenticate
 class string_schema(Schema):
     _text = fields.String()
 
 
 # /users/me/consents
 class consent_schema(Schema):
     user_id = fields.String()
@@ -38,16 +38,16 @@
 
 
 # -------------------------------------------------------------------------
 # Schemas for Response type return value (Response, redirect, ...)
 # only for API purpose
 
 
-# /banned-users-generic/
-# /banned-users/
+# /bans/perun-idm
+# /bans
 class response_schema(Schema):
     response = fields.String(load_default="flask.Response class is returned")
 
 
 # /save_consent
 class redirect_schema(Schema):
     response = fields.String(
```

### Comparing `perun.proxygui-5.2.1/perun/proxygui/tests/shared_test_data.py` & `perun.proxygui-6.0.0/perun/proxygui/tests/shared_test_data.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/tests/test_ban_api.py` & `perun.proxygui-6.0.0/perun/proxygui/tests/test_ban_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     )
     cursor_mock.execute.return_value.fetchone.return_value._asdict.return_value = (
         BAN_IN_DB_1
     )
 
     mock_get_ban_table.return_value = TestTable.__table__
 
-    response = client.get(f"/proxygui/ban/{BAN_IN_DB_1['id']}")
+    response = client.get(f"/proxygui/bans/{BAN_IN_DB_1['id']}")
     result = json.loads(json.loads(response.data.decode()).get("_text", {}))
 
     for key, value in BAN_IN_DB_1.items():
         assert result.get(key) == value
 
 
 @patch("perun.proxygui.api.ban_api.get_ban_table")
@@ -100,15 +100,15 @@
         mock_get_ban_engine.return_value.connect.return_value.__enter__.return_value
     )
     cursor_mock.execute.return_value.fetchone.return_value._asdict.return_value = None
     mock_get_ban_table.return_value = TestTable.__table__
 
     not_in_db_ban_id = -1
 
-    response = client.get(f"/proxygui/ban/{not_in_db_ban_id}")
+    response = client.get(f"/proxygui/bans/{not_in_db_ban_id}")
     result = json.loads(json.loads(response.data.decode()).get("_text", {}))
 
     assert result == {}
 
 
 @patch("perun.proxygui.api.ban_api.remove_outdated_bans_from_db")
 @patch("perun.connector.AdaptersManager.get_user_attributes")
@@ -136,15 +136,15 @@
     mock_get_ban_engine.return_value.connect.return_value.__enter__.return_value = None
     mock_is_ban_in_db.return_value = True
     mock_user_manager_logout.return_value = None
 
     user_bans_in_db = {ban["userId"]: ban for ban in BANS_IN_DB}
 
     client.put(
-        "/proxygui/banned-users/",
+        "/proxygui/bans",
         json=user_bans_in_db,
         headers={"Content-type": "application/json", "Accept": "application/json"},
     )
     assert not mock_user_manager_logout.called
 
 
 @patch("perun.proxygui.api.ban_api.remove_outdated_bans_from_db")
@@ -189,15 +189,15 @@
     number_of_bans_in_db = len(BANS_IN_DB)
     number_of_bans_not_in_db = len(BANS_NOT_IN_DB)
 
     mock_logout.side_effect = logout_from_test
 
     assert len(test_ban_db) == number_of_bans_in_db
 
-    client.put("/proxygui/banned-users/", json=all_user_bans)
+    client.put("/proxygui/bans", json=all_user_bans)
 
     assert len(test_ban_db) == number_of_bans_in_db + number_of_bans_not_in_db
 
     for ban in BANS_IN_DB + BANS_NOT_IN_DB:
         assert ban in test_ban_db
 
     for ban in BANS_NOT_IN_DB:
@@ -221,15 +221,15 @@
         tar.addfile(info, file_data)
     tar.name = "sent_data"
 
     buffer.seek(0)
     gzipped_data = gzip.compress(buffer.read())
 
     response = client.put(
-        "/proxygui/banned-users-generic/",
+        "/proxygui/bans/perun-idm",
         content_type="application/x-tar",
         data=gzipped_data,
     )
     assert response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY
 
 
 @patch("perun.proxygui.api.ban_api.replace_one_in_db")
@@ -273,13 +273,13 @@
         tar.addfile(info, file_data)
     tar.name = "data"
 
     buffer.seek(0)
     gzipped_data = gzip.compress(buffer.read())
 
     client.put(
-        "/proxygui/banned-users-generic/",
+        "/proxygui/bans/perun-idm",
         content_type="application/x-tar",
         data=gzipped_data,
     )
 
     assert len(test_db) == 1
```

### Comparing `perun.proxygui-5.2.1/perun/proxygui/tests/test_consent_api.py` & `perun.proxygui-6.0.0/perun/proxygui/tests/test_consent_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/tests/test_consent_db.py` & `perun.proxygui-6.0.0/perun/proxygui/tests/test_consent_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/tests/test_consent_request_db.py` & `perun.proxygui-6.0.0/perun/proxygui/tests/test_consent_request_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/proxygui/tests/test_gui.py` & `perun.proxygui-6.0.0/perun/proxygui/tests/test_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         with tempfile.TemporaryDirectory() as temp_session_folder:
             app.config["SESSION_FILE_DIR"] = temp_session_folder
         Session(app)
         yield app.test_client()
 
 
 def test_is_testing_sp(client):
-    response = client.get("/proxygui/IsTestingSP")
+    response = client.get("/proxygui/is-testing-sp")
     is_testing_sp_text = (
         "You are about to access service, which is in testing environment."
         # noqa
     )
     is_testing_sp_text_2 = "Continue"
 
     result = response.data.decode()
@@ -84,33 +84,33 @@
     is_testing_sp_text_3 = "For more information about this service please visit this "  # noqa
     is_testing_sp_text_4 = (
         "If you think you should have an access contact service operator at "
         # noqa
     )
     is_testing_sp_text_5 = "Problem with login to service: "
     mock_method.return_value = test_data
-    response = client.get("/proxygui/authorization/example")
+    response = client.post("/proxygui/authorization/example")
 
     result = response.data.decode()
     assert is_testing_sp_text in result
     assert is_testing_sp_text_2 in result
     assert is_testing_sp_text_3 in result
     assert is_testing_sp_text_4 in result
     assert is_testing_sp_text_5 in result
     assert response.status_code == 200
 
 
 def test_sp_authorization_error(client):
-    response = client.get("/proxygui/SPAuthorization")
+    response = client.get("/proxygui/sp-authorization")
 
     assert response.status_code == 404
 
 
 def test_logout_cookies_missing(client):
-    response = client.get("/proxygui/logout")
+    response = client.get("/proxygui/logout-system")
     result = response.data.decode()
     cookies_missing = "cookies are missing"
     assert cookies_missing in result
 
 
 def test_logout_overview(client):
     with patch(
@@ -123,28 +123,28 @@
         "perun.proxygui.user_manager.UserManager.get_active_client_ids_for_session",
         return_value=[MOCK_SESSIONS[0]],
     ), patch(
         "perun.proxygui.user_manager.UserManager.get_all_rp_names",
         return_value=MOCK_SERVICE_NAMES,
     ):
         client.set_cookie(key="SimpleSAMLSessionID", value="123456")
-        response = client.get("/proxygui/logout")
+        response = client.get("/proxygui/logout-system")
         result = response.data.decode()
         session_services, device_services = result.split("on your other devices")
         assert "Client 1" in session_services
         assert "Client 2" not in session_services
         assert "Client 1" in device_services
         assert "Client 2" in device_services
 
 
 def test_logout_state_wrong_flow(client):
     client.set_cookie(key="SimpleSAMLSessionID", value="123456")
-    response = client.get("/proxygui/logout_state", follow_redirects=False)
+    response = client.get("/proxygui/logout-state", follow_redirects=False)
     redirected_url = response.headers["Location"]
-    assert redirected_url.endswith("/logout")
+    assert redirected_url.endswith("/logout-system")
 
 
 def test_logout_state_iframe(client):
     with patch(
         "perun.proxygui.user_manager.UserManager._get_ssp_session_by_key",
         return_value={"eduperson_principal_name": 123},
     ), patch(
@@ -162,15 +162,15 @@
     ), patch(
         "perun.proxygui.user_manager.UserManager.sub_to_user_id", return_value="1"
     ):
         client.set_cookie(key="SimpleSAMLSessionID", value="123456")
         with client.session_transaction() as session:
             session["logout_params"] = {}
             session["init_logged_out_service"] = {}
-        response = client.get("/proxygui/logout_state", follow_redirects=True)
+        response = client.get("/proxygui/logout-state", follow_redirects=True)
         iframe_pattern = re.compile(r'<iframe.*?src="/test_logout_uri".*?</iframe>')
         assert iframe_pattern.search(response.text) is not None
 
 
 @patch("perun.proxygui.jwt.JWTService.verify_jwt")
 def test_sp_authorization(mock_method, client):
     test_data = {
@@ -181,14 +181,14 @@
     is_testing_sp_text = "You are not authorized to access the service "
     is_testing_sp_text_2 = (
         "We will now redirect you to a registration page, "
         + "where you will apply for the access."
     )
     is_testing_sp_text_3 = "Proceed to registration"
     mock_method.return_value = test_data
-    response = client.get("/proxygui/SPAuthorization/example")
+    response = client.post("/proxygui/sp-authorization/example")
 
     result = response.data.decode()
     assert is_testing_sp_text in result
     assert is_testing_sp_text_2 in result
     assert is_testing_sp_text_3 in result
     assert response.status_code == 200
```

### Comparing `perun.proxygui-5.2.1/perun/proxygui/tests/test_kerberos_auth_api.py` & `perun.proxygui-6.0.0/perun/proxygui/tests/test_kerberos_auth_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 # prevent client from being "unused" during static code analysis, it is injected to
 # the tests upon launch
 _ = client
 
 
 def test_auth_no_auth_header_sent(client):
-    response = client.get("/proxygui/AuthenticateKerberosTicket")
+    response = client.get("/proxygui/kerberos/authenticate")
 
     no_auth_header_msg = "Negotiate"
 
     assert response.status_code == HTTPStatus.UNAUTHORIZED
     assert no_auth_header_msg in response.headers.get("WWW-Authenticate")
 
 
 def test_auth_invalid_format_auth_header(client):
     headers = {"Authorization": "Something wrong here"}
-    response = client.get("/proxygui/AuthenticateKerberosTicket", headers=headers)
+    response = client.get("/proxygui/kerberos/authenticate", headers=headers)
 
     invalid_format_auth_header_msg = (
         "Kerberos ticket in authorization "
         "header must start with 'Negotiate'. "
         "Incorrect format was provided in "
         "authorization header."
     )  # noqa
```

### Comparing `perun.proxygui-5.2.1/perun/proxygui/user_manager.py` & `perun.proxygui-6.0.0/perun/proxygui/user_manager.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/ConfigStore.py` & `perun.proxygui-6.0.0/perun/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/CustomRPHandler.py` & `perun.proxygui-6.0.0/perun/utils/CustomRPHandler.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/DatabaseService.py` & `perun.proxygui-6.0.0/perun/utils/DatabaseService.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/EmailService.py` & `perun.proxygui-6.0.0/perun/utils/EmailService.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/Utils.py` & `perun.proxygui-6.0.0/perun/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/auth_event_loggig/AuthEventLoggingDbModels.py` & `perun.proxygui-6.0.0/perun/utils/auth_event_loggig/AuthEventLoggingDbModels.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/consent_framework/consent.py` & `perun.proxygui-6.0.0/perun/utils/consent_framework/consent.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/consent_framework/consent_db.py` & `perun.proxygui-6.0.0/perun/utils/consent_framework/consent_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/consent_framework/consent_manager.py` & `perun.proxygui-6.0.0/perun/utils/consent_framework/consent_manager.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/consent_framework/consent_request.py` & `perun.proxygui-6.0.0/perun/utils/consent_framework/consent_request.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/consent_framework/consent_request_db.py` & `perun.proxygui-6.0.0/perun/utils/consent_framework/consent_request_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/logout_requests/BackchannelLogoutRequest.py` & `perun.proxygui-6.0.0/perun/utils/logout_requests/BackchannelLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/logout_requests/FrontchannelLogoutRequest.py` & `perun.proxygui-6.0.0/perun/utils/logout_requests/FrontchannelLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/logout_requests/GraphLogoutRequest.py` & `perun.proxygui-6.0.0/perun/utils/logout_requests/GraphLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/logout_requests/LogoutRequest.py` & `perun.proxygui-6.0.0/perun/utils/logout_requests/LogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun/utils/logout_requests/SamlLogoutRequest.py` & `perun.proxygui-6.0.0/perun/utils/logout_requests/SamlLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun.proxygui.egg-info/PKG-INFO` & `perun.proxygui-6.0.0/perun.proxygui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxygui
-Version: 5.2.1
+Version: 6.0.0
 Summary: Module with GUI and API for Perun ProxyIdP
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/proxyidp-gui.git
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Authlib==1.3.0
 Requires-Dist: setuptools
@@ -122,15 +122,15 @@
 
 ### local development
 
 ```sh
 python3 perun/proxygui/app.py
 ```
 
-Now the app is available at `http://localhost:5000/` (e.g. `http://localhost:5000/banned-users/`).
+Now the app is available at `http://localhost:5000/` (e.g. `http://localhost:5000/bans`).
 
 ### local OpenAPI development
 
 To create local, temporal OpenAPI scheme from current version run following command:
 
 ```sh
 flask --app perun.proxygui.app:get_openapi openapi write --format=yaml "temp_out_file.yaml"
@@ -156,23 +156,23 @@
 
 In `openapi.yaml` is OpenAPI specification openable in editors (e.g. [Swagger Editor](https://editor.swagger.io/))
 
 ### Heuristic page
 
 Provides information about user authentication events gathered by the AuthEventLogging microservice, to confirm their identity e.g. during a MFA reset.
 
-**Endpoint:** `/HeuristicGetID`
+**Endpoint:** `/heuristics`
 
 **Description:** Used to gather ID of searched user
 
 **Result:**
 
 - `HTTP OK [200]` indicating successfull load of search page
 
-**Endpoint:** `/GetHeuristic`
+**Endpoint:** `/heuristics/<user_id>`
 
 **Method:** `GET`
 
 **Description:** Used for showing gathered information about past athentications of user, and showing statistics based on that data.
 
 **Performed MFA:** Gathered logs are checked if MFA was performed while handeling original logging event. Upstream ACRs values are compared to two hardcoded values: `https://refeds.org/profile/mfa` and `http://schemas.microsoft.com/claims/multipleauthn`
```

### Comparing `perun.proxygui-5.2.1/perun.proxygui.egg-info/SOURCES.txt` & `perun.proxygui-6.0.0/perun.proxygui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/perun.proxygui.egg-info/requires.txt` & `perun.proxygui-6.0.0/perun.proxygui.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.2.1/setup.py` & `perun.proxygui-6.0.0/setup.py`

 * *Files identical despite different names*

