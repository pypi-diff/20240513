# Comparing `tmp/sotoki-2.1.1.tar.gz` & `tmp/sotoki-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotoki-2.1.1.tar", last modified: Tue May  7 14:51:25 2024, max compression
+gzip compressed data, was "sotoki-2.1.2.tar", last modified: Mon May 13 09:26:40 2024, max compression
```

## Comparing `sotoki-2.1.1.tar` & `sotoki-2.1.2.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.583782 sotoki-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-07 14:51:08.000000 sotoki-2.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-07 14:51:08.000000 sotoki-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 14:51:08.000000 sotoki-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-07 14:51:25.583782 sotoki-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-07 14:51:08.000000 sotoki-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-07 14:51:08.000000 sotoki-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:51:25.583782 sotoki-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-07 14:51:08.000000 sotoki-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.559781 sotoki-2.1.1/src/sotoki/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.563781 sotoki-2.1.1/src/sotoki/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 14:51:20.000000 sotoki-2.1.1/src/sotoki/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-07 14:51:20.000000 sotoki-2.1.1/src/sotoki/__pycache__/dependencies.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/archives.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.563781 sotoki-2.1.1/src/sotoki/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/developer-story/
--rw-r--r--   0 runner    (1001) docker     (127)    28241 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/developer-story/timeline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki/assets/Img/fatarrows.png
--rw-r--r--   0 runner    (1001) docker     (127)    88992 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/favicons-sprite16-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    90236 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/favicons-sprite16.png
--rw-r--r--   0 runner    (1001) docker     (127)   277754 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/favicons-sprite32-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)   283322 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/favicons-sprite32.png
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/filter-sprites.png
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/filter-sprites.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/Img/forms/icon-disabled.svg
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/Img/forms/icon-error.svg
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/forms/icon-success.svg
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/Img/forms/icon-warning.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/hero/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/hero/anonymousHeroBackground.svg
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/Img/icon-envelope-fill-gray.png
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/Img/icon-envelope-fill-gray.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/img-upload.png
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/img-upload.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/open-graph/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki/assets/Img/open-graph/checkmark.png
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/progress-dots.gif
--rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/share-sprite-new.png
--rw-r--r--   0 runner    (1001) docker     (127)    23665 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/share-sprite-new.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/share-sprite.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/unified/
--rw-r--r--   0 runner    (1001) docker     (127)    20630 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/unified/sprites.png
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/unified/sprites.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/unified/wmd-buttons-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/unified/wmd-buttons.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/unifiedmeta/
--rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/unifiedmeta/sprites.png
--rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/unifiedmeta/sprites.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/user-profile-sprite.png
--rw-r--r--   0 runner    (1001) docker     (127)    15404 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/user-profile-sprite.svg
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki/assets/Img/user.svg
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/README
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/css/highlight.default.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/css/sotoki.css
--rw-r--r--   0 runner    (1001) docker     (127)   828990 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/css/stacks.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.571781 sotoki-2.1.1/src/sotoki/assets/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/img/external-link-ltr-icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    63532 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/MathJax.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/config/
--rw-r--r--   0 runner    (1001) docker     (127)   314739 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/config/TeX-AMS_HTML-full.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)    38244 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/extensions/MathMenu.js
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/extensions/MathZoom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/extensions/TeX/
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/extensions/TeX/begingroup.js
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/js/fromnow.js
--rw-r--r--   0 runner    (1001) docker     (127)   108999 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/js/hljs-trigger.js
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/js/identicons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/element/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/element/mml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/jax/element/mml/optable/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/element/mml/optable/BasicLatin.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/GreekItalic.js
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/MathItalic.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/GreekItalic.js
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/MathItalic.js
--rw-r--r--   0 runner    (1001) docker     (127)    38364 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/fontdata.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/TeX/
--rw-r--r--   0 runner    (1001) docker     (127)    44346 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/TeX/fontdata.js
--rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jdenticon.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/js/mathjax-config.js
--rw-r--r--   0 runner    (1001) docker     (127)    58890 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/moment.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   519055 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/stack-icons.js
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/js/tags-filter.js
--rw-r--r--   0 runner    (1001) docker     (127)   794389 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/tex-mml-chtml.js
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/webp-handler.js
--rw-r--r--   0 runner    (1001) docker     (127)   343139 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/webp-hero.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/webp-hero.polyfill.js
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    10919 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/posts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.579782 sotoki-2.1.1/src/sotoki/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/about.html
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/linked_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/pagination.html
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/post_layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/question.html
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/question_list_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/questions.html
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/single_comment.html
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/tag.html
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/tags.html
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/user.html
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/user_card.html
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/users.html
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.579782 sotoki-2.1.1/src/sotoki/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.583782 sotoki-2.1.1/src/sotoki/utils/database/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/database/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/database/posts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/database/redisdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/database/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/database/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/imager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22583 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/preparation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/sevenzip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.583782 sotoki-2.1.1/src/sotoki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.713821 sotoki-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-13 09:26:20.000000 sotoki-2.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-13 09:26:20.000000 sotoki-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 09:26:20.000000 sotoki-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-13 09:26:40.713821 sotoki-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-13 09:26:20.000000 sotoki-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-13 09:26:20.000000 sotoki-2.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:26:40.713821 sotoki-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-13 09:26:20.000000 sotoki-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.685821 sotoki-2.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.693821 sotoki-2.1.2/src/sotoki/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.693821 sotoki-2.1.2/src/sotoki/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-13 09:26:34.000000 sotoki-2.1.2/src/sotoki/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-13 09:26:34.000000 sotoki-2.1.2/src/sotoki/__pycache__/dependencies.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/archives.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.693821 sotoki-2.1.2/src/sotoki/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.697821 sotoki-2.1.2/src/sotoki/assets/Img/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.697821 sotoki-2.1.2/src/sotoki/assets/Img/developer-story/
+-rw-r--r--   0 runner    (1001) docker     (127)    28241 2024-05-13 09:26:38.000000 sotoki-2.1.2/src/sotoki/assets/Img/developer-story/timeline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-13 09:26:40.000000 sotoki-2.1.2/src/sotoki/assets/Img/fatarrows.png
+-rw-r--r--   0 runner    (1001) docker     (127)    88992 2024-05-13 09:26:39.000000 sotoki-2.1.2/src/sotoki/assets/Img/favicons-sprite16-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90236 2024-05-13 09:26:39.000000 sotoki-2.1.2/src/sotoki/assets/Img/favicons-sprite16.png
+-rw-r--r--   0 runner    (1001) docker     (127)   277754 2024-05-13 09:26:39.000000 sotoki-2.1.2/src/sotoki/assets/Img/favicons-sprite32-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)   283322 2024-05-13 09:26:39.000000 sotoki-2.1.2/src/sotoki/assets/Img/favicons-sprite32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-13 09:26:39.000000 sotoki-2.1.2/src/sotoki/assets/Img/filter-sprites.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-13 09:26:39.000000 sotoki-2.1.2/src/sotoki/assets/Img/filter-sprites.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.697821 sotoki-2.1.2/src/sotoki/assets/Img/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-13 09:26:37.000000 sotoki-2.1.2/src/sotoki/assets/Img/forms/icon-disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-13 09:26:37.000000 sotoki-2.1.2/src/sotoki/assets/Img/forms/icon-error.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-13 09:26:37.000000 sotoki-2.1.2/src/sotoki/assets/Img/forms/icon-success.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-13 09:26:37.000000 sotoki-2.1.2/src/sotoki/assets/Img/forms/icon-warning.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.697821 sotoki-2.1.2/src/sotoki/assets/Img/hero/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-13 09:26:38.000000 sotoki-2.1.2/src/sotoki/assets/Img/hero/anonymousHeroBackground.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-13 09:26:37.000000 sotoki-2.1.2/src/sotoki/assets/Img/icon-envelope-fill-gray.png
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-13 09:26:37.000000 sotoki-2.1.2/src/sotoki/assets/Img/icon-envelope-fill-gray.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-13 09:26:38.000000 sotoki-2.1.2/src/sotoki/assets/Img/img-upload.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-05-13 09:26:39.000000 sotoki-2.1.2/src/sotoki/assets/Img/img-upload.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.701821 sotoki-2.1.2/src/sotoki/assets/Img/open-graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-13 09:26:40.000000 sotoki-2.1.2/src/sotoki/assets/Img/open-graph/checkmark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-13 09:26:38.000000 sotoki-2.1.2/src/sotoki/assets/Img/progress-dots.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-05-13 09:26:39.000000 sotoki-2.1.2/src/sotoki/assets/Img/share-sprite-new.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23665 2024-05-13 09:26:39.000000 sotoki-2.1.2/src/sotoki/assets/Img/share-sprite-new.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-13 09:26:38.000000 sotoki-2.1.2/src/sotoki/assets/Img/share-sprite.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.701821 sotoki-2.1.2/src/sotoki/assets/Img/unified/
+-rw-r--r--   0 runner    (1001) docker     (127)    20630 2024-05-13 09:26:38.000000 sotoki-2.1.2/src/sotoki/assets/Img/unified/sprites.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-13 09:26:38.000000 sotoki-2.1.2/src/sotoki/assets/Img/unified/sprites.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-05-13 09:26:38.000000 sotoki-2.1.2/src/sotoki/assets/Img/unified/wmd-buttons-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-05-13 09:26:38.000000 sotoki-2.1.2/src/sotoki/assets/Img/unified/wmd-buttons.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.701821 sotoki-2.1.2/src/sotoki/assets/Img/unifiedmeta/
+-rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-05-13 09:26:38.000000 sotoki-2.1.2/src/sotoki/assets/Img/unifiedmeta/sprites.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-13 09:26:38.000000 sotoki-2.1.2/src/sotoki/assets/Img/unifiedmeta/sprites.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-13 09:26:38.000000 sotoki-2.1.2/src/sotoki/assets/Img/user-profile-sprite.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15404 2024-05-13 09:26:39.000000 sotoki-2.1.2/src/sotoki/assets/Img/user-profile-sprite.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-13 09:26:39.000000 sotoki-2.1.2/src/sotoki/assets/Img/user.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/assets/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.689821 sotoki-2.1.2/src/sotoki/assets/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.701821 sotoki-2.1.2/src/sotoki/assets/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/css/highlight.default.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/assets/static/css/sotoki.css
+-rw-r--r--   0 runner    (1001) docker     (127)   828990 2024-05-13 09:26:35.000000 sotoki-2.1.2/src/sotoki/assets/static/css/stacks.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.701821 sotoki-2.1.2/src/sotoki/assets/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/assets/static/img/external-link-ltr-icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.705821 sotoki-2.1.2/src/sotoki/assets/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    63532 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/js/MathJax.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.705821 sotoki-2.1.2/src/sotoki/assets/static/js/config/
+-rw-r--r--   0 runner    (1001) docker     (127)   314739 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/js/config/TeX-AMS_HTML-full.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.709821 sotoki-2.1.2/src/sotoki/assets/static/js/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)    38244 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/js/extensions/MathMenu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/js/extensions/MathZoom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.709821 sotoki-2.1.2/src/sotoki/assets/static/js/extensions/TeX/
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/js/extensions/TeX/begingroup.js
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/assets/static/js/fromnow.js
+-rw-r--r--   0 runner    (1001) docker     (127)   108999 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/assets/static/js/hljs-trigger.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/assets/static/js/identicons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.689821 sotoki-2.1.2/src/sotoki/assets/static/js/jax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.689821 sotoki-2.1.2/src/sotoki/assets/static/js/jax/element/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.689821 sotoki-2.1.2/src/sotoki/assets/static/js/jax/element/mml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.709821 sotoki-2.1.2/src/sotoki/assets/static/js/jax/element/mml/optable/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/js/jax/element/mml/optable/BasicLatin.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.689821 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.689821 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.689821 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.709821 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.689821 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.709821 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-13 09:26:37.000000 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/GreekItalic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-13 09:26:37.000000 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/MathItalic.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.709821 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-13 09:26:37.000000 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/GreekItalic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-13 09:26:37.000000 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/MathItalic.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38364 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/fontdata.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.709821 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/TeX/
+-rw-r--r--   0 runner    (1001) docker     (127)    44346 2024-05-13 09:26:37.000000 sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/TeX/fontdata.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/js/jdenticon.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/assets/static/js/mathjax-config.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58890 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/js/moment.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   519055 2024-05-13 09:26:35.000000 sotoki-2.1.2/src/sotoki/assets/static/js/stack-icons.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/assets/static/js/tags-filter.js
+-rw-r--r--   0 runner    (1001) docker     (127)   794389 2024-05-13 09:26:35.000000 sotoki-2.1.2/src/sotoki/assets/static/js/tex-mml-chtml.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/js/webp-handler.js
+-rw-r--r--   0 runner    (1001) docker     (127)   343139 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/js/webp-hero.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-13 09:26:36.000000 sotoki-2.1.2/src/sotoki/assets/static/js/webp-hero.polyfill.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10919 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.709821 sotoki-2.1.2/src/sotoki/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/about.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/linked_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/post_layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/question.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/question_list_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/questions.html
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/single_comment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/tags.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/user_card.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/templates/users.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.713821 sotoki-2.1.2/src/sotoki/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.713821 sotoki-2.1.2/src/sotoki/utils/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/database/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/database/posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/database/redisdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/database/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/database/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/preparation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/sevenzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-13 09:26:20.000000 sotoki-2.1.2/src/sotoki/utils/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:40.713821 sotoki-2.1.2/src/sotoki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-13 09:26:40.000000 sotoki-2.1.2/src/sotoki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-13 09:26:40.000000 sotoki-2.1.2/src/sotoki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:26:40.000000 sotoki-2.1.2/src/sotoki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 09:26:40.000000 sotoki-2.1.2/src/sotoki.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:26:40.000000 sotoki-2.1.2/src/sotoki.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-13 09:26:40.000000 sotoki-2.1.2/src/sotoki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 09:26:40.000000 sotoki-2.1.2/src/sotoki.egg-info/top_level.txt
```

### Comparing `sotoki-2.1.1/CHANGELOG.md` & `sotoki-2.1.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 ## Changelog
 
 All notable changes to this project are documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) (as of version 2.0.1).
 
+## [2.1.2] - 2024-05-13
+
+## Fixed
+
+- User icons don't load properly (#301)
+- Revert adaptations to upstream XML format changes (#313)
+
 ## [2.1.1] - 2024-05-07
 
 ## Fixed
 
 - Adapt to upstream XML format changes (#305)
 - Add continuous delivery to Pypi (#303)
```

### Comparing `sotoki-2.1.1/LICENSE` & `sotoki-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/PKG-INFO` & `sotoki-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotoki
-Version: 2.1.1
+Version: 2.1.2
 Summary: Turn StackExchange dumps into ZIM files for offline usage
 Home-page: https://github.com/openzim/sotoki
 Author: Kiwix
 Author-email: contact+dev@kiwix.org
 License: GPLv3+
 Keywords: kiwix zim offline stackechange stackoverflow
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sotoki-2.1.1/README.md` & `sotoki-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/setup.py` & `sotoki-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/__pycache__/dependencies.cpython-38.pyc` & `sotoki-2.1.2/src/sotoki/__pycache__/dependencies.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue May  7 14:51:08 2024 UTC, .py size: 7885 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 dc3f 3a66 cd1e 0000  U........?:f....
+00000000: 550d 0d0a 0000 0000 bcdc 4166 cd1e 0000  U.........Af....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0035 0000 0040 0000 0073 a400 0000 6400  .5...@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6405 6406 6407 6408 6409  ..d.d.d.d.d.d.d.
 00000050: 640a 640b 640c 640d 640e 640f 6410 6411  d.d.d.d.d.d.d.d.
 00000060: 6412 6413 6414 6415 6416 6417 6418 6419  d.d.d.d.d.d.d.d.
 00000070: 641a 641b 641c 641d 641e 641f 6420 6421  d.d.d.d.d.d.d d!
@@ -35,15 +35,15 @@
 00000220: 2f6d 6f6d 656e 746a 732e 636f 6d2f 646f  /momentjs.com/do
 00000230: 776e 6c6f 6164 732f 6d6f 6d65 6e74 2e6d  wnloads/moment.m
 00000240: 696e 2e6a 7329 027a 1a73 7461 7469 632f  in.js).z.static/
 00000250: 6a73 2f6a 6465 6e74 6963 6f6e 2e6d 696e  js/jdenticon.min
 00000260: 2e6a 737a 4f68 7474 7073 3a2f 2f72 6177  .jszOhttps://raw
 00000270: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
 00000280: 6e74 2e63 6f6d 2f64 6d65 7374 6572 2f6a  nt.com/dmester/j
-00000290: 6465 6e74 6963 6f6e 2f33 2e31 2e30 2f64  denticon/3.1.0/d
+00000290: 6465 6e74 6963 6f6e 2f33 2e33 2e30 2f64  denticon/3.3.0/d
 000002a0: 6973 742f 6a64 656e 7469 636f 6e2e 6d69  ist/jdenticon.mi
 000002b0: 6e2e 6a73 2902 7a24 7374 6174 6963 2f63  n.js).z$static/c
 000002c0: 7373 2f68 6967 686c 6967 6874 2e64 6566  ss/highlight.def
 000002d0: 6175 6c74 2e6d 696e 2e63 7373 7a51 6874  ault.min.csszQht
 000002e0: 7470 733a 2f2f 6364 6e6a 732e 636c 6f75  tps://cdnjs.clou
 000002f0: 6466 6c61 7265 2e63 6f6d 2f61 6a61 782f  dflare.com/ajax/
 00000300: 6c69 6273 2f68 6967 686c 6967 6874 2e6a  libs/highlight.j
```

### Comparing `sotoki-2.1.1/src/sotoki/archives.py` & `sotoki-2.1.2/src/sotoki/archives.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 from .utils.shared import Global, logger
 from .utils.misc import has_binary
 from .utils.sevenzip import extract_7z
 from .utils.preparation import (
     merge_users_with_badges,
     merge_posts_with_answers_comments,
-    reencode_file,
 )
 
 
 class ArchiveManager:
     """Handle retrieval and processing of StackExchange dump files
 
     Each website is available as a single 7z archive
@@ -89,18 +88,14 @@
             Global.progresser.update(incr=1)
 
             # remove other files from ark that we won't need
             for fp in self.build_dir.iterdir():
                 if fp.suffix != ".xml" or fp.stem not in self.dump_parts:
                     fp.unlink()
 
-            # reencode xml files
-            for fp in self.build_dir.iterdir():
-                reencode_file(fp)
-
         futures = {}
         executor = cf.ThreadPoolExecutor(max_workers=len(self.archives))
 
         for ark in self.archives:
             url = f"{self.mirror}/{ark.name}"
             kwargs = {"url": url, "fpath": ark}
             future = executor.submit(_run, **kwargs)
```

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/developer-story/timeline.svg` & `sotoki-2.1.2/src/sotoki/assets/Img/developer-story/timeline.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/fatarrows.png` & `sotoki-2.1.2/src/sotoki/assets/Img/fatarrows.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/favicons-sprite16-dark.png` & `sotoki-2.1.2/src/sotoki/assets/Img/favicons-sprite16-dark.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/favicons-sprite16.png` & `sotoki-2.1.2/src/sotoki/assets/Img/favicons-sprite16.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/favicons-sprite32-dark.png` & `sotoki-2.1.2/src/sotoki/assets/Img/favicons-sprite32-dark.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/favicons-sprite32.png` & `sotoki-2.1.2/src/sotoki/assets/Img/favicons-sprite32.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/filter-sprites.png` & `sotoki-2.1.2/src/sotoki/assets/Img/filter-sprites.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/filter-sprites.svg` & `sotoki-2.1.2/src/sotoki/assets/Img/filter-sprites.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/hero/anonymousHeroBackground.svg` & `sotoki-2.1.2/src/sotoki/assets/Img/hero/anonymousHeroBackground.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/icon-envelope-fill-gray.svg` & `sotoki-2.1.2/src/sotoki/assets/Img/icon-envelope-fill-gray.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/img-upload.png` & `sotoki-2.1.2/src/sotoki/assets/Img/img-upload.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/img-upload.svg` & `sotoki-2.1.2/src/sotoki/assets/Img/img-upload.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/open-graph/checkmark.png` & `sotoki-2.1.2/src/sotoki/assets/Img/open-graph/checkmark.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/share-sprite-new.png` & `sotoki-2.1.2/src/sotoki/assets/Img/share-sprite-new.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/share-sprite-new.svg` & `sotoki-2.1.2/src/sotoki/assets/Img/share-sprite-new.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/share-sprite.png` & `sotoki-2.1.2/src/sotoki/assets/Img/share-sprite.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/unified/sprites.png` & `sotoki-2.1.2/src/sotoki/assets/Img/unified/sprites.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/unified/sprites.svg` & `sotoki-2.1.2/src/sotoki/assets/Img/unified/sprites.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/unified/wmd-buttons-dark.svg` & `sotoki-2.1.2/src/sotoki/assets/Img/unified/wmd-buttons-dark.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/unified/wmd-buttons.svg` & `sotoki-2.1.2/src/sotoki/assets/Img/unified/wmd-buttons.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/unifiedmeta/sprites.png` & `sotoki-2.1.2/src/sotoki/assets/Img/unifiedmeta/sprites.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/unifiedmeta/sprites.svg` & `sotoki-2.1.2/src/sotoki/assets/Img/unifiedmeta/sprites.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/user-profile-sprite.png` & `sotoki-2.1.2/src/sotoki/assets/Img/user-profile-sprite.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/Img/user-profile-sprite.svg` & `sotoki-2.1.2/src/sotoki/assets/Img/user-profile-sprite.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/css/highlight.default.min.css` & `sotoki-2.1.2/src/sotoki/assets/static/css/highlight.default.min.css`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/css/sotoki.css` & `sotoki-2.1.2/src/sotoki/assets/static/css/sotoki.css`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/css/stacks.css` & `sotoki-2.1.2/src/sotoki/assets/static/css/stacks.css`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/MathJax.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/MathJax.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/config/TeX-AMS_HTML-full.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/config/TeX-AMS_HTML-full.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/extensions/MathMenu.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/extensions/MathMenu.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/extensions/MathZoom.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/extensions/MathZoom.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/extensions/TeX/begingroup.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/extensions/TeX/begingroup.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/highlight.min.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/identicons.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/identicons.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/jax/element/mml/optable/BasicLatin.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/jax/element/mml/optable/BasicLatin.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/GreekItalic.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/GreekItalic.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/MathItalic.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/MathItalic.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/GreekItalic.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/GreekItalic.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/MathItalic.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/MathItalic.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/fontdata.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/fontdata.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/TeX/fontdata.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/TeX/fontdata.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/jdenticon.min.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/jdenticon.min.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,427 +1,444 @@
-// Jdenticon 3.1.0 | jdenticon.com | MIT licensed | (c) 2014-2020 Daniel Mester Pirttijärvi
+// Jdenticon 3.3.0 | jdenticon.com | MIT licensed | (c) 2014-2024 Daniel Mester Pirttijärvi
 ! function(t, n) {
-    var i = function(t) {
+    var e = function(t) {
         "use strict";
 
-        function n(t, n, i) {
-            return parseInt(t.substr(n, i), 16)
+        function n(t, n, e) {
+            return parseInt(t.substr(n, e), 16)
         }
 
-        function i(t) {
+        function e(t) {
             return (t |= 0) < 0 ? "00" : t < 16 ? "0" + t.toString(16) : t < 256 ? t.toString(16) : "ff"
         }
 
-        function e(t, n, e) {
-            return i(255 * ((e = e < 0 ? e + 6 : e > 6 ? e - 6 : e) < 1 ? t + (n - t) * e : e < 3 ? n : e < 4 ? t + (n - t) * (4 - e) : t))
+        function i(t, n, i) {
+            return e(255 * ((i = i < 0 ? i + 6 : i > 6 ? i - 6 : i) < 1 ? t + (n - t) * i : i < 3 ? n : i < 4 ? t + (n - t) * (4 - i) : t))
         }
 
         function r(t) {
             if (/^#[0-9a-f]{3,8}$/i.test(t)) {
-                var n, i = t.length;
-                if (i < 6) {
-                    var e = t[1],
+                var n, e = t.length;
+                if (e < 6) {
+                    var i = t[1],
                         r = t[2],
                         o = t[3],
                         u = t[4] || "";
-                    n = "#" + e + e + r + r + o + o + u + u
+                    n = "#" + i + i + r + r + o + o + u + u
                 }
-                return (7 == i || i > 8) && (n = t), n
+                return (7 == e || e > 8) && (n = t), n
             }
         }
 
         function o(t) {
-            var i, e = n(t, 7, 2);
-            isNaN(e) ? i = t : i = "rgba(" + n(t, 1, 2) + "," + n(t, 3, 2) + "," + n(t, 5, 2) + "," + (e / 255).toFixed(2) + ")";
-            return i
+            var e, i = n(t, 7, 2);
+            isNaN(i) ? e = t : e = "rgba(" + n(t, 1, 2) + "," + n(t, 3, 2) + "," + n(t, 5, 2) + "," + (i / 255).toFixed(2) + ")";
+            return e
         }
 
         function u(t, n, r) {
             var o;
             if (0 == n) {
-                var u = i(255 * r);
+                var u = e(255 * r);
                 o = u + u + u
             } else {
                 var f = r <= .5 ? r * (n + 1) : r + n - r * n,
-                    h = 2 * r - f;
-                o = e(h, f, 6 * t + 2) + e(h, f, 6 * t) + e(h, f, 6 * t - 2)
+                    a = 2 * r - f;
+                o = i(a, f, 6 * t + 2) + i(a, f, 6 * t) + i(a, f, 6 * t - 2)
             }
             return "#" + o
         }
 
-        function f(t, n, i) {
-            var e = [.55, .5, .5, .46, .6, .55, .55][6 * t + .5 | 0];
-            return u(t, n, i = i < .5 ? i * e * 2 : e + (i - .5) * (1 - e) * 2)
+        function f(t, n, e) {
+            var i = [.55, .5, .5, .46, .6, .55, .55][6 * t + .5 | 0];
+            return u(t, n, e = e < .5 ? e * i * 2 : i + (e - .5) * (1 - i) * 2)
         }
-        var h = t,
+        var a = t,
             s = {
                 G: "jdenticon_config",
                 n: "config"
             },
-            a = {};
+            h = {};
 
         function c(t) {
-            a = t
+            h = t
         }
 
         function v(t) {
-            return arguments.length && (a[s.n] = t), a[s.n]
+            return arguments.length && (h[s.n] = t), h[s.n]
         }
 
-        function l(t, n) {
-            var i = "object" == typeof t && t || a[s.n] || h[s.G] || {},
-                e = i.lightness || {},
-                o = i.saturation || {},
+        function d(t, n) {
+            var e = "object" == typeof t && t || h[s.n] || a[s.G] || {},
+                i = e.lightness || {},
+                o = e.saturation || {},
                 u = "color" in o ? o.color : o,
                 f = o.grayscale,
-                c = i.backColor,
-                v = i.padding;
+                c = e.backColor,
+                v = e.padding;
 
-            function l(t, n) {
-                var i = e[t];
-                return i && i.length > 1 || (i = n),
+            function d(t, n) {
+                var e = i[t];
+                return e && e.length > 1 || (e = n),
                     function(t) {
-                        return (t = i[0] + t * (i[1] - i[0])) < 0 ? 0 : t > 1 ? 1 : t
+                        return (t = e[0] + t * (e[1] - e[0])) < 0 ? 0 : t > 1 ? 1 : t
                     }
             }
 
-            function g(t) {
-                var n, e = i.hues;
-                return e && e.length > 0 && (n = e[0 | .999 * t * e.length]), "number" == typeof n ? (n / 360 % 1 + 1) % 1 : t
+            function l(t) {
+                var n, i = e.hues;
+                return i && i.length > 0 && (n = i[0 | .999 * t * i.length]), "number" == typeof n ? (n / 360 % 1 + 1) % 1 : t
             }
             return {
-                X: g,
+                X: l,
                 p: "number" == typeof u ? u : .5,
                 H: "number" == typeof f ? f : 0,
-                q: l("color", [.4, .8]),
-                I: l("grayscale", [.3, .9]),
+                q: d("color", [.4, .8]),
+                I: d("grayscale", [.3, .9]),
                 J: r(c),
                 Y: "number" == typeof t ? t : "number" == typeof v ? v : n
             }
         }
-        var g = 1,
-            d = 2,
+        var l = 1,
+            g = 2,
             p = {
                 t: "data-jdenticon-hash",
                 o: "data-jdenticon-value"
             },
-            y = "[" + p.t + "],[" + p.o + "]",
-            m = "undefined" != typeof document && document.querySelectorAll.bind(document);
+            y = "jdenticonRendered",
+            m = "[" + p.t + "],[" + p.o + "]",
+            w = "undefined" != typeof document && document.querySelectorAll.bind(document);
 
         function b(t) {
             if (t) {
                 var n = t.tagName;
-                if (/^svg$/i.test(n)) return g;
-                if (/^canvas$/i.test(n) && "getContext" in t) return d
+                if (/^svg$/i.test(n)) return l;
+                if (/^canvas$/i.test(n) && "getContext" in t) return g
             }
         }
 
-        function w(t) {
+        function x(t) {
+            function n() {
+                document.removeEventListener("DOMContentLoaded", n), window.removeEventListener("load", n), setTimeout(t, 0)
+            }
+            "undefined" != typeof document && "undefined" != typeof window && "undefined" != typeof setTimeout && ("loading" === document.readyState ? (document.addEventListener("DOMContentLoaded", n), window.addEventListener("load", n)) : setTimeout(t, 0))
+        }
+
+        function A(t) {
             "undefined" != typeof MutationObserver && new MutationObserver((function(n) {
-                for (var i = 0; i < n.length; i++) {
-                    for (var e = n[i], r = e.addedNodes, o = 0; r && o < r.length; o++) {
+                for (var e = 0; e < n.length; e++) {
+                    for (var i = n[e], r = i.addedNodes, o = 0; r && o < r.length; o++) {
                         var u = r[o];
                         if (1 == u.nodeType)
                             if (b(u)) t(u);
                             else
-                                for (var f = u.querySelectorAll(y), h = 0; h < f.length; h++) t(f[h])
+                                for (var f = u.querySelectorAll(m), a = 0; a < f.length; a++) t(f[a])
                     }
-                    "attributes" == e.type && b(e.target) && t(e.target)
+                    "attributes" == i.type && b(i.target) && t(i.target)
                 }
             })).observe(document.body, {
                 childList: !0,
                 attributes: !0,
                 attributeFilter: [p.o, p.t, "width", "height"],
                 subtree: !0
             })
         }
 
-        function x(t, n) {
+        function S(t, n) {
             this.x = t, this.y = n
         }
 
-        function A(t, n, i, e) {
-            this.u = t, this.v = n, this.K = i, this.Z = e
+        function j(t, n, e, i) {
+            this.u = t, this.v = n, this.K = e, this.Z = i
         }
-        A.prototype.L = function(t, n, i, e) {
+        j.prototype.L = function(t, n, e, i) {
             var r = this.u + this.K,
                 o = this.v + this.K,
                 u = this.Z;
-            return 1 === u ? new x(r - n - (e || 0), this.v + t) : 2 === u ? new x(r - t - (i || 0), o - n - (e || 0)) : 3 === u ? new x(this.u + n, o - t - (i || 0)) : new x(this.u + t, this.v + n)
+            return 1 === u ? new S(r - n - (i || 0), this.v + t) : 2 === u ? new S(r - t - (e || 0), o - n - (i || 0)) : 3 === u ? new S(this.u + n, o - t - (e || 0)) : new S(this.u + t, this.v + n)
         };
-        var S = new A(0, 0, 0, 0);
+        var C = new j(0, 0, 0, 0);
 
-        function j(t) {
-            this.M = t, this.A = S
+        function M(t) {
+            this.M = t, this.A = C
         }
-        var C = j.prototype;
+        var L = M.prototype;
 
-        function M(t, n, i, e) {
-            var r, o, u, f, h, s;
-            (t %= 14) ? 1 == t ? (u = 0 | .5 * i, f = 0 | .8 * i, n.j(i - u, 0, u, f, 2)) : 2 == t ? (u = 0 | i / 3, n.i(u, u, i - u, i - u)) : 3 == t ? (s = i < 6 ? 1 : i < 8 ? 2 : 0 | .25 * i, h = (h = .1 * i) > 1 ? 0 | h : h > .5 ? 1 : h, n.i(s, s, i - h - s, i - h - s)) : 4 == t ? (o = 0 | .15 * i, u = 0 | .5 * i, n.h(i - u - o, i - u - o, u)) : 5 == t ? ((s = 4 * (h = .1 * i)) > 3 && (s |= 0), n.i(0, 0, i, i), n.g([s, s, i - h, s, s + (i - s - h) / 2, i - h], !0)) : 6 == t ? n.g([0, 0, i, 0, i, .7 * i, .4 * i, .4 * i, .7 * i, i, 0, i]) : 7 == t ? n.j(i / 2, i / 2, i / 2, i / 2, 3) : 8 == t ? (n.i(0, 0, i, i / 2), n.i(0, i / 2, i / 2, i / 2), n.j(i / 2, i / 2, i / 2, i / 2, 1)) : 9 == t ? (h = .14 * i, s = i < 4 ? 1 : i < 6 ? 2 : 0 | .35 * i, h = i < 8 ? h : 0 | h, n.i(0, 0, i, i), n.i(s, s, i - s - h, i - s - h, !0)) : 10 == t ? (s = 3 * (h = .12 * i), n.i(0, 0, i, i), n.h(s, s, i - h - s, !0)) : 11 == t ? n.j(i / 2, i / 2, i / 2, i / 2, 3) : 12 == t ? (o = .25 * i, n.i(0, 0, i, i), n.N(o, o, i - o, i - o, !0)) : !e && (o = .4 * i, u = 1.2 * i, n.h(o, o, u)): (r = .42 * i, n.g([0, 0, i, 0, i, i - 2 * r, i - r, i, 0, i]))
+        function N(t, n, e, i) {
+            var r, o, u, f, a, s;
+            (t %= 14) ? 1 == t ? (u = 0 | .5 * e, f = 0 | .8 * e, n.j(e - u, 0, u, f, 2)) : 2 == t ? (u = 0 | e / 3, n.i(u, u, e - u, e - u)) : 3 == t ? (s = e < 6 ? 1 : e < 8 ? 2 : 0 | .25 * e, a = (a = .1 * e) > 1 ? 0 | a : a > .5 ? 1 : a, n.i(s, s, e - a - s, e - a - s)) : 4 == t ? (o = 0 | .15 * e, u = 0 | .5 * e, n.h(e - u - o, e - u - o, u)) : 5 == t ? ((s = 4 * (a = .1 * e)) > 3 && (s |= 0), n.i(0, 0, e, e), n.g([s, s, e - a, s, s + (e - s - a) / 2, e - a], !0)) : 6 == t ? n.g([0, 0, e, 0, e, .7 * e, .4 * e, .4 * e, .7 * e, e, 0, e]) : 7 == t ? n.j(e / 2, e / 2, e / 2, e / 2, 3) : 8 == t ? (n.i(0, 0, e, e / 2), n.i(0, e / 2, e / 2, e / 2), n.j(e / 2, e / 2, e / 2, e / 2, 1)) : 9 == t ? (a = .14 * e, s = e < 4 ? 1 : e < 6 ? 2 : 0 | .35 * e, a = e < 8 ? a : 0 | a, n.i(0, 0, e, e), n.i(s, s, e - s - a, e - s - a, !0)) : 10 == t ? (s = 3 * (a = .12 * e), n.i(0, 0, e, e), n.h(s, s, e - a - s, !0)) : 11 == t ? n.j(e / 2, e / 2, e / 2, e / 2, 3) : 12 == t ? (o = .25 * e, n.i(0, 0, e, e), n.N(o, o, e - o, e - o, !0)) : !i && (o = .4 * e, u = 1.2 * e, n.h(o, o, u)): (r = .42 * e, n.g([0, 0, e, 0, e, e - 2 * r, e - r, e, 0, e]))
         }
 
-        function N(t, n, i) {
-            var e;
-            (t %= 4) ? 1 == t ? n.j(0, i / 2, i, i / 2, 0) : 2 == t ? n.N(0, 0, i, i) : (e = i / 6, n.h(e, e, i - 2 * e)): n.j(0, 0, i, i, 0)
+        function O(t, n, e) {
+            var i;
+            (t %= 4) ? 1 == t ? n.j(0, e / 2, e, e / 2, 0) : 2 == t ? n.N(0, 0, e, e) : (i = e / 6, n.h(i, i, e - 2 * i)): n.j(0, 0, e, e, 0)
         }
 
         function T(t, n) {
             return [f(t = n.X(t), n.H, n.I(0)), f(t, n.p, n.q(.5)), f(t, n.H, n.I(1)), f(t, n.p, n.q(1)), f(t, n.p, n.q(0))]
         }
 
-        function k(t, i, e) {
-            var r = l(e, .08);
+        function k(t, e, i) {
+            var r = d(i, .08);
             r.J && t.m(r.J);
             var o = t.k,
                 u = .5 + o * r.Y | 0;
             o -= 2 * u;
-            var f = new j(t),
-                h = 0 | o / 4,
-                s = 0 | u + o / 2 - 2 * h,
-                a = 0 | u + o / 2 - 2 * h;
-
-            function c(e, r, o, u, c) {
-                var v = n(i, o, 1),
-                    l = u ? n(i, u, 1) : 0;
-                t.O(g[d[e]]);
-                for (var p = 0; p < c.length; p++) f.A = new A(s + c[p][0] * h, a + c[p][1] * h, h, l++ % 4), r(v, f, h, p);
+            var f = new M(t),
+                a = 0 | o / 4,
+                s = 0 | u + o / 2 - 2 * a,
+                h = 0 | u + o / 2 - 2 * a;
+
+            function c(i, r, o, u, c) {
+                var v = n(e, o, 1),
+                    d = u ? n(e, u, 1) : 0;
+                t.O(l[g[i]]);
+                for (var p = 0; p < c.length; p++) f.A = new j(s + c[p][0] * a, h + c[p][1] * a, a, d++ % 4), r(v, f, a, p);
                 t.P()
             }
-            var v, g = T(n(i, -7) / 268435455, r),
-                d = [];
+            var v, l = T(n(e, -7) / 268435455, r),
+                g = [];
 
             function p(t) {
                 if (t.indexOf(v) >= 0)
                     for (var n = 0; n < t.length; n++)
-                        if (d.indexOf(t[n]) >= 0) return !0
+                        if (g.indexOf(t[n]) >= 0) return !0
             }
-            for (var y = 0; y < 3; y++) v = n(i, 8 + y, 1) % g.length, (p([0, 4]) || p([2, 3])) && (v = 1), d.push(v);
-            c(0, N, 2, 3, [
+            for (var y = 0; y < 3; y++) v = n(e, 8 + y, 1) % l.length, (p([0, 4]) || p([2, 3])) && (v = 1), g.push(v);
+            c(0, O, 2, 3, [
                 [1, 0],
                 [2, 0],
                 [2, 3],
                 [1, 3],
                 [0, 1],
                 [3, 1],
                 [3, 2],
                 [0, 2]
-            ]), c(1, N, 4, 5, [
+            ]), c(1, O, 4, 5, [
                 [0, 0],
                 [3, 0],
                 [3, 3],
                 [0, 3]
-            ]), c(2, M, 1, null, [
+            ]), c(2, N, 1, null, [
                 [1, 1],
                 [2, 1],
                 [2, 2],
                 [1, 2]
             ]), t.finish()
         }
 
         function I(t) {
-            var n, i = 40,
-                e = 16,
+            var n, e = 40,
+                i = 16,
                 r = 0,
                 o = 0,
                 u = encodeURI(t) + "%80",
                 f = [],
-                h = [],
+                a = [],
                 s = 1732584193,
-                a = 4023233417,
+                h = 4023233417,
                 c = ~s,
-                v = ~a,
-                l = 3285377520,
-                g = [s, a, c, v, l],
-                d = 0,
+                v = ~h,
+                d = 3285377520,
+                l = [s, h, c, v, d],
+                g = 0,
                 p = "";
 
             function y(t, n) {
                 return t << n | t >>> 32 - n
             }
             for (; r < u.length; o++) f[o >> 2] = f[o >> 2] | ("%" == u[r] ? parseInt(u.substring(r + 1, r += 3), 16) : u.charCodeAt(r++)) << 8 * (3 - (3 & o));
-            for (f[(n = (1 + (o + 7 >> 6)) * e) - 1] = 8 * o - 8; d < n; d += e) {
-                for (r = 0; r < 80; r++) o = y(s, 5) + l + (r < 20 ? 1518500249 + (a & c ^ ~a & v) : r < 40 ? 1859775393 + (a ^ c ^ v) : r < 60 ? 2400959708 + (a & c ^ a & v ^ c & v) : 3395469782 + (a ^ c ^ v)) + (h[r] = r < e ? 0 | f[d + r] : y(h[r - 3] ^ h[r - 8] ^ h[r - 14] ^ h[r - 16], 1)), l = v, v = c, c = y(a, 30), a = s, s = o;
-                g[0] = s = g[0] + s | 0, g[1] = a = g[1] + a | 0, g[2] = c = g[2] + c | 0, g[3] = v = g[3] + v | 0, g[4] = l = g[4] + l | 0
+            for (f[(n = (1 + (o + 7 >> 6)) * i) - 1] = 8 * o - 8; g < n; g += i) {
+                for (r = 0; r < 80; r++) o = y(s, 5) + d + (r < 20 ? 1518500249 + (h & c ^ ~h & v) : r < 40 ? 1859775393 + (h ^ c ^ v) : r < 60 ? 2400959708 + (h & c ^ h & v ^ c & v) : 3395469782 + (h ^ c ^ v)) + (a[r] = r < i ? 0 | f[g + r] : y(a[r - 3] ^ a[r - 8] ^ a[r - 14] ^ a[r - 16], 1)), d = v, v = c, c = y(h, 30), h = s, s = o;
+                l[0] = s = l[0] + s | 0, l[1] = h = l[1] + h | 0, l[2] = c = l[2] + c | 0, l[3] = v = l[3] + v | 0, l[4] = d = l[4] + d | 0
             }
-            for (r = 0; r < i; r++) p += (g[r >> 3] >>> 4 * (7 - (7 & r)) & 15).toString(16);
+            for (r = 0; r < e; r++) p += (l[r >> 3] >>> 4 * (7 - (7 & r)) & 15).toString(16);
             return p
         }
 
-        function O(t) {
+        function P(t) {
             return /^[0-9a-f]{11,}$/i.test(t) && t
         }
 
-        function P(t) {
+        function R(t) {
             return I(null == t ? "" : "" + t)
         }
 
         function F(t, n) {
-            var i = t.canvas,
-                e = i.width,
-                r = i.height;
-            t.save(), n || (n = Math.min(e, r), t.translate((e - n) / 2 | 0, (r - n) / 2 | 0)), this.l = t, this.k = n, t.clearRect(0, 0, n, n)
+            var e = t.canvas,
+                i = e.width,
+                r = e.height;
+            t.save(), n || (n = Math.min(i, r), t.translate((i - n) / 2 | 0, (r - n) / 2 | 0)), this.l = t, this.k = n, t.clearRect(0, 0, n, n)
         }
-        C.g = function(t, n) {
-            for (var i = this, e = n ? -2 : 2, r = [], o = n ? t.length - 2 : 0; o < t.length && o >= 0; o += e) r.push(i.A.L(t[o], t[o + 1]));
+        L.g = function(t, n) {
+            for (var e = this, i = n ? -2 : 2, r = [], o = n ? t.length - 2 : 0; o < t.length && o >= 0; o += i) r.push(e.A.L(t[o], t[o + 1]));
             this.M.g(r)
-        }, C.h = function(t, n, i, e) {
-            var r = this.A.L(t, n, i, i);
-            this.M.h(r, i, e)
-        }, C.i = function(t, n, i, e, r) {
-            this.g([t, n, t + i, n, t + i, n + e, t, n + e], r)
-        }, C.j = function(t, n, i, e, r, o) {
-            var u = [t + i, n, t + i, n + e, t, n + e, t, n];
+        }, L.h = function(t, n, e, i) {
+            var r = this.A.L(t, n, e, e);
+            this.M.h(r, e, i)
+        }, L.i = function(t, n, e, i, r) {
+            this.g([t, n, t + e, n, t + e, n + i, t, n + i], r)
+        }, L.j = function(t, n, e, i, r, o) {
+            var u = [t + e, n, t + e, n + i, t, n + i, t, n];
             u.splice((r || 0) % 4 * 2, 2), this.g(u, o)
-        }, C.N = function(t, n, i, e, r) {
-            this.g([t + i / 2, n, t + i, n + e / 2, t + i / 2, n + e, t, n + e / 2], r)
+        }, L.N = function(t, n, e, i, r) {
+            this.g([t + e / 2, n, t + e, n + i / 2, t + e / 2, n + i, t, n + i / 2], r)
         };
-        var R = F.prototype;
+        var q = F.prototype;
 
-        function q(t, n, i, e) {
+        function B(t, n, e, i) {
             if (!t) throw new Error("No canvas specified.");
-            k(new F(t, i), O(n) || P(n), e)
+            k(new F(t, e), P(n) || R(n), i);
+            var r = t.canvas;
+            r && (r[y] = !0)
         }
 
-        function B(t) {
+        function D(t) {
             return (10 * t + .5 | 0) / 10
         }
 
-        function L() {
+        function E() {
             this.B = ""
         }
-        R.m = function(t) {
+        q.m = function(t) {
             var n = this.l,
-                i = this.k;
-            n.fillStyle = o(t), n.fillRect(0, 0, i, i)
-        }, R.O = function(t) {
+                e = this.k;
+            n.fillStyle = o(t), n.fillRect(0, 0, e, e)
+        }, q.O = function(t) {
             var n = this.l;
             n.fillStyle = o(t), n.beginPath()
-        }, R.P = function() {
+        }, q.P = function() {
             this.l.fill()
-        }, R.g = function(t) {
+        }, q.g = function(t) {
             var n = this.l;
             n.moveTo(t[0].x, t[0].y);
-            for (var i = 1; i < t.length; i++) n.lineTo(t[i].x, t[i].y);
+            for (var e = 1; e < t.length; e++) n.lineTo(t[e].x, t[e].y);
             n.closePath()
-        }, R.h = function(t, n, i) {
-            var e = this.l,
+        }, q.h = function(t, n, e) {
+            var i = this.l,
                 r = n / 2;
-            e.moveTo(t.x + r, t.y + r), e.arc(t.x + r, t.y + r, r, 0, 2 * Math.PI, i), e.closePath()
-        }, R.finish = function() {
+            i.moveTo(t.x + r, t.y + r), i.arc(t.x + r, t.y + r, r, 0, 2 * Math.PI, e), i.closePath()
+        }, q.finish = function() {
             this.l.restore()
         };
-        var D = L.prototype;
+        var U = E.prototype;
 
-        function U(t) {
+        function $(t) {
             this.C, this.D = {}, this.R = t, this.k = t.k
         }
-        D.g = function(t) {
-            for (var n = "", i = 0; i < t.length; i++) n += (i ? "L" : "M") + B(t[i].x) + " " + B(t[i].y);
+        U.g = function(t) {
+            for (var n = "", e = 0; e < t.length; e++) n += (e ? "L" : "M") + D(t[e].x) + " " + D(t[e].y);
             this.B += n + "Z"
-        }, D.h = function(t, n, i) {
-            var e = i ? 0 : 1,
-                r = B(n / 2),
-                o = B(n),
-                u = "a" + r + "," + r + " 0 1," + e + " ";
-            this.B += "M" + B(t.x) + " " + B(t.y + n / 2) + u + o + ",0" + u + -o + ",0"
+        }, U.h = function(t, n, e) {
+            var i = e ? 0 : 1,
+                r = D(n / 2),
+                o = D(n),
+                u = "a" + r + "," + r + " 0 1," + i + " ";
+            this.B += "M" + D(t.x) + " " + D(t.y + n / 2) + u + o + ",0" + u + -o + ",0"
         };
-        var $ = U.prototype;
-        $.m = function(t) {
-            var i = /^(#......)(..)?/.exec(t),
-                e = i[2] ? n(i[2], 0) / 255 : 1;
-            this.R.m(i[1], e)
-        }, $.O = function(t) {
-            this.C = this.D[t] || (this.D[t] = new L)
-        }, $.P = function() {}, $.g = function(t) {
+        var G = $.prototype;
+        G.m = function(t) {
+            var e = /^(#......)(..)?/.exec(t),
+                i = e[2] ? n(e[2], 0) / 255 : 1;
+            this.R.m(e[1], i)
+        }, G.O = function(t) {
+            this.C = this.D[t] || (this.D[t] = new E)
+        }, G.P = function() {}, G.g = function(t) {
             this.C.g(t)
-        }, $.h = function(t, n, i) {
-            this.C.h(t, n, i)
-        }, $.finish = function() {
+        }, G.h = function(t, n, e) {
+            this.C.h(t, n, e)
+        }, G.finish = function() {
             var t = this,
                 n = this.D;
-            for (var i in n) n.hasOwnProperty(i) && t.R.S(i, n[i].B)
+            for (var e in n) n.hasOwnProperty(e) && t.R.S(e, n[e].B)
         };
-        var G = {
+        var H = {
             T: "http://www.w3.org/2000/svg",
             U: "width",
             V: "height"
         };
 
-        function H(t) {
-            this.k = t, this.F = '<svg xmlns="' + G.T + '" width="' + t + '" height="' + t + '" viewBox="0 0 ' + t + " " + t + '">'
+        function J(t) {
+            this.k = t, this.F = '<svg xmlns="' + H.T + '" width="' + t + '" height="' + t + '" viewBox="0 0 ' + t + " " + t + '">'
         }
-        var J = H.prototype;
+        var K = J.prototype;
 
-        function K(t, n, i) {
-            var e = new H(n);
-            return k(new U(e), O(t) || P(t), i), e.toString()
+        function V(t, n, e) {
+            var i = new J(n);
+            return k(new $(i), P(t) || R(t), e), i.toString()
         }
 
-        function V(t, n) {
-            for (var i = [], e = arguments.length - 2; e-- > 0;) i[e] = arguments[e + 2];
-            for (var r = document.createElementNS(G.T, n), o = 0; o + 1 < i.length; o += 2) r.setAttribute(i[o], i[o + 1]);
+        function W(t, n) {
+            for (var e = [], i = arguments.length - 2; i-- > 0;) e[i] = arguments[i + 2];
+            for (var r = document.createElementNS(H.T, n), o = 0; o + 1 < e.length; o += 2) r.setAttribute(e[o], e[o + 1]);
             t.appendChild(r)
         }
 
-        function W(t) {
-            var n = this.k = Math.min(Number(t.getAttribute(G.U)) || 100, Number(t.getAttribute(G.V)) || 100);
+        function Y(t) {
+            var n = this.k = Math.min(Number(t.getAttribute(H.U)) || 100, Number(t.getAttribute(H.V)) || 100);
             for (this.W = t; t.firstChild;) t.removeChild(t.firstChild);
             t.setAttribute("viewBox", "0 0 " + n + " " + n), t.setAttribute("preserveAspectRatio", "xMidYMid meet")
         }
-        J.m = function(t, n) {
+        K.m = function(t, n) {
             n && (this.F += '<rect width="100%" height="100%" fill="' + t + '" opacity="' + n.toFixed(2) + '"/>')
-        }, J.S = function(t, n) {
+        }, K.S = function(t, n) {
             this.F += '<path fill="' + t + '" d="' + n + '"/>'
-        }, J.toString = function() {
+        }, K.toString = function() {
             return this.F + "</svg>"
         };
-        var Y = W.prototype;
+        var Z = Y.prototype;
+
+        function X() {
+            w && _(m)
+        }
 
-        function Z() {
-            m && E(y)
+        function Q() {
+            if (w)
+                for (var t = w(m), n = 0; n < t.length; n++) {
+                    var e = t[n];
+                    e[y] || _(e)
+                }
         }
 
-        function E(t, n, i) {
-            X(t, n, i, (function(t, n) {
-                if (n) return n == g ? new U(new W(t)) : new F(t.getContext("2d"))
+        function _(t, n, e) {
+            z(t, n, e, (function(t, n) {
+                if (n) return n == l ? new $(new Y(t)) : new F(t.getContext("2d"))
             }))
         }
 
-        function X(t, n, i, e) {
+        function z(t, n, e, i) {
             if ("string" != typeof t) {
-                var r = O(n) || null != n && P(n) || O(t.getAttribute(p.t)) || t.hasAttribute(p.o) && P(t.getAttribute(p.o));
+                var r = P(n) || null != n && R(n) || P(t.getAttribute(p.t)) || t.hasAttribute(p.o) && R(t.getAttribute(p.o));
                 if (r) {
-                    var o = e(t, b(t));
-                    o && k(o, r, i)
+                    var o = i(t, b(t));
+                    o && (k(o, r, e), t[y] = !0)
                 }
-            } else if (m)
-                for (var u = m(t), f = 0; f < u.length; f++) X(u[f], n, i, e)
+            } else if (w)
+                for (var u = w(t), f = 0; f < u.length; f++) z(u[f], n, e, i)
         }
 
-        function Q(t, n) {
-            return this.each((function(i, e) {
-                E(e, t, n)
+        function tt(t, n) {
+            return this.each((function(e, i) {
+                _(i, t, n)
             })), this
         }
-        Y.m = function(t, n) {
-            n && V(this.W, "rect", G.U, "100%", G.V, "100%", "fill", t, "opacity", n)
-        }, Y.S = function(t, n) {
-            V(this.W, "path", "fill", t, "d", n)
+        Z.m = function(t, n) {
+            n && W(this.W, "rect", H.U, "100%", H.V, "100%", "fill", t, "opacity", n)
+        }, Z.S = function(t, n) {
+            W(this.W, "path", "fill", t, "d", n)
         };
-        var _ = Z;
-        c(_), _.configure = v, _.drawIcon = q, _.toSvg = K, _.update = E, _.updateCanvas = E, _.updateSvg = E, _.version = "3.1.0", _.bundle = "browser-umd";
-        var z = h.jQuery;
-        z && (z.fn.jdenticon = Q);
-
-        function tt() {
-            var t = (_[s.n] || h[s.G] || {}).replaceMode;
-            "never" != t && (Z(), "observe" == t && w(E))
+        var nt = X;
+        c(nt), nt.configure = v, nt.drawIcon = B, nt.toSvg = V, nt.update = _, nt.updateCanvas = _, nt.updateSvg = _, nt.version = "3.3.0", nt.bundle = "browser-umd";
+        var et = a.jQuery;
+        et && (et.fn.jdenticon = tt);
+
+        function it() {
+            var t = (nt[s.n] || a[s.G] || {}).replaceMode;
+            "never" != t && (Q(), "observe" == t && A(_))
         }
-        "function" == typeof setTimeout && setTimeout(tt, 0);
-        return _
+        return x(it), nt
     }(t);
-    "undefined" != typeof module && "exports" in module ? module.exports = i : "function" == typeof define && define.amd ? define([], (function() {
-        return i
-    })) : t.jdenticon = i
+    "undefined" != typeof module && "exports" in module ? module.exports = e : "function" == typeof define && define.amd ? define([], (function() {
+        return e
+    })) : t.jdenticon = e
 }("undefined" != typeof self ? self : this);
 //# sourceMappingURL=jdenticon.min.js.map
```

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/mathjax-config.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/mathjax-config.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/moment.min.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/stack-icons.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/stack-icons.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/tags-filter.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/tags-filter.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/tex-mml-chtml.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/tex-mml-chtml.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/webp-handler.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/webp-handler.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/webp-hero.bundle.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/webp-hero.bundle.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/assets/static/js/webp-hero.polyfill.js` & `sotoki-2.1.2/src/sotoki/assets/static/js/webp-hero.polyfill.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/constants.py` & `sotoki-2.1.2/src/sotoki/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 ROOT_DIR = pathlib.Path(__file__).parent
 NAME = ROOT_DIR.name
 
 with open(ROOT_DIR.joinpath("VERSION"), "r") as fh:
     VERSION = fh.read().strip()
 
 UTF8 = "utf-8"
-UTF16LE = "utf-16-le"
 SCRAPER = f"{NAME} {VERSION}"
 USER_AGENT = (
     f"{NAME}/{VERSION} (https://github.com/openzim/sotoki; "
     f"contact+crawl@kiwix.org) requests/{requests.__version__}"
 )
 DOWNLOAD_ROOT = "https://archive.org/download/stackexchange"
 # some domains have changed names overtime but SE's Sites.xml still reference old Url
```

### Comparing `sotoki-2.1.1/src/sotoki/dependencies.py` & `sotoki-2.1.2/src/sotoki/dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     (
         "static/js/stack-icons.js",
         "https://unpkg.com/@stackoverflow/stacks-icons@2.20.0/build/index.js",
     ),
     ("static/js/moment.min.js", "https://momentjs.com/downloads/moment.min.js"),
     (
         "static/js/jdenticon.min.js",
-        "https://raw.githubusercontent.com/dmester/jdenticon/3.1.0"
+        "https://raw.githubusercontent.com/dmester/jdenticon/3.3.0"
         "/dist/jdenticon.min.js",
     ),
     (
         "static/css/highlight.default.min.css",
         "https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.1.0/styles/"
         "default.min.css",
     ),
```

### Comparing `sotoki-2.1.1/src/sotoki/entrypoint.py` & `sotoki-2.1.2/src/sotoki/entrypoint.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/posts.py` & `sotoki-2.1.2/src/sotoki/posts.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/renderer.py` & `sotoki-2.1.2/src/sotoki/renderer.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/scraper.py` & `sotoki-2.1.2/src/sotoki/scraper.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/tags.py` & `sotoki-2.1.2/src/sotoki/tags.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/templates/about.html` & `sotoki-2.1.2/src/sotoki/templates/about.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/templates/base.html` & `sotoki-2.1.2/src/sotoki/templates/base.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/templates/pagination.html` & `sotoki-2.1.2/src/sotoki/templates/pagination.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/templates/post_layout.html` & `sotoki-2.1.2/src/sotoki/templates/post_layout.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/templates/question.html` & `sotoki-2.1.2/src/sotoki/templates/question.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/templates/question_list_item.html` & `sotoki-2.1.2/src/sotoki/templates/question_list_item.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/templates/questions.html` & `sotoki-2.1.2/src/sotoki/templates/questions.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/templates/single_comment.html` & `sotoki-2.1.2/src/sotoki/templates/single_comment.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/templates/tag.html` & `sotoki-2.1.2/src/sotoki/templates/tag.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/templates/tags.html` & `sotoki-2.1.2/src/sotoki/templates/tags.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/templates/user.html` & `sotoki-2.1.2/src/sotoki/templates/user.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/templates/user_card.html` & `sotoki-2.1.2/src/sotoki/templates/user_card.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/templates/users.html` & `sotoki-2.1.2/src/sotoki/templates/users.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/users.py` & `sotoki-2.1.2/src/sotoki/users.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/database/common.py` & `sotoki-2.1.2/src/sotoki/utils/database/common.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/database/posts.py` & `sotoki-2.1.2/src/sotoki/utils/database/posts.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/database/redisdb.py` & `sotoki-2.1.2/src/sotoki/utils/database/redisdb.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/database/tags.py` & `sotoki-2.1.2/src/sotoki/utils/database/tags.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/database/users.py` & `sotoki-2.1.2/src/sotoki/utils/database/users.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/executor.py` & `sotoki-2.1.2/src/sotoki/utils/executor.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/generator.py` & `sotoki-2.1.2/src/sotoki/utils/generator.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/html.py` & `sotoki-2.1.2/src/sotoki/utils/html.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/imager.py` & `sotoki-2.1.2/src/sotoki/utils/imager.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/misc.py` & `sotoki-2.1.2/src/sotoki/utils/misc.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/paginator.py` & `sotoki-2.1.2/src/sotoki/utils/paginator.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/preparation.py` & `sotoki-2.1.2/src/sotoki/utils/preparation.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,40 +12,19 @@
 import pathlib
 import xml.sax.saxutils
 import subprocess
 from typing import Union
 
 from .shared import logger
 from .misc import has_binary, get_available_memory
-from ..constants import UTF8, UTF16LE
+from ..constants import UTF8
 
 has_gnusort = has_binary("sort")
 
 
-def reencode_file(src: pathlib.Path):
-    """Reencode a file from dump format (UTF-16-LE as of March 2024) to expected format (UTF8)
-
-    This is based on a streaming on-the-fly reencoding of file chunks to limit memory pressure.
-
-    Content is read line-by-line to ensure it is not split in the middle of a grapheme cluster.
-
-    During reencoding, there will be two versions of the same content on the filesystem, one in
-    previous encoding and one in target encoding, filesystem needs enough space for that.
-    """
-    tmp = src.with_suffix(src.suffix + ".tmp")
-    with open(src, "r", encoding=UTF16LE) as sourceFile:
-        with open(tmp, "w", encoding=UTF8) as targetFile:
-            while True:
-                contents = sourceFile.readline()
-                if not contents:
-                    break
-                targetFile.write(contents)
-    src.unlink()
-    tmp.rename(src)
-
 def get_within_chars(nb_chars_glue: int, nb_ids: int) -> int:
     """nb of chars to combine `nb_ids`'s values with `nb_chars_glue`
 
     Used to compute `within` value for get_id_in()"""
     max_id_len = 8  # 8 chars can contain up to 99M ids
     return nb_chars_glue + (max_id_len * nb_ids)
 
@@ -229,31 +208,31 @@
         # read first badges line so we can compare it in loop
         current_sub = read_sub()
 
         # loop on main file as this is our base that we'll complete with sub rows
         for main_line in mainfh:
             main_id = get_id_in(main_line, field_index_in_main)
 
-            # write main line to dest; removing tag end (/>) and LF
-            dsth.write(main_line[:-3])
+            # write main line to dest; removing tag end (/>) and CRLF
+            dsth.write(main_line[:-4])
             dsth.write(b">")
 
             # fetch subs matching this ID (IDs are sorted so it's continuous)
             has_subs = False
             while current_sub is not None and current_sub[0] < main_id:
                 current_sub = read_sub()
             while current_sub is not None and current_sub[0] == main_id:
                 if not has_subs:
                     dsth.write(nodes_start)
                     has_subs = True
 
                 dsth.write(node_start)
-                # write the sub line removing node name (<row) and trailing LF as well. node already
-                # self closed in source
-                dsth.write(current_sub[1][4:-1])
+                # write the sub line removing the 2 heading spaces, node name (<row) and trailing
+                # CRLF as well. node already self closed in source
+                dsth.write(current_sub[1][6:-2])
                 current_sub = read_sub()
 
             if has_subs:
                 dsth.write(nodes_end)
             has_subs = False
             dsth.write(b"</row>\n")
 
@@ -330,17 +309,17 @@
     with open(src, "rb") as srch:
         for line in srch:
             try:
                 found_id = get_id_in(line, index, within=pattern_len)
             except IndexError:
                 break
             try:
-                # rewrite with new name replacing `<row` and `row>LF`
+                # rewrite with new name, removing 2 spaces, tag open (<row), tag end (/>) and CRLF
                 fhs[found_id].write(starts[found_id])
-                fhs[found_id].write(line[4:-5])
+                fhs[found_id].write(line[6:-5])
                 fhs[found_id].write(ends[found_id])
             except KeyError:
                 continue
 
     # close file descriptors
     _ = {fh.close() for fh in fhs.values()}
 
@@ -399,17 +378,17 @@
                 if current_csv is None:
                     break
 
             if current_csv is None:
                 break
 
             if current_csv[0] == post_id:
-                # write user line to dest; removing tag open (<row), tag end (/>) and LF
+                # write user line to dest; removing 2 spaces, tag open (<row), tag end (/>) and CRLF
                 dsth.write(b"<link")
-                dsth.write(line[4:-3])
+                dsth.write(line[6:-4])
                 # CSV title already includes appropriate quoting
                 dsth.write(b" PostName=")
                 dsth.write(current_csv[1])
                 dsth.write(b" />\n")
 
     if delete_src:
         links_src.unlink()
```

### Comparing `sotoki-2.1.1/src/sotoki/utils/progress.py` & `sotoki-2.1.2/src/sotoki/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/s3.py` & `sotoki-2.1.2/src/sotoki/utils/s3.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/sevenzip.py` & `sotoki-2.1.2/src/sotoki/utils/sevenzip.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/shared.py` & `sotoki-2.1.2/src/sotoki/utils/shared.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki/utils/sites.py` & `sotoki-2.1.2/src/sotoki/utils/sites.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.1.1/src/sotoki.egg-info/PKG-INFO` & `sotoki-2.1.2/src/sotoki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotoki
-Version: 2.1.1
+Version: 2.1.2
 Summary: Turn StackExchange dumps into ZIM files for offline usage
 Home-page: https://github.com/openzim/sotoki
 Author: Kiwix
 Author-email: contact+dev@kiwix.org
 License: GPLv3+
 Keywords: kiwix zim offline stackechange stackoverflow
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sotoki-2.1.1/src/sotoki.egg-info/SOURCES.txt` & `sotoki-2.1.2/src/sotoki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

