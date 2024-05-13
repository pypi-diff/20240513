# Comparing `tmp/wagtail_editorjs-1.6.2.tar.gz` & `tmp/wagtail_editorjs-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_editorjs-1.6.2.tar", last modified: Mon May 13 16:17:19 2024, max compression
+gzip compressed data, was "wagtail_editorjs-1.6.3.tar", last modified: Mon May 13 16:33:39 2024, max compression
```

## Comparing `wagtail_editorjs-1.6.2.tar` & `wagtail_editorjs-1.6.3.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.919174 wagtail_editorjs-1.6.2/
--rw-rw-rw-   0        0        0    18429 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.2/LICENSE
--rw-rw-rw-   0        0        0      272 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6694 2024-05-13 16:17:19.919174 wagtail_editorjs-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     5560 2024-05-13 14:38:18.000000 wagtail_editorjs-1.6.2/README.md
--rw-rw-rw-   0        0        0       90 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.2/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2024-05-13 16:17:19.920173 wagtail_editorjs-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-03-27 00:40:18.000000 wagtail_editorjs-1.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.739292 wagtail_editorjs-1.6.2/wagtail_editorjs/
--rw-rw-rw-   0        0        0      331 2024-05-13 16:17:16.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/__init__.py
--rw-rw-rw-   0        0        0      169 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/apps.py
--rw-rw-rw-   0        0        0     1985 2024-03-29 17:31:47.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/blocks.py
--rw-rw-rw-   0        0        0     2569 2024-04-08 19:06:41.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/django_editor.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.798323 wagtail_editorjs-1.6.2/wagtail_editorjs/features/
--rw-rw-rw-   0        0        0      668 2024-05-13 14:46:42.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/__init__.py
--rw-rw-rw-   0        0        0    15854 2024-05-13 16:14:30.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/blocks.py
--rw-rw-rw-   0        0        0     6818 2024-03-31 07:04:36.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/documents.py
--rw-rw-rw-   0        0        0     9823 2024-04-16 19:24:08.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/images.py
--rw-rw-rw-   0        0        0     7721 2024-05-01 07:39:27.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/inlines.py
--rw-rw-rw-   0        0        0     5164 2024-03-27 20:40:47.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/lists.py
--rw-rw-rw-   0        0        0     3983 2024-04-18 21:15:27.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/features/tunes.py
--rw-rw-rw-   0        0        0     1785 2024-04-16 12:46:42.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/fields.py
--rw-rw-rw-   0        0        0     6874 2024-04-26 08:34:08.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/forms.py
--rw-rw-rw-   0        0        0      319 2024-03-27 21:25:26.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/hooks.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.800329 wagtail_editorjs-1.6.2/wagtail_editorjs/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.801323 wagtail_editorjs-1.6.2/wagtail_editorjs/migrations/__pycache__/
--rw-rw-rw-   0        0        0      218 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/migrations/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.805326 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/
--rw-rw-rw-   0        0        0      932 2024-05-13 14:22:20.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.815659 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/
--rw-rw-rw-   0        0        0      255 2024-05-13 14:22:16.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/__init__.py
--rw-rw-rw-   0        0        0     2073 2024-03-28 19:01:37.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/attrs.py
--rw-rw-rw-   0        0        0     5110 2024-05-13 14:43:24.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/element.py
--rw-rw-rw-   0        0        0     1525 2024-03-27 14:19:36.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/utils.py
--rw-rw-rw-   0        0        0     7265 2024-03-27 21:04:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/feature_registry.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.825991 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/
--rw-rw-rw-   0        0        0      340 2024-04-18 21:14:51.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/__init__.py
--rw-rw-rw-   0        0        0     7600 2024-05-13 15:20:31.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/base.py
--rw-rw-rw-   0        0        0     2235 2024-04-18 09:40:47.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/basic.py
--rw-rw-rw-   0        0        0     8877 2024-04-26 13:03:15.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/inlines.py
--rw-rw-rw-   0        0        0      674 2024-04-18 21:56:20.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/snippets_inlines.py
--rw-rw-rw-   0        0        0     1258 2024-03-27 20:13:06.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/view.py
--rw-rw-rw-   0        0        0     3311 2024-04-16 12:34:49.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/registry/value.py
--rw-rw-rw-   0        0        0     5353 2024-04-18 10:11:04.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/render.py
--rw-rw-rw-   0        0        0     1042 2024-04-08 19:04:03.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.709475 wagtail_editorjs-1.6.2/wagtail_editorjs/static/
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.712431 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.828992 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/css/
--rw-rw-rw-   0        0        0    10098 2024-04-26 12:36:15.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css
--rw-rw-rw-   0        0        0    14154 2024-04-26 13:11:26.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.833990 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/
--rw-rw-rw-   0        0        0     1371 2024-03-29 17:29:46.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
--rw-rw-rw-   0        0        0     1155 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
--rw-rw-rw-   0        0        0     2913 2024-04-26 11:54:42.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.836990 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/init/
--rw-rw-rw-   0        0        0       86 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
--rw-rw-rw-   0        0        0       94 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.848992 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/
--rw-rw-rw-   0        0        0      364 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.851990 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/
--rw-rw-rw-   0        0        0     2661 2024-04-27 00:14:45.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js
--rw-rw-rw-   0        0        0     4464 2024-04-26 12:37:59.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js
--rw-rw-rw-   0        0        0    12378 2024-04-18 09:49:54.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
--rw-rw-rw-   0        0        0     3378 2024-05-13 13:49:05.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js
--rw-rw-rw-   0        0        0     5510 2024-04-18 21:24:20.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
--rw-rw-rw-   0        0        0     3595 2024-04-26 10:29:04.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
--rw-rw-rw-   0        0        0    11260 2024-04-18 09:47:53.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
--rw-rw-rw-   0        0        0     3277 2024-03-26 20:38:45.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
--rw-rw-rw-   0        0        0     7883 2024-04-18 08:43:02.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
--rw-rw-rw-   0        0        0    16447 2024-04-18 09:47:21.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
--rw-rw-rw-   0        0        0     4197 2024-04-26 12:35:50.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js
--rw-rw-rw-   0        0        0     6225 2024-04-18 22:11:04.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.714115 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.855992 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/
--rw-rw-rw-   0        0        0   208234 2024-03-28 10:17:35.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.880990 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/
--rw-rw-rw-   0        0        0    34797 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js
--rw-rw-rw-   0        0        0     7233 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js
--rw-rw-rw-   0        0        0     3222 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js
--rw-rw-rw-   0        0        0     1864 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js
--rw-rw-rw-   0        0        0    10151 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js
--rw-rw-rw-   0        0        0     6946 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js
--rw-rw-rw-   0        0        0    29531 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js
--rw-rw-rw-   0        0        0     2440 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js
--rw-rw-rw-   0        0        0    33560 2024-03-27 17:16:55.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js
--rw-rw-rw-   0        0        0    30466 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js
--rw-rw-rw-   0        0        0     2550 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js
--rw-rw-rw-   0        0        0    10575 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js
--rw-rw-rw-   0        0        0     3142 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js
--rw-rw-rw-   0        0        0     5481 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js
--rw-rw-rw-   0        0        0     3198 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js
--rw-rw-rw-   0        0        0    23954 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
--rw-rw-rw-   0        0        0     9463 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
--rw-rw-rw-   0        0        0     9644 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
--rw-rw-rw-   0        0        0     8007 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
--rw-rw-rw-   0        0        0    19237 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
--rw-rw-rw-   0        0        0     3713 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
--rw-rw-rw-   0        0        0    20734 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.882994 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/
--rw-rw-rw-   0        0        0    44137 2024-04-16 19:19:37.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.887990 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE
--rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js
--rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.715127 wagtail_editorjs-1.6.2/wagtail_editorjs/templates/
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.888990 wagtail_editorjs-1.6.2/wagtail_editorjs/templates/wagtail_editorjs/
--rw-rw-rw-   0        0        0      123 2024-03-29 14:30:09.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.890814 wagtail_editorjs-1.6.2/wagtail_editorjs/templates/wagtail_editorjs/widgets/
--rw-rw-rw-   0        0        0      555 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.892636 wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.894636 wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      220 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     2309 2024-04-25 19:47:38.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
--rw-rw-rw-   0        0        0     1497 2024-04-25 19:47:36.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/editorjs.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.896796 wagtail_editorjs-1.6.2/wagtail_editorjs/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.898803 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/__init__.py
--rw-rw-rw-   0        0        0      168 2024-04-08 18:30:48.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.899808 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.908865 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-03-26 23:51:58.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     2310 2024-04-08 19:05:43.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/base.py
--rw-rw-rw-   0        0        0     2585 2024-04-08 18:38:20.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_attrs.py
--rw-rw-rw-   0        0        0     2731 2024-05-13 16:16:35.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     2041 2024-04-08 18:42:47.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_inlines.py
--rw-rw-rw-   0        0        0     5862 2024-04-08 18:58:38.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_render.py
--rw-rw-rw-   0        0        0      707 2024-04-08 18:29:14.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.913165 wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3826 2024-04-08 19:17:04.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/settings.py
--rw-rw-rw-   0        0        0     1176 2024-04-08 18:42:23.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/urls.py
--rw-rw-rw-   0        0        0      429 2024-04-08 18:29:49.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.918178 wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/
--rw-rw-rw-   0        0        0       74 2024-04-16 12:19:31.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     7364 2024-04-26 09:19:37.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/features.py
--rw-rw-rw-   0        0        0      646 2024-03-27 20:14:22.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0      777 2024-04-16 12:19:25.000000 wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:17:19.770643 wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/
--rw-rw-rw-   0        0        0     6694 2024-05-13 16:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6006 2024-05-13 16:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 16:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-13 16:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-13 16:17:19.000000 wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.987107 wagtail_editorjs-1.6.3/
+-rw-rw-rw-   0        0        0    18429 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0      272 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6666 2024-05-13 16:33:39.987107 wagtail_editorjs-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5532 2024-05-13 16:18:48.000000 wagtail_editorjs-1.6.3/README.md
+-rw-rw-rw-   0        0        0       90 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2024-05-13 16:33:39.988118 wagtail_editorjs-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-03-27 00:40:18.000000 wagtail_editorjs-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.843926 wagtail_editorjs-1.6.3/wagtail_editorjs/
+-rw-rw-rw-   0        0        0      331 2024-05-13 16:33:37.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/__init__.py
+-rw-rw-rw-   0        0        0      169 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/apps.py
+-rw-rw-rw-   0        0        0     1985 2024-03-29 17:31:47.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/blocks.py
+-rw-rw-rw-   0        0        0     2569 2024-04-08 19:06:41.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/django_editor.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.862994 wagtail_editorjs-1.6.3/wagtail_editorjs/features/
+-rw-rw-rw-   0        0        0      668 2024-05-13 14:46:42.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/features/__init__.py
+-rw-rw-rw-   0        0        0    15830 2024-05-13 16:33:28.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/features/blocks.py
+-rw-rw-rw-   0        0        0     6818 2024-03-31 07:04:36.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/features/documents.py
+-rw-rw-rw-   0        0        0     9823 2024-04-16 19:24:08.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/features/images.py
+-rw-rw-rw-   0        0        0     7721 2024-05-01 07:39:27.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/features/inlines.py
+-rw-rw-rw-   0        0        0     5164 2024-03-27 20:40:47.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/features/lists.py
+-rw-rw-rw-   0        0        0     3983 2024-04-18 21:15:27.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/features/tunes.py
+-rw-rw-rw-   0        0        0     1785 2024-04-16 12:46:42.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/fields.py
+-rw-rw-rw-   0        0        0     6874 2024-04-26 08:34:08.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/forms.py
+-rw-rw-rw-   0        0        0      319 2024-03-27 21:25:26.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/hooks.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.865048 wagtail_editorjs-1.6.3/wagtail_editorjs/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.866056 wagtail_editorjs-1.6.3/wagtail_editorjs/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      218 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/migrations/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.871416 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/
+-rw-rw-rw-   0        0        0      932 2024-05-13 14:22:20.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.875930 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/element/
+-rw-rw-rw-   0        0        0      255 2024-05-13 14:22:16.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/element/__init__.py
+-rw-rw-rw-   0        0        0     2073 2024-03-28 19:01:37.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/element/attrs.py
+-rw-rw-rw-   0        0        0     5110 2024-05-13 14:43:24.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/element/element.py
+-rw-rw-rw-   0        0        0     1525 2024-03-27 14:19:36.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/element/utils.py
+-rw-rw-rw-   0        0        0     7265 2024-03-27 21:04:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/feature_registry.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.887871 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/features/
+-rw-rw-rw-   0        0        0      340 2024-04-18 21:14:51.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/features/__init__.py
+-rw-rw-rw-   0        0        0     7600 2024-05-13 15:20:31.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/features/base.py
+-rw-rw-rw-   0        0        0     2235 2024-04-18 09:40:47.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/features/basic.py
+-rw-rw-rw-   0        0        0     8877 2024-04-26 13:03:15.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/features/inlines.py
+-rw-rw-rw-   0        0        0      674 2024-04-18 21:56:20.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/features/snippets_inlines.py
+-rw-rw-rw-   0        0        0     1258 2024-03-27 20:13:06.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/features/view.py
+-rw-rw-rw-   0        0        0     3311 2024-04-16 12:34:49.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/registry/value.py
+-rw-rw-rw-   0        0        0     5353 2024-04-18 10:11:04.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/render.py
+-rw-rw-rw-   0        0        0     1042 2024-04-08 19:04:03.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.809036 wagtail_editorjs-1.6.3/wagtail_editorjs/static/
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.813037 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.890868 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/css/
+-rw-rw-rw-   0        0        0    10098 2024-04-26 12:36:15.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css
+-rw-rw-rw-   0        0        0    14154 2024-04-26 13:11:26.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.895164 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/
+-rw-rw-rw-   0        0        0     1371 2024-03-29 17:29:46.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
+-rw-rw-rw-   0        0        0     1155 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
+-rw-rw-rw-   0        0        0     2913 2024-04-26 11:54:42.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.897703 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/init/
+-rw-rw-rw-   0        0        0       86 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
+-rw-rw-rw-   0        0        0       94 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.909220 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/
+-rw-rw-rw-   0        0        0      364 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.913222 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/
+-rw-rw-rw-   0        0        0     2661 2024-04-27 00:14:45.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js
+-rw-rw-rw-   0        0        0     4464 2024-04-26 12:37:59.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js
+-rw-rw-rw-   0        0        0    12378 2024-04-18 09:49:54.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
+-rw-rw-rw-   0        0        0     3378 2024-05-13 13:49:05.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js
+-rw-rw-rw-   0        0        0     5510 2024-04-18 21:24:20.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
+-rw-rw-rw-   0        0        0     3595 2024-04-26 10:29:04.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
+-rw-rw-rw-   0        0        0    11260 2024-04-18 09:47:53.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
+-rw-rw-rw-   0        0        0     3277 2024-03-26 20:38:45.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
+-rw-rw-rw-   0        0        0     7883 2024-04-18 08:43:02.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
+-rw-rw-rw-   0        0        0    16447 2024-04-18 09:47:21.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
+-rw-rw-rw-   0        0        0     4197 2024-04-26 12:35:50.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js
+-rw-rw-rw-   0        0        0     6225 2024-04-18 22:11:04.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.815065 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.917250 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/
+-rw-rw-rw-   0        0        0   208234 2024-03-28 10:17:35.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.947974 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/
+-rw-rw-rw-   0        0        0    34797 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js
+-rw-rw-rw-   0        0        0     7233 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js
+-rw-rw-rw-   0        0        0     3222 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js
+-rw-rw-rw-   0        0        0     1864 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js
+-rw-rw-rw-   0        0        0    10151 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js
+-rw-rw-rw-   0        0        0     6946 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js
+-rw-rw-rw-   0        0        0    29531 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js
+-rw-rw-rw-   0        0        0     2440 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js
+-rw-rw-rw-   0        0        0    33560 2024-03-27 17:16:55.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js
+-rw-rw-rw-   0        0        0    30466 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js
+-rw-rw-rw-   0        0        0     2550 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js
+-rw-rw-rw-   0        0        0    10575 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js
+-rw-rw-rw-   0        0        0     3142 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js
+-rw-rw-rw-   0        0        0     5481 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js
+-rw-rw-rw-   0        0        0     3198 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js
+-rw-rw-rw-   0        0        0    23954 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
+-rw-rw-rw-   0        0        0     9463 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
+-rw-rw-rw-   0        0        0     9644 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
+-rw-rw-rw-   0        0        0     8007 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
+-rw-rw-rw-   0        0        0    19237 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
+-rw-rw-rw-   0        0        0     3713 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
+-rw-rw-rw-   0        0        0    20734 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.948971 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/
+-rw-rw-rw-   0        0        0    44137 2024-04-16 19:19:37.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.953486 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE
+-rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js
+-rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.816066 wagtail_editorjs-1.6.3/wagtail_editorjs/templates/
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.954491 wagtail_editorjs-1.6.3/wagtail_editorjs/templates/wagtail_editorjs/
+-rw-rw-rw-   0        0        0      123 2024-03-29 14:30:09.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.955494 wagtail_editorjs-1.6.3/wagtail_editorjs/templates/wagtail_editorjs/widgets/
+-rw-rw-rw-   0        0        0      555 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.957495 wagtail_editorjs-1.6.3/wagtail_editorjs/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.959494 wagtail_editorjs-1.6.3/wagtail_editorjs/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      220 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2309 2024-04-25 19:47:38.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1497 2024-04-25 19:47:36.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/templatetags/editorjs.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.963004 wagtail_editorjs-1.6.3/wagtail_editorjs/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.966012 wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/__init__.py
+-rw-rw-rw-   0        0        0      168 2024-04-08 18:30:48.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.967327 wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.973841 wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-26 23:51:58.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     2310 2024-04-08 19:05:43.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     2585 2024-04-08 18:38:20.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/tests/test_attrs.py
+-rw-rw-rw-   0        0        0     2731 2024-05-13 16:16:35.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     2041 2024-04-08 18:42:47.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/tests/test_inlines.py
+-rw-rw-rw-   0        0        0     5862 2024-04-08 18:58:38.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/tests/test_render.py
+-rw-rw-rw-   0        0        0      707 2024-04-08 18:29:14.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.980847 wagtail_editorjs-1.6.3/wagtail_editorjs/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3826 2024-04-08 19:17:04.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/testapp/settings.py
+-rw-rw-rw-   0        0        0     1176 2024-04-08 18:42:23.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      429 2024-04-08 18:29:49.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/test/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.986109 wagtail_editorjs-1.6.3/wagtail_editorjs/wagtail_hooks/
+-rw-rw-rw-   0        0        0       74 2024-04-16 12:19:31.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     7364 2024-04-26 09:19:37.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/wagtail_hooks/features.py
+-rw-rw-rw-   0        0        0      646 2024-03-27 20:14:22.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0      777 2024-04-16 12:19:25.000000 wagtail_editorjs-1.6.3/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:33:39.852983 wagtail_editorjs-1.6.3/wagtail_editorjs.egg-info/
+-rw-rw-rw-   0        0        0     6666 2024-05-13 16:33:39.000000 wagtail_editorjs-1.6.3/wagtail_editorjs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6006 2024-05-13 16:33:39.000000 wagtail_editorjs-1.6.3/wagtail_editorjs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 16:33:39.000000 wagtail_editorjs-1.6.3/wagtail_editorjs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-13 16:33:39.000000 wagtail_editorjs-1.6.3/wagtail_editorjs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-13 16:33:39.000000 wagtail_editorjs-1.6.3/wagtail_editorjs.egg-info/top_level.txt
```

### Comparing `wagtail_editorjs-1.6.2/LICENSE` & `wagtail_editorjs-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/PKG-INFO` & `wagtail_editorjs-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_editorjs
-Version: 1.6.2
+Version: 1.6.3
 Summary: EditorJS as a widget for Wagtail, with Page- and Image chooser support
 Home-page: https://github.com/Nigel2392/wagtail_editorjs
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -194,21 +194,21 @@
     )
 ```
 
 The block will then be rendered as any structblock, but it will be wrapped in a div with the class `wagtail-text-block` (the feature name).
 
 Example:
     
-    ```html
-    <div class="wagtail-text-block">
-        <h1>My title</h1>
-        <h2>My subtitle</h2>
-        <p>My body</p>
-    </div>
-    ```
+```html
+<div class="wagtail-text-block">
+    <h1>My title</h1>
+    <h2>My subtitle</h2>
+    <p>My body</p>
+</div>
+```
 
 ## Settings
 
 ### `EDITORJS_CLEAN_HTML`
 
 Default: `True`
 Clean the HTML output on rendering.
```

### Comparing `wagtail_editorjs-1.6.2/README.md` & `wagtail_editorjs-1.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -166,21 +166,21 @@
     )
 ```
 
 The block will then be rendered as any structblock, but it will be wrapped in a div with the class `wagtail-text-block` (the feature name).
 
 Example:
     
-    ```html
-    <div class="wagtail-text-block">
-        <h1>My title</h1>
-        <h2>My subtitle</h2>
-        <p>My body</p>
-    </div>
-    ```
+```html
+<div class="wagtail-text-block">
+    <h1>My title</h1>
+    <h2>My subtitle</h2>
+    <p>My body</p>
+</div>
+```
 
 ## Settings
 
 ### `EDITORJS_CLEAN_HTML`
 
 Default: `True`
 Clean the HTML output on rendering.
```

### Comparing `wagtail_editorjs-1.6.2/setup.cfg` & `wagtail_editorjs-1.6.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f65 6469 746f   = wagtail_edito
 00000020: 726a 730d 0a76 6572 7369 6f6e 203d 2031  rjs..version = 1
-00000030: 2e36 2e32 0d0a 6465 7363 7269 7074 696f  .6.2..descriptio
+00000030: 2e36 2e33 0d0a 6465 7363 7269 7074 696f  .6.3..descriptio
 00000040: 6e20 3d20 4564 6974 6f72 4a53 2061 7320  n = EditorJS as 
 00000050: 6120 7769 6467 6574 2066 6f72 2057 6167  a widget for Wag
 00000060: 7461 696c 2c20 7769 7468 2050 6167 652d  tail, with Page-
 00000070: 2061 6e64 2049 6d61 6765 2063 686f 6f73   and Image choos
 00000080: 6572 2073 7570 706f 7274 0d0a 6c6f 6e67  er support..long
 00000090: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 000000a0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
```

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/blocks.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/django_editor.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/django_editor.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/features/__init__.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/features/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/features/blocks.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/features/blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
         if "block" not in data["data"]:
             raise forms.ValidationError("Invalid block value")
 
         value: blocks.StructValue = self.block.value_from_datadict(
             data["data"].get("block", {}), {}, prefix,
         )
         
-        data["data"]["block"] = self.block.clean(
+        self.block.clean(
             value,
         )
     
     def render_block_data(self, block: EditorJSBlock, context=None) -> EditorJSElement:
         prefix = block["data"].get("__prefix__") or ""
         value: blocks.StructValue = self.block.value_from_datadict(block["data"].get("block", {}), {}, prefix)
         return EditorJSSoupElement(f"<div class=\"{self.tool_name}\">{ self.block.render(value) }</div>")
```

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/features/documents.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/features/documents.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/features/images.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/features/images.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/features/inlines.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/features/inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/features/lists.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/features/lists.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/features/tunes.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/features/tunes.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/fields.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/forms.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/__init__.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/attrs.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/registry/element/attrs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/element.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/registry/element/element.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/element/utils.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/registry/element/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/feature_registry.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/registry/feature_registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/base.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/registry/features/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/basic.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/registry/features/basic.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/inlines.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/registry/features/inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/snippets_inlines.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/registry/features/snippets_inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/features/view.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/registry/features/view.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/registry/value.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/registry/value.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/render.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/render.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/settings.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js` & `wagtail_editorjs-1.6.3/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html` & `wagtail_editorjs-1.6.3/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc` & `wagtail_editorjs-1.6.3/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/templatetags/editorjs.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/templatetags/editorjs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/base.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_attrs.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_blocks.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_inlines.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/tests/test_inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/test/core/tests/test_render.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/test/core/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/test/manage.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/settings.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/test/testapp/urls.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/features.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/wagtail_hooks/features.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/urls.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/wagtail_hooks/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py` & `wagtail_editorjs-1.6.3/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/PKG-INFO` & `wagtail_editorjs-1.6.3/wagtail_editorjs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-editorjs
-Version: 1.6.2
+Version: 1.6.3
 Summary: EditorJS as a widget for Wagtail, with Page- and Image chooser support
 Home-page: https://github.com/Nigel2392/wagtail_editorjs
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -194,21 +194,21 @@
     )
 ```
 
 The block will then be rendered as any structblock, but it will be wrapped in a div with the class `wagtail-text-block` (the feature name).
 
 Example:
     
-    ```html
-    <div class="wagtail-text-block">
-        <h1>My title</h1>
-        <h2>My subtitle</h2>
-        <p>My body</p>
-    </div>
-    ```
+```html
+<div class="wagtail-text-block">
+    <h1>My title</h1>
+    <h2>My subtitle</h2>
+    <p>My body</p>
+</div>
+```
 
 ## Settings
 
 ### `EDITORJS_CLEAN_HTML`
 
 Default: `True`
 Clean the HTML output on rendering.
```

### Comparing `wagtail_editorjs-1.6.2/wagtail_editorjs.egg-info/SOURCES.txt` & `wagtail_editorjs-1.6.3/wagtail_editorjs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

