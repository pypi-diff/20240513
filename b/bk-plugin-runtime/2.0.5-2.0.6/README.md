# Comparing `tmp/bk-plugin-runtime-2.0.5.tar.gz` & `tmp/bk-plugin-runtime-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk-plugin-runtime-2.0.5.tar", max compression
+gzip compressed data, was "bk-plugin-runtime-2.0.6.tar", max compression
```

## Comparing `bk-plugin-runtime-2.0.5.tar` & `bk-plugin-runtime-2.0.6.tar`

### file list

```diff
@@ -1,278 +1,278 @@
--rw-r--r--   0        0        0      730 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/__init__.py
--rw-r--r--   0        0        0      753 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/__version__.py
--rw-r--r--   0        0        0     1892 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/config/__init__.py
--rw-r--r--   0        0        0     9400 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/config/default.py
--rw-r--r--   0        0        0     3464 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/config/dev.py
--rw-r--r--   0        0        0     1137 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/config/prod.py
--rw-r--r--   0        0        0     1232 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/config/stag.py
--rw-r--r--   0        0        0      951 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/manage.py
--rw-r--r--   0        0        0       53 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/__init__.py
--rw-r--r--   0        0        0     2177 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/README.md
--rw-r--r--   0        0        0       24 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/__init__.py
--rw-r--r--   0        0        0       24 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/__init__.py
--rw-r--r--   0        0        0     1293 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/bk_login.py
--rw-r--r--   0        0        0      405 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/bk_paas.py
--rw-r--r--   0        0        0    29361 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/cc.py
--rw-r--r--   0        0        0     1865 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/cmsi.py
--rw-r--r--   0        0        0     1341 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/gse.py
--rw-r--r--   0        0        0     2333 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/itsm.py
--rw-r--r--   0        0        0     6053 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/job.py
--rw-r--r--   0        0        0     5864 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/jobv3.py
--rw-r--r--   0        0        0    18432 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/monitor_v3.py
--rw-r--r--   0        0        0     7698 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/sops.py
--rw-r--r--   0        0        0     1916 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/usermanage.py
--rw-r--r--   0        0        0     3914 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/base.py
--rw-r--r--   0        0        0     5219 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/client.py
--rw-r--r--   0        0        0      922 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/collections.py
--rw-r--r--   0        0        0      247 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/compat.py
--rw-r--r--   0        0        0      582 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/conf.py
--rw-r--r--   0        0        0      506 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/exceptions.py
--rw-r--r--   0        0        0     1548 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/shortcuts.py
--rw-r--r--   0        0        0      859 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/utils.py
--rw-r--r--   0        0        0      390 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/tests/README.md
--rw-r--r--   0        0        0        0 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/tests/__init__.py
--rw-r--r--   0        0        0     3298 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/tests/test_client.py
--rw-r--r--   0        0        0     1501 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/tests/test_shortcuts.py
--rw-r--r--   0        0        0      830 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/tests/test_utils.py
--rw-r--r--   0        0        0        0 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/tests/utils/__init__.py
--rw-r--r--   0        0        0      479 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/tests/utils/utils.py
--rw-r--r--   0        0        0     1573 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/settings.py
--rw-r--r--   0        0        0     1684 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/account/login.js
--rw-r--r--   0        0        0    16066 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/base.css
--rw-r--r--   0        0        0     6170 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/changelists.css
--rw-r--r--   0        0        0      412 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/dashboard.css
--rw-r--r--   0        0        0      423 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/fonts.css
--rw-r--r--   0        0        0     8173 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/forms.css
--rw-r--r--   0        0        0     1203 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/login.css
--rw-r--r--   0        0        0     3731 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/rtl.css
--rw-r--r--   0        0        0    10340 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/widgets.css
--rw-r--r--   0        0        0    11358 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/fonts/LICENSE.txt
--rw-r--r--   0        0        0      137 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/fonts/README.txt
--rw-r--r--   0        0        0    82564 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/fonts/Roboto-Bold-webfont.woff
--rw-r--r--   0        0        0    81348 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/fonts/Roboto-Light-webfont.woff
--rw-r--r--   0        0        0    80304 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/fonts/Roboto-Regular-webfont.woff
--rw-r--r--   0        0        0     1081 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/LICENSE
--rw-r--r--   0        0        0      318 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/README.txt
--rw-r--r--   0        0        0     1094 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/calendar-icons.svg
--rw-r--r--   0        0        0     1129 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/gis/move_vertex_off.svg
--rw-r--r--   0        0        0     1129 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/gis/move_vertex_on.svg
--rw-r--r--   0        0        0      331 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-addlink.svg
--rw-r--r--   0        0        0      504 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-alert.svg
--rw-r--r--   0        0        0     1086 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-calendar.svg
--rw-r--r--   0        0        0      380 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-changelink.svg
--rw-r--r--   0        0        0      677 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-clock.svg
--rw-r--r--   0        0        0      392 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-deletelink.svg
--rw-r--r--   0        0        0      560 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-no.svg
--rw-r--r--   0        0        0      655 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-unknown-alt.svg
--rw-r--r--   0        0        0      655 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-unknown.svg
--rw-r--r--   0        0        0      436 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-yes.svg
--rw-r--r--   0        0        0      560 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/inline-delete.svg
--rw-r--r--   0        0        0      458 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/search.svg
--rw-r--r--   0        0        0     3291 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/selector-icons.svg
--rw-r--r--   0        0        0     1097 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/sorting-icons.svg
--rw-r--r--   0        0        0      331 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/tooltag-add.svg
--rw-r--r--   0        0        0      280 2023-12-07 11:43:43.771468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/tooltag-arrowright.svg
--rw-r--r--   0        0        0     5755 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/SelectBox.js
--rw-r--r--   0        0        0    12389 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/SelectFilter2.js
--rw-r--r--   0        0        0     6501 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/actions.js
--rw-r--r--   0        0        0     3162 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/actions.min.js
--rw-r--r--   0        0        0    20529 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/admin/DateTimeShortcuts.js
--rw-r--r--   0        0        0     6591 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/admin/RelatedObjectLookups.js
--rw-r--r--   0        0        0     7790 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/calendar.js
--rw-r--r--   0        0        0      204 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/cancel.js
--rw-r--r--   0        0        0      712 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/change_form.js
--rw-r--r--   0        0        0     1151 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/collapse.js
--rw-r--r--   0        0        0      649 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/collapse.min.js
--rw-r--r--   0        0        0     7976 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/core.js
--rw-r--r--   0        0        0    13665 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/inlines.js
--rw-r--r--   0        0        0     4831 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/inlines.min.js
--rw-r--r--   0        0        0      363 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/jquery.init.js
--rw-r--r--   0        0        0      569 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/popup_response.js
--rw-r--r--   0        0        0     1538 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/prepopulate.js
--rw-r--r--   0        0        0      372 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/prepopulate.min.js
--rw-r--r--   0        0        0      495 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/prepopulate_init.js
--rw-r--r--   0        0        0     2984 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/timeparse.js
--rw-r--r--   0        0        0     8186 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/urlify.js
--rw-r--r--   0        0        0     1282 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/vendor/jquery/LICENSE-JQUERY.txt
--rw-r--r--   0        0        0   258648 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/vendor/jquery/jquery.js
--rw-r--r--   0        0        0    85659 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/vendor/jquery/jquery.min.js
--rw-r--r--   0        0        0     1103 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/vendor/xregexp/LICENSE-XREGEXP.txt
--rw-r--r--   0        0        0   128820 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/vendor/xregexp/xregexp.js
--rw-r--r--   0        0        0    62474 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/vendor/xregexp/xregexp.min.js
--rw-r--r--   0        0        0     5171 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/css/5.ae7e5a9.css
--rw-r--r--   0        0        0      129 2023-12-07 11:43:43.775468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/css/6.b5b1595.css
--rw-r--r--   0        0        0   664641 2023-12-07 11:43:43.779468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/css/app.1acbc76.css
--rw-r--r--   0        0        0    56484 2023-12-07 11:43:43.779468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/fonts/codicon.a609dc0.ttf
--rw-r--r--   0        0        0    28200 2023-12-07 11:43:43.779468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/fonts/element-icons.535877f.woff
--rw-r--r--   0        0        0    55956 2023-12-07 11:43:43.779468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/fonts/element-icons.732389d.ttf
--rw-r--r--   0        0        0    25264 2023-12-07 11:43:43.779468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/fonts/iconcool.73b7ae4.woff
--rw-r--r--   0        0        0    49544 2023-12-07 11:43:43.779468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/fonts/iconcool.92e669c.eot
--rw-r--r--   0        0        0    49376 2023-12-07 11:43:43.779468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/fonts/iconcool.99a84d9.ttf
--rw-r--r--   0        0        0   205924 2023-12-07 11:43:43.779468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/img/iconcool.3a0bc10.svg
--rw-r--r--   0        0        0      769 2023-12-07 11:43:43.779468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/index.html
--rw-r--r--   0        0        0     5129 2023-12-07 11:43:43.779468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/0.6f48290.js
--rw-r--r--   0        0        0   108134 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/10.ef732e8.js
--rw-r--r--   0        0        0     5311 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/11.bb40970.js
--rw-r--r--   0        0        0     3979 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/12.026ec67.js
--rw-r--r--   0        0        0      856 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/13.2df68e4.js
--rw-r--r--   0        0        0     1855 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/14.163c19b.js
--rw-r--r--   0        0        0     2047 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/15.9cceaac.js
--rw-r--r--   0        0        0     9651 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/16.7831443.js
--rw-r--r--   0        0        0     3600 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/17.d898c63.js
--rw-r--r--   0        0        0     4545 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/18.252413c.js
--rw-r--r--   0        0        0     1429 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/19.d8557b5.js
--rw-r--r--   0        0        0     4497 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/20.3cd824a.js
--rw-r--r--   0        0        0     1844 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/21.9bbb4b1.js
--rw-r--r--   0        0        0     2991 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/22.3386c8f.js
--rw-r--r--   0        0        0     2665 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/23.a8df42e.js
--rw-r--r--   0        0        0     2268 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/24.11efd4d.js
--rw-r--r--   0        0        0     6170 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/25.e926bde.js
--rw-r--r--   0        0        0     4554 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/26.5a0e1a2.js
--rw-r--r--   0        0        0     1111 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/27.c58f59a.js
--rw-r--r--   0        0        0     2979 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/28.e01b321.js
--rw-r--r--   0        0        0     3447 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/29.15d37be.js
--rw-r--r--   0        0        0     3904 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/30.2db8ef1.js
--rw-r--r--   0        0        0     2131 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/31.7fca48c.js
--rw-r--r--   0        0        0     3807 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/32.e08e913.js
--rw-r--r--   0        0        0     2587 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/33.c35bad7.js
--rw-r--r--   0        0        0     4922 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/34.dca80a3.js
--rw-r--r--   0        0        0    14506 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/35.e6d327b.js
--rw-r--r--   0        0        0     2410 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/36.5227523.js
--rw-r--r--   0        0        0     2994 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/37.1e2646a.js
--rw-r--r--   0        0        0     2008 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/38.5d6a58b.js
--rw-r--r--   0        0        0     8263 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/39.ad974a2.js
--rw-r--r--   0        0        0    23036 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/4.b54f74b.js
--rw-r--r--   0        0        0    17638 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/40.8b7f991.js
--rw-r--r--   0        0        0     8035 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/41.3534381.js
--rw-r--r--   0        0        0     7864 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/42.5c565de.js
--rw-r--r--   0        0        0    16947 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/43.7ee2459.js
--rw-r--r--   0        0        0     3277 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/44.6635592.js
--rw-r--r--   0        0        0     4838 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/45.1853c81.js
--rw-r--r--   0        0        0     3250 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/46.6767649.js
--rw-r--r--   0        0        0     2843 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/47.c0bc734.js
--rw-r--r--   0        0        0     8458 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/48.487d563.js
--rw-r--r--   0        0        0     3564 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/49.c3f1524.js
--rw-r--r--   0        0        0   258432 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/5.cdcdd1a.js
--rw-r--r--   0        0        0    11790 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/50.7ab35af.js
--rw-r--r--   0        0        0     3959 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/51.71cba7d.js
--rw-r--r--   0        0        0     8513 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/52.5c54aa2.js
--rw-r--r--   0        0        0     3932 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/53.c400082.js
--rw-r--r--   0        0        0     1837 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/54.d2b1b7c.js
--rw-r--r--   0        0        0     1777 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/55.2dbca9d.js
--rw-r--r--   0        0        0     6417 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/56.1fb1bd7.js
--rw-r--r--   0        0        0     2936 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/57.7de2a14.js
--rw-r--r--   0        0        0    18605 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/58.f34b8a9.js
--rw-r--r--   0        0        0     2772 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/59.7151d24.js
--rw-r--r--   0        0        0     1094 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/6.1bfd752.js
--rw-r--r--   0        0        0    18247 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/60.b678d5d.js
--rw-r--r--   0        0        0     7394 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/61.b6fd4a6.js
--rw-r--r--   0        0        0     4333 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/62.d223027.js
--rw-r--r--   0        0        0     3581 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/63.cbfa021.js
--rw-r--r--   0        0        0     5986 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/64.d024764.js
--rw-r--r--   0        0        0     5078 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/65.1cb549f.js
--rw-r--r--   0        0        0     5825 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/66.efb2feb.js
--rw-r--r--   0        0        0     1747 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/67.2ce57c6.js
--rw-r--r--   0        0        0     3550 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/68.fd98371.js
--rw-r--r--   0        0        0    22685 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/69.d3dc8a2.js
--rw-r--r--   0        0        0     6025 2023-12-07 11:43:43.783469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/7.11b138a.js
--rw-r--r--   0        0        0   702763 2023-12-07 11:43:43.787469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/8.3d810bf.js
--rw-r--r--   0        0        0   413469 2023-12-07 11:43:43.787469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/9.7d32151.js
--rw-r--r--   0        0        0  5296491 2023-12-07 11:43:43.807469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/app.4115d0f.js
--rw-r--r--   0        0        0     4869 2023-12-07 11:43:43.807469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/runtime.fe89973.js
--rw-r--r--   0        0        0   143318 2023-12-07 11:43:43.807469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/vue-lib.e5e31c4.js
--rw-r--r--   0        0        0       82 2023-12-07 11:43:43.807469 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/djcelery/style.css
--rw-r--r--   0        0        0   126005 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/editor.worker.js
--rw-r--r--   0        0        0      657 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/images/favicon.png
--rw-r--r--   0        0        0     1165 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/js/csrftoken.js
--rw-r--r--   0        0        0     2450 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/js/settings.js
--rw-r--r--   0        0        0   235031 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/json.worker.js
--rw-r--r--   0        0        0   177649 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/css/bk.css
--rw-r--r--   0        0        0   145999 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/css/bootstrap_noresponsive.css
--rw-r--r--   0        0        0     5154 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/css/index.css
--rw-r--r--   0        0        0     1150 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/favicon.ico
--rw-r--r--   0        0        0     1126 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/crown.png
--rw-r--r--   0        0        0    59790 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/dev-guide.png
--rw-r--r--   0        0        0    40979 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/expre_403.png
--rw-r--r--   0        0        0    31582 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/expre_500.png
--rw-r--r--   0        0        0    32117 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/expre_login.png
--rw-r--r--   0        0        0     2300 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/getheadimg.jpg
--rw-r--r--   0        0        0     2037 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/icom_01.png
--rw-r--r--   0        0        0     1997 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/icom_02.png
--rw-r--r--   0        0        0     2142 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/icom_03.png
--rw-r--r--   0        0        0    21926 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/weixin_icom.png
--rw-r--r--   0        0        0       32 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/analysis.js
--rw-r--r--   0        0        0     1288 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/Gruntfile.js
--rw-r--r--   0        0        0     1340 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/LICENSE.md
--rw-r--r--   0        0        0     1992 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/README.md
--rw-r--r--   0        0        0     9929 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/css/ui-dialog.css
--rw-r--r--   0        0        0     9928 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/new/css/artDialog.css
--rw-r--r--   0        0        0    10000 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/new/js/artDialog.min.js
--rw-r--r--   0        0        0      650 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/package.json
--rw-r--r--   0        0        0    16359 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artdialog/jquery.artDialog.js
--rw-r--r--   0        0        0      381 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artdialog/skins/icons/loading.gif
--rw-r--r--   0        0        0     5951 2023-12-07 11:43:43.811468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artdialog/skins/simple.css
--rw-r--r--   0        0        0    93432 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/jquery/jquery-1.7.2.min.js
--rw-r--r--   0        0        0     2177 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/jquery/jquery.json-2.3.min.js
--rw-r--r--   0        0        0    22608 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap-theme.css
--rw-r--r--   0        0        0    43339 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap-theme.css.map
--rw-r--r--   0        0        0    19963 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap-theme.min.css
--rw-r--r--   0        0        0   141622 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap.css
--rw-r--r--   0        0        0   380986 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap.css.map
--rw-r--r--   0        0        0   117305 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap.min.css
--rw-r--r--   0        0        0   146000 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap_noresponsive.css
--rw-r--r--   0        0        0        0 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0        0        0   108738 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0        0        0        0 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0        0        0        0 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0        0        0        0 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0        0        0    11614 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/bootstrap-treeview.js
--rw-r--r--   0        0        0    67546 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/bootstrap.js
--rw-r--r--   0        0        0    35951 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/bootstrap.min.js
--rw-r--r--   0        0        0      484 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/npm.js
--rw-r--r--   0        0        0   273199 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/external/jquery/jquery.js
--rw-r--r--   0        0        0     1738 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/animated-overlay.gif
--rw-r--r--   0        0        0      418 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_diagonals-thick_18_b81900_40x40.png
--rw-r--r--   0        0        0      312 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_diagonals-thick_20_666666_40x40.png
--rw-r--r--   0        0        0      205 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_flat_10_000000_40x100.png
--rw-r--r--   0        0        0      247 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_flat_75_ffffff_40x100.png
--rw-r--r--   0        0        0      262 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_glass_100_f6f6f6_1x400.png
--rw-r--r--   0        0        0      348 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_glass_100_fdf5ce_1x400.png
--rw-r--r--   0        0        0      246 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0        0        0      246 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0        0        0      301 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0        0        0      301 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0        0        0     5815 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_gloss-wave_35_f6a828_500x100.png
--rw-r--r--   0        0        0      278 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_highlight-soft_100_eeeeee_1x100.png
--rw-r--r--   0        0        0      319 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0        0        0      328 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_highlight-soft_75_ffe45c_1x100.png
--rw-r--r--   0        0        0     6922 2023-12-07 11:43:43.815468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4549 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_228ef1_256x240.png
--rw-r--r--   0        0        0     7071 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     7092 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_888888_256x240.png
--rw-r--r--   0        0        0     4549 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_ef8c08_256x240.png
--rw-r--r--   0        0        0     4549 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_ffd27a_256x240.png
--rw-r--r--   0        0        0     6299 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    31712 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/index.html
--rw-r--r--   0        0        0    32704 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.css
--rw-r--r--   0        0        0   461387 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.js
--rw-r--r--   0        0        0    27848 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.min.css
--rw-r--r--   0        0        0   237548 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.min.js
--rw-r--r--   0        0        0    15663 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.structure.css
--rw-r--r--   0        0        0    12454 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.structure.min.css
--rw-r--r--   0        0        0    17339 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.theme.css
--rw-r--r--   0        0        0    13868 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.theme.min.css
--rw-r--r--   0        0        0    93107 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/js/jquery-1.10.2.min.js
--rw-r--r--   0        0        0     7199 2023-12-07 11:43:43.819468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/js/jquery-migrate-1.2.1.min.js
--rw-r--r--   0        0        0   149031 2023-12-07 11:43:43.823468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/bk/css/bk.css
--rw-r--r--   0        0        0        0 2023-12-07 11:43:43.823468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/bk/js/bk.js
--rw-r--r--   0        0        0      375 2023-12-07 11:43:43.823468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/templates/403.html
--rw-r--r--   0        0        0      369 2023-12-07 11:43:43.823468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/templates/500.html
--rw-r--r--   0        0        0      234 2023-12-07 11:43:43.823468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/templates/admin/base_site.html
--rw-r--r--   0        0        0      848 2023-12-07 11:43:43.823468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/templates/admin/login.html
--rw-r--r--   0        0        0     7373 2023-12-07 11:43:43.823468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/templates/base.html
--rw-r--r--   0        0        0      769 2023-12-07 11:43:43.823468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/templates/debug_panel.html
--rw-r--r--   0        0        0     2047 2023-12-07 11:43:43.823468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/urls.py
--rw-r--r--   0        0        0      893 2023-12-07 11:43:43.823468 bk-plugin-runtime-2.0.5/bk_plugin_runtime/wsgi.py
--rw-r--r--   0        0        0      875 2023-12-07 11:43:43.823468 bk-plugin-runtime-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     3510 2023-12-07 11:43:59.256717 bk-plugin-runtime-2.0.5/setup.py
--rw-r--r--   0        0        0     1169 2023-12-07 11:43:59.257001 bk-plugin-runtime-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0      730 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/__init__.py
+-rw-r--r--   0        0        0      753 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/__version__.py
+-rw-r--r--   0        0        0     1892 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/config/__init__.py
+-rw-r--r--   0        0        0     9460 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/config/default.py
+-rw-r--r--   0        0        0     3464 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/config/dev.py
+-rw-r--r--   0        0        0     1137 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/config/prod.py
+-rw-r--r--   0        0        0     1232 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/config/stag.py
+-rw-r--r--   0        0        0      951 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/manage.py
+-rw-r--r--   0        0        0       53 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/__init__.py
+-rw-r--r--   0        0        0     2177 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/README.md
+-rw-r--r--   0        0        0       24 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/__init__.py
+-rw-r--r--   0        0        0     1293 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/bk_login.py
+-rw-r--r--   0        0        0      405 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/bk_paas.py
+-rw-r--r--   0        0        0    29361 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/cc.py
+-rw-r--r--   0        0        0     1865 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/cmsi.py
+-rw-r--r--   0        0        0     1341 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/gse.py
+-rw-r--r--   0        0        0     2333 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/itsm.py
+-rw-r--r--   0        0        0     6053 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/job.py
+-rw-r--r--   0        0        0     5864 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/jobv3.py
+-rw-r--r--   0        0        0    18432 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/monitor_v3.py
+-rw-r--r--   0        0        0     7698 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/sops.py
+-rw-r--r--   0        0        0     1916 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/usermanage.py
+-rw-r--r--   0        0        0     3914 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/base.py
+-rw-r--r--   0        0        0     5219 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/client.py
+-rw-r--r--   0        0        0      922 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/collections.py
+-rw-r--r--   0        0        0      247 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/compat.py
+-rw-r--r--   0        0        0      582 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/conf.py
+-rw-r--r--   0        0        0      506 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/exceptions.py
+-rw-r--r--   0        0        0     1548 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/shortcuts.py
+-rw-r--r--   0        0        0      859 2024-05-13 11:54:36.675370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/utils.py
+-rw-r--r--   0        0        0      390 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/tests/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/tests/__init__.py
+-rw-r--r--   0        0        0     3298 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/tests/test_client.py
+-rw-r--r--   0        0        0     1501 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/tests/test_shortcuts.py
+-rw-r--r--   0        0        0      830 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/tests/utils/__init__.py
+-rw-r--r--   0        0        0      479 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/tests/utils/utils.py
+-rw-r--r--   0        0        0     1573 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/settings.py
+-rw-r--r--   0        0        0     1684 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/account/login.js
+-rw-r--r--   0        0        0    16066 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/base.css
+-rw-r--r--   0        0        0     6170 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/changelists.css
+-rw-r--r--   0        0        0      412 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/dashboard.css
+-rw-r--r--   0        0        0      423 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/fonts.css
+-rw-r--r--   0        0        0     8173 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/forms.css
+-rw-r--r--   0        0        0     1203 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/login.css
+-rw-r--r--   0        0        0     3731 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/rtl.css
+-rw-r--r--   0        0        0    10340 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/widgets.css
+-rw-r--r--   0        0        0    11358 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/fonts/LICENSE.txt
+-rw-r--r--   0        0        0      137 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/fonts/README.txt
+-rw-r--r--   0        0        0    82564 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/fonts/Roboto-Bold-webfont.woff
+-rw-r--r--   0        0        0    81348 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/fonts/Roboto-Light-webfont.woff
+-rw-r--r--   0        0        0    80304 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/fonts/Roboto-Regular-webfont.woff
+-rw-r--r--   0        0        0     1081 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/LICENSE
+-rw-r--r--   0        0        0      318 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/README.txt
+-rw-r--r--   0        0        0     1094 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/calendar-icons.svg
+-rw-r--r--   0        0        0     1129 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/gis/move_vertex_off.svg
+-rw-r--r--   0        0        0     1129 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/gis/move_vertex_on.svg
+-rw-r--r--   0        0        0      331 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-addlink.svg
+-rw-r--r--   0        0        0      504 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-alert.svg
+-rw-r--r--   0        0        0     1086 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-calendar.svg
+-rw-r--r--   0        0        0      380 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-changelink.svg
+-rw-r--r--   0        0        0      677 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-clock.svg
+-rw-r--r--   0        0        0      392 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-deletelink.svg
+-rw-r--r--   0        0        0      560 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-no.svg
+-rw-r--r--   0        0        0      655 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-unknown-alt.svg
+-rw-r--r--   0        0        0      655 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-unknown.svg
+-rw-r--r--   0        0        0      436 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-yes.svg
+-rw-r--r--   0        0        0      560 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/inline-delete.svg
+-rw-r--r--   0        0        0      458 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/search.svg
+-rw-r--r--   0        0        0     3291 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/selector-icons.svg
+-rw-r--r--   0        0        0     1097 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/sorting-icons.svg
+-rw-r--r--   0        0        0      331 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/tooltag-add.svg
+-rw-r--r--   0        0        0      280 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/tooltag-arrowright.svg
+-rw-r--r--   0        0        0     5755 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/SelectBox.js
+-rw-r--r--   0        0        0    12389 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/SelectFilter2.js
+-rw-r--r--   0        0        0     6501 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/actions.js
+-rw-r--r--   0        0        0     3162 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/actions.min.js
+-rw-r--r--   0        0        0    20529 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/admin/DateTimeShortcuts.js
+-rw-r--r--   0        0        0     6591 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/admin/RelatedObjectLookups.js
+-rw-r--r--   0        0        0     7790 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/calendar.js
+-rw-r--r--   0        0        0      204 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/cancel.js
+-rw-r--r--   0        0        0      712 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/change_form.js
+-rw-r--r--   0        0        0     1151 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/collapse.js
+-rw-r--r--   0        0        0      649 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/collapse.min.js
+-rw-r--r--   0        0        0     7976 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/core.js
+-rw-r--r--   0        0        0    13665 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/inlines.js
+-rw-r--r--   0        0        0     4831 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/inlines.min.js
+-rw-r--r--   0        0        0      363 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/jquery.init.js
+-rw-r--r--   0        0        0      569 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/popup_response.js
+-rw-r--r--   0        0        0     1538 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/prepopulate.js
+-rw-r--r--   0        0        0      372 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/prepopulate.min.js
+-rw-r--r--   0        0        0      495 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/prepopulate_init.js
+-rw-r--r--   0        0        0     2984 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/timeparse.js
+-rw-r--r--   0        0        0     8186 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/urlify.js
+-rw-r--r--   0        0        0     1282 2024-05-13 11:54:36.679370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/vendor/jquery/LICENSE-JQUERY.txt
+-rw-r--r--   0        0        0   258648 2024-05-13 11:54:36.683370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/vendor/jquery/jquery.js
+-rw-r--r--   0        0        0    85659 2024-05-13 11:54:36.683370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/vendor/jquery/jquery.min.js
+-rw-r--r--   0        0        0     1103 2024-05-13 11:54:36.683370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/vendor/xregexp/LICENSE-XREGEXP.txt
+-rw-r--r--   0        0        0   128820 2024-05-13 11:54:36.683370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/vendor/xregexp/xregexp.js
+-rw-r--r--   0        0        0    62474 2024-05-13 11:54:36.683370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/vendor/xregexp/xregexp.min.js
+-rw-r--r--   0        0        0     5171 2024-05-13 11:54:36.683370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/css/5.ae7e5a9.css
+-rw-r--r--   0        0        0      129 2024-05-13 11:54:36.683370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/css/6.b5b1595.css
+-rw-r--r--   0        0        0   664641 2024-05-13 11:54:36.683370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/css/app.1acbc76.css
+-rw-r--r--   0        0        0    56484 2024-05-13 11:54:36.683370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/fonts/codicon.a609dc0.ttf
+-rw-r--r--   0        0        0    28200 2024-05-13 11:54:36.683370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/fonts/element-icons.535877f.woff
+-rw-r--r--   0        0        0    55956 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/fonts/element-icons.732389d.ttf
+-rw-r--r--   0        0        0    25264 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/fonts/iconcool.73b7ae4.woff
+-rw-r--r--   0        0        0    49544 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/fonts/iconcool.92e669c.eot
+-rw-r--r--   0        0        0    49376 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/fonts/iconcool.99a84d9.ttf
+-rw-r--r--   0        0        0   205924 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/img/iconcool.3a0bc10.svg
+-rw-r--r--   0        0        0      769 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/index.html
+-rw-r--r--   0        0        0     5129 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/0.6f48290.js
+-rw-r--r--   0        0        0   108134 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/10.ef732e8.js
+-rw-r--r--   0        0        0     5311 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/11.bb40970.js
+-rw-r--r--   0        0        0     3979 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/12.026ec67.js
+-rw-r--r--   0        0        0      856 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/13.2df68e4.js
+-rw-r--r--   0        0        0     1855 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/14.163c19b.js
+-rw-r--r--   0        0        0     2047 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/15.9cceaac.js
+-rw-r--r--   0        0        0     9651 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/16.7831443.js
+-rw-r--r--   0        0        0     3600 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/17.d898c63.js
+-rw-r--r--   0        0        0     4545 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/18.252413c.js
+-rw-r--r--   0        0        0     1429 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/19.d8557b5.js
+-rw-r--r--   0        0        0     4497 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/20.3cd824a.js
+-rw-r--r--   0        0        0     1844 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/21.9bbb4b1.js
+-rw-r--r--   0        0        0     2991 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/22.3386c8f.js
+-rw-r--r--   0        0        0     2665 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/23.a8df42e.js
+-rw-r--r--   0        0        0     2268 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/24.11efd4d.js
+-rw-r--r--   0        0        0     6170 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/25.e926bde.js
+-rw-r--r--   0        0        0     4554 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/26.5a0e1a2.js
+-rw-r--r--   0        0        0     1111 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/27.c58f59a.js
+-rw-r--r--   0        0        0     2979 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/28.e01b321.js
+-rw-r--r--   0        0        0     3447 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/29.15d37be.js
+-rw-r--r--   0        0        0     3904 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/30.2db8ef1.js
+-rw-r--r--   0        0        0     2131 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/31.7fca48c.js
+-rw-r--r--   0        0        0     3807 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/32.e08e913.js
+-rw-r--r--   0        0        0     2587 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/33.c35bad7.js
+-rw-r--r--   0        0        0     4922 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/34.dca80a3.js
+-rw-r--r--   0        0        0    14506 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/35.e6d327b.js
+-rw-r--r--   0        0        0     2410 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/36.5227523.js
+-rw-r--r--   0        0        0     2994 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/37.1e2646a.js
+-rw-r--r--   0        0        0     2008 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/38.5d6a58b.js
+-rw-r--r--   0        0        0     8263 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/39.ad974a2.js
+-rw-r--r--   0        0        0    23036 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/4.b54f74b.js
+-rw-r--r--   0        0        0    17638 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/40.8b7f991.js
+-rw-r--r--   0        0        0     8035 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/41.3534381.js
+-rw-r--r--   0        0        0     7864 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/42.5c565de.js
+-rw-r--r--   0        0        0    16947 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/43.7ee2459.js
+-rw-r--r--   0        0        0     3277 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/44.6635592.js
+-rw-r--r--   0        0        0     4838 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/45.1853c81.js
+-rw-r--r--   0        0        0     3250 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/46.6767649.js
+-rw-r--r--   0        0        0     2843 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/47.c0bc734.js
+-rw-r--r--   0        0        0     8458 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/48.487d563.js
+-rw-r--r--   0        0        0     3564 2024-05-13 11:54:36.687370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/49.c3f1524.js
+-rw-r--r--   0        0        0   258432 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/5.cdcdd1a.js
+-rw-r--r--   0        0        0    11790 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/50.7ab35af.js
+-rw-r--r--   0        0        0     3959 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/51.71cba7d.js
+-rw-r--r--   0        0        0     8513 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/52.5c54aa2.js
+-rw-r--r--   0        0        0     3932 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/53.c400082.js
+-rw-r--r--   0        0        0     1837 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/54.d2b1b7c.js
+-rw-r--r--   0        0        0     1777 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/55.2dbca9d.js
+-rw-r--r--   0        0        0     6417 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/56.1fb1bd7.js
+-rw-r--r--   0        0        0     2936 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/57.7de2a14.js
+-rw-r--r--   0        0        0    18605 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/58.f34b8a9.js
+-rw-r--r--   0        0        0     2772 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/59.7151d24.js
+-rw-r--r--   0        0        0     1094 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/6.1bfd752.js
+-rw-r--r--   0        0        0    18247 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/60.b678d5d.js
+-rw-r--r--   0        0        0     7394 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/61.b6fd4a6.js
+-rw-r--r--   0        0        0     4333 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/62.d223027.js
+-rw-r--r--   0        0        0     3581 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/63.cbfa021.js
+-rw-r--r--   0        0        0     5986 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/64.d024764.js
+-rw-r--r--   0        0        0     5078 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/65.1cb549f.js
+-rw-r--r--   0        0        0     5825 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/66.efb2feb.js
+-rw-r--r--   0        0        0     1747 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/67.2ce57c6.js
+-rw-r--r--   0        0        0     3550 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/68.fd98371.js
+-rw-r--r--   0        0        0    22685 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/69.d3dc8a2.js
+-rw-r--r--   0        0        0     6025 2024-05-13 11:54:36.691370 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/7.11b138a.js
+-rw-r--r--   0        0        0   702763 2024-05-13 11:54:36.695371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/8.3d810bf.js
+-rw-r--r--   0        0        0   413469 2024-05-13 11:54:36.695371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/9.7d32151.js
+-rw-r--r--   0        0        0  5296491 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/app.4115d0f.js
+-rw-r--r--   0        0        0     4869 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/runtime.fe89973.js
+-rw-r--r--   0        0        0   143318 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/vue-lib.e5e31c4.js
+-rw-r--r--   0        0        0       82 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/djcelery/style.css
+-rw-r--r--   0        0        0   126005 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/editor.worker.js
+-rw-r--r--   0        0        0      657 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/images/favicon.png
+-rw-r--r--   0        0        0     1165 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/js/csrftoken.js
+-rw-r--r--   0        0        0     2450 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/js/settings.js
+-rw-r--r--   0        0        0   235031 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/json.worker.js
+-rw-r--r--   0        0        0   177649 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/css/bk.css
+-rw-r--r--   0        0        0   145999 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/css/bootstrap_noresponsive.css
+-rw-r--r--   0        0        0     5154 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/css/index.css
+-rw-r--r--   0        0        0     1150 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/favicon.ico
+-rw-r--r--   0        0        0     1126 2024-05-13 11:54:36.715371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/crown.png
+-rw-r--r--   0        0        0    59790 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/dev-guide.png
+-rw-r--r--   0        0        0    40979 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/expre_403.png
+-rw-r--r--   0        0        0    31582 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/expre_500.png
+-rw-r--r--   0        0        0    32117 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/expre_login.png
+-rw-r--r--   0        0        0     2300 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/getheadimg.jpg
+-rw-r--r--   0        0        0     2037 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/icom_01.png
+-rw-r--r--   0        0        0     1997 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/icom_02.png
+-rw-r--r--   0        0        0     2142 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/icom_03.png
+-rw-r--r--   0        0        0    21926 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/weixin_icom.png
+-rw-r--r--   0        0        0       32 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/analysis.js
+-rw-r--r--   0        0        0     1288 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/Gruntfile.js
+-rw-r--r--   0        0        0     1340 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/LICENSE.md
+-rw-r--r--   0        0        0     1992 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/README.md
+-rw-r--r--   0        0        0     9929 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/css/ui-dialog.css
+-rw-r--r--   0        0        0     9928 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/new/css/artDialog.css
+-rw-r--r--   0        0        0    10000 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/new/js/artDialog.min.js
+-rw-r--r--   0        0        0      650 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/package.json
+-rw-r--r--   0        0        0    16359 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artdialog/jquery.artDialog.js
+-rw-r--r--   0        0        0      381 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artdialog/skins/icons/loading.gif
+-rw-r--r--   0        0        0     5951 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artdialog/skins/simple.css
+-rw-r--r--   0        0        0    93432 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/jquery/jquery-1.7.2.min.js
+-rw-r--r--   0        0        0     2177 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/jquery/jquery.json-2.3.min.js
+-rw-r--r--   0        0        0    22608 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap-theme.css
+-rw-r--r--   0        0        0    43339 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap-theme.css.map
+-rw-r--r--   0        0        0    19963 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap-theme.min.css
+-rw-r--r--   0        0        0   141622 2024-05-13 11:54:36.719371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap.css
+-rw-r--r--   0        0        0   380986 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap.css.map
+-rw-r--r--   0        0        0   117305 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap.min.css
+-rw-r--r--   0        0        0   146000 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap_noresponsive.css
+-rw-r--r--   0        0        0        0 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0        0        0   108738 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0        0        0        0 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0        0 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0        0 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0        0        0    11614 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/bootstrap-treeview.js
+-rw-r--r--   0        0        0    67546 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/bootstrap.js
+-rw-r--r--   0        0        0    35951 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/bootstrap.min.js
+-rw-r--r--   0        0        0      484 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/npm.js
+-rw-r--r--   0        0        0   273199 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/external/jquery/jquery.js
+-rw-r--r--   0        0        0     1738 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/animated-overlay.gif
+-rw-r--r--   0        0        0      418 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_diagonals-thick_18_b81900_40x40.png
+-rw-r--r--   0        0        0      312 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_diagonals-thick_20_666666_40x40.png
+-rw-r--r--   0        0        0      205 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_flat_10_000000_40x100.png
+-rw-r--r--   0        0        0      247 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_flat_75_ffffff_40x100.png
+-rw-r--r--   0        0        0      262 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_glass_100_f6f6f6_1x400.png
+-rw-r--r--   0        0        0      348 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_glass_100_fdf5ce_1x400.png
+-rw-r--r--   0        0        0      246 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0        0        0      246 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0        0        0      301 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0        0        0      301 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0        0        0     5815 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_gloss-wave_35_f6a828_500x100.png
+-rw-r--r--   0        0        0      278 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_highlight-soft_100_eeeeee_1x100.png
+-rw-r--r--   0        0        0      319 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0        0        0      328 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_highlight-soft_75_ffe45c_1x100.png
+-rw-r--r--   0        0        0     6922 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_222222_256x240.png
+-rw-r--r--   0        0        0     4549 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_228ef1_256x240.png
+-rw-r--r--   0        0        0     7071 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_454545_256x240.png
+-rw-r--r--   0        0        0     7092 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_888888_256x240.png
+-rw-r--r--   0        0        0     4549 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_ef8c08_256x240.png
+-rw-r--r--   0        0        0     4549 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_ffd27a_256x240.png
+-rw-r--r--   0        0        0     6299 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    31712 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/index.html
+-rw-r--r--   0        0        0    32704 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.css
+-rw-r--r--   0        0        0   461387 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.js
+-rw-r--r--   0        0        0    27848 2024-05-13 11:54:36.723371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.min.css
+-rw-r--r--   0        0        0   237548 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.min.js
+-rw-r--r--   0        0        0    15663 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.structure.css
+-rw-r--r--   0        0        0    12454 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.structure.min.css
+-rw-r--r--   0        0        0    17339 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.theme.css
+-rw-r--r--   0        0        0    13868 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.theme.min.css
+-rw-r--r--   0        0        0    93107 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/js/jquery-1.10.2.min.js
+-rw-r--r--   0        0        0     7199 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/js/jquery-migrate-1.2.1.min.js
+-rw-r--r--   0        0        0   149031 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/bk/css/bk.css
+-rw-r--r--   0        0        0        0 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/bk/js/bk.js
+-rw-r--r--   0        0        0      375 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/templates/403.html
+-rw-r--r--   0        0        0      369 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/templates/500.html
+-rw-r--r--   0        0        0      234 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/templates/admin/base_site.html
+-rw-r--r--   0        0        0      848 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/templates/admin/login.html
+-rw-r--r--   0        0        0     7373 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/templates/base.html
+-rw-r--r--   0        0        0      769 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/templates/debug_panel.html
+-rw-r--r--   0        0        0     2047 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/urls.py
+-rw-r--r--   0        0        0      893 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/bk_plugin_runtime/wsgi.py
+-rw-r--r--   0        0        0      891 2024-05-13 11:54:36.727371 bk-plugin-runtime-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3498 2024-05-13 11:54:52.098238 bk-plugin-runtime-2.0.6/setup.py
+-rw-r--r--   0        0        0     1107 2024-05-13 11:54:52.098517 bk-plugin-runtime-2.0.6/PKG-INFO
```

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/__init__.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/__version__.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
```

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/config/__init__.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/config/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/config/default.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/config/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,11 +237,12 @@
 
 BK_PLUGIN_APIGW_BACKEND_HOST = json.loads(os.getenv("BKPAAS_DEFAULT_PREALLOCATED_URLS", "{}")).get(
     BKPAAS_ENVIRONMENT, ""
 )
 url_parse = urllib.parse.urlparse(BK_PLUGIN_APIGW_BACKEND_HOST)
 BK_PLUGIN_APIGW_BACKEND_NETLOC = url_parse.netloc
 BK_PLUGIN_APIGW_BACKEND_SUB_PATH = url_parse.path.lstrip("/")
+BK_PLUGIN_APIGW_BACKEND_SCHEME = url_parse.scheme or "http"
 
 BK_APIGW_CORS_ALLOW_ORIGINS = [s for s in os.getenv("BK_APIGW_CORS_ALLOW_ORIGINS", "").split(",") if s]
 BK_APIGW_CORS_ALLOW_METHODS = [s for s in os.getenv("BK_APIGW_CORS_ALLOW_METHODS", "").split(",") if s]
 BK_APIGW_CORS_ALLOW_HEADERS = [s for s in os.getenv("BK_APIGW_CORS_ALLOW_HEADERS", "").split(",") if s]
```

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/config/dev.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/config/dev.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/config/prod.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/config/prod.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/config/stag.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/config/stag.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/manage.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/manage.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/README.md` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/README.md`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/bk_login.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/bk_login.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/cc.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/cc.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/cmsi.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/cmsi.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/gse.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/gse.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/itsm.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/itsm.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/job.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/job.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/jobv3.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/jobv3.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/monitor_v3.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/monitor_v3.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/sops.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/sops.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/apis/usermanage.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/apis/usermanage.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/base.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/base.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/client.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/client.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/collections.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/collections.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/conf.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/conf.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/shortcuts.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/component/utils.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/component/utils.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/tests/test_client.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/tests/test_shortcuts.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/packages/open/blueking/tests/test_utils.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/packages/open/blueking/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/settings.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/settings.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/account/login.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/account/login.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/base.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/base.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/changelists.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/changelists.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/forms.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/forms.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/login.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/login.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/rtl.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/rtl.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/css/widgets.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/css/widgets.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/fonts/LICENSE.txt` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/fonts/Roboto-Bold-webfont.woff` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/fonts/Roboto-Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/fonts/Roboto-Light-webfont.woff` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/fonts/Roboto-Light-webfont.woff`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/fonts/Roboto-Regular-webfont.woff` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/fonts/Roboto-Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/LICENSE` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/LICENSE`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/calendar-icons.svg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/calendar-icons.svg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/gis/move_vertex_off.svg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/gis/move_vertex_off.svg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/gis/move_vertex_on.svg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/gis/move_vertex_on.svg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-calendar.svg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-calendar.svg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-clock.svg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-clock.svg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-no.svg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-no.svg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-unknown-alt.svg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-unknown-alt.svg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/icon-unknown.svg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/icon-unknown.svg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/inline-delete.svg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/inline-delete.svg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/selector-icons.svg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/selector-icons.svg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/img/sorting-icons.svg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/img/sorting-icons.svg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/SelectBox.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/SelectBox.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/SelectFilter2.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/SelectFilter2.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/actions.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/actions.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/actions.min.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/actions.min.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/admin/DateTimeShortcuts.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/admin/DateTimeShortcuts.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/admin/RelatedObjectLookups.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/admin/RelatedObjectLookups.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/calendar.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/calendar.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/change_form.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/change_form.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/collapse.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/collapse.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/collapse.min.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/collapse.min.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/core.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/core.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/inlines.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/inlines.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/inlines.min.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/inlines.min.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/popup_response.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/popup_response.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/prepopulate.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/prepopulate.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/timeparse.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/timeparse.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/urlify.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/urlify.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/vendor/jquery/LICENSE-JQUERY.txt` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/vendor/jquery/LICENSE-JQUERY.txt`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/vendor/jquery/jquery.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/vendor/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/vendor/jquery/jquery.min.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/vendor/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/vendor/xregexp/LICENSE-XREGEXP.txt` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/vendor/xregexp/LICENSE-XREGEXP.txt`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/vendor/xregexp/xregexp.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/vendor/xregexp/xregexp.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/admin/js/vendor/xregexp/xregexp.min.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/admin/js/vendor/xregexp/xregexp.min.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/css/5.ae7e5a9.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/css/5.ae7e5a9.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/css/app.1acbc76.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/css/app.1acbc76.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/fonts/codicon.a609dc0.ttf` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/fonts/codicon.a609dc0.ttf`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/fonts/element-icons.535877f.woff` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/fonts/element-icons.535877f.woff`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/fonts/element-icons.732389d.ttf` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/fonts/element-icons.732389d.ttf`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/fonts/iconcool.73b7ae4.woff` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/fonts/iconcool.73b7ae4.woff`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/fonts/iconcool.92e669c.eot` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/fonts/iconcool.92e669c.eot`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/fonts/iconcool.99a84d9.ttf` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/fonts/iconcool.99a84d9.ttf`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/img/iconcool.3a0bc10.svg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/img/iconcool.3a0bc10.svg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/index.html` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/index.html`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/0.6f48290.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/0.6f48290.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/10.ef732e8.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/10.ef732e8.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/11.bb40970.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/11.bb40970.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/12.026ec67.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/12.026ec67.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/13.2df68e4.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/13.2df68e4.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/14.163c19b.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/14.163c19b.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/15.9cceaac.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/15.9cceaac.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/16.7831443.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/16.7831443.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/17.d898c63.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/17.d898c63.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/18.252413c.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/18.252413c.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/19.d8557b5.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/19.d8557b5.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/20.3cd824a.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/20.3cd824a.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/21.9bbb4b1.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/21.9bbb4b1.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/22.3386c8f.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/22.3386c8f.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/23.a8df42e.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/23.a8df42e.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/24.11efd4d.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/24.11efd4d.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/25.e926bde.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/25.e926bde.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/26.5a0e1a2.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/26.5a0e1a2.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/27.c58f59a.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/27.c58f59a.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/28.e01b321.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/28.e01b321.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/29.15d37be.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/29.15d37be.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/30.2db8ef1.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/30.2db8ef1.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/31.7fca48c.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/31.7fca48c.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/32.e08e913.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/32.e08e913.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/33.c35bad7.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/33.c35bad7.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/34.dca80a3.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/34.dca80a3.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/35.e6d327b.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/35.e6d327b.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/36.5227523.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/36.5227523.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/37.1e2646a.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/37.1e2646a.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/38.5d6a58b.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/38.5d6a58b.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/39.ad974a2.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/39.ad974a2.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/4.b54f74b.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/4.b54f74b.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/40.8b7f991.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/40.8b7f991.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/41.3534381.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/41.3534381.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/42.5c565de.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/42.5c565de.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/43.7ee2459.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/43.7ee2459.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/44.6635592.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/44.6635592.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/45.1853c81.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/45.1853c81.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/46.6767649.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/46.6767649.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/47.c0bc734.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/47.c0bc734.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/48.487d563.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/48.487d563.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/49.c3f1524.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/49.c3f1524.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/5.cdcdd1a.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/5.cdcdd1a.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/50.7ab35af.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/50.7ab35af.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/51.71cba7d.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/51.71cba7d.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/52.5c54aa2.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/52.5c54aa2.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/53.c400082.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/53.c400082.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/54.d2b1b7c.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/54.d2b1b7c.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/55.2dbca9d.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/55.2dbca9d.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/56.1fb1bd7.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/56.1fb1bd7.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/57.7de2a14.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/57.7de2a14.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/58.f34b8a9.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/58.f34b8a9.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/59.7151d24.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/59.7151d24.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/6.1bfd752.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/6.1bfd752.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/60.b678d5d.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/60.b678d5d.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/61.b6fd4a6.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/61.b6fd4a6.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/62.d223027.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/62.d223027.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/63.cbfa021.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/63.cbfa021.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/64.d024764.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/64.d024764.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/65.1cb549f.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/65.1cb549f.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/66.efb2feb.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/66.efb2feb.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/67.2ce57c6.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/67.2ce57c6.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/68.fd98371.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/68.fd98371.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/69.d3dc8a2.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/69.d3dc8a2.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/7.11b138a.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/7.11b138a.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/8.3d810bf.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/8.3d810bf.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/9.7d32151.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/9.7d32151.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/app.4115d0f.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/app.4115d0f.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/runtime.fe89973.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/runtime.fe89973.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/assets/js/vue-lib.e5e31c4.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/assets/js/vue-lib.e5e31c4.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/editor.worker.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/editor.worker.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/images/favicon.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/js/csrftoken.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/js/csrftoken.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/js/settings.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/js/settings.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/json.worker.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/json.worker.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/css/bk.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/css/bk.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/css/bootstrap_noresponsive.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/css/bootstrap_noresponsive.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/css/index.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/css/index.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/favicon.ico` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/favicon.ico`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/crown.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/crown.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/dev-guide.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/dev-guide.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/expre_403.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/expre_403.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/expre_500.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/expre_500.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/expre_login.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/expre_login.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/getheadimg.jpg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/getheadimg.jpg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/icom_01.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/icom_01.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/icom_02.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/icom_02.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/icom_03.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/icom_03.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/open/img/weixin_icom.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/open/img/weixin_icom.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/Gruntfile.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/LICENSE.md` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/README.md` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/css/ui-dialog.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/css/ui-dialog.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/new/css/artDialog.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/new/css/artDialog.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/new/js/artDialog.min.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/new/js/artDialog.min.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artDialog-6.0.4/package.json` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artDialog-6.0.4/package.json`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artdialog/jquery.artDialog.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artdialog/jquery.artDialog.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/artdialog/skins/simple.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/artdialog/skins/simple.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/jquery/jquery-1.7.2.min.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/jquery/jquery-1.7.2.min.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/jquery/jquery.json-2.3.min.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/jquery/jquery.json-2.3.min.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap-theme.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap-theme.css.map` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap-theme.min.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap.css.map` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap.min.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap_noresponsive.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/css/bootstrap_noresponsive.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/fonts/glyphicons-halflings-regular.svg` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/bootstrap-treeview.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/bootstrap-treeview.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/bootstrap.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/bootstrap.min.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/bootstrap-3.3.4/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/external/jquery/jquery.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/external/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/animated-overlay.gif` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/animated-overlay.gif`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_gloss-wave_35_f6a828_500x100.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-bg_gloss-wave_35_f6a828_500x100.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_222222_256x240.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_228ef1_256x240.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_228ef1_256x240.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_454545_256x240.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_888888_256x240.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_ef8c08_256x240.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_ef8c08_256x240.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_ffd27a_256x240.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_ffd27a_256x240.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_ffffff_256x240.png` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/index.html` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/index.html`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.min.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.min.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.structure.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.structure.min.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.theme.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.theme.min.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/jquery-ui-1.11.0.custom/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/js/jquery-1.10.2.min.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/js/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/assets/js/jquery-migrate-1.2.1.min.js` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/assets/js/jquery-migrate-1.2.1.min.js`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/static/remote/v3/bk/css/bk.css` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/static/remote/v3/bk/css/bk.css`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/templates/admin/login.html` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/templates/base.html` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/templates/base.html`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/templates/debug_panel.html` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/templates/debug_panel.html`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/urls.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/urls.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/bk_plugin_runtime/wsgi.py` & `bk-plugin-runtime-2.0.6/bk_plugin_runtime/wsgi.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-runtime-2.0.5/pyproject.toml` & `bk-plugin-runtime-2.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "bk-plugin-runtime"
-version = "2.0.5"
+version = "2.0.6"
 description = "bk plugin python django runtime"
 authors = ["Your Name <you@example.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.6"
-redis = "^2.10.5"
-Django = "^2.2.6"
-gunicorn = "^19.6.0"
+python = "^3.6.1,<4.0"
+redis = ">=2.10.5,<4"
+Django = ">=2.2.6,<5"
+gunicorn = ">=19.6.0"
 djangorestframework = "^3.12.4"
 drf-yasg = "^1.20.0"
 raven = "^6.5.0"
 ddtrace = "^0.14.1"
 django-cors-headers = "^3.8.0"
 django-dbconn-retry = "^0.1.5"
 blueapps = {version = "4.5.0", extras = ["opentelemetry"]}
```

### Comparing `bk-plugin-runtime-2.0.5/setup.py` & `bk-plugin-runtime-2.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,40 +51,40 @@
                        'static/remote/v3/assets/js/*',
                        'static/remote/v3/bk/css/*',
                        'static/remote/v3/bk/js/*',
                        'templates/*',
                        'templates/admin/*']}
 
 install_requires = \
-['Django>=2.2.6,<3.0.0',
+['Django>=2.2.6,<5',
  'blueapps[opentelemetry]==4.5.0',
  'celery>=4.4.0,<5.0.0',
  'ddtrace>=0.14.1,<0.15.0',
  'django-celery-beat>=2.0.0,<3.0.0',
  'django-celery-results>=1.2.1,<2.0.0',
  'django-cors-headers>=3.8.0,<4.0.0',
  'django-dbconn-retry>=0.1.5,<0.2.0',
  'djangorestframework>=3.12.4,<4.0.0',
  'drf-yasg>=1.20.0,<2.0.0',
- 'gunicorn>=19.6.0,<20.0.0',
+ 'gunicorn>=19.6.0',
  'protobuf==3.19.4',
  'raven>=6.5.0,<7.0.0',
- 'redis>=2.10.5,<3.0.0']
+ 'redis>=2.10.5,<4']
 
 setup_kwargs = {
     'name': 'bk-plugin-runtime',
-    'version': '2.0.5',
+    'version': '2.0.6',
     'description': 'bk plugin python django runtime',
     'long_description': None,
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.6.1,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `bk-plugin-runtime-2.0.5/PKG-INFO` & `bk-plugin-runtime-2.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: bk-plugin-runtime
-Version: 2.0.5
+Version: 2.0.6
 Summary: bk plugin python django runtime
 License: MIT
 Author: Your Name
 Author-email: you@example.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Django (>=2.2.6,<3.0.0)
+Requires-Dist: Django (>=2.2.6,<5)
 Requires-Dist: blueapps[opentelemetry] (==4.5.0)
 Requires-Dist: celery (>=4.4.0,<5.0.0)
 Requires-Dist: ddtrace (>=0.14.1,<0.15.0)
 Requires-Dist: django-celery-beat (>=2.0.0,<3.0.0)
 Requires-Dist: django-celery-results (>=1.2.1,<2.0.0)
 Requires-Dist: django-cors-headers (>=3.8.0,<4.0.0)
 Requires-Dist: django-dbconn-retry (>=0.1.5,<0.2.0)
 Requires-Dist: djangorestframework (>=3.12.4,<4.0.0)
 Requires-Dist: drf-yasg (>=1.20.0,<2.0.0)
-Requires-Dist: gunicorn (>=19.6.0,<20.0.0)
+Requires-Dist: gunicorn (>=19.6.0)
 Requires-Dist: protobuf (==3.19.4)
 Requires-Dist: raven (>=6.5.0,<7.0.0)
-Requires-Dist: redis (>=2.10.5,<3.0.0)
+Requires-Dist: redis (>=2.10.5,<4)
```

