# Comparing `tmp/wagtail_editorjs-1.6.1rc3.tar.gz` & `tmp/wagtail_editorjs-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_editorjs-1.6.1rc3.tar", last modified: Sat Apr 27 00:01:42 2024, max compression
+gzip compressed data, was "wagtail_editorjs-1.6.2.tar", last modified: Mon May 13 16:17:19 2024, max compression
```

## Comparing `wagtail_editorjs-1.6.1rc3.tar` & `wagtail_editorjs-1.6.2.tar`

### file list

```diff
@@ -1,146 +1,148 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.497547 wagtail_editorjs-1.6.1rc3/
--rw-rw-rw-   0        0        0    18429 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.1rc3/LICENSE
--rw-rw-rw-   0        0        0      272 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.1rc3/MANIFEST.in
--rw-rw-rw-   0        0        0     4987 2024-04-27 00:01:42.497547 wagtail_editorjs-1.6.1rc3/PKG-INFO
--rw-rw-rw-   0        0        0     3850 2024-04-26 23:55:47.000000 wagtail_editorjs-1.6.1rc3/README.md
--rw-rw-rw-   0        0        0       90 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.1rc3/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-04-27 00:01:42.510084 wagtail_editorjs-1.6.1rc3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-03-27 00:40:18.000000 wagtail_editorjs-1.6.1rc3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.364014 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/
--rw-rw-rw-   0        0        0      334 2024-04-27 00:01:39.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/__init__.py
--rw-rw-rw-   0        0        0      169 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/apps.py
--rw-rw-rw-   0        0        0     1985 2024-03-29 17:31:47.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/blocks.py
--rw-rw-rw-   0        0        0     2569 2024-04-08 19:06:41.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/django_editor.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.391552 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/
--rw-rw-rw-   0        0        0      609 2024-04-26 08:36:30.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/__init__.py
--rw-rw-rw-   0        0        0    10474 2024-04-18 21:16:10.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/blocks.py
--rw-rw-rw-   0        0        0     6818 2024-03-31 07:04:36.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/documents.py
--rw-rw-rw-   0        0        0     9823 2024-04-16 19:24:08.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/images.py
--rw-rw-rw-   0        0        0     6849 2024-04-26 22:00:46.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/inlines.py
--rw-rw-rw-   0        0        0     5164 2024-03-27 20:40:47.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/lists.py
--rw-rw-rw-   0        0        0     3983 2024-04-18 21:15:27.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/tunes.py
--rw-rw-rw-   0        0        0     1785 2024-04-16 12:46:42.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/fields.py
--rw-rw-rw-   0        0        0     6874 2024-04-26 08:34:08.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/forms.py
--rw-rw-rw-   0        0        0      319 2024-03-27 21:25:26.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.393067 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.395094 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/migrations/__pycache__/
--rw-rw-rw-   0        0        0      218 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/migrations/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.398104 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/
--rw-rw-rw-   0        0        0      906 2024-04-18 21:15:11.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.402113 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/element/
--rw-rw-rw-   0        0        0      229 2024-03-29 10:32:13.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/element/__init__.py
--rw-rw-rw-   0        0        0     2073 2024-03-28 19:01:37.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/element/attrs.py
--rw-rw-rw-   0        0        0     3494 2024-03-29 14:48:28.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/element/element.py
--rw-rw-rw-   0        0        0     1525 2024-03-27 14:19:36.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/element/utils.py
--rw-rw-rw-   0        0        0     7265 2024-03-27 21:04:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/feature_registry.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.411862 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/features/
--rw-rw-rw-   0        0        0      340 2024-04-18 21:14:51.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/features/__init__.py
--rw-rw-rw-   0        0        0     7487 2024-04-26 08:32:56.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/features/base.py
--rw-rw-rw-   0        0        0     2235 2024-04-18 09:40:47.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/features/basic.py
--rw-rw-rw-   0        0        0     8877 2024-04-26 13:03:15.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/features/inlines.py
--rw-rw-rw-   0        0        0      674 2024-04-18 21:56:20.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/features/snippets_inlines.py
--rw-rw-rw-   0        0        0     1258 2024-03-27 20:13:06.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/features/view.py
--rw-rw-rw-   0        0        0     3311 2024-04-16 12:34:49.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/value.py
--rw-rw-rw-   0        0        0     5353 2024-04-18 10:11:04.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/render.py
--rw-rw-rw-   0        0        0     1042 2024-04-08 19:04:03.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.331329 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.333850 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.413884 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/css/
--rw-rw-rw-   0        0        0    10098 2024-04-26 12:36:15.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css
--rw-rw-rw-   0        0        0    14154 2024-04-26 13:11:26.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.416889 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/
--rw-rw-rw-   0        0        0     1371 2024-03-29 17:29:46.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
--rw-rw-rw-   0        0        0     1155 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
--rw-rw-rw-   0        0        0     2913 2024-04-26 11:54:42.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.418884 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/init/
--rw-rw-rw-   0        0        0       86 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
--rw-rw-rw-   0        0        0       94 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.431080 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/
--rw-rw-rw-   0        0        0      364 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.433589 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/
--rw-rw-rw-   0        0        0     2460 2024-04-26 21:59:35.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js
--rw-rw-rw-   0        0        0     4464 2024-04-26 12:37:59.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js
--rw-rw-rw-   0        0        0    12378 2024-04-18 09:49:54.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
--rw-rw-rw-   0        0        0     5510 2024-04-18 21:24:20.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
--rw-rw-rw-   0        0        0     3595 2024-04-26 10:29:04.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
--rw-rw-rw-   0        0        0    11260 2024-04-18 09:47:53.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
--rw-rw-rw-   0        0        0     3277 2024-03-26 20:38:45.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
--rw-rw-rw-   0        0        0     7883 2024-04-18 08:43:02.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
--rw-rw-rw-   0        0        0    16447 2024-04-18 09:47:21.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
--rw-rw-rw-   0        0        0     4197 2024-04-26 12:35:50.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js
--rw-rw-rw-   0        0        0     6225 2024-04-18 22:11:04.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.334962 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.434597 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/
--rw-rw-rw-   0        0        0   208234 2024-03-28 10:17:35.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.459889 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/
--rw-rw-rw-   0        0        0    34797 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js
--rw-rw-rw-   0        0        0     7233 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js
--rw-rw-rw-   0        0        0     3222 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js
--rw-rw-rw-   0        0        0     1864 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js
--rw-rw-rw-   0        0        0    10151 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js
--rw-rw-rw-   0        0        0     6946 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js
--rw-rw-rw-   0        0        0    29531 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js
--rw-rw-rw-   0        0        0     2440 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js
--rw-rw-rw-   0        0        0    33560 2024-03-27 17:16:55.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js
--rw-rw-rw-   0        0        0    30466 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js
--rw-rw-rw-   0        0        0     2550 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js
--rw-rw-rw-   0        0        0    10575 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js
--rw-rw-rw-   0        0        0     3142 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js
--rw-rw-rw-   0        0        0     5481 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js
--rw-rw-rw-   0        0        0     3198 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js
--rw-rw-rw-   0        0        0    23954 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
--rw-rw-rw-   0        0        0     9463 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
--rw-rw-rw-   0        0        0     9644 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
--rw-rw-rw-   0        0        0     8007 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
--rw-rw-rw-   0        0        0    19237 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
--rw-rw-rw-   0        0        0     3713 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
--rw-rw-rw-   0        0        0    20734 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.461889 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/
--rw-rw-rw-   0        0        0    44137 2024-04-16 19:19:37.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.466407 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE
--rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js
--rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.337291 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templates/
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.467410 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templates/wagtail_editorjs/
--rw-rw-rw-   0        0        0      123 2024-03-29 14:30:09.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.469409 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templates/wagtail_editorjs/widgets/
--rw-rw-rw-   0        0        0      555 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.471408 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.475936 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      220 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     2309 2024-04-25 19:47:38.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
--rw-rw-rw-   0        0        0     1497 2024-04-25 19:47:36.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templatetags/editorjs.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.478934 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.480933 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/__init__.py
--rw-rw-rw-   0        0        0      168 2024-04-08 18:30:48.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.481934 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.487033 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-03-26 23:51:58.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     2310 2024-04-08 19:05:43.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/tests/base.py
--rw-rw-rw-   0        0        0     2585 2024-04-08 18:38:20.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/tests/test_attrs.py
--rw-rw-rw-   0        0        0     2041 2024-04-08 18:42:47.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/tests/test_inlines.py
--rw-rw-rw-   0        0        0     5862 2024-04-08 18:58:38.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/tests/test_render.py
--rw-rw-rw-   0        0        0      707 2024-04-08 18:29:14.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.492031 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3826 2024-04-08 19:17:04.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/testapp/settings.py
--rw-rw-rw-   0        0        0     1176 2024-04-08 18:42:23.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/testapp/urls.py
--rw-rw-rw-   0        0        0      429 2024-04-08 18:29:49.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.496548 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/wagtail_hooks/
--rw-rw-rw-   0        0        0       74 2024-04-16 12:19:31.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     7364 2024-04-26 09:19:37.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/wagtail_hooks/features.py
--rw-rw-rw-   0        0        0      646 2024-03-27 20:14:22.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0      777 2024-04-16 12:19:25.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:01:42.383179 wagtail_editorjs-1.6.1rc3/wagtail_editorjs.egg-info/
--rw-rw-rw-   0        0        0     4987 2024-04-27 00:01:42.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5891 2024-04-27 00:01:42.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 00:01:42.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-27 00:01:42.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 00:01:42.000000 wagtail_editorjs-1.6.1rc3/wagtail_editorjs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.919174 wagtail_editorjs-1.6.2/
+-rw-rw-rw-   0        0        0    18429 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.2/LICENSE
+-rw-rw-rw-   0        0        0      272 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6694 2024-05-13 16:17:19.919174 wagtail_editorjs-1.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5560 2024-05-13 14:38:18.000000 wagtail_editorjs-1.6.2/README.md
+-rw-rw-rw-   0        0        0       90 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2024-05-13 16:17:19.920173 wagtail_editorjs-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-03-27 00:40:18.000000 wagtail_editorjs-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.739292 wagtail_editorjs-1.6.2/wagtail_editorjs/
+-rw-rw-rw-   0        0        0      331 2024-05-13 16:17:16.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/__init__.py
+-rw-rw-rw-   0        0        0      169 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/apps.py
+-rw-rw-rw-   0        0        0     1985 2024-03-29 17:31:47.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/blocks.py
+-rw-rw-rw-   0        0        0     2569 2024-04-08 19:06:41.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/django_editor.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.798323 wagtail_editorjs-1.6.2/wagtail_editorjs/features/
+-rw-rw-rw-   0        0        0      668 2024-05-13 14:46:42.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/__init__.py
+-rw-rw-rw-   0        0        0    15854 2024-05-13 16:14:30.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/blocks.py
+-rw-rw-rw-   0        0        0     6818 2024-03-31 07:04:36.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/documents.py
+-rw-rw-rw-   0        0        0     9823 2024-04-16 19:24:08.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/images.py
+-rw-rw-rw-   0        0        0     7721 2024-05-01 07:39:27.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/inlines.py
+-rw-rw-rw-   0        0        0     5164 2024-03-27 20:40:47.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/lists.py
+-rw-rw-rw-   0        0        0     3983 2024-04-18 21:15:27.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/tunes.py
+-rw-rw-rw-   0        0        0     1785 2024-04-16 12:46:42.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/fields.py
+-rw-rw-rw-   0        0        0     6874 2024-04-26 08:34:08.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/forms.py
+-rw-rw-rw-   0        0        0      319 2024-03-27 21:25:26.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/hooks.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.800329 wagtail_editorjs-1.6.2/wagtail_editorjs/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.801323 wagtail_editorjs-1.6.2/wagtail_editorjs/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      218 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/migrations/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.805326 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/
+-rw-rw-rw-   0        0        0      932 2024-05-13 14:22:20.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.815659 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/
+-rw-rw-rw-   0        0        0      255 2024-05-13 14:22:16.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/__init__.py
+-rw-rw-rw-   0        0        0     2073 2024-03-28 19:01:37.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/attrs.py
+-rw-rw-rw-   0        0        0     5110 2024-05-13 14:43:24.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/element.py
+-rw-rw-rw-   0        0        0     1525 2024-03-27 14:19:36.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/utils.py
+-rw-rw-rw-   0        0        0     7265 2024-03-27 21:04:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/feature_registry.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.825991 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/
+-rw-rw-rw-   0        0        0      340 2024-04-18 21:14:51.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/__init__.py
+-rw-rw-rw-   0        0        0     7600 2024-05-13 15:20:31.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/base.py
+-rw-rw-rw-   0        0        0     2235 2024-04-18 09:40:47.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/basic.py
+-rw-rw-rw-   0        0        0     8877 2024-04-26 13:03:15.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/inlines.py
+-rw-rw-rw-   0        0        0      674 2024-04-18 21:56:20.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/snippets_inlines.py
+-rw-rw-rw-   0        0        0     1258 2024-03-27 20:13:06.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/view.py
+-rw-rw-rw-   0        0        0     3311 2024-04-16 12:34:49.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/value.py
+-rw-rw-rw-   0        0        0     5353 2024-04-18 10:11:04.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/render.py
+-rw-rw-rw-   0        0        0     1042 2024-04-08 19:04:03.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.709475 wagtail_editorjs-1.6.2/wagtail_editorjs/static/
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.712431 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.828992 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/css/
+-rw-rw-rw-   0        0        0    10098 2024-04-26 12:36:15.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css
+-rw-rw-rw-   0        0        0    14154 2024-04-26 13:11:26.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.833990 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/
+-rw-rw-rw-   0        0        0     1371 2024-03-29 17:29:46.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
+-rw-rw-rw-   0        0        0     1155 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
+-rw-rw-rw-   0        0        0     2913 2024-04-26 11:54:42.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.836990 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/init/
+-rw-rw-rw-   0        0        0       86 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
+-rw-rw-rw-   0        0        0       94 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.848992 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/
+-rw-rw-rw-   0        0        0      364 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.851990 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/
+-rw-rw-rw-   0        0        0     2661 2024-04-27 00:14:45.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js
+-rw-rw-rw-   0        0        0     4464 2024-04-26 12:37:59.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js
+-rw-rw-rw-   0        0        0    12378 2024-04-18 09:49:54.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
+-rw-rw-rw-   0        0        0     3378 2024-05-13 13:49:05.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js
+-rw-rw-rw-   0        0        0     5510 2024-04-18 21:24:20.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
+-rw-rw-rw-   0        0        0     3595 2024-04-26 10:29:04.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
+-rw-rw-rw-   0        0        0    11260 2024-04-18 09:47:53.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
+-rw-rw-rw-   0        0        0     3277 2024-03-26 20:38:45.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
+-rw-rw-rw-   0        0        0     7883 2024-04-18 08:43:02.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
+-rw-rw-rw-   0        0        0    16447 2024-04-18 09:47:21.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
+-rw-rw-rw-   0        0        0     4197 2024-04-26 12:35:50.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js
+-rw-rw-rw-   0        0        0     6225 2024-04-18 22:11:04.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.714115 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.855992 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/
+-rw-rw-rw-   0        0        0   208234 2024-03-28 10:17:35.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.880990 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/
+-rw-rw-rw-   0        0        0    34797 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js
+-rw-rw-rw-   0        0        0     7233 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js
+-rw-rw-rw-   0        0        0     3222 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js
+-rw-rw-rw-   0        0        0     1864 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js
+-rw-rw-rw-   0        0        0    10151 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js
+-rw-rw-rw-   0        0        0     6946 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js
+-rw-rw-rw-   0        0        0    29531 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js
+-rw-rw-rw-   0        0        0     2440 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js
+-rw-rw-rw-   0        0        0    33560 2024-03-27 17:16:55.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js
+-rw-rw-rw-   0        0        0    30466 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js
+-rw-rw-rw-   0        0        0     2550 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js
+-rw-rw-rw-   0        0        0    10575 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js
+-rw-rw-rw-   0        0        0     3142 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js
+-rw-rw-rw-   0        0        0     5481 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js
+-rw-rw-rw-   0        0        0     3198 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js
+-rw-rw-rw-   0        0        0    23954 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
+-rw-rw-rw-   0        0        0     9463 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
+-rw-rw-rw-   0        0        0     9644 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
+-rw-rw-rw-   0        0        0     8007 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
+-rw-rw-rw-   0        0        0    19237 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
+-rw-rw-rw-   0        0        0     3713 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
+-rw-rw-rw-   0        0        0    20734 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.882994 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/
+-rw-rw-rw-   0        0        0    44137 2024-04-16 19:19:37.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.887990 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE
+-rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js
+-rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.715127 wagtail_editorjs-1.6.2/wagtail_editorjs/templates/
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.888990 wagtail_editorjs-1.6.2/wagtail_editorjs/templates/wagtail_editorjs/
+-rw-rw-rw-   0        0        0      123 2024-03-29 14:30:09.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.890814 wagtail_editorjs-1.6.2/wagtail_editorjs/templates/wagtail_editorjs/widgets/
+-rw-rw-rw-   0        0        0      555 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.892636 wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.894636 wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      220 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2309 2024-04-25 19:47:38.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1497 2024-04-25 19:47:36.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/editorjs.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.896796 wagtail_editorjs-1.6.2/wagtail_editorjs/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.898803 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/__init__.py
+-rw-rw-rw-   0        0        0      168 2024-04-08 18:30:48.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.899808 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.908865 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-26 23:51:58.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     2310 2024-04-08 19:05:43.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     2585 2024-04-08 18:38:20.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_attrs.py
+-rw-rw-rw-   0        0        0     2731 2024-05-13 16:16:35.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     2041 2024-04-08 18:42:47.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_inlines.py
+-rw-rw-rw-   0        0        0     5862 2024-04-08 18:58:38.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_render.py
+-rw-rw-rw-   0        0        0      707 2024-04-08 18:29:14.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.913165 wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3826 2024-04-08 19:17:04.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/settings.py
+-rw-rw-rw-   0        0        0     1176 2024-04-08 18:42:23.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      429 2024-04-08 18:29:49.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.918178 wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/
+-rw-rw-rw-   0        0        0       74 2024-04-16 12:19:31.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     7364 2024-04-26 09:19:37.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/features.py
+-rw-rw-rw-   0        0        0      646 2024-03-27 20:14:22.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0      777 2024-04-16 12:19:25.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.770643 wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/
+-rw-rw-rw-   0        0        0     6694 2024-05-13 16:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6006 2024-05-13 16:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 16:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-13 16:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-13 16:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/top_level.txt
```

### Comparing `wagtail_editorjs-1.6.1rc3/LICENSE` & `wagtail_editorjs-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/PKG-INFO` & `wagtail_editorjs-1.6.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_editorjs
-Version: 1.6.1rc3
+Version: 1.6.2
 Summary: EditorJS as a widget for Wagtail, with Page- and Image chooser support
 Home-page: https://github.com/Nigel2392/wagtail_editorjs
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -76,40 +76,40 @@
            FieldPanel("editor_field"),
            FieldPanel("content"),
        ]
        editor_field = EditorJSField(
            # All supported features
            features=[
                'attaches',
+               'background-color-tune',
+               'button',
                'checklist',
                'code',
                'delimiter',
+               'document',
+               'drag-drop',
                'header',
+               'image',
+               'images',
                'inline-code',
+               'link',
+               'link-autocomplete',
                'marker',
                'nested-list',
                'paragraph',
                'quote',
                'raw',
                'table',
-               'underline',
-               'warning',
-               'link-autocomplete',
-               'button',
-               'tooltip',
-               'link',
-               'image',
-               'images',
-               'document',
                'text-alignment-tune',
-               'text-variant-tune',
-               'background-color-tune',
                'text-color-tune',
+               'text-variant-tune',
+               'tooltip',
+               'underline',
                'undo-redo',
-               'drag-drop'
+               'warning'
             ],
            blank=True,
            null=True,
        )
 
        # Or as a block
        content = fields.StreamField([
@@ -134,14 +134,82 @@
 
    ```python
    from wagtail_editorjs.registry import EDITOR_JS_FEATURES
    print(EDITOR_JS_FEATURES.keys())
    dict_keys([... all registered features ...])
    ```
 
+##  Register a Wagtail block as a feature
+
+It is also possible to register a Wagtail block as a feature.
+
+This may be a `Fieldblock` (like `Charblock`, or `TextBlock`), or a `StructBlock`.
+
+It is **not** allowed to be or include:
+
+* A `StreamBlock`
+* A `ListBlock`
+* Any type of `ChooserBlock`
+* A `RichTextBlock`
+
+Example:
+
+```python
+from wagtail import hooks
+from wagtail_editorjs.features import (
+    WagtailBlockFeature,
+    EditorJSFeatureStructBlock,
+)
+from wagtail_editorjs.registry import (
+    EditorJSFeatures,
+)
+from wagtail_editorjs.hooks import REGISTER_HOOK_NAME
+
+from wagtail import blocks
+
+class HeadingBlock(blocks.StructBlock):
+    title = blocks.CharBlock()
+    subtitle = blocks.CharBlock()
+
+class TextBlock(EditorJSFeatureStructBlock):
+    heading = HeadingBlock()
+    body = blocks.TextBlock()
+
+    class Meta:
+        template = "myapp/text_block.html"
+        allowed_tags = ["h1", "h2", "p"]
+        # Html looks like:
+        #  <h1>{{ self.heading.title }}</h1>
+        #  <h2>{{ self.heading.subtitle }}</h2>
+        #  <p>{{ self.body }}</p>
+
+@hooks.register(REGISTER_HOOK_NAME)
+def register_editor_js_features(registry: EditorJSFeatures):
+
+    registry.register(
+        "wagtail-text-block",
+        WagtailBlockFeature(
+            "wagtail-text-block",
+            block=TextBlock(),
+        ),
+    )
+```
+
+The block will then be rendered as any structblock, but it will be wrapped in a div with the class `wagtail-text-block` (the feature name).
+
+Example:
+    
+    ```html
+    <div class="wagtail-text-block">
+        <h1>My title</h1>
+        <h2>My subtitle</h2>
+        <p>My body</p>
+    </div>
+    ```
+
 ## Settings
 
 ### `EDITORJS_CLEAN_HTML`
 
 Default: `True`
 Clean the HTML output on rendering.
 This happens every time the field is rendered.
```

### Comparing `wagtail_editorjs-1.6.1rc3/README.md` & `wagtail_editorjs-1.6.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -48,40 +48,40 @@
            FieldPanel("editor_field"),
            FieldPanel("content"),
        ]
        editor_field = EditorJSField(
            # All supported features
            features=[
                'attaches',
+               'background-color-tune',
+               'button',
                'checklist',
                'code',
                'delimiter',
+               'document',
+               'drag-drop',
                'header',
+               'image',
+               'images',
                'inline-code',
+               'link',
+               'link-autocomplete',
                'marker',
                'nested-list',
                'paragraph',
                'quote',
                'raw',
                'table',
-               'underline',
-               'warning',
-               'link-autocomplete',
-               'button',
-               'tooltip',
-               'link',
-               'image',
-               'images',
-               'document',
                'text-alignment-tune',
-               'text-variant-tune',
-               'background-color-tune',
                'text-color-tune',
+               'text-variant-tune',
+               'tooltip',
+               'underline',
                'undo-redo',
-               'drag-drop'
+               'warning'
             ],
            blank=True,
            null=True,
        )
 
        # Or as a block
        content = fields.StreamField([
@@ -106,14 +106,82 @@
 
    ```python
    from wagtail_editorjs.registry import EDITOR_JS_FEATURES
    print(EDITOR_JS_FEATURES.keys())
    dict_keys([... all registered features ...])
    ```
 
+##  Register a Wagtail block as a feature
+
+It is also possible to register a Wagtail block as a feature.
+
+This may be a `Fieldblock` (like `Charblock`, or `TextBlock`), or a `StructBlock`.
+
+It is **not** allowed to be or include:
+
+* A `StreamBlock`
+* A `ListBlock`
+* Any type of `ChooserBlock`
+* A `RichTextBlock`
+
+Example:
+
+```python
+from wagtail import hooks
+from wagtail_editorjs.features import (
+    WagtailBlockFeature,
+    EditorJSFeatureStructBlock,
+)
+from wagtail_editorjs.registry import (
+    EditorJSFeatures,
+)
+from wagtail_editorjs.hooks import REGISTER_HOOK_NAME
+
+from wagtail import blocks
+
+class HeadingBlock(blocks.StructBlock):
+    title = blocks.CharBlock()
+    subtitle = blocks.CharBlock()
+
+class TextBlock(EditorJSFeatureStructBlock):
+    heading = HeadingBlock()
+    body = blocks.TextBlock()
+
+    class Meta:
+        template = "myapp/text_block.html"
+        allowed_tags = ["h1", "h2", "p"]
+        # Html looks like:
+        #  <h1>{{ self.heading.title }}</h1>
+        #  <h2>{{ self.heading.subtitle }}</h2>
+        #  <p>{{ self.body }}</p>
+
+@hooks.register(REGISTER_HOOK_NAME)
+def register_editor_js_features(registry: EditorJSFeatures):
+
+    registry.register(
+        "wagtail-text-block",
+        WagtailBlockFeature(
+            "wagtail-text-block",
+            block=TextBlock(),
+        ),
+    )
+```
+
+The block will then be rendered as any structblock, but it will be wrapped in a div with the class `wagtail-text-block` (the feature name).
+
+Example:
+    
+    ```html
+    <div class="wagtail-text-block">
+        <h1>My title</h1>
+        <h2>My subtitle</h2>
+        <p>My body</p>
+    </div>
+    ```
+
 ## Settings
 
 ### `EDITORJS_CLEAN_HTML`
 
 Default: `True`
 Clean the HTML output on rendering.
 This happens every time the field is rendered.
```

### Comparing `wagtail_editorjs-1.6.1rc3/setup.cfg` & `wagtail_editorjs-1.6.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f65 6469 746f   = wagtail_edito
 00000020: 726a 730d 0a76 6572 7369 6f6e 203d 2031  rjs..version = 1
-00000030: 2e36 2e31 7263 330d 0a64 6573 6372 6970  .6.1rc3..descrip
-00000040: 7469 6f6e 203d 2045 6469 746f 724a 5320  tion = EditorJS 
-00000050: 6173 2061 2077 6964 6765 7420 666f 7220  as a widget for 
-00000060: 5761 6774 6169 6c2c 2077 6974 6820 5061  Wagtail, with Pa
-00000070: 6765 2d20 616e 6420 496d 6167 6520 6368  ge- and Image ch
-00000080: 6f6f 7365 7220 7375 7070 6f72 740d 0a6c  ooser support..l
-00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-000000a0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-000000b0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-000000c0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000000d0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-000000e0: 0d0a 6175 7468 6f72 203d 204e 6967 656c  ..author = Nigel
-000000f0: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
-00000100: 206e 6967 656c 4067 6f6f 6461 6476 6963   nigel@goodadvic
-00000110: 652e 6974 0d0a 7572 6c20 3d20 6874 7470  e.it..url = http
-00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4e  s://github.com/N
-00000130: 6967 656c 3233 3932 2f77 6167 7461 696c  igel2392/wagtail
-00000140: 5f65 6469 746f 726a 730d 0a6c 6963 656e  _editorjs..licen
-00000150: 7365 203d 2047 504c 2d33 2e30 2d6f 6e6c  se = GPL-3.0-onl
-00000160: 790d 0a63 6c61 7373 6966 6965 7273 203d  y..classifiers =
-00000170: 200d 0a09 456e 7669 726f 6e6d 656e 7420   ...Environment 
-00000180: 3a3a 2057 6562 2045 6e76 6972 6f6e 6d65  :: Web Environme
-00000190: 6e74 0d0a 0946 7261 6d65 776f 726b 203a  nt...Framework :
-000001a0: 3a20 446a 616e 676f 0d0a 0946 7261 6d65  : Django...Frame
-000001b0: 776f 726b 203a 3a20 446a 616e 676f 203a  work :: Django :
-000001c0: 3a20 342e 320d 0a09 4672 616d 6577 6f72  : 4.2...Framewor
-000001d0: 6b20 3a3a 2057 6167 7461 696c 0d0a 0946  k :: Wagtail...F
-000001e0: 7261 6d65 776f 726b 203a 3a20 5761 6774  ramework :: Wagt
-000001f0: 6169 6c20 3a3a 2035 0d0a 0946 7261 6d65  ail :: 5...Frame
-00000200: 776f 726b 203a 3a20 5761 6774 6169 6c20  work :: Wagtail 
-00000210: 3a3a 2036 0d0a 0949 6e74 656e 6465 6420  :: 6...Intended 
-00000220: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
-00000230: 6c6f 7065 7273 0d0a 094c 6963 656e 7365  lopers...License
-00000240: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000250: 203a 3a20 474e 5520 4765 6e65 7261 6c20   :: GNU General 
-00000260: 5075 626c 6963 204c 6963 656e 7365 2076  Public License v
-00000270: 3320 6f72 206c 6174 6572 2028 4750 4c76  3 or later (GPLv
-00000280: 332b 290d 0a09 4f70 6572 6174 696e 6720  3+)...Operating 
-00000290: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-000002a0: 6570 656e 6465 6e74 0d0a 0950 726f 6772  ependent...Progr
-000002b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000002c0: 3a3a 2050 7974 686f 6e0d 0a09 5072 6f67  :: Python...Prog
-000002d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000002e0: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
-000002f0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000300: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000310: 203a 3a20 3320 3a3a 204f 6e6c 790d 0a09   :: 3 :: Only...
-00000320: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000330: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000340: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
-00000350: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000360: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
-00000370: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
-00000380: 7420 3a3a 2057 5757 2f48 5454 500d 0a09  t :: WWW/HTTP...
-00000390: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
-000003a0: 7420 3a3a 2057 5757 2f48 5454 5020 3a3a  t :: WWW/HTTP ::
-000003b0: 2044 796e 616d 6963 2043 6f6e 7465 6e74   Dynamic Content
-000003c0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a69  ....[options]..i
-000003d0: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-000003e0: 6174 6120 3d20 7472 7565 0d0a 7061 636b  ata = true..pack
-000003f0: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
-00000400: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000410: 3e3d 332e 380d 0a69 6e73 7461 6c6c 5f72  >=3.8..install_r
-00000420: 6571 7569 7265 7320 3d20 0d0a 0944 6a61  equires = ...Dja
-00000430: 6e67 6f20 3e3d 2034 2e32 0d0a 0957 6167  ngo >= 4.2...Wag
-00000440: 7461 696c 203e 3d20 352e 300d 0a09 6265  tail >= 5.0...be
-00000450: 6175 7469 6675 6c73 6f75 7034 203e 3d20  autifulsoup4 >= 
-00000460: 342e 392e 330d 0a09 626c 6561 6368 203e  4.9.3...bleach >
-00000470: 3d20 362e 302e 300d 0a0d 0a5b 6567 675f  = 6.0.0....[egg_
-00000480: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000490: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-000004a0: 300d 0a0d 0a                             0....
+00000030: 2e36 2e32 0d0a 6465 7363 7269 7074 696f  .6.2..descriptio
+00000040: 6e20 3d20 4564 6974 6f72 4a53 2061 7320  n = EditorJS as 
+00000050: 6120 7769 6467 6574 2066 6f72 2057 6167  a widget for Wag
+00000060: 7461 696c 2c20 7769 7468 2050 6167 652d  tail, with Page-
+00000070: 2061 6e64 2049 6d61 6765 2063 686f 6f73   and Image choos
+00000080: 6572 2073 7570 706f 7274 0d0a 6c6f 6e67  er support..long
+00000090: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+000000a0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
+000000b0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000c0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+000000d0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a61  text/markdown..a
+000000e0: 7574 686f 7220 3d20 4e69 6765 6c0d 0a61  uthor = Nigel..a
+000000f0: 7574 686f 725f 656d 6169 6c20 3d20 6e69  uthor_email = ni
+00000100: 6765 6c40 676f 6f64 6164 7669 6365 2e69  gel@goodadvice.i
+00000110: 740d 0a75 726c 203d 2068 7474 7073 3a2f  t..url = https:/
+00000120: 2f67 6974 6875 622e 636f 6d2f 4e69 6765  /github.com/Nige
+00000130: 6c32 3339 322f 7761 6774 6169 6c5f 6564  l2392/wagtail_ed
+00000140: 6974 6f72 6a73 0d0a 6c69 6365 6e73 6520  itorjs..license 
+00000150: 3d20 4750 4c2d 332e 302d 6f6e 6c79 0d0a  = GPL-3.0-only..
+00000160: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
+00000170: 0945 6e76 6972 6f6e 6d65 6e74 203a 3a20  .Environment :: 
+00000180: 5765 6220 456e 7669 726f 6e6d 656e 740d  Web Environment.
+00000190: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
+000001a0: 6a61 6e67 6f0d 0a09 4672 616d 6577 6f72  jango...Framewor
+000001b0: 6b20 3a3a 2044 6a61 6e67 6f20 3a3a 2034  k :: Django :: 4
+000001c0: 2e32 0d0a 0946 7261 6d65 776f 726b 203a  .2...Framework :
+000001d0: 3a20 5761 6774 6169 6c0d 0a09 4672 616d  : Wagtail...Fram
+000001e0: 6577 6f72 6b20 3a3a 2057 6167 7461 696c  ework :: Wagtail
+000001f0: 203a 3a20 350d 0a09 4672 616d 6577 6f72   :: 5...Framewor
+00000200: 6b20 3a3a 2057 6167 7461 696c 203a 3a20  k :: Wagtail :: 
+00000210: 360d 0a09 496e 7465 6e64 6564 2041 7564  6...Intended Aud
+00000220: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+00000230: 6572 730d 0a09 4c69 6365 6e73 6520 3a3a  ers...License ::
+00000240: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000250: 2047 4e55 2047 656e 6572 616c 2050 7562   GNU General Pub
+00000260: 6c69 6320 4c69 6365 6e73 6520 7633 206f  lic License v3 o
+00000270: 7220 6c61 7465 7220 2847 504c 7633 2b29  r later (GPLv3+)
+00000280: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+00000290: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000002a0: 6e64 656e 740d 0a09 5072 6f67 7261 6d6d  ndent...Programm
+000002b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002c0: 5079 7468 6f6e 0d0a 0950 726f 6772 616d  Python...Program
+000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002e0: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
+000002f0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000300: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000310: 2033 203a 3a20 4f6e 6c79 0d0a 0950 726f   3 :: Only...Pro
+00000320: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000330: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000340: 2e38 0d0a 0950 726f 6772 616d 6d69 6e67  .8...Programming
+00000350: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000360: 686f 6e20 3a3a 2033 2e39 0d0a 0954 6f70  hon :: 3.9...Top
+00000370: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
+00000380: 3a20 5757 572f 4854 5450 0d0a 0954 6f70  : WWW/HTTP...Top
+00000390: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
+000003a0: 3a20 5757 572f 4854 5450 203a 3a20 4479  : WWW/HTTP :: Dy
+000003b0: 6e61 6d69 6320 436f 6e74 656e 740d 0a0d  namic Content...
+000003c0: 0a5b 6f70 7469 6f6e 735d 0d0a 696e 636c  .[options]..incl
+000003d0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
+000003e0: 203d 2074 7275 650d 0a70 6163 6b61 6765   = true..package
+000003f0: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
+00000400: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000410: 2e38 0d0a 696e 7374 616c 6c5f 7265 7175  .8..install_requ
+00000420: 6972 6573 203d 200d 0a09 446a 616e 676f  ires = ...Django
+00000430: 203e 3d20 342e 320d 0a09 5761 6774 6169   >= 4.2...Wagtai
+00000440: 6c20 3e3d 2035 2e30 0d0a 0962 6561 7574  l >= 5.0...beaut
+00000450: 6966 756c 736f 7570 3420 3e3d 2034 2e39  ifulsoup4 >= 4.9
+00000460: 2e33 0d0a 0962 6c65 6163 6820 3e3d 2036  .3...bleach >= 6
+00000470: 2e30 2e30 0d0a 0d0a 5b65 6767 5f69 6e66  .0.0....[egg_inf
+00000480: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000490: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+000004a0: 0d0a                                     ..
```

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/blocks.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/django_editor.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/django_editor.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/__init__.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/features/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,16 @@
     CodeFeature,
     DelimiterFeature,
     HeaderFeature,
     HTMLFeature,
     WarningFeature,
     TableFeature,
     BlockQuoteFeature,
+    WagtailBlockFeature,
+    EditorJSFeatureStructBlock,
     ButtonFeature,
 )
 from .lists import (
     NestedListFeature,
     CheckListFeature,
 )
 from .documents import (
```

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/blocks.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/features/images.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,363 +1,316 @@
-from typing import Any
+from typing import Any, TYPE_CHECKING
 from django import forms
+from django.urls import reverse, path
+from django.shortcuts import get_object_or_404
 from django.utils.translation import gettext_lazy as _
-from django.utils.functional import cached_property
+from django.http import (
+    HttpRequest,
+    FileResponse,
+    HttpResponse,
+)
+
+from wagtail.images.widgets import AdminImageChooser
+from wagtail.images import get_image_model
+from wagtail.images.models import SourceImageIOError
 
-import bleach
+if TYPE_CHECKING:
+    from wagtail.images.models import Image as AbstractImage
 
+from ..settings import (
+    USE_FULL_URLS,
+)
 from ..registry import (
-    PageChooserURLsMixin,
     EditorJSFeature,
     EditorJSBlock,
     EditorJSElement,
-    wrap_tag,
+    FeatureViewMixin,
+    wrapper,
 )
 
+Image = get_image_model()
 
 
-class CodeFeature(EditorJSFeature):
-    allowed_tags = ["code"]
-    allowed_attributes = ["class"]
-    klass="CodeTool"
-    js=[
-        "wagtail_editorjs/vendor/editorjs/tools/code.js",
-    ]
+class BaseImageFeature(FeatureViewMixin, EditorJSFeature):
 
-    def validate(self, data: Any):
-        super().validate(data)
-
-        if 'code' not in data['data']:
-            raise forms.ValidationError('Invalid code value')
-    
-    def render_block_data(self, block: EditorJSBlock, context = None) -> EditorJSElement:
-        return EditorJSElement("code", block["data"]["code"], attrs={"class": "code"})
-    
-    @classmethod
-    def get_test_data(cls):
+    def get_urlpatterns(self):
         return [
-            {
-                "code": "print('Hello, World!')",
-            }
+            path(
+                f"{self.tool_name}/",
+                self.handler,
+                name=f"{self.tool_name}_for_id_fmt",
+            ),
+            path(
+                f"{self.tool_name}/<int:image_id>/",
+                self.handler,
+                name=self.tool_name,
+            )
         ]
 
+    def handle_get(self, request: HttpRequest, image_id: int) -> "AbstractImage":
+        image: "AbstractImage" = get_object_or_404(Image, pk=image_id)
 
-class DelimiterFeature(EditorJSFeature):
-    allowed_tags = ["hr"]
-    allowed_attributes = ["class"]
-    klass="Delimiter"
-    js = [
-        "wagtail_editorjs/vendor/editorjs/tools/delimiter.js",
-    ]
-
-    def render_block_data(self, block: EditorJSBlock, context = None) -> EditorJSElement:
-        return EditorJSElement("hr", close_tag=False, attrs={"class": "delimiter"})
-    
-    @classmethod
-    def get_test_data(cls):
-        return [{}, {}, {}]
-
+        # Get/generate the rendition
+        try:
+            rendition = image.get_rendition("original")
+        except SourceImageIOError:
+            return HttpResponse(
+                "Source image file not found", content_type="text/plain", status=410
+            )
 
-class HeaderFeature(EditorJSFeature):
-    allowed_tags = ["h1", "h2", "h3", "h4", "h5", "h6"]
-    allowed_attributes = ["class"]
-    klass="Header"
-    js=[
-        "wagtail_editorjs/vendor/editorjs/tools/header.js",
-    ]
+        with rendition.get_willow_image() as willow_image:
+            mime_type = willow_image.mime_type
 
-    def validate(self, data: Any):
-        super().validate(data)
+        # Serve the file
+        f = rendition.file.open("rb")
+        response = FileResponse(f, filename=image.filename, content_type=mime_type)
+        response["Content-Length"] = f.size
+        return response
+
+
+class ImageFeature(BaseImageFeature):
+    allowed_tags = ["img", "figure", "figcaption"]
+    allowed_attributes = {
+        "img": ["src", "alt", "class", "style"],
+        "figure": ["class", "style"],
+        "figcaption": ["class"],
+    }
+    klass = "WagtailImageTool"
 
-        level = data["data"].get("level")
-        if level > 6 or level < 1:
-            raise forms.ValidationError("Invalid level value")
-    
-    def render_block_data(self, block: EditorJSBlock, context = None) -> EditorJSElement:
-        return EditorJSElement(
-            "h" + str(block["data"]["level"]),
-            block["data"].get("text")
-        )
-    
-    @classmethod
-    def get_test_data(cls):
+    @property
+    def js(self):
         return [
-            {
-                "level": heading,
-                "text": f"Header {heading}",
-            } for heading in range(1, 7)
+            *(AdminImageChooser().media._js or []),
+            "wagtail_editorjs/js/tools/wagtail-image.js",
         ]
-
-
-class HTMLFeature(EditorJSFeature):
-    allowed_tags = bleach.ALLOWED_TAGS
-    allowed_attributes = bleach.ALLOWED_ATTRIBUTES
-    klass="RawTool"
-    js = [
-        "wagtail_editorjs/vendor/editorjs/tools/raw.js",
-    ]
-
-    def validate(self, data: Any):
-        super().validate(data)
-
-        if "html" not in data["data"]:
-            raise forms.ValidationError("Invalid html value")
     
-    def render_block_data(self, block: EditorJSBlock, context = None) -> EditorJSElement:
-        return EditorJSElement("div", block["data"]["html"], attrs={"class": "html"})
-    
-    @classmethod
-    def get_test_data(cls):
-        return [
-            {
-                "html": "<p>This is a HTML block.</p>",
-            }
-        ]
+    @js.setter
+    def js(self, value): pass
 
-class WarningFeature(EditorJSFeature):
-    allowed_tags = ["div", "h2", "p"]
-    allowed_attributes = ["class"]
-    klass="Warning"
-    js = [
-        "wagtail_editorjs/vendor/editorjs/tools/warning.js",
-    ]
+    def get_config(self, context: dict[str, Any]):
+        config = super().get_config() or {}
+        config.setdefault("config", {})
+        config["config"]["imageChooserId"] =\
+            f"editorjs-image-chooser-{context['widget']['attrs']['id']}"
+        config["config"]["getImageUrl"] = reverse(f"wagtail_editorjs:{self.tool_name}_for_id_fmt")
+        return config
 
     def validate(self, data: Any):
         super().validate(data)
 
-        if "title" not in data["data"]:
-            raise forms.ValidationError("Invalid title value")
+        d = data["data"]
+        if "imageId" not in d:
+            raise forms.ValidationError("Invalid imageId value")
+            
         
-        if "message" not in data["data"]:
-            raise forms.ValidationError("Invalid message value")
-    
-    def render_block_data(self, block: EditorJSBlock, context = None) -> EditorJSElement:
-        return EditorJSElement(
-            "div",
-            attrs={
-                "class": "warning",
-            },
-            content=[
-                EditorJSElement(
-                    "h2",
-                    block["data"]["title"],
-                ),
-                EditorJSElement(
-                    "p",
-                    block["data"]["message"],
-                ),
-            ]
+    def render_template(self, context: dict[str, Any] = None):
+        widget_id = f"editorjs-image-chooser-{context['widget']['attrs']['id']}"
+        return AdminImageChooser().render_html(
+            widget_id,
+            None,
+            {"id": widget_id}
         )
     
-    @classmethod
-    def get_test_data(cls):
-        return [
-            {
-                "title": "Warning",
-                "message": "This is a warning message.",
-            }
-        ]
-
-
-class TableFeature(EditorJSFeature):
-    allowed_tags = ["table", "tr", "th", "td", "thead", "tbody", "tfoot"]
-    allowed_attributes = ["class"]
-    klass="Table"
-    js = [
-        "wagtail_editorjs/vendor/editorjs/tools/table.js",
-    ]
-
-    def validate(self, data: Any):
-        super().validate(data)
-
-        if "content" not in data["data"]:
-            raise forms.ValidationError("Invalid content value")
-        
-        if "withHeadings" not in data["data"]:
-            raise forms.ValidationError("Invalid withHeadings value")
-
     def render_block_data(self, block: EditorJSBlock, context = None) -> EditorJSElement:
-        table = []
+        image = block["data"].get("imageId")
+        image = Image.objects.get(id=image)
 
-        if block["data"]["withHeadings"]:
-            headings = block["data"]["content"][0]
-            table.append(EditorJSElement(
-                "thead",
-                EditorJSElement(
-                    "tr",
-                    [
-                        EditorJSElement("th", heading)
-                        for heading in headings
-                    ]
-                )
-            ))
+        classlist = []
+        styles = {}
+        if block["data"].get("withBorder"):
+            classlist.append("with-border")
+
+        if block["data"].get("stretched"):
+            classlist.append("stretched")
+
+        if block["data"].get("backgroundColor"):
+            styles["--figure-bg"] = block["data"]["backgroundColor"]
+            classlist.append("with-background")
+
+        attrs = {}
+        if classlist:
+            attrs["class"] = classlist
+
+        if styles:
+            attrs["style"] = styles
+
+        url = image.file.url
+        if not any([url.startswith(i) for i in ["http://", "https://", "//"]])\
+                and context\
+                and "request" in context\
+                and USE_FULL_URLS:
+            request = context.get("request")
+            if request:
+                url = request.build_absolute_uri(url)
 
-            content = block["data"]["content"][1:]
-        else:
-            content = block["data"]["content"]
+        # Caption last - we are wrapping the image in a figure tag
+                
+        imgTag = EditorJSElement(
+            "img",
+            close_tag=False,
+            attrs={
+                "src": url,
+                "alt": block["data"].get("alt"),
+            },
+        )
 
-        tbody = EditorJSElement("tbody")
-        for row in content:
-            tbody.append(
-                EditorJSElement(
-                    "tr",
-                    [
-                        EditorJSElement("td", cell)
-                        for cell in row
-                    ]
-                )
+        if block["data"].get("usingCaption"):
+            caption = block["data"].get("alt")
+            w = EditorJSElement(
+                "figure",
+                close_tag=True,
             )
+            figcaption = EditorJSElement(
+                "figcaption",
+                caption,
+            )
+            w.append(imgTag)
+            w.append(figcaption)
+        else:
+            w = imgTag
 
-        table.append(tbody)
-
-        return EditorJSElement("table", table)
-
+        return wrapper(w, attrs=attrs)
+    
     @classmethod
     def get_test_data(cls):
+        instance = Image.objects.first()
         return [
             {
-                "withHeadings": False,
-                "content": [
-                    ["1", "2", "3"],
-                    ["4", "5", "6"],
-                    ["7", "8", "9"],
-                ],
+                "imageId": instance.pk,
+                "withBorder": True,
+                "stretched": False,
+                "backgroundColor": "#000000",
+                "usingCaption": False,
+                "alt": "Image",
+                "caption": "Image",
             },
             {
-                "withHeadings": True,
-                "content": [
-                    ["Heading 1", "Heading 2", "Heading 3"],
-                    ["1", "2", "3"],
-                    ["4", "5", "6"],
-                    ["7", "8", "9"],
-                ],
+                "imageId": instance.pk,
+                "withBorder": False,
+                "stretched": True,
+                "backgroundColor": None,
+                "usingCaption": True,
+                "alt": "Image",
+                "caption": "Image",
             }
         ]
 
 
-class BlockQuoteFeature(EditorJSFeature):
-    allowed_tags = ["blockquote", "footer"]
-    allowed_attributes = ["class"]
-    klass="Quote"
-    js = [
-        "wagtail_editorjs/vendor/editorjs/tools/quote.js",
-    ]
+class ImageRowFeature(BaseImageFeature):
+    allowed_tags = ["div", "img"]
+    allowed_attributes = ["class", "style"]
+    klass = "ImageRowTool"
+    # js = [
+        # "wagtail_editorjs/js/tools/wagtail-image-row.js",
+    # ]
 
-    def validate(self, data: Any):
-        super().validate(data)
-
-        if "text" not in data["data"]:
-            raise forms.ValidationError("Invalid text value")
-        
-        if "caption" not in data["data"]:
-            raise forms.ValidationError("Invalid caption value")
-        
-    
-    def render_block_data(self, block: EditorJSBlock, context = None) -> EditorJSElement:
-        text = block["data"]["text"]
-        caption = block["data"]["caption"]
-        return EditorJSElement(
-            "blockquote",
-            [
-                text,
-                wrap_tag("footer", {}, caption),
-            ],
-            {
-                "class": "blockquote",
-            }
-        )
-    
-    @classmethod
-    def get_test_data(cls):
+    @property
+    def js(self):
         return [
-            {
-                "text": "This is a quote.",
-                "caption": "Anonymous",
-            }
+            *(AdminImageChooser().media._js or []),
+            "wagtail_editorjs/vendor/sortable/sortable.min.js",
+            "wagtail_editorjs/js/tools/wagtail-image-row.js",
         ]
-
-from wagtail.models import Page
-from wagtail.admin.widgets import AdminPageChooser
-
-class ButtonFeature(PageChooserURLsMixin, EditorJSFeature):
-    allowed_tags:       list[str]            = ["a"]
-    allowed_attributes: dict[str, list[str]] = {
-        "a": ["href", "class"]
-    }
-    chooser_class = AdminPageChooser
-    model         = Page
-    klass         = "PageButtonTool"
-    js            = [
-        "wagtail_editorjs/js/tools/wagtail-button-tool.js",
-    ]
-
-    @cached_property
-    def widget(self):
-        if self.chooser_class is None:
-            return None
-        
-        return self.chooser_class()
     
-    def validate(self, data: Any):
-        super().validate(data)
-
-        if "pageId" not in data["data"]:
-            raise forms.ValidationError("Invalid id value")
-        
-        if "text" not in data["data"]:
-            raise forms.ValidationError("Invalid text value")
+    @js.setter
+    def js(self, value): pass
 
     def get_config(self, context: dict[str, Any]):
         config = super().get_config() or {}
         config.setdefault("config", {})
-        config["config"][
-            "chooserId"
-        ] = f"editorjs-{self.model._meta.model_name}-button-chooser-{context['widget']['attrs']['id']}"
+        config["config"]["imageChooserId"] =\
+            f"editorjs-images-chooser-{context['widget']['attrs']['id']}"
+        config["config"]["getImageUrl"] = reverse(f"wagtail_editorjs:{self.tool_name}_for_id_fmt")
         return config
     
-    def render_block_data(self, block: EditorJSBlock, context=None) -> EditorJSElement:
-        try:
-            page = self.model.objects.get(id=block["data"]["pageId"])
-        except self.model.DoesNotExist:
-            return None
-
-        request = None
-        if context:
-            request = context.get("request")
-
-        anchor = EditorJSElement(
-            "a",
-            block["data"]["text"],
-            {
-                "href": page.get_url(request),
-                "class": "editor-button",
-            }
+    def render_template(self, context: dict[str, Any] = None):
+        widget_id = f"editorjs-images-chooser-{context['widget']['attrs']['id']}"
+        return AdminImageChooser().render_html(
+            widget_id,
+            None,
+            {"id": widget_id}
         )
 
-        return EditorJSElement(
-            "div", anchor, {"class": "editor-button-container"},
-        )
+    def validate(self, data: Any):
+        super().validate(data)
 
-    def render_template(self, context: dict[str, Any] = None):
-        if not self.widget:
-            return super().render_template(context)
+        if "images" not in data["data"]:
+            raise forms.ValidationError("Invalid images value")
         
-        return self.widget.render_html(
-            f"editorjs-{self.model._meta.model_name}-button-chooser-{context['widget']['attrs']['id']}",
-            None,
-            {
-                "id": f"editorjs-{self.model._meta.model_name}-button-chooser-{context['widget']['attrs']['id']}"
-            },
+        if not data["data"]["images"]:
+            raise forms.ValidationError("Invalid images value")
+        
+        if "settings" not in data["data"] or data["data"]["settings"] is None:
+            raise forms.ValidationError("Invalid settings value")
+        
+        for image in data["data"]["images"]:
+            if "id" not in image:
+                raise forms.ValidationError("Invalid id value")
+            
+            if "title" not in image:
+                raise forms.ValidationError("Invalid title value")
+    
+    def render_block_data(self, block: EditorJSBlock, context = None) -> EditorJSElement:
+        images = block["data"]["images"]
+        ids = []
+        for image in images:
+            ids.append(image["id"])
+
+        images = Image.objects.in_bulk(ids)
+        s = []
+        for id in ids:
+            try:
+                id = int(id)
+            except ValueError:
+                pass
+            image = images[id]
+            url = image.file.url
+            if not any([url.startswith(i) for i in ["http://", "https://", "//"]])\
+                    and context\
+                    and "request" in context\
+                    and USE_FULL_URLS:
+                request = context.get("request")
+                if request:
+                    url = request.build_absolute_uri(url)
+
+
+            s.append(EditorJSElement(
+                "div",
+                EditorJSElement(
+                    "img",
+                    close_tag=False,
+                    attrs={
+                        "src": url,
+                        "alt": image.title,
+                    }
+                ),
+                attrs={
+                    "class": "image-wrapper",
+                }
+            ))
+
+
+        return wrapper(
+            EditorJSElement("div", s, attrs={
+                "class": "image-row",
+            }),
+            attrs={
+                "class": "stretched"
+            } if block["data"]["settings"].get("stretched") else {}
         )
 
     @classmethod
     def get_test_data(cls):
-        pages = cls.model.objects.all()[:5]
-
+        images = Image.objects.all()[0:3]
         return [
             {
-                "pageId": page.id,
-                "text": page.title,
+                "images": [
+                    {
+                        "id": image.pk,
+                        "title": image.title,
+                    } for image in images
+                ],
+                "settings": {
+                    "stretched": True,
+                },
             }
-            for page in pages
         ]
-
```

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/documents.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/features/documents.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/inlines.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/features/inlines.py`

 * *Files 13% similar despite different names*

```diff
@@ -83,347 +83,401 @@
 00000520: 6564 6974 6f72 6a73 2f6a 732f 746f 6f6c  editorjs/js/tool
 00000530: 732f 746f 6f6c 7469 7073 2f66 726f 6e74  s/tooltips/front
 00000540: 656e 642e 6a73 222c 0d0a 2020 2020 5d0d  end.js",..    ].
 00000550: 0a0d 0a20 2020 2040 636c 6173 736d 6574  ...    @classmet
 00000560: 686f 640d 0a20 2020 2064 6566 2067 6574  hod..    def get
 00000570: 5f74 6573 745f 6461 7461 2863 6c73 293a  _test_data(cls):
 00000580: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00000590: 205b 5d0d 0a0d 0a20 2020 2064 6566 2062   []....    def b
-000005a0: 7569 6c64 5f65 6c65 6d65 6e74 7328 7365  uild_elements(se
-000005b0: 6c66 2c20 696e 6c69 6e65 5f64 6174 613a  lf, inline_data:
-000005c0: 206c 6973 742c 2063 6f6e 7465 7874 3a20   list, context: 
-000005d0: 6469 6374 5b73 7472 2c20 416e 795d 203d  dict[str, Any] =
-000005e0: 204e 6f6e 6529 202d 3e20 6c69 7374 3a0d   None) -> list:.
-000005f0: 0a20 2020 2020 2020 2066 6f72 2065 6c65  .        for ele
-00000600: 6d65 6e74 2c20 6174 7472 7320 696e 2069  ment, attrs in i
-00000610: 6e6c 696e 655f 6461 7461 3a0d 0a0d 0a20  nline_data:.... 
-00000620: 2020 2020 2020 2020 2020 2065 6c65 6d65             eleme
-00000630: 6e74 5b22 6461 7461 2d74 6970 7079 2d66  nt["data-tippy-f
-00000640: 6f6c 6c6f 772d 6375 7273 6f72 225d 203d  ollow-cursor"] =
-00000650: 2022 686f 7269 7a6f 6e74 616c 220d 0a0d   "horizontal"...
-00000660: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00000670: 206b 2c20 7620 696e 2061 7474 7273 2e69   k, v in attrs.i
-00000680: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-00000690: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-000006a0: 6b2e 7374 6172 7473 7769 7468 2822 6461  k.startswith("da
-000006b0: 7461 2d77 2d74 6f6f 6c74 6970 2d22 2920  ta-w-tooltip-") 
-000006c0: 6f72 206e 6f74 206b 2e65 6e64 7377 6974  or not k.endswit
-000006d0: 6828 222d 7661 6c75 6522 293a 0d0a 2020  h("-value"):..  
-000006e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006f0: 2020 636f 6e74 696e 7565 0d0a 0d0a 2020    continue....  
-00000700: 2020 2020 2020 2020 2020 2020 2020 6b20                k 
-00000710: 3d20 6b2e 7265 706c 6163 6528 2264 6174  = k.replace("dat
-00000720: 612d 772d 746f 6f6c 7469 702d 222c 2022  a-w-tooltip-", "
-00000730: 6461 7461 2d74 6970 7079 2d22 290d 0a20  data-tippy-").. 
-00000740: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00000750: 203d 206b 5b3a 2d36 5d0d 0a0d 0a20 2020   = k[:-6]....   
-00000760: 2020 2020 2020 2020 2020 2020 2065 6c65               ele
-00000770: 6d65 6e74 5b6b 5d20 3d20 760d 0a0d 0a0d  ment[k] = v.....
-00000780: 0a63 6c61 7373 2042 6173 6550 6167 654c  .class BasePageL
-00000790: 696e 6b4d 6978 696e 2850 6167 6543 686f  inkMixin(PageCho
-000007a0: 6f73 6572 5552 4c73 4d69 7869 6e29 3a0d  oserURLsMixin):.
-000007b0: 0a20 2020 2061 6c6c 6f77 6564 5f61 7474  .    allowed_att
-000007c0: 7269 6275 7465 7320 3d20 5b22 7461 7267  ributes = ["targ
-000007d0: 6574 222c 2022 7265 6c22 5d0d 0a20 2020  et", "rel"]..   
-000007e0: 2063 616e 5f68 6176 655f 6174 7472 7320   can_have_attrs 
-000007f0: 3d20 7b0d 0a20 2020 2020 2020 2022 6461  = {..        "da
-00000800: 7461 2d74 6172 6765 7422 3a20 4e6f 6e65  ta-target": None
-00000810: 2c0d 0a20 2020 2020 2020 2022 6461 7461  ,..        "data
-00000820: 2d72 656c 223a 204e 6f6e 652c 0d0a 2020  -rel": None,..  
-00000830: 2020 7d0d 0a0d 0a20 2020 2064 6566 2062    }....    def b
-00000840: 7569 6c64 5f65 6c65 6d65 6e74 2873 656c  uild_element(sel
-00000850: 662c 2069 7465 6d2c 206f 626a 2c20 636f  f, item, obj, co
-00000860: 6e74 6578 743a 2064 6963 745b 7374 722c  ntext: dict[str,
-00000870: 2041 6e79 5d20 3d20 4e6f 6e65 2c20 6461   Any] = None, da
-00000880: 7461 3a20 6469 6374 5b73 7472 2c20 416e  ta: dict[str, An
-00000890: 795d 203d 204e 6f6e 6529 3a0d 0a20 2020  y] = None):..   
-000008a0: 2020 2020 2022 2222 4275 696c 6420 7468       """Build th
-000008b0: 6520 656c 656d 656e 7420 6672 6f6d 2074  e element from t
-000008c0: 6865 206f 626a 6563 742e 2222 220d 0a20  he object.""".. 
-000008d0: 2020 2020 2020 2073 7570 6572 2829 2e62         super().b
-000008e0: 7569 6c64 5f65 6c65 6d65 6e74 2869 7465  uild_element(ite
-000008f0: 6d2c 206f 626a 2c20 636f 6e74 6578 742c  m, obj, context,
-00000900: 2064 6174 6129 0d0a 2020 2020 2020 2020   data)..        
-00000910: 6966 2022 6461 7461 2d74 6172 6765 7422  if "data-target"
-00000920: 2069 6e20 6461 7461 2061 6e64 2064 6174   in data and dat
-00000930: 615b 2264 6174 612d 7461 7267 6574 225d  a["data-target"]
-00000940: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00000950: 7465 6d5b 2274 6172 6765 7422 5d20 3d20  tem["target"] = 
-00000960: 6461 7461 5b22 6461 7461 2d74 6172 6765  data["data-targe
-00000970: 7422 5d0d 0a20 2020 2020 2020 2069 6620  t"]..        if 
-00000980: 2264 6174 612d 7265 6c22 2069 6e20 6461  "data-rel" in da
-00000990: 7461 2061 6e64 2064 6174 615b 2264 6174  ta and data["dat
-000009a0: 612d 7265 6c22 5d3a 0d0a 2020 2020 2020  a-rel"]:..      
-000009b0: 2020 2020 2020 6974 656d 5b22 7265 6c22        item["rel"
-000009c0: 5d20 3d20 6461 7461 5b22 6461 7461 2d72  ] = data["data-r
-000009d0: 656c 225d 0d0a 0d0a 2020 2020 4063 6c61  el"]....    @cla
-000009e0: 7373 6d65 7468 6f64 0d0a 2020 2020 6465  ssmethod..    de
-000009f0: 6620 6765 745f 7572 6c28 636c 732c 2069  f get_url(cls, i
-00000a00: 6e73 7461 6e63 6529 3a0d 0a20 2020 2020  nstance):..     
-00000a10: 2020 2072 6574 7572 6e20 696e 7374 616e     return instan
-00000a20: 6365 2e67 6574 5f75 726c 2829 0d0a 0d0a  ce.get_url()....
-00000a30: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00000a40: 0d0a 2020 2020 6465 6620 6765 745f 6675  ..    def get_fu
-00000a50: 6c6c 5f75 726c 2863 6c73 2c20 696e 7374  ll_url(cls, inst
-00000a60: 616e 6365 2c20 7265 7175 6573 7429 3a0d  ance, request):.
-00000a70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000a80: 696e 7374 616e 6365 2e67 6574 5f66 756c  instance.get_ful
-00000a90: 6c5f 7572 6c28 7265 7175 6573 7429 0d0a  l_url(request)..
-00000aa0: 2020 2020 0d0a 2020 2020 4063 6c61 7373      ..    @class
-00000ab0: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
-00000ac0: 6765 745f 7465 7374 5f71 7565 7279 7365  get_test_queryse
-00000ad0: 7428 636c 7329 3a0d 0a20 2020 2020 2020  t(cls):..       
-00000ae0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-00000af0: 6765 745f 7465 7374 5f71 7565 7279 7365  get_test_queryse
-00000b00: 7428 292e 6669 6c74 6572 2864 6570 7468  t().filter(depth
-00000b10: 5f5f 6774 3d31 290d 0a0d 0a63 6c61 7373  __gt=1)....class
-00000b20: 204c 696e 6b46 6561 7475 7265 2842 6173   LinkFeature(Bas
-00000b30: 6550 6167 654c 696e 6b4d 6978 696e 2c20  ePageLinkMixin, 
-00000b40: 4d6f 6465 6c49 6e6c 696e 6545 6469 746f  ModelInlineEdito
-00000b50: 724a 5346 6561 7475 7265 293a 0d0a 2020  rJSFeature):..  
-00000b60: 2020 616c 6c6f 7765 645f 7461 6773 203d    allowed_tags =
-00000b70: 205b 2261 225d 0d0a 2020 2020 616c 6c6f   ["a"]..    allo
-00000b80: 7765 645f 6174 7472 6962 7574 6573 203d  wed_attributes =
-00000b90: 2042 6173 6550 6167 654c 696e 6b4d 6978   BasePageLinkMix
-00000ba0: 696e 2e61 6c6c 6f77 6564 5f61 7474 7269  in.allowed_attri
-00000bb0: 6275 7465 7320 2b20 5b0d 0a20 2020 2020  butes + [..     
-00000bc0: 2020 2022 636c 6173 7322 2c20 2268 7265     "class", "hre
-00000bd0: 6622 2c20 2264 6174 612d 6964 220d 0a20  f", "data-id".. 
-00000be0: 2020 205d 0d0a 2020 2020 6d75 7374 5f68     ]..    must_h
-00000bf0: 6176 655f 6174 7472 7320 3d20 7b0d 0a20  ave_attrs = {.. 
-00000c00: 2020 2020 2020 2022 6461 7461 2d70 6172         "data-par
-00000c10: 656e 742d 6964 223a 204e 6f6e 652c 0d0a  ent-id": None,..
-00000c20: 2020 2020 7d0d 0a20 2020 2063 686f 6f73      }..    choos
-00000c30: 6572 5f63 6c61 7373 203d 2041 646d 696e  er_class = Admin
-00000c40: 5061 6765 4368 6f6f 7365 720d 0a20 2020  PageChooser..   
-00000c50: 206d 6f64 656c 203d 2050 6167 650d 0a0d   model = Page...
-00000c60: 0a20 2020 206b 6c61 7373 3d22 5761 6774  .    klass="Wagt
-00000c70: 6169 6c4c 696e 6b54 6f6f 6c22 0d0a 2020  ailLinkTool"..  
-00000c80: 2020 6a73 203d 205b 0d0a 2020 2020 2020    js = [..      
-00000c90: 2020 2277 6167 7461 696c 5f65 6469 746f    "wagtail_edito
-00000ca0: 726a 732f 6a73 2f74 6f6f 6c73 2f77 6167  rjs/js/tools/wag
-00000cb0: 7461 696c 2d63 686f 6f73 6572 2d74 6f6f  tail-chooser-too
-00000cc0: 6c2e 6a73 222c 0d0a 2020 2020 2020 2020  l.js",..        
-00000cd0: 2277 6167 7461 696c 5f65 6469 746f 726a  "wagtail_editorj
-00000ce0: 732f 6a73 2f74 6f6f 6c73 2f77 6167 7461  s/js/tools/wagta
-00000cf0: 696c 2d6c 696e 6b2e 6a73 222c 0d0a 2020  il-link.js",..  
-00000d00: 2020 5d0d 0a0d 0a20 2020 2040 636c 6173    ]....    @clas
-00000d10: 736d 6574 686f 640d 0a20 2020 2064 6566  smethod..    def
-00000d20: 2067 6574 5f74 6573 745f 6461 7461 2863   get_test_data(c
-00000d30: 6c73 293a 0d0a 2020 2020 2020 2020 6d6f  ls):..        mo
-00000d40: 6465 6c73 203d 2063 6c73 2e67 6574 5f74  dels = cls.get_t
-00000d50: 6573 745f 7175 6572 7973 6574 2829 5b30  est_queryset()[0
-00000d60: 3a35 5d0d 0a20 2020 2020 2020 2072 6574  :5]..        ret
-00000d70: 7572 6e20 5b0d 0a20 2020 2020 2020 2020  urn [..         
-00000d80: 2020 2028 0d0a 2020 2020 2020 2020 2020     (..          
-00000d90: 2020 2020 2020 2320 4f76 6572 7269 6465        # Override
-00000da0: 2074 6f20 6164 6420 6461 7461 2d61 7574   to add data-aut
-00000db0: 6f63 6f6d 706c 6574 652e 0d0a 2020 2020  ocomplete...    
-00000dc0: 2020 2020 2020 2020 2020 2020 6622 3c61              f"<a
-00000dd0: 2064 6174 612d 6964 3d27 7b6d 6f64 656c   data-id='{model
-00000de0: 2e69 647d 2720 6461 7461 2d7b 636c 732e  .id}' data-{cls.
-00000df0: 6d6f 6465 6c2e 5f6d 6574 612e 6d6f 6465  model._meta.mode
-00000e00: 6c5f 6e61 6d65 7d3d 2754 7275 6527 2064  l_name}='True' d
-00000e10: 6174 612d 7061 7265 6e74 2d69 643d 2774  ata-parent-id='t
-00000e20: 6869 732d 646f 6573 6e74 2d67 6574 2d75  his-doesnt-get-u
-00000e30: 7365 6427 3e3c 2f61 3e22 2c0d 0a20 2020  sed'></a>",..   
-00000e40: 2020 2020 2020 2020 2020 2020 2066 223c               f"<
-00000e50: 6120 6872 6566 3d27 7b63 6c73 2e67 6574  a href='{cls.get
-00000e60: 5f75 726c 286d 6f64 656c 297d 2720 636c  _url(model)}' cl
-00000e70: 6173 733d 277b 636c 732e 6d6f 6465 6c2e  ass='{cls.model.
-00000e80: 5f6d 6574 612e 6d6f 6465 6c5f 6e61 6d65  _meta.model_name
-00000e90: 7d2d 6c69 6e6b 273e 3c2f 613e 222c 0d0a  }-link'></a>",..
-00000ea0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00000eb0: 2020 2020 2020 2020 2020 2066 6f72 206d             for m
-00000ec0: 6f64 656c 2069 6e20 6d6f 6465 6c73 0d0a  odel in models..
-00000ed0: 2020 2020 2020 2020 5d0d 0a0d 0a0d 0a53          ]......S
-00000ee0: 4541 5243 485f 5155 4552 595f 5041 5241  EARCH_QUERY_PARA
-00000ef0: 4d20 3d20 2273 6561 7263 6822 0d0a 434f  M = "search"..CO
-00000f00: 4e53 5452 5543 545f 5041 4745 5f51 5545  NSTRUCT_PAGE_QUE
-00000f10: 5259 5345 5420 3d20 2263 6f6e 7374 7275  RYSET = "constru
-00000f20: 6374 5f70 6167 655f 7175 6572 7973 6574  ct_page_queryset
-00000f30: 220d 0a42 5549 4c44 5f50 4147 455f 4441  "..BUILD_PAGE_DA
-00000f40: 5441 203d 2022 6275 696c 645f 7061 6765  TA = "build_page
-00000f50: 5f64 6174 6122 0d0a 0d0a 0d0a 636c 6173  _data"......clas
-00000f60: 7320 4c69 6e6b 4175 746f 436f 6d70 6c65  s LinkAutoComple
-00000f70: 7465 4665 6174 7572 6528 4665 6174 7572  teFeature(Featur
-00000f80: 6556 6965 774d 6978 696e 2c20 4261 7365  eViewMixin, Base
-00000f90: 5061 6765 4c69 6e6b 4d69 7869 6e2c 204d  PageLinkMixin, M
-00000fa0: 6f64 656c 496e 6c69 6e65 4564 6974 6f72  odelInlineEditor
-00000fb0: 4a53 4665 6174 7572 6529 3a0d 0a20 2020  JSFeature):..   
-00000fc0: 2061 6c6c 6f77 6564 5f74 6167 7320 3d20   allowed_tags = 
-00000fd0: 5b22 6122 5d0d 0a20 2020 2061 6c6c 6f77  ["a"]..    allow
-00000fe0: 6564 5f61 7474 7269 6275 7465 7320 3d20  ed_attributes = 
-00000ff0: 4261 7365 5061 6765 4c69 6e6b 4d69 7869  BasePageLinkMixi
-00001000: 6e2e 616c 6c6f 7765 645f 6174 7472 6962  n.allowed_attrib
-00001010: 7574 6573 202b 205b 0d0a 2020 2020 2020  utes + [..      
-00001020: 2020 2263 6c61 7373 222c 2022 6872 6566    "class", "href
-00001030: 222c 2022 6461 7461 2d69 6422 0d0a 2020  ", "data-id"..  
-00001040: 2020 5d0d 0a20 2020 206d 7573 745f 6861    ]..    must_ha
-00001050: 7665 5f61 7474 7273 203d 207b 0d0a 2020  ve_attrs = {..  
-00001060: 2020 2020 2020 2264 6174 612d 6175 746f        "data-auto
-00001070: 636f 6d70 6c65 7465 223a 2022 7061 6765  complete": "page
-00001080: 222c 0d0a 2020 2020 7d0d 0a20 2020 2063  ",..    }..    c
-00001090: 686f 6f73 6572 5f63 6c61 7373 203d 2041  hooser_class = A
-000010a0: 646d 696e 5061 6765 4368 6f6f 7365 720d  dminPageChooser.
-000010b0: 0a20 2020 206d 6f64 656c 203d 2050 6167  .    model = Pag
-000010c0: 650d 0a20 2020 206b 6c61 7373 3d22 4c69  e..    klass="Li
-000010d0: 6e6b 4175 746f 636f 6d70 6c65 7465 220d  nkAutocomplete".
-000010e0: 0a20 2020 206a 7320 3d20 5b0d 0a20 2020  .    js = [..   
-000010f0: 2020 2020 2022 7761 6774 6169 6c5f 6564       "wagtail_ed
-00001100: 6974 6f72 6a73 2f76 656e 646f 722f 6564  itorjs/vendor/ed
-00001110: 6974 6f72 6a73 2f74 6f6f 6c73 2f6c 696e  itorjs/tools/lin
-00001120: 6b2d 6175 746f 636f 6d70 6c65 7465 2e6a  k-autocomplete.j
-00001130: 7322 2c0d 0a20 2020 205d 0d0a 0d0a 2020  s",..    ]....  
-00001140: 2020 6465 6620 6765 745f 636f 6e66 6967    def get_config
-00001150: 2873 656c 662c 2063 6f6e 7465 7874 3a20  (self, context: 
-00001160: 6469 6374 5b73 7472 2c20 416e 795d 293a  dict[str, Any]):
-00001170: 0d0a 2020 2020 2020 2020 636f 6e66 6967  ..        config
-00001180: 203d 2073 7570 6572 284d 6f64 656c 496e   = super(ModelIn
-00001190: 6c69 6e65 4564 6974 6f72 4a53 4665 6174  lineEditorJSFeat
-000011a0: 7572 652c 2073 656c 6629 2e67 6574 5f63  ure, self).get_c
-000011b0: 6f6e 6669 6728 636f 6e74 6578 7429 0d0a  onfig(context)..
-000011c0: 2020 2020 2020 2020 636f 6e66 6967 2e73          config.s
-000011d0: 6574 6465 6661 756c 7428 2263 6f6e 6669  etdefault("confi
-000011e0: 6722 2c20 7b7d 290d 0a20 2020 2020 2020  g", {})..       
-000011f0: 2063 6f6e 6669 675b 2263 6f6e 6669 6722   config["config"
-00001200: 5d5b 2265 6e64 706f 696e 7422 5d20 3d20  ]["endpoint"] = 
-00001210: 7265 7665 7273 6528 6622 7761 6774 6169  reverse(f"wagtai
-00001220: 6c5f 6564 6974 6f72 6a73 3a7b 7365 6c66  l_editorjs:{self
-00001230: 2e74 6f6f 6c5f 6e61 6d65 7d22 290d 0a20  .tool_name}").. 
-00001240: 2020 2020 2020 2063 6f6e 6669 675b 2263         config["c
-00001250: 6f6e 6669 6722 5d5b 2271 7565 7279 5061  onfig"]["queryPa
-00001260: 7261 6d22 5d20 3d20 2273 6561 7263 6822  ram"] = "search"
-00001270: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001280: 2063 6f6e 6669 670d 0a0d 0a20 2020 2040   config....    @
-00001290: 636c 6173 736d 6574 686f 640d 0a20 2020  classmethod..   
-000012a0: 2064 6566 2067 6574 5f74 6573 745f 6461   def get_test_da
-000012b0: 7461 2863 6c73 293a 0d0a 2020 2020 2020  ta(cls):..      
-000012c0: 2020 6d6f 6465 6c73 203d 2063 6c73 2e67    models = cls.g
-000012d0: 6574 5f74 6573 745f 7175 6572 7973 6574  et_test_queryset
-000012e0: 2829 5b30 3a35 5d0d 0a20 2020 2020 2020  ()[0:5]..       
-000012f0: 2072 6574 7572 6e20 5b0d 0a20 2020 2020   return [..     
-00001300: 2020 2020 2020 2028 0d0a 2020 2020 2020         (..      
-00001310: 2020 2020 2020 2020 2020 2320 4f76 6572            # Over
-00001320: 7269 6465 2074 6f20 6164 6420 6461 7461  ride to add data
-00001330: 2d61 7574 6f63 6f6d 706c 6574 652e 0d0a  -autocomplete...
-00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001350: 6622 3c61 2064 6174 612d 6964 3d27 7b6d  f"<a data-id='{m
-00001360: 6f64 656c 2e69 647d 2720 6461 7461 2d7b  odel.id}' data-{
-00001370: 636c 732e 6d6f 6465 6c2e 5f6d 6574 612e  cls.model._meta.
-00001380: 6d6f 6465 6c5f 6e61 6d65 7d3d 2754 7275  model_name}='Tru
-00001390: 6527 2064 6174 612d 6175 746f 636f 6d70  e' data-autocomp
-000013a0: 6c65 7465 3d27 7061 6765 273e 3c2f 613e  lete='page'></a>
-000013b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000013c0: 2020 2020 6622 3c61 2068 7265 663d 277b      f"<a href='{
-000013d0: 636c 732e 6765 745f 7572 6c28 6d6f 6465  cls.get_url(mode
-000013e0: 6c29 7d27 2063 6c61 7373 3d27 7b63 6c73  l)}' class='{cls
-000013f0: 2e6d 6f64 656c 2e5f 6d65 7461 2e6d 6f64  .model._meta.mod
-00001400: 656c 5f6e 616d 657d 2d6c 696e 6b27 3e3c  el_name}-link'><
-00001410: 2f61 3e22 2c0d 0a20 2020 2020 2020 2020  /a>",..         
-00001420: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-00001430: 2020 666f 7220 6d6f 6465 6c20 696e 206d    for model in m
-00001440: 6f64 656c 730d 0a20 2020 2020 2020 205d  odels..        ]
-00001450: 0d0a 0d0a 2020 2020 6465 6620 6861 6e64  ....    def hand
-00001460: 6c65 5f67 6574 2873 656c 662c 2072 6571  le_get(self, req
-00001470: 7565 7374 293a 0d0a 2020 2020 2020 2020  uest):..        
-00001480: 2222 220d 0a20 2020 2020 2020 2041 7574  """..        Aut
-00001490: 6f63 6f6d 706c 6574 6520 666f 7220 696e  ocomplete for in
-000014a0: 7465 726e 616c 206c 696e 6b73 0d0a 2020  ternal links..  
-000014b0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000014c0: 2020 2073 6561 7263 6820 3d20 7265 7175     search = requ
-000014d0: 6573 742e 4745 542e 6765 7428 5345 4152  est.GET.get(SEAR
-000014e0: 4348 5f51 5545 5259 5f50 4152 414d 290d  CH_QUERY_PARAM).
-000014f0: 0a0d 0a20 2020 2020 2020 2070 6167 6573  ...        pages
-00001500: 203d 2050 6167 652e 6f62 6a65 6374 732e   = Page.objects.
-00001510: 616c 6c28 295c 0d0a 2020 2020 2020 2020  all()\..        
-00001520: 2020 2020 2e6c 6976 6528 295c 0d0a 2020      .live()\..  
-00001530: 2020 2020 2020 2020 2020 2e73 7065 6369            .speci
-00001540: 6669 6328 290d 0a0d 0a20 2020 2020 2020  fic()....       
-00001550: 2066 6f72 2066 6e20 696e 2068 6f6f 6b73   for fn in hooks
-00001560: 2e67 6574 5f68 6f6f 6b73 2843 4f4e 5354  .get_hooks(CONST
-00001570: 5255 4354 5f50 4147 455f 5155 4552 5953  RUCT_PAGE_QUERYS
-00001580: 4554 293a 0d0a 2020 2020 2020 2020 2020  ET):..          
-00001590: 2020 7061 6765 7320 3d20 666e 2872 6571    pages = fn(req
-000015a0: 7565 7374 2c20 7061 6765 732c 2073 6561  uest, pages, sea
-000015b0: 7263 6829 0d0a 0d0a 2020 2020 2020 2020  rch)....        
-000015c0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000015d0: 6528 7061 6765 732c 2048 7474 7052 6573  e(pages, HttpRes
-000015e0: 706f 6e73 6529 3a0d 0a20 2020 2020 2020  ponse):..       
-000015f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001600: 7061 6765 730d 0a0d 0a20 2020 2020 2020  pages....       
-00001610: 2069 6620 7365 6172 6368 3a0d 0a20 2020   if search:..   
-00001620: 2020 2020 2020 2020 2070 6167 6573 203d           pages =
-00001630: 2070 6167 6573 2e73 6561 7263 6828 7365   pages.search(se
-00001640: 6172 6368 290d 0a0d 0a0d 0a20 2020 2020  arch)......     
-00001650: 2020 2070 6167 655f 6c69 7374 203d 205b     page_list = [
-00001660: 5d0d 0a20 2020 2020 2020 2070 6167 655f  ]..        page_
-00001670: 6461 7461 5f68 6f6f 6b73 203d 2068 6f6f  data_hooks = hoo
-00001680: 6b73 2e67 6574 5f68 6f6f 6b73 2842 5549  ks.get_hooks(BUI
-00001690: 4c44 5f50 4147 455f 4441 5441 290d 0a20  LD_PAGE_DATA).. 
-000016a0: 2020 2020 2020 2066 6f72 2070 6167 6520         for page 
-000016b0: 696e 2070 6167 6573 3a0d 0a20 2020 2020  in pages:..     
-000016c0: 2020 2020 2020 2064 6174 6120 3d20 7b0d         data = {.
-000016d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000016e0: 2027 6964 273a 2070 6167 652e 6964 2c0d   'id': page.id,.
-000016f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001700: 2027 6e61 6d65 273a 2070 6167 652e 7469   'name': page.ti
-00001710: 746c 652c 0d0a 2020 2020 2020 2020 2020  tle,..          
-00001720: 2020 2020 2020 2768 7265 6627 3a20 7061        'href': pa
-00001730: 6765 2e67 6574 5f75 726c 2872 6571 7565  ge.get_url(reque
-00001740: 7374 292c 0d0a 2020 2020 2020 2020 2020  st),..          
-00001750: 2020 2020 2020 2764 6573 6372 6970 7469        'descripti
-00001760: 6f6e 273a 2070 6167 652e 7365 6172 6368  on': page.search
-00001770: 5f64 6573 6372 6970 7469 6f6e 2c0d 0a20  _description,.. 
-00001780: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001790: 6175 746f 636f 6d70 6c65 7465 273a 2027  autocomplete': '
-000017a0: 7061 6765 272c 0d0a 2020 2020 2020 2020  page',..        
-000017b0: 2020 2020 2020 2020 2770 6167 6527 3a20          'page': 
-000017c0: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-000017d0: 2020 207d 0d0a 0d0a 2020 2020 2020 2020     }....        
-000017e0: 2020 2020 666f 7220 686f 6f6b 2069 6e20      for hook in 
-000017f0: 7061 6765 5f64 6174 615f 686f 6f6b 733a  page_data_hooks:
-00001800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001810: 2020 686f 6f6b 2872 6571 7565 7374 2c20    hook(request, 
-00001820: 7061 6765 2c20 6461 7461 290d 0a0d 0a20  page, data).... 
-00001830: 2020 2020 2020 2020 2020 2070 6167 655f             page_
-00001840: 6c69 7374 2e61 7070 656e 6428 6461 7461  list.append(data
-00001850: 290d 0a0d 0a0d 0a20 2020 2020 2020 2072  )......        r
-00001860: 6574 7572 6e20 4a73 6f6e 5265 7370 6f6e  eturn JsonRespon
-00001870: 7365 287b 0d0a 2020 2020 2020 2020 2020  se({..          
-00001880: 2020 2020 2020 2273 7563 6365 7373 223a        "success":
-00001890: 2054 7275 652c 0d0a 2020 2020 2020 2020   True,..        
-000018a0: 2020 2020 2020 2020 2269 7465 6d73 223a          "items":
-000018b0: 2070 6167 655f 6c69 7374 2c0d 0a20 2020   page_list,..   
-000018c0: 2020 2020 2020 2020 207d 2c0d 0a20 2020           },..   
-000018d0: 2020 2020 2020 2020 2073 7461 7475 733d           status=
-000018e0: 3230 302c 0d0a 2020 2020 2020 2020 290d  200,..        ).
-000018f0: 0a0d 0a0d 0a63 6c61 7373 2044 6f63 756d  .....class Docum
-00001900: 656e 7446 6561 7475 7265 284d 6f64 656c  entFeature(Model
-00001910: 496e 6c69 6e65 4564 6974 6f72 4a53 4665  InlineEditorJSFe
-00001920: 6174 7572 6529 3a0d 0a20 2020 2061 6c6c  ature):..    all
-00001930: 6f77 6564 5f74 6167 7320 3d20 5b22 6122  owed_tags = ["a"
-00001940: 5d0d 0a20 2020 2061 6c6c 6f77 6564 5f61  ]..    allowed_a
-00001950: 7474 7269 6275 7465 7320 3d20 5b22 636c  ttributes = ["cl
-00001960: 6173 7322 2c20 2268 7265 6622 2c20 2264  ass", "href", "d
-00001970: 6174 612d 6964 225d 0d0a 2020 2020 6368  ata-id"]..    ch
-00001980: 6f6f 7365 725f 636c 6173 7320 3d20 4164  ooser_class = Ad
-00001990: 6d69 6e44 6f63 756d 656e 7443 686f 6f73  minDocumentChoos
-000019a0: 6572 0d0a 2020 2020 6d6f 6465 6c20 3d20  er..    model = 
-000019b0: 446f 6375 6d65 6e74 0d0a 2020 2020 6b6c  Document..    kl
-000019c0: 6173 7320 3d20 2257 6167 7461 696c 446f  ass = "WagtailDo
-000019d0: 6375 6d65 6e74 546f 6f6c 220d 0a20 2020  cumentTool"..   
-000019e0: 206a 7320 3d20 5b0d 0a20 2020 2020 2020   js = [..       
-000019f0: 2022 7761 6774 6169 6c5f 6564 6974 6f72   "wagtail_editor
-00001a00: 6a73 2f6a 732f 746f 6f6c 732f 7761 6774  js/js/tools/wagt
-00001a10: 6169 6c2d 6368 6f6f 7365 722d 746f 6f6c  ail-chooser-tool
-00001a20: 2e6a 7322 2c0d 0a20 2020 2020 2020 2022  .js",..        "
-00001a30: 7761 6774 6169 6c5f 6564 6974 6f72 6a73  wagtail_editorjs
-00001a40: 2f6a 732f 746f 6f6c 732f 7761 6774 6169  /js/tools/wagtai
-00001a50: 6c2d 646f 6375 6d65 6e74 2e6a 7322 2c0d  l-document.js",.
-00001a60: 0a20 2020 205d 0d0a 0d0a 2020 2020 4063  .    ]....    @c
-00001a70: 6c61 7373 6d65 7468 6f64 0d0a 2020 2020  lassmethod..    
-00001a80: 6465 6620 6765 745f 7572 6c28 636c 732c  def get_url(cls,
-00001a90: 2069 6e73 7461 6e63 6529 3a0d 0a20 2020   instance):..   
-00001aa0: 2020 2020 2072 6574 7572 6e20 696e 7374       return inst
-00001ab0: 616e 6365 2e66 696c 652e 7572 6c0d 0a0d  ance.file.url...
-00001ac0: 0a                                       .
+00000590: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+000005a0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+000005b0: 2020 2066 223c 7370 616e 2063 6c61 7373     f"<span class
+000005c0: 3d27 7761 6774 6169 6c2d 746f 6f6c 7469  ='wagtail-toolti
+000005d0: 7027 2064 6174 612d 772d 746f 6f6c 7469  p' data-w-toolti
+000005e0: 702d 636f 6e74 656e 742d 7661 6c75 653d  p-content-value=
+000005f0: 2754 6f6f 6c74 6970 2063 6f6e 7465 6e74  'Tooltip content
+00000600: 273e 3c2f 7370 616e 3e22 2c0d 0a20 2020  '></span>",..   
+00000610: 2020 2020 2020 2020 2020 2020 2066 223c               f"<
+00000620: 7370 616e 2063 6c61 7373 3d27 7761 6774  span class='wagt
+00000630: 6169 6c2d 746f 6f6c 7469 7027 2064 6174  ail-tooltip' dat
+00000640: 612d 7469 7070 792d 636f 6e74 656e 743d  a-tippy-content=
+00000650: 2754 6f6f 6c74 6970 2063 6f6e 7465 6e74  'Tooltip content
+00000660: 2720 6461 7461 2d74 6970 7079 2d70 6c61  ' data-tippy-pla
+00000670: 6365 6d65 6e74 3d27 626f 7474 6f6d 2720  cement='bottom' 
+00000680: 6461 7461 2d74 6970 7079 2d66 6f6c 6c6f  data-tippy-follo
+00000690: 772d 6375 7273 6f72 3d27 686f 7269 7a6f  w-cursor='horizo
+000006a0: 6e74 616c 273e 3c2f 7370 616e 3e22 2c0d  ntal'></span>",.
+000006b0: 0a20 2020 2020 2020 2020 2020 2029 2c0d  .            ),.
+000006c0: 0a20 2020 2020 2020 2020 2020 2028 0d0a  .            (..
+000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006e0: 6622 3c73 7061 6e20 636c 6173 733d 2777  f"<span class='w
+000006f0: 6167 7461 696c 2d74 6f6f 6c74 6970 2720  agtail-tooltip' 
+00000700: 6461 7461 2d77 2d74 6f6f 6c74 6970 2d63  data-w-tooltip-c
+00000710: 6f6e 7465 6e74 2d76 616c 7565 3d27 546f  ontent-value='To
+00000720: 6f6c 7469 7020 636f 6e74 656e 7427 2064  oltip content' d
+00000730: 6174 612d 772d 746f 6f6c 7469 702d 706c  ata-w-tooltip-pl
+00000740: 6163 656d 656e 742d 7661 6c75 653d 2774  acement-value='t
+00000750: 6f70 273e 3c2f 7370 616e 3e22 2c0d 0a20  op'></span>",.. 
+00000760: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00000770: 223c 7370 616e 2063 6c61 7373 3d27 7761  "<span class='wa
+00000780: 6774 6169 6c2d 746f 6f6c 7469 7027 2064  gtail-tooltip' d
+00000790: 6174 612d 7469 7070 792d 636f 6e74 656e  ata-tippy-conten
+000007a0: 743d 2754 6f6f 6c74 6970 2063 6f6e 7465  t='Tooltip conte
+000007b0: 6e74 2720 6461 7461 2d74 6970 7079 2d70  nt' data-tippy-p
+000007c0: 6c61 6365 6d65 6e74 3d27 746f 7027 2064  lacement='top' d
+000007d0: 6174 612d 7469 7070 792d 666f 6c6c 6f77  ata-tippy-follow
+000007e0: 2d63 7572 736f 723d 2768 6f72 697a 6f6e  -cursor='horizon
+000007f0: 7461 6c27 3e3c 2f73 7061 6e3e 222c 0d0a  tal'></span>",..
+00000800: 2020 2020 2020 2020 2020 2020 292c 0d0a              ),..
+00000810: 2020 2020 2020 2020 5d0d 0a0d 0a20 2020          ]....   
+00000820: 2064 6566 2062 7569 6c64 5f65 6c65 6d65   def build_eleme
+00000830: 6e74 7328 7365 6c66 2c20 696e 6c69 6e65  nts(self, inline
+00000840: 5f64 6174 613a 206c 6973 742c 2063 6f6e  _data: list, con
+00000850: 7465 7874 3a20 6469 6374 5b73 7472 2c20  text: dict[str, 
+00000860: 416e 795d 203d 204e 6f6e 6529 202d 3e20  Any] = None) -> 
+00000870: 6c69 7374 3a0d 0a20 2020 2020 2020 2066  list:..        f
+00000880: 6f72 2065 6c65 6d65 6e74 2c20 6174 7472  or element, attr
+00000890: 7320 696e 2069 6e6c 696e 655f 6461 7461  s in inline_data
+000008a0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+000008b0: 2065 6c65 6d65 6e74 2e61 7474 7273 2e63   element.attrs.c
+000008c0: 6c65 6172 2829 0d0a 2020 2020 2020 2020  lear()..        
+000008d0: 2020 2020 656c 656d 656e 745b 2263 6c61      element["cla
+000008e0: 7373 225d 203d 2022 7761 6774 6169 6c2d  ss"] = "wagtail-
+000008f0: 746f 6f6c 7469 7022 0d0a 0d0a 2020 2020  tooltip"....    
+00000900: 2020 2020 2020 2020 656c 656d 656e 745b          element[
+00000910: 2264 6174 612d 7469 7070 792d 666f 6c6c  "data-tippy-foll
+00000920: 6f77 2d63 7572 736f 7222 5d20 3d20 2268  ow-cursor"] = "h
+00000930: 6f72 697a 6f6e 7461 6c22 0d0a 0d0a 2020  orizontal"....  
+00000940: 2020 2020 2020 2020 2020 2320 4173 2070            # As p
+00000950: 6572 2077 6167 7461 696c 2064 6f63 756d  er wagtail docum
+00000960: 656e 7461 7469 6f6e 2064 6566 6175 6c74  entation default
+00000970: 2069 7320 626f 7474 6f6d 2e0d 0a20 2020   is bottom...   
+00000980: 2020 2020 2020 2020 2061 7474 7273 2e73           attrs.s
+00000990: 6574 6465 6661 756c 7428 2264 6174 612d  etdefault("data-
+000009a0: 772d 746f 6f6c 7469 702d 706c 6163 656d  w-tooltip-placem
+000009b0: 656e 742d 7661 6c75 6522 2c20 2262 6f74  ent-value", "bot
+000009c0: 746f 6d22 290d 0a0d 0a20 2020 2020 2020  tom")....       
+000009d0: 2020 2020 2066 6f72 206b 2c20 7620 696e       for k, v in
+000009e0: 2061 7474 7273 2e69 7465 6d73 2829 3a0d   attrs.items():.
+000009f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a00: 2069 6620 6e6f 7420 6b2e 7374 6172 7473   if not k.starts
+00000a10: 7769 7468 2822 6461 7461 2d77 2d74 6f6f  with("data-w-too
+00000a20: 6c74 6970 2d22 2920 6f72 206e 6f74 206b  ltip-") or not k
+00000a30: 2e65 6e64 7377 6974 6828 222d 7661 6c75  .endswith("-valu
+00000a40: 6522 293a 0d0a 2020 2020 2020 2020 2020  e"):..          
+00000a50: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00000a60: 7565 0d0a 0d0a 2020 2020 2020 2020 2020  ue....          
+00000a70: 2020 2020 2020 6b20 3d20 6b2e 7265 706c        k = k.repl
+00000a80: 6163 6528 2264 6174 612d 772d 746f 6f6c  ace("data-w-tool
+00000a90: 7469 702d 222c 2022 6461 7461 2d74 6970  tip-", "data-tip
+00000aa0: 7079 2d22 290d 0a20 2020 2020 2020 2020  py-")..         
+00000ab0: 2020 2020 2020 206b 203d 206b 5b3a 2d36         k = k[:-6
+00000ac0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00000ad0: 2020 2020 2065 6c65 6d65 6e74 5b6b 5d20       element[k] 
+00000ae0: 3d20 760d 0a0d 0a0d 0a63 6c61 7373 2042  = v......class B
+00000af0: 6173 6550 6167 654c 696e 6b4d 6978 696e  asePageLinkMixin
+00000b00: 2850 6167 6543 686f 6f73 6572 5552 4c73  (PageChooserURLs
+00000b10: 4d69 7869 6e29 3a0d 0a20 2020 2061 6c6c  Mixin):..    all
+00000b20: 6f77 6564 5f61 7474 7269 6275 7465 7320  owed_attributes 
+00000b30: 3d20 5b22 7461 7267 6574 222c 2022 7265  = ["target", "re
+00000b40: 6c22 5d0d 0a20 2020 2063 616e 5f68 6176  l"]..    can_hav
+00000b50: 655f 6174 7472 7320 3d20 7b0d 0a20 2020  e_attrs = {..   
+00000b60: 2020 2020 2022 6461 7461 2d74 6172 6765       "data-targe
+00000b70: 7422 3a20 4e6f 6e65 2c0d 0a20 2020 2020  t": None,..     
+00000b80: 2020 2022 6461 7461 2d72 656c 223a 204e     "data-rel": N
+00000b90: 6f6e 652c 0d0a 2020 2020 7d0d 0a0d 0a20  one,..    }.... 
+00000ba0: 2020 2064 6566 2062 7569 6c64 5f65 6c65     def build_ele
+00000bb0: 6d65 6e74 2873 656c 662c 2069 7465 6d2c  ment(self, item,
+00000bc0: 206f 626a 2c20 636f 6e74 6578 743a 2064   obj, context: d
+00000bd0: 6963 745b 7374 722c 2041 6e79 5d20 3d20  ict[str, Any] = 
+00000be0: 4e6f 6e65 2c20 6461 7461 3a20 6469 6374  None, data: dict
+00000bf0: 5b73 7472 2c20 416e 795d 203d 204e 6f6e  [str, Any] = Non
+00000c00: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
+00000c10: 4275 696c 6420 7468 6520 656c 656d 656e  Build the elemen
+00000c20: 7420 6672 6f6d 2074 6865 206f 626a 6563  t from the objec
+00000c30: 742e 2222 220d 0a20 2020 2020 2020 2073  t."""..        s
+00000c40: 7570 6572 2829 2e62 7569 6c64 5f65 6c65  uper().build_ele
+00000c50: 6d65 6e74 2869 7465 6d2c 206f 626a 2c20  ment(item, obj, 
+00000c60: 636f 6e74 6578 742c 2064 6174 6129 0d0a  context, data)..
+00000c70: 2020 2020 2020 2020 6966 2022 6461 7461          if "data
+00000c80: 2d74 6172 6765 7422 2069 6e20 6461 7461  -target" in data
+00000c90: 2061 6e64 2064 6174 615b 2264 6174 612d   and data["data-
+00000ca0: 7461 7267 6574 225d 3a0d 0a20 2020 2020  target"]:..     
+00000cb0: 2020 2020 2020 2069 7465 6d5b 2274 6172         item["tar
+00000cc0: 6765 7422 5d20 3d20 6461 7461 5b22 6461  get"] = data["da
+00000cd0: 7461 2d74 6172 6765 7422 5d0d 0a20 2020  ta-target"]..   
+00000ce0: 2020 2020 2069 6620 2264 6174 612d 7265       if "data-re
+00000cf0: 6c22 2069 6e20 6461 7461 2061 6e64 2064  l" in data and d
+00000d00: 6174 615b 2264 6174 612d 7265 6c22 5d3a  ata["data-rel"]:
+00000d10: 0d0a 2020 2020 2020 2020 2020 2020 6974  ..            it
+00000d20: 656d 5b22 7265 6c22 5d20 3d20 6461 7461  em["rel"] = data
+00000d30: 5b22 6461 7461 2d72 656c 225d 0d0a 0d0a  ["data-rel"]....
+00000d40: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00000d50: 0d0a 2020 2020 6465 6620 6765 745f 7572  ..    def get_ur
+00000d60: 6c28 636c 732c 2069 6e73 7461 6e63 6529  l(cls, instance)
+00000d70: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+00000d80: 6e20 696e 7374 616e 6365 2e67 6574 5f75  n instance.get_u
+00000d90: 726c 2829 0d0a 0d0a 2020 2020 4063 6c61  rl()....    @cla
+00000da0: 7373 6d65 7468 6f64 0d0a 2020 2020 6465  ssmethod..    de
+00000db0: 6620 6765 745f 6675 6c6c 5f75 726c 2863  f get_full_url(c
+00000dc0: 6c73 2c20 696e 7374 616e 6365 2c20 7265  ls, instance, re
+00000dd0: 7175 6573 7429 3a0d 0a20 2020 2020 2020  quest):..       
+00000de0: 2072 6574 7572 6e20 696e 7374 616e 6365   return instance
+00000df0: 2e67 6574 5f66 756c 6c5f 7572 6c28 7265  .get_full_url(re
+00000e00: 7175 6573 7429 0d0a 2020 2020 0d0a 2020  quest)..    ..  
+00000e10: 2020 4063 6c61 7373 6d65 7468 6f64 0d0a    @classmethod..
+00000e20: 2020 2020 6465 6620 6765 745f 7465 7374      def get_test
+00000e30: 5f71 7565 7279 7365 7428 636c 7329 3a0d  _queryset(cls):.
+00000e40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000e50: 7375 7065 7228 292e 6765 745f 7465 7374  super().get_test
+00000e60: 5f71 7565 7279 7365 7428 292e 6669 6c74  _queryset().filt
+00000e70: 6572 2864 6570 7468 5f5f 6774 3d31 290d  er(depth__gt=1).
+00000e80: 0a0d 0a63 6c61 7373 204c 696e 6b46 6561  ...class LinkFea
+00000e90: 7475 7265 2842 6173 6550 6167 654c 696e  ture(BasePageLin
+00000ea0: 6b4d 6978 696e 2c20 4d6f 6465 6c49 6e6c  kMixin, ModelInl
+00000eb0: 696e 6545 6469 746f 724a 5346 6561 7475  ineEditorJSFeatu
+00000ec0: 7265 293a 0d0a 2020 2020 616c 6c6f 7765  re):..    allowe
+00000ed0: 645f 7461 6773 203d 205b 2261 225d 0d0a  d_tags = ["a"]..
+00000ee0: 2020 2020 616c 6c6f 7765 645f 6174 7472      allowed_attr
+00000ef0: 6962 7574 6573 203d 2042 6173 6550 6167  ibutes = BasePag
+00000f00: 654c 696e 6b4d 6978 696e 2e61 6c6c 6f77  eLinkMixin.allow
+00000f10: 6564 5f61 7474 7269 6275 7465 7320 2b20  ed_attributes + 
+00000f20: 5b0d 0a20 2020 2020 2020 2022 636c 6173  [..        "clas
+00000f30: 7322 2c20 2268 7265 6622 2c20 2264 6174  s", "href", "dat
+00000f40: 612d 6964 220d 0a20 2020 205d 0d0a 2020  a-id"..    ]..  
+00000f50: 2020 6d75 7374 5f68 6176 655f 6174 7472    must_have_attr
+00000f60: 7320 3d20 7b0d 0a20 2020 2020 2020 2022  s = {..        "
+00000f70: 6461 7461 2d70 6172 656e 742d 6964 223a  data-parent-id":
+00000f80: 204e 6f6e 652c 0d0a 2020 2020 7d0d 0a20   None,..    }.. 
+00000f90: 2020 2063 686f 6f73 6572 5f63 6c61 7373     chooser_class
+00000fa0: 203d 2041 646d 696e 5061 6765 4368 6f6f   = AdminPageChoo
+00000fb0: 7365 720d 0a20 2020 206d 6f64 656c 203d  ser..    model =
+00000fc0: 2050 6167 650d 0a0d 0a20 2020 206b 6c61   Page....    kla
+00000fd0: 7373 3d22 5761 6774 6169 6c4c 696e 6b54  ss="WagtailLinkT
+00000fe0: 6f6f 6c22 0d0a 2020 2020 6a73 203d 205b  ool"..    js = [
+00000ff0: 0d0a 2020 2020 2020 2020 2277 6167 7461  ..        "wagta
+00001000: 696c 5f65 6469 746f 726a 732f 6a73 2f74  il_editorjs/js/t
+00001010: 6f6f 6c73 2f77 6167 7461 696c 2d63 686f  ools/wagtail-cho
+00001020: 6f73 6572 2d74 6f6f 6c2e 6a73 222c 0d0a  oser-tool.js",..
+00001030: 2020 2020 2020 2020 2277 6167 7461 696c          "wagtail
+00001040: 5f65 6469 746f 726a 732f 6a73 2f74 6f6f  _editorjs/js/too
+00001050: 6c73 2f77 6167 7461 696c 2d6c 696e 6b2e  ls/wagtail-link.
+00001060: 6a73 222c 0d0a 2020 2020 5d0d 0a0d 0a20  js",..    ].... 
+00001070: 2020 2040 636c 6173 736d 6574 686f 640d     @classmethod.
+00001080: 0a20 2020 2064 6566 2067 6574 5f74 6573  .    def get_tes
+00001090: 745f 6461 7461 2863 6c73 293a 0d0a 2020  t_data(cls):..  
+000010a0: 2020 2020 2020 6d6f 6465 6c73 203d 2063        models = c
+000010b0: 6c73 2e67 6574 5f74 6573 745f 7175 6572  ls.get_test_quer
+000010c0: 7973 6574 2829 5b30 3a35 5d0d 0a20 2020  yset()[0:5]..   
+000010d0: 2020 2020 2072 6574 7572 6e20 5b0d 0a20       return [.. 
+000010e0: 2020 2020 2020 2020 2020 2028 0d0a 2020             (..  
+000010f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00001100: 4f76 6572 7269 6465 2074 6f20 6164 6420  Override to add 
+00001110: 6461 7461 2d61 7574 6f63 6f6d 706c 6574  data-autocomplet
+00001120: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
+00001130: 2020 2020 6622 3c61 2064 6174 612d 6964      f"<a data-id
+00001140: 3d27 7b6d 6f64 656c 2e69 647d 2720 6461  ='{model.id}' da
+00001150: 7461 2d7b 636c 732e 6d6f 6465 6c2e 5f6d  ta-{cls.model._m
+00001160: 6574 612e 6d6f 6465 6c5f 6e61 6d65 7d3d  eta.model_name}=
+00001170: 2754 7275 6527 2064 6174 612d 7061 7265  'True' data-pare
+00001180: 6e74 2d69 643d 2774 6869 732d 646f 6573  nt-id='this-does
+00001190: 6e74 2d67 6574 2d75 7365 6427 3e3c 2f61  nt-get-used'></a
+000011a0: 3e22 2c0d 0a20 2020 2020 2020 2020 2020  >",..           
+000011b0: 2020 2020 2066 223c 6120 6872 6566 3d27       f"<a href='
+000011c0: 7b63 6c73 2e67 6574 5f75 726c 286d 6f64  {cls.get_url(mod
+000011d0: 656c 297d 2720 636c 6173 733d 277b 636c  el)}' class='{cl
+000011e0: 732e 6d6f 6465 6c2e 5f6d 6574 612e 6d6f  s.model._meta.mo
+000011f0: 6465 6c5f 6e61 6d65 7d2d 6c69 6e6b 273e  del_name}-link'>
+00001200: 3c2f 613e 222c 0d0a 2020 2020 2020 2020  </a>",..        
+00001210: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00001220: 2020 2066 6f72 206d 6f64 656c 2069 6e20     for model in 
+00001230: 6d6f 6465 6c73 0d0a 2020 2020 2020 2020  models..        
+00001240: 5d0d 0a0d 0a0d 0a53 4541 5243 485f 5155  ]......SEARCH_QU
+00001250: 4552 595f 5041 5241 4d20 3d20 2273 6561  ERY_PARAM = "sea
+00001260: 7263 6822 0d0a 434f 4e53 5452 5543 545f  rch"..CONSTRUCT_
+00001270: 5041 4745 5f51 5545 5259 5345 5420 3d20  PAGE_QUERYSET = 
+00001280: 2263 6f6e 7374 7275 6374 5f70 6167 655f  "construct_page_
+00001290: 7175 6572 7973 6574 220d 0a42 5549 4c44  queryset"..BUILD
+000012a0: 5f50 4147 455f 4441 5441 203d 2022 6275  _PAGE_DATA = "bu
+000012b0: 696c 645f 7061 6765 5f64 6174 6122 0d0a  ild_page_data"..
+000012c0: 0d0a 0d0a 636c 6173 7320 4c69 6e6b 4175  ....class LinkAu
+000012d0: 746f 436f 6d70 6c65 7465 4665 6174 7572  toCompleteFeatur
+000012e0: 6528 4665 6174 7572 6556 6965 774d 6978  e(FeatureViewMix
+000012f0: 696e 2c20 4261 7365 5061 6765 4c69 6e6b  in, BasePageLink
+00001300: 4d69 7869 6e2c 204d 6f64 656c 496e 6c69  Mixin, ModelInli
+00001310: 6e65 4564 6974 6f72 4a53 4665 6174 7572  neEditorJSFeatur
+00001320: 6529 3a0d 0a20 2020 2061 6c6c 6f77 6564  e):..    allowed
+00001330: 5f74 6167 7320 3d20 5b22 6122 5d0d 0a20  _tags = ["a"].. 
+00001340: 2020 2061 6c6c 6f77 6564 5f61 7474 7269     allowed_attri
+00001350: 6275 7465 7320 3d20 4261 7365 5061 6765  butes = BasePage
+00001360: 4c69 6e6b 4d69 7869 6e2e 616c 6c6f 7765  LinkMixin.allowe
+00001370: 645f 6174 7472 6962 7574 6573 202b 205b  d_attributes + [
+00001380: 0d0a 2020 2020 2020 2020 2263 6c61 7373  ..        "class
+00001390: 222c 2022 6872 6566 222c 2022 6461 7461  ", "href", "data
+000013a0: 2d69 6422 0d0a 2020 2020 5d0d 0a20 2020  -id"..    ]..   
+000013b0: 206d 7573 745f 6861 7665 5f61 7474 7273   must_have_attrs
+000013c0: 203d 207b 0d0a 2020 2020 2020 2020 2264   = {..        "d
+000013d0: 6174 612d 6175 746f 636f 6d70 6c65 7465  ata-autocomplete
+000013e0: 223a 2022 7061 6765 222c 0d0a 2020 2020  ": "page",..    
+000013f0: 7d0d 0a20 2020 2063 686f 6f73 6572 5f63  }..    chooser_c
+00001400: 6c61 7373 203d 2041 646d 696e 5061 6765  lass = AdminPage
+00001410: 4368 6f6f 7365 720d 0a20 2020 206d 6f64  Chooser..    mod
+00001420: 656c 203d 2050 6167 650d 0a20 2020 206b  el = Page..    k
+00001430: 6c61 7373 3d22 4c69 6e6b 4175 746f 636f  lass="LinkAutoco
+00001440: 6d70 6c65 7465 220d 0a20 2020 206a 7320  mplete"..    js 
+00001450: 3d20 5b0d 0a20 2020 2020 2020 2022 7761  = [..        "wa
+00001460: 6774 6169 6c5f 6564 6974 6f72 6a73 2f76  gtail_editorjs/v
+00001470: 656e 646f 722f 6564 6974 6f72 6a73 2f74  endor/editorjs/t
+00001480: 6f6f 6c73 2f6c 696e 6b2d 6175 746f 636f  ools/link-autoco
+00001490: 6d70 6c65 7465 2e6a 7322 2c0d 0a20 2020  mplete.js",..   
+000014a0: 205d 0d0a 0d0a 2020 2020 6465 6620 6765   ]....    def ge
+000014b0: 745f 636f 6e66 6967 2873 656c 662c 2063  t_config(self, c
+000014c0: 6f6e 7465 7874 3a20 6469 6374 5b73 7472  ontext: dict[str
+000014d0: 2c20 416e 795d 293a 0d0a 2020 2020 2020  , Any]):..      
+000014e0: 2020 636f 6e66 6967 203d 2073 7570 6572    config = super
+000014f0: 284d 6f64 656c 496e 6c69 6e65 4564 6974  (ModelInlineEdit
+00001500: 6f72 4a53 4665 6174 7572 652c 2073 656c  orJSFeature, sel
+00001510: 6629 2e67 6574 5f63 6f6e 6669 6728 636f  f).get_config(co
+00001520: 6e74 6578 7429 0d0a 2020 2020 2020 2020  ntext)..        
+00001530: 636f 6e66 6967 2e73 6574 6465 6661 756c  config.setdefaul
+00001540: 7428 2263 6f6e 6669 6722 2c20 7b7d 290d  t("config", {}).
+00001550: 0a20 2020 2020 2020 2063 6f6e 6669 675b  .        config[
+00001560: 2263 6f6e 6669 6722 5d5b 2265 6e64 706f  "config"]["endpo
+00001570: 696e 7422 5d20 3d20 7265 7665 7273 6528  int"] = reverse(
+00001580: 6622 7761 6774 6169 6c5f 6564 6974 6f72  f"wagtail_editor
+00001590: 6a73 3a7b 7365 6c66 2e74 6f6f 6c5f 6e61  js:{self.tool_na
+000015a0: 6d65 7d22 290d 0a20 2020 2020 2020 2063  me}")..        c
+000015b0: 6f6e 6669 675b 2263 6f6e 6669 6722 5d5b  onfig["config"][
+000015c0: 2271 7565 7279 5061 7261 6d22 5d20 3d20  "queryParam"] = 
+000015d0: 2273 6561 7263 6822 0d0a 2020 2020 2020  "search"..      
+000015e0: 2020 7265 7475 726e 2063 6f6e 6669 670d    return config.
+000015f0: 0a0d 0a20 2020 2040 636c 6173 736d 6574  ...    @classmet
+00001600: 686f 640d 0a20 2020 2064 6566 2067 6574  hod..    def get
+00001610: 5f74 6573 745f 6461 7461 2863 6c73 293a  _test_data(cls):
+00001620: 0d0a 2020 2020 2020 2020 6d6f 6465 6c73  ..        models
+00001630: 203d 2063 6c73 2e67 6574 5f74 6573 745f   = cls.get_test_
+00001640: 7175 6572 7973 6574 2829 5b30 3a35 5d0d  queryset()[0:5].
+00001650: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001660: 5b0d 0a20 2020 2020 2020 2020 2020 2028  [..            (
+00001670: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001680: 2020 2320 4f76 6572 7269 6465 2074 6f20    # Override to 
+00001690: 6164 6420 6461 7461 2d61 7574 6f63 6f6d  add data-autocom
+000016a0: 706c 6574 652e 0d0a 2020 2020 2020 2020  plete...        
+000016b0: 2020 2020 2020 2020 6622 3c61 2064 6174          f"<a dat
+000016c0: 612d 6964 3d27 7b6d 6f64 656c 2e69 647d  a-id='{model.id}
+000016d0: 2720 6461 7461 2d7b 636c 732e 6d6f 6465  ' data-{cls.mode
+000016e0: 6c2e 5f6d 6574 612e 6d6f 6465 6c5f 6e61  l._meta.model_na
+000016f0: 6d65 7d3d 2754 7275 6527 2064 6174 612d  me}='True' data-
+00001700: 6175 746f 636f 6d70 6c65 7465 3d27 7061  autocomplete='pa
+00001710: 6765 273e 3c2f 613e 222c 0d0a 2020 2020  ge'></a>",..    
+00001720: 2020 2020 2020 2020 2020 2020 6622 3c61              f"<a
+00001730: 2068 7265 663d 277b 636c 732e 6765 745f   href='{cls.get_
+00001740: 7572 6c28 6d6f 6465 6c29 7d27 2063 6c61  url(model)}' cla
+00001750: 7373 3d27 7b63 6c73 2e6d 6f64 656c 2e5f  ss='{cls.model._
+00001760: 6d65 7461 2e6d 6f64 656c 5f6e 616d 657d  meta.model_name}
+00001770: 2d6c 696e 6b27 3e3c 2f61 3e22 2c0d 0a20  -link'></a>",.. 
+00001780: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00001790: 2020 2020 2020 2020 2020 666f 7220 6d6f            for mo
+000017a0: 6465 6c20 696e 206d 6f64 656c 730d 0a20  del in models.. 
+000017b0: 2020 2020 2020 205d 0d0a 0d0a 2020 2020         ]....    
+000017c0: 6465 6620 6861 6e64 6c65 5f67 6574 2873  def handle_get(s
+000017d0: 656c 662c 2072 6571 7565 7374 293a 0d0a  elf, request):..
+000017e0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+000017f0: 2020 2020 2041 7574 6f63 6f6d 706c 6574       Autocomplet
+00001800: 6520 666f 7220 696e 7465 726e 616c 206c  e for internal l
+00001810: 696e 6b73 0d0a 2020 2020 2020 2020 2222  inks..        ""
+00001820: 220d 0a20 2020 2020 2020 2073 6561 7263  "..        searc
+00001830: 6820 3d20 7265 7175 6573 742e 4745 542e  h = request.GET.
+00001840: 6765 7428 5345 4152 4348 5f51 5545 5259  get(SEARCH_QUERY
+00001850: 5f50 4152 414d 290d 0a0d 0a20 2020 2020  _PARAM)....     
+00001860: 2020 2070 6167 6573 203d 2050 6167 652e     pages = Page.
+00001870: 6f62 6a65 6374 732e 616c 6c28 295c 0d0a  objects.all()\..
+00001880: 2020 2020 2020 2020 2020 2020 2e6c 6976              .liv
+00001890: 6528 295c 0d0a 2020 2020 2020 2020 2020  e()\..          
+000018a0: 2020 2e73 7065 6369 6669 6328 290d 0a0d    .specific()...
+000018b0: 0a20 2020 2020 2020 2066 6f72 2066 6e20  .        for fn 
+000018c0: 696e 2068 6f6f 6b73 2e67 6574 5f68 6f6f  in hooks.get_hoo
+000018d0: 6b73 2843 4f4e 5354 5255 4354 5f50 4147  ks(CONSTRUCT_PAG
+000018e0: 455f 5155 4552 5953 4554 293a 0d0a 2020  E_QUERYSET):..  
+000018f0: 2020 2020 2020 2020 2020 7061 6765 7320            pages 
+00001900: 3d20 666e 2872 6571 7565 7374 2c20 7061  = fn(request, pa
+00001910: 6765 732c 2073 6561 7263 6829 0d0a 0d0a  ges, search)....
+00001920: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00001930: 7369 6e73 7461 6e63 6528 7061 6765 732c  sinstance(pages,
+00001940: 2048 7474 7052 6573 706f 6e73 6529 3a0d   HttpResponse):.
+00001950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001960: 2072 6574 7572 6e20 7061 6765 730d 0a0d   return pages...
+00001970: 0a20 2020 2020 2020 2069 6620 7365 6172  .        if sear
+00001980: 6368 3a0d 0a20 2020 2020 2020 2020 2020  ch:..           
+00001990: 2070 6167 6573 203d 2070 6167 6573 2e73   pages = pages.s
+000019a0: 6561 7263 6828 7365 6172 6368 290d 0a0d  earch(search)...
+000019b0: 0a0d 0a20 2020 2020 2020 2070 6167 655f  ...        page_
+000019c0: 6c69 7374 203d 205b 5d0d 0a20 2020 2020  list = []..     
+000019d0: 2020 2070 6167 655f 6461 7461 5f68 6f6f     page_data_hoo
+000019e0: 6b73 203d 2068 6f6f 6b73 2e67 6574 5f68  ks = hooks.get_h
+000019f0: 6f6f 6b73 2842 5549 4c44 5f50 4147 455f  ooks(BUILD_PAGE_
+00001a00: 4441 5441 290d 0a20 2020 2020 2020 2066  DATA)..        f
+00001a10: 6f72 2070 6167 6520 696e 2070 6167 6573  or page in pages
+00001a20: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+00001a30: 6174 6120 3d20 7b0d 0a20 2020 2020 2020  ata = {..       
+00001a40: 2020 2020 2020 2020 2027 6964 273a 2070           'id': p
+00001a50: 6167 652e 6964 2c0d 0a20 2020 2020 2020  age.id,..       
+00001a60: 2020 2020 2020 2020 2027 6e61 6d65 273a           'name':
+00001a70: 2070 6167 652e 7469 746c 652c 0d0a 2020   page.title,..  
+00001a80: 2020 2020 2020 2020 2020 2020 2020 2768                'h
+00001a90: 7265 6627 3a20 7061 6765 2e67 6574 5f75  ref': page.get_u
+00001aa0: 726c 2872 6571 7565 7374 292c 0d0a 2020  rl(request),..  
+00001ab0: 2020 2020 2020 2020 2020 2020 2020 2764                'd
+00001ac0: 6573 6372 6970 7469 6f6e 273a 2070 6167  escription': pag
+00001ad0: 652e 7365 6172 6368 5f64 6573 6372 6970  e.search_descrip
+00001ae0: 7469 6f6e 2c0d 0a20 2020 2020 2020 2020  tion,..         
+00001af0: 2020 2020 2020 2027 6175 746f 636f 6d70         'autocomp
+00001b00: 6c65 7465 273a 2027 7061 6765 272c 0d0a  lete': 'page',..
+00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b20: 2770 6167 6527 3a20 5472 7565 2c0d 0a20  'page': True,.. 
+00001b30: 2020 2020 2020 2020 2020 207d 0d0a 0d0a             }....
+00001b40: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00001b50: 686f 6f6b 2069 6e20 7061 6765 5f64 6174  hook in page_dat
+00001b60: 615f 686f 6f6b 733a 0d0a 2020 2020 2020  a_hooks:..      
+00001b70: 2020 2020 2020 2020 2020 686f 6f6b 2872            hook(r
+00001b80: 6571 7565 7374 2c20 7061 6765 2c20 6461  equest, page, da
+00001b90: 7461 290d 0a0d 0a20 2020 2020 2020 2020  ta)....         
+00001ba0: 2020 2070 6167 655f 6c69 7374 2e61 7070     page_list.app
+00001bb0: 656e 6428 6461 7461 290d 0a0d 0a0d 0a20  end(data)...... 
+00001bc0: 2020 2020 2020 2072 6574 7572 6e20 4a73         return Js
+00001bd0: 6f6e 5265 7370 6f6e 7365 287b 0d0a 2020  onResponse({..  
+00001be0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00001bf0: 7563 6365 7373 223a 2054 7275 652c 0d0a  uccess": True,..
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c10: 2269 7465 6d73 223a 2070 6167 655f 6c69  "items": page_li
+00001c20: 7374 2c0d 0a20 2020 2020 2020 2020 2020  st,..           
+00001c30: 207d 2c0d 0a20 2020 2020 2020 2020 2020   },..           
+00001c40: 2073 7461 7475 733d 3230 302c 0d0a 2020   status=200,..  
+00001c50: 2020 2020 2020 290d 0a0d 0a0d 0a63 6c61        )......cla
+00001c60: 7373 2044 6f63 756d 656e 7446 6561 7475  ss DocumentFeatu
+00001c70: 7265 284d 6f64 656c 496e 6c69 6e65 4564  re(ModelInlineEd
+00001c80: 6974 6f72 4a53 4665 6174 7572 6529 3a0d  itorJSFeature):.
+00001c90: 0a20 2020 2061 6c6c 6f77 6564 5f74 6167  .    allowed_tag
+00001ca0: 7320 3d20 5b22 6122 5d0d 0a20 2020 2061  s = ["a"]..    a
+00001cb0: 6c6c 6f77 6564 5f61 7474 7269 6275 7465  llowed_attribute
+00001cc0: 7320 3d20 5b22 636c 6173 7322 2c20 2268  s = ["class", "h
+00001cd0: 7265 6622 2c20 2264 6174 612d 6964 225d  ref", "data-id"]
+00001ce0: 0d0a 2020 2020 6368 6f6f 7365 725f 636c  ..    chooser_cl
+00001cf0: 6173 7320 3d20 4164 6d69 6e44 6f63 756d  ass = AdminDocum
+00001d00: 656e 7443 686f 6f73 6572 0d0a 2020 2020  entChooser..    
+00001d10: 6d6f 6465 6c20 3d20 446f 6375 6d65 6e74  model = Document
+00001d20: 0d0a 2020 2020 6b6c 6173 7320 3d20 2257  ..    klass = "W
+00001d30: 6167 7461 696c 446f 6375 6d65 6e74 546f  agtailDocumentTo
+00001d40: 6f6c 220d 0a20 2020 206a 7320 3d20 5b0d  ol"..    js = [.
+00001d50: 0a20 2020 2020 2020 2022 7761 6774 6169  .        "wagtai
+00001d60: 6c5f 6564 6974 6f72 6a73 2f6a 732f 746f  l_editorjs/js/to
+00001d70: 6f6c 732f 7761 6774 6169 6c2d 6368 6f6f  ols/wagtail-choo
+00001d80: 7365 722d 746f 6f6c 2e6a 7322 2c0d 0a20  ser-tool.js",.. 
+00001d90: 2020 2020 2020 2022 7761 6774 6169 6c5f         "wagtail_
+00001da0: 6564 6974 6f72 6a73 2f6a 732f 746f 6f6c  editorjs/js/tool
+00001db0: 732f 7761 6774 6169 6c2d 646f 6375 6d65  s/wagtail-docume
+00001dc0: 6e74 2e6a 7322 2c0d 0a20 2020 205d 0d0a  nt.js",..    ]..
+00001dd0: 0d0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+00001de0: 6f64 0d0a 2020 2020 6465 6620 6765 745f  od..    def get_
+00001df0: 7572 6c28 636c 732c 2069 6e73 7461 6e63  url(cls, instanc
+00001e00: 6529 3a0d 0a20 2020 2020 2020 2072 6574  e):..        ret
+00001e10: 7572 6e20 696e 7374 616e 6365 2e66 696c  urn instance.fil
+00001e20: 652e 7572 6c0d 0a0d 0a                   e.url....
```

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/lists.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/features/lists.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/features/tunes.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/features/tunes.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/fields.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/forms.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/__init__.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 )
 from .value import (
     EditorJSBlock,
     EditorJSValue,
 )
 from .element import (
     EditorJSElement,
+    EditorJSSoupElement,
     EditorJSWrapper,
     wrapper,
     EditorJSElementAttribute,
     EditorJSStyleAttribute,
     wrap_tag,
     add_attributes,
 )
```

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/element/attrs.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/attrs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/element/utils.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/feature_registry.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/feature_registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/features/base.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,38 +57,31 @@
             config: dict = None,
             weight: int = 0, # Weight is used to manage which features.js files are loaded first.
             allowed_tags: list[str] = None,
             allowed_attributes: dict[str, list[str]] = None,
             **kwargs
         ):
 
-        css = css or []
-        js = js or []
-
-        if self.css:
-            css.extend(self.css)
-
-        if self.js:
-            js.extend(self.js)
-
         if not klass and not self.klass:
             raise ValueError("klass must be provided")
         
         if not klass:
             klass = self.klass
         
         self.tool_name = tool_name
         self.klass = klass
-        self.js = js
-        self.css = css
         self.config = config or dict()
         self.kwargs = kwargs
         self.weight = weight
         self.include_template = include_template
 
+        self.init_static(
+            css, js,
+        )
+
         if not isinstance(allowed_tags, (list, tuple, set)) and allowed_tags is not None:
             raise ValueError("allowed_tags must be a list, tuple or set")
         
         if not isinstance(allowed_attributes, dict) and allowed_attributes is not None:
             raise ValueError("allowed_attributes must be a dict")
 
         allowed_tags = allowed_tags or []
@@ -110,14 +103,27 @@
                     allowed_attributes[tag] = set(allowed_attributes.get(tag, []) + self.allowed_attributes)
             else:
                 raise ValueError("Invalid allowed attributes type, self.allowed_attributes must be dict or list")
 
         self.allowed_tags = set(allowed_tags)
         self.allowed_attributes = allowed_attributes
 
+    def init_static(self, css, js):
+        css = css or []
+        js = js or []
+
+        if self.css:
+            css.extend(self.css)
+
+        if self.js:
+            js.extend(self.js)
+            
+        self.js = js
+        self.css = css
+
     def on_register(self, registry: "EditorJSFeatures"):
         """
             Called when the feature is registered.
             This can be used to say; register URLs
             required for this feature to work.
         """
         pass
```

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/features/basic.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/basic.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/features/inlines.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/features/snippets_inlines.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/snippets_inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/features/view.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/view.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/registry/value.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/value.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/render.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/render.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/settings.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
     }
 
     init() {
         if (!window.tippy) {
             console.debug("Tippy tooltips disabled");
             return;
         }
-        tippy(this.element, this.tooltipConfig);
+        this.tippy = tippy(this.element, this.tooltipConfig);
     }
 
     makeConfig() {
         const cfg = {}
         for (const attr of this.element.attributes) {
             if (attr.name.startsWith("data-tippy-")) {
                 const key = attr
@@ -44,14 +44,19 @@
 
 (function() {
     const documentReadyFn = () => {
         const initTippyNode = (node) => {
             if (node.classList && node.classList.contains("wagtail-tooltip") && !node._tippy) {
                 node._tippy = new TippyTooltip(node);
             }
+
+            const tooltipNodes = node.querySelectorAll(".wagtail-tooltip");
+            if (tooltipNodes.length) {
+                tooltipNodes.forEach(initTippyNode);
+            }
         };
 
         const observerFunc = (mutationsList, observer) => {
             for (const mutation of mutationsList) {
                 if (mutation.type === "childList") {
                     for (const node of mutation.addedNodes) {
                         initTippyNode(node);
```

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js` & `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html` & `wagtail_editorjs-1.6.2/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc` & `wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/templatetags/editorjs.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/editorjs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/tests/base.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/tests/test_attrs.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/tests/test_inlines.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/core/tests/test_render.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/manage.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/testapp/settings.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/test/testapp/urls.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/wagtail_hooks/features.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/features.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/wagtail_hooks/urls.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py` & `wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs.egg-info/PKG-INFO` & `wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-editorjs
-Version: 1.6.1rc3
+Version: 1.6.2
 Summary: EditorJS as a widget for Wagtail, with Page- and Image chooser support
 Home-page: https://github.com/Nigel2392/wagtail_editorjs
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -76,40 +76,40 @@
            FieldPanel("editor_field"),
            FieldPanel("content"),
        ]
        editor_field = EditorJSField(
            # All supported features
            features=[
                'attaches',
+               'background-color-tune',
+               'button',
                'checklist',
                'code',
                'delimiter',
+               'document',
+               'drag-drop',
                'header',
+               'image',
+               'images',
                'inline-code',
+               'link',
+               'link-autocomplete',
                'marker',
                'nested-list',
                'paragraph',
                'quote',
                'raw',
                'table',
-               'underline',
-               'warning',
-               'link-autocomplete',
-               'button',
-               'tooltip',
-               'link',
-               'image',
-               'images',
-               'document',
                'text-alignment-tune',
-               'text-variant-tune',
-               'background-color-tune',
                'text-color-tune',
+               'text-variant-tune',
+               'tooltip',
+               'underline',
                'undo-redo',
-               'drag-drop'
+               'warning'
             ],
            blank=True,
            null=True,
        )
 
        # Or as a block
        content = fields.StreamField([
@@ -134,14 +134,82 @@
 
    ```python
    from wagtail_editorjs.registry import EDITOR_JS_FEATURES
    print(EDITOR_JS_FEATURES.keys())
    dict_keys([... all registered features ...])
    ```
 
+##  Register a Wagtail block as a feature
+
+It is also possible to register a Wagtail block as a feature.
+
+This may be a `Fieldblock` (like `Charblock`, or `TextBlock`), or a `StructBlock`.
+
+It is **not** allowed to be or include:
+
+* A `StreamBlock`
+* A `ListBlock`
+* Any type of `ChooserBlock`
+* A `RichTextBlock`
+
+Example:
+
+```python
+from wagtail import hooks
+from wagtail_editorjs.features import (
+    WagtailBlockFeature,
+    EditorJSFeatureStructBlock,
+)
+from wagtail_editorjs.registry import (
+    EditorJSFeatures,
+)
+from wagtail_editorjs.hooks import REGISTER_HOOK_NAME
+
+from wagtail import blocks
+
+class HeadingBlock(blocks.StructBlock):
+    title = blocks.CharBlock()
+    subtitle = blocks.CharBlock()
+
+class TextBlock(EditorJSFeatureStructBlock):
+    heading = HeadingBlock()
+    body = blocks.TextBlock()
+
+    class Meta:
+        template = "myapp/text_block.html"
+        allowed_tags = ["h1", "h2", "p"]
+        # Html looks like:
+        #  <h1>{{ self.heading.title }}</h1>
+        #  <h2>{{ self.heading.subtitle }}</h2>
+        #  <p>{{ self.body }}</p>
+
+@hooks.register(REGISTER_HOOK_NAME)
+def register_editor_js_features(registry: EditorJSFeatures):
+
+    registry.register(
+        "wagtail-text-block",
+        WagtailBlockFeature(
+            "wagtail-text-block",
+            block=TextBlock(),
+        ),
+    )
+```
+
+The block will then be rendered as any structblock, but it will be wrapped in a div with the class `wagtail-text-block` (the feature name).
+
+Example:
+    
+    ```html
+    <div class="wagtail-text-block">
+        <h1>My title</h1>
+        <h2>My subtitle</h2>
+        <p>My body</p>
+    </div>
+    ```
+
 ## Settings
 
 ### `EDITORJS_CLEAN_HTML`
 
 Default: `True`
 Clean the HTML output on rendering.
 This happens every time the field is rendered.
```

### Comparing `wagtail_editorjs-1.6.1rc3/wagtail_editorjs.egg-info/SOURCES.txt` & `wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
 wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
 wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
 wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
 wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
+wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js
@@ -96,14 +97,15 @@
 wagtail_editorjs/test/manage.py
 wagtail_editorjs/test/core/__init__.py
 wagtail_editorjs/test/core/apps.py
 wagtail_editorjs/test/core/migrations/__init__.py
 wagtail_editorjs/test/core/tests/__init__.py
 wagtail_editorjs/test/core/tests/base.py
 wagtail_editorjs/test/core/tests/test_attrs.py
+wagtail_editorjs/test/core/tests/test_blocks.py
 wagtail_editorjs/test/core/tests/test_inlines.py
 wagtail_editorjs/test/core/tests/test_render.py
 wagtail_editorjs/test/testapp/__init__.py
 wagtail_editorjs/test/testapp/asgi.py
 wagtail_editorjs/test/testapp/settings.py
 wagtail_editorjs/test/testapp/urls.py
 wagtail_editorjs/test/testapp/wsgi.py
```

