# Comparing `tmp/solara_ui-1.32.1.tar.gz` & `tmp/solara_ui-1.32.2.tar.gz`

## Comparing `solara_ui-1.32.1.tar` & `solara_ui-1.32.2.tar`

### file list

```diff
@@ -1,578 +1,578 @@
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 solara_ui-1.32.1/prefix/etc/jupyter/jupyter_notebook_config.d/solara.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 solara_ui-1.32.1/prefix/etc/jupyter/jupyter_server_config.d/solara.json
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/__init__.py
--rw-r--r--   0        0        0    23656 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/__main__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/alias.py
--rw-r--r--   0        0        0    22677 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/autorouting.py
--rw-r--r--   0        0        0    10500 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/cache.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/checks.html
--rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/checks.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/comm.py
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/datatypes.py
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/express.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/kitchensink.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/layout.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lifecycle.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/minisettings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/py.typed
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/reactive.py
--rw-r--r--   0        0        0     9143 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/routing.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/settings.py
--rw-r--r--   0        0        0    30075 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/tasks.py
--rw-r--r--   0        0        0    23570 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/toestand.py
--rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/util.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/__init__.py
--rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/alert.py
--rw-r--r--   0        0        0    16621 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/applayout.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/button.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/card.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/checkbox.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/code_highlight_css.py
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/code_highlight_css.vue
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/columns.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/component_vue.py
--rw-r--r--   0        0        0    13663 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/cross_filter.py
--rw-r--r--   0        0        0    21033 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/dataframe.py
--rw-r--r--   0        0        0     7836 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/datatable.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/datatable.vue
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/details.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/download.vue
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/echarts.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/echarts.vue
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/figure_altair.py
--rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/file_browser.py
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/file_download.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/file_drop.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/file_drop.vue
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/file_list_widget.vue
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/head.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/head_tag.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/head_tag.vue
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/image.py
--rw-r--r--   0        0        0    14585 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/input.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/link.py
--rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/markdown.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/markdown_editor.py
--rw-r--r--   0        0        0     8864 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/markdown_editor.vue
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/matplotlib.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/meta.py
--rw-r--r--   0        0        0    12473 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/misc.py
--rw-r--r--   0        0        0     9938 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/pivot_table.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/pivot_table.vue
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/progress.py
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/select.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/select.vue
--rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/slider.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/slider_date.vue
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/spinner-solara.vue
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/spinner.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/sql_code.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/sql_code.vue
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/style.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/switch.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/tab_navigation.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/title.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/title.vue
--rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/togglebuttons.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/components/tooltip.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/hooks/__init__.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/hooks/dataframe.py
--rw-r--r--   0        0        0     7885 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/hooks/misc.py
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/hooks/use_reactive.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/hooks/use_thread.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/toestand.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/components/__init__.py
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/components/chat.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/components/confirmation_dialog.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/components/cross_filter.py
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/components/input_date.py
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/components/menu.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/components/menu.vue
--rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/components/tabs.py
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/components/theming.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/components/theming.vue
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/hooks/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/hooks/dataframe.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/utils/__init__.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/utils/cookies.py
--rw-r--r--   0        0        0     4258 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/utils/dataframe.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/lab/utils/headers.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/scope/__init__.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/scope/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/__init__.py
--rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/app.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/cdn_helper.py
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/esm.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/fastapi.py
--rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/flask.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/jupytertools.py
--rw-r--r--   0        0        0    11092 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/kernel.py
--rw-r--r--   0        0        0    16718 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/kernel_context.py
--rw-r--r--   0        0        0    18788 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/patch.py
--rw-r--r--   0        0        0     9531 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/reload.py
--rw-r--r--   0        0        0    15746 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/server.py
--rw-r--r--   0        0        0     7340 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/settings.py
--rw-r--r--   0        0        0     8677 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/shell.py
--rw-r--r--   0        0        0    23600 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/starlette.py
--rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/telemetry.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/threaded.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/utils.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/websocket.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/assets/custom.css
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/assets/custom.js
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/assets/favicon.png
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/assets/favicon.svg
--rw-r--r--   0        0        0    40341 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/assets/style.css
--rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/assets/theme-dark.css
--rw-r--r--   0        0        0    15637 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/assets/theme-light.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/assets/theme.js
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/jupyter/__init__.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/jupyter/cdn_handler.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/jupyter/server_extension.py
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/static/ansi.js
--rw-r--r--   0        0        0     6809 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/static/highlight-dark.css
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/static/highlight.css
--rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/static/main-vuetify.js
--rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/static/main.js
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/static/solara_bootstrap.py
--rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/static/sun.svg
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/static/webworker.js
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/templates/index.html.j2
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/templates/loader-plain.css
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/templates/loader-plain.html
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/templates/loader-solara.css
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/templates/loader-solara.html
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/templates/plain.html
--rw-r--r--   0        0        0    19668 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/server/templates/solara.html.j2
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/button.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/markdown.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/.flake8
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/LICENSE
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/Procfile
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/mypy.ini
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/pyproject.toml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/__init__.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/data.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/components/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/components/article.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/components/data.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/components/header.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/components/layout.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/content/articles/equis-in-vidi.md
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/content/articles/substiterat-vati.md
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/pages/__init__.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/pages/tabular.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/pages/article/__init__.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/pages/viz/__init__.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/template/portal/solara_portal/pages/viz/overview.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/test/__init__.py
--rw-r--r--   0        0        0    26284 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/test/pytest_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/utils.py
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/assets/custom.css
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/assets/theme.js
--rw-r--r--   0        0        0    86383 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/assets/images/logo-small.png
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/assets/images/logo.svg
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/assets/images/logo_white.svg
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/components/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/components/algolia.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/components/algolia.vue
--rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/components/algolia_api.vue
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/components/docs.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/components/header.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/components/hero.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/components/mailchimp.py
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/components/mailchimp.vue
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/components/markdown.py
--rw-r--r--   0        0        0     6867 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/components/notebook.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/components/sidebar.py
--rw-r--r--   0        0        0    31602 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/__init__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/doc_use_download.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/docutils.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/apps/__init__.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/apps/jupyter-dashboard-1.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/apps/layout-demo.py
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/apps/scatter.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/apps/scrolling.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/apps/tutorial-streamlit.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/apps/authorization/__init__.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/apps/authorization/admin.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/apps/authorization/users.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/apps/multipage/__init__.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/apps/multipage/page1.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/apps/multipage/page2.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/changelog/__init__.py
--rw-r--r--   0        0        0    13493 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/changelog/changelog.md
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/contact/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/contact/contact.md
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/__init__.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/00-overview.md
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/10-howto/00-overview.md
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/10-howto/10-multipage.md
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/10-howto/20-layout.md
--rw-r--r--   0        0        0    19197 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/10-howto/30-testing.md
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/10-howto/31-debugging.md
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/10-howto/40-embed.md
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/10-howto/50-ipywidget_libraries.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/00-overview.md
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/40-static_files.md
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/41-asset-files.md
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/60-static-site-generation.md
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/70-search.md
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/80-reloading.md
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/90-notebook-support.md
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/95-caching.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/00-introduction.md
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/05-ipywidgets.md
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/06-ipyvuetify.md
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/10-reacton.md
--rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/12-reacton-basics.md
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/15-anatomy.md
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/17-rules-of-hooks.md
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/18-containers.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/20-solara.md
--rw-r--r--   0        0        0     9669 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/40-routing.md
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/50-solara-server.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/60-voila.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/30-enterprise/00-overview.md
--rw-r--r--   0        0        0     9095 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/30-enterprise/10-oauth.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/40-development/00-overview.md
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/40-development/01-contribute.md
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/40-development/10-setup.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/cross_filter/__init__.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/cross_filter/cross_filter_dataframe.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/cross_filter/cross_filter_report.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/cross_filter/cross_filter_select.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/cross_filter/cross_filter_slider.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_cross_filter.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_dark_effective.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_effect.md
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_effect.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_exception.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_memo.md
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_memo.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_previous.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_reactive.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_state.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_state_or_update.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_thread.md
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_thread.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_trait_observe.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/routing/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/routing/generate_routes.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/routing/generate_routes_directory.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/routing/resolve_path.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/routing/route.py
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/routing/use_route.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/routing/use_router.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/utilities/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/utilities/component_vue.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/utilities/computed.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/utilities/display.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/utilities/get_kernel_id.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/utilities/get_session_id.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/utilities/memoize.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/utilities/on_kernel_start.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/utilities/reactive.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/api/utilities/widget.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/__init__.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/common.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/advanced/__init__.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/advanced/link.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/advanced/meta.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/advanced/style.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/data/__init__.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/data/dataframe.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/data/pivot_table.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/enterprise/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/enterprise/avatar.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/enterprise/avatar_menu.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/input/__init__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/input/button.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/input/checkbox.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/input/file_browser.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/input/file_drop.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/input/input.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/input/select.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/input/slider.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/input/switch.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/input/togglebuttons.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/lab/__init__.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/lab/chat.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/lab/confirmation_dialog.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/lab/cookies_headers.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/lab/input_date.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/lab/menu.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/lab/tab.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/lab/tabs.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/lab/task.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/lab/theming.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/lab/use_task.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/app_bar.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/app_bar_title.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/app_layout.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/card.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/card_actions.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/column.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/columns.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/columns_responsive.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/griddraggable.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/gridfixed.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/hbox.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/row.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/sidebar.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/layout/vbox.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/output/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/output/file_download.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/output/html.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/output/image.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/output/markdown.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/output/markdown_editor.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/output/sql_code.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/output/tooltip.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/page/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/page/head.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/page/title.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/status/__init__.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/status/error.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/status/info.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/status/progress.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/status/spinner.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/status/success.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/status/warning.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/viz/__init__.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/viz/altair.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/viz/echarts.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/viz/matplotlib.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/viz/plotly.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/components/viz/plotly_express.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/__init__.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/ipycanvas.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/ai/__init__.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/ai/chatbot.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/ai/tokenizer.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/basics/__init__.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/basics/sine.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/fullscreen/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/fullscreen/authorization.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/fullscreen/layout_demo.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/fullscreen/multipage.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/fullscreen/scatter.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/fullscreen/scrolling.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/fullscreen/tutorial_streamlit.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/general/__init__.py
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/general/custom_storage.py
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/general/deploy_model.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/general/live_update.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/general/login_oauth.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/general/mycard.vue
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/general/pokemon_search.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/general/vue_component.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/libraries/__init__.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/libraries/altair.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/libraries/bqplot.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/libraries/ipyleaflet.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/libraries/ipyleaflet_advanced.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/utilities/__init__.py
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/utilities/calculator.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/utilities/countdown_timer.py
--rw-r--r--   0        0        0     6480 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/utilities/todo.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/visualization/__init__.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/visualization/annotator.py
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/visualization/linked_views.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/examples/visualization/plotly.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/faq/__init__.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/faq/content/99-faq.md
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/__init__.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/00-quickstart.md
--rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/01-introduction.md
--rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/02-installing.md
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/80-what-is-lab.md
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/90-troubleshoot.md
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/00-overview.md
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/10_data_science.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/20-web-app.md
--rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/30-ipywidgets.md
--rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/40-streamlit.md
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/50-dash.md
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/60-jupyter-dashboard-part1.py
--rw-r--r--   0        0        0   575276 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/SF_crime_sample.csv.gz
--rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/_data_science.ipynb
--rw-r--r--   0        0        0    57417 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/_jupyter_dashboard_1.ipynb
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/05-fundamentals/00-overview.md
--rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/05-fundamentals/10-components.md
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/05-fundamentals/50-state-management.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/07-deploying/00-overview.md
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/07-deploying/10-self-hosted.md
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/07-deploying/20-cloud-hosted.md
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/showcase/__init__.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/showcase/domino_code_assist.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/showcase/planeto_tessa.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/showcase/solara_dev.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/showcase/solarathon_2023_team_2.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/showcase/solarathon_2023_team_4.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/showcase/solarathon_2023_team_5.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/showcase/solarathon_2023_team_6.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/pages/showcase/wanderlust.py
--rw-r--r--   0        0        0    37437 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/public/beach.jpeg
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/public/logo.svg
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/public/success.html
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/public/social/discord.svg
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/public/social/github.svg
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/public/social/twitter.svg
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/website/templates/index.html.j2
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/widgets/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/widgets/widgets.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/widgets/vue/gridlayout.vue
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/widgets/vue/html.vue
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/widgets/vue/navigator.vue
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 solara_ui-1.32.1/solara/widgets/vue/vegalite.vue
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/__init__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/conftest.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/docs/docs_howto_event_with_future_test.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/docs/docs_howto_event_with_polling_test.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/docs/docs_howto_no_browser_api_find_testing_test.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/docs/docs_howto_no_browser_testing_test.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/docs/docs_howto_no_browser_threaded_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/api_test.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/app_widget.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/assets_test.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/async_test.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/cdn_test.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/cmdline_test.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/conftest.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/create_test.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/error_test.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/esm_test.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/file_download_test.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/flask_test.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/input_date_test.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/latex_test.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/lifecycle_test.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/markdown_test.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/menu_test.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/popout_test.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/reconnect_test.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/router_test.py
--rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/server_test.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/ssg_test.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/starlette_test.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/test.vue
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/testapp.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/widget_test.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/assets/assets1/common.js
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/assets/assets1/unique1.js
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/assets/assets2/common.js
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/assets/assets2/custom.css
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/assets/assets2/custom.js
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/assets/assets2/unique2.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/enterprise/__init__.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/enterprise/oauth_test.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/integration/reload/apps.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-7-changed-reference.png
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-7-reference.png
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-8-changed-reference.png
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-8-reference.png
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-7-reference.png
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-8-reference.png
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-7-reference.png
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-8-reference.png
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-7-reference.png
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-8-reference.png
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-7-reference.png
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-8-reference.png
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-7-reference.png
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-8-reference.png
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_lab-chromium-linux-reference.png
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_notebook-chromium-linux-reference.png
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-solara-chromium-linux-reference.png
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-voila-chromium-linux-reference.png
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-starlette-solara-chromium-linux-reference.png
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-ipyvuetify3-reference.png
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-reference.png
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-ipyvuetify3-reference.png
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-reference.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/__init__.py
--rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/app_test.py
--rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/applayout_test.py
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/autorouting_test.py
--rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/cache_test.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/cdn_helper_test.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/chat_test.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/checkbox_test.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/common.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/component_frontend_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/component_vue_test.vue
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/confirmation_dialog_test.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/conftest.py
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/cross_filter_component_test.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/cross_filter_test.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/dataframe_test.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/datatable_test.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/display_test.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/express_test.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/file_browser_test.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/file_download_test.py
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/hooks_test.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/input_date_test.py
--rw-r--r--   0        0        0     8001 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/input_test.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/kernel_test.py
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/lifecycle_test.py
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/matplotlib_test.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/no_solara_test.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/output_widget_test.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/patch_test.py
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/pivottable_test.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/reload_test.py
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/router_test.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/select_test.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/settings_test.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/shell_test.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/slider_test.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/switch_test.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/tabs_test.py
--rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/task_test.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/telemetry_tests.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/toestand_computed_reload.py
--rw-r--r--   0        0        0    38498 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/toestand_test.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/toggle_button_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/lab/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/kernel_start.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/notebookapp_component.ipynb
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/notebookapp_element.ipynb
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/notebookapp_widget.ipynb
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/single_file.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/single_file_multiple_routes.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/single_file_routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/food/__init__.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/food/food.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/food/index.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage/01-home.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage/02-my_fruit.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage/03-some-markdown.md
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage/05-and-notebooks.ipynb
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage/06-custom-routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage/99-some_other_python_script.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage/some_other_file.txt
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage/04-a_directory/00-another-markdown.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage/04-a_directory/01-not-an-app.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage/04-a_directory/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage/10-single-file-directory/single-file.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage-widgets/00-overview.md
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage-widgets/01-views.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage-widgets/02-likes.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage-widgets/03-volume.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 solara_ui-1.32.1/tests/unit/solara_test_apps/multipage-widgets/04-color.ipynb
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 solara_ui-1.32.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 solara_ui-1.32.1/LICENSE
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 solara_ui-1.32.1/README.md
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 solara_ui-1.32.1/pyproject.toml
--rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 solara_ui-1.32.1/PKG-INFO
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 solara_ui-1.32.2/prefix/etc/jupyter/jupyter_notebook_config.d/solara.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 solara_ui-1.32.2/prefix/etc/jupyter/jupyter_server_config.d/solara.json
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/__init__.py
+-rw-r--r--   0        0        0    23656 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/__main__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/alias.py
+-rw-r--r--   0        0        0    22677 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/autorouting.py
+-rw-r--r--   0        0        0    10500 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/cache.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/checks.html
+-rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/checks.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/comm.py
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/datatypes.py
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/express.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/kitchensink.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/layout.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lifecycle.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/minisettings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/py.typed
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/reactive.py
+-rw-r--r--   0        0        0     9143 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/routing.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/settings.py
+-rw-r--r--   0        0        0    30075 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/tasks.py
+-rw-r--r--   0        0        0    23570 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/toestand.py
+-rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/util.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/__init__.py
+-rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/alert.py
+-rw-r--r--   0        0        0    16621 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/applayout.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/button.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/card.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/checkbox.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/code_highlight_css.py
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/code_highlight_css.vue
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/columns.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/component_vue.py
+-rw-r--r--   0        0        0    13663 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/cross_filter.py
+-rw-r--r--   0        0        0    21033 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/dataframe.py
+-rw-r--r--   0        0        0     7836 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/datatable.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/datatable.vue
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/details.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/download.vue
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/echarts.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/echarts.vue
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/figure_altair.py
+-rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/file_browser.py
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/file_download.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/file_drop.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/file_drop.vue
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/file_list_widget.vue
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/head.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/head_tag.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/head_tag.vue
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/image.py
+-rw-r--r--   0        0        0    14585 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/input.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/link.py
+-rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/markdown.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/markdown_editor.py
+-rw-r--r--   0        0        0     8864 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/markdown_editor.vue
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/matplotlib.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/meta.py
+-rw-r--r--   0        0        0    12473 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/misc.py
+-rw-r--r--   0        0        0     9938 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/pivot_table.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/pivot_table.vue
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/progress.py
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/select.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/select.vue
+-rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/slider.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/slider_date.vue
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/spinner-solara.vue
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/spinner.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/sql_code.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/sql_code.vue
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/style.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/switch.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/tab_navigation.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/title.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/title.vue
+-rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/togglebuttons.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/components/tooltip.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/hooks/__init__.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/hooks/dataframe.py
+-rw-r--r--   0        0        0     7885 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/hooks/misc.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/hooks/use_reactive.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/hooks/use_thread.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/toestand.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/components/__init__.py
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/components/chat.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/components/confirmation_dialog.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/components/cross_filter.py
+-rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/components/input_date.py
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/components/menu.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/components/menu.vue
+-rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/components/tabs.py
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/components/theming.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/components/theming.vue
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/hooks/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/hooks/dataframe.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/utils/__init__.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/utils/cookies.py
+-rw-r--r--   0        0        0     4258 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/utils/dataframe.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/lab/utils/headers.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/scope/__init__.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/scope/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/__init__.py
+-rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/app.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/cdn_helper.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/esm.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/fastapi.py
+-rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/flask.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/jupytertools.py
+-rw-r--r--   0        0        0    11092 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/kernel.py
+-rw-r--r--   0        0        0    16718 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/kernel_context.py
+-rw-r--r--   0        0        0    18788 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/patch.py
+-rw-r--r--   0        0        0     9531 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/reload.py
+-rw-r--r--   0        0        0    15746 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/server.py
+-rw-r--r--   0        0        0     7340 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/settings.py
+-rw-r--r--   0        0        0     8677 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/shell.py
+-rw-r--r--   0        0        0    23600 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/starlette.py
+-rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/telemetry.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/threaded.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/utils.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/websocket.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/assets/custom.css
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/assets/custom.js
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/assets/favicon.png
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/assets/favicon.svg
+-rw-r--r--   0        0        0    40341 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/assets/style.css
+-rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/assets/theme-dark.css
+-rw-r--r--   0        0        0    15637 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/assets/theme-light.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/assets/theme.js
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/jupyter/__init__.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/jupyter/cdn_handler.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/jupyter/server_extension.py
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/static/ansi.js
+-rw-r--r--   0        0        0     6809 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/static/highlight-dark.css
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/static/highlight.css
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/static/main-vuetify.js
+-rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/static/main.js
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/static/solara_bootstrap.py
+-rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/static/sun.svg
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/static/webworker.js
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/templates/index.html.j2
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/templates/loader-plain.css
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/templates/loader-plain.html
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/templates/loader-solara.css
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/templates/loader-solara.html
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/templates/plain.html
+-rw-r--r--   0        0        0    19658 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/server/templates/solara.html.j2
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/button.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/markdown.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/.flake8
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/LICENSE
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/Procfile
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/mypy.ini
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/pyproject.toml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/__init__.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/data.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/components/__init__.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/components/article.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/components/data.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/components/header.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/components/layout.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/content/articles/equis-in-vidi.md
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/content/articles/substiterat-vati.md
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/pages/__init__.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/pages/tabular.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/pages/article/__init__.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/pages/viz/__init__.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/template/portal/solara_portal/pages/viz/overview.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/test/__init__.py
+-rw-r--r--   0        0        0    26284 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/test/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/utils.py
+-rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/assets/custom.css
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/assets/theme.js
+-rw-r--r--   0        0        0    86383 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/assets/images/logo-small.png
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/assets/images/logo.svg
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/assets/images/logo_white.svg
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/components/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/components/algolia.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/components/algolia.vue
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/components/algolia_api.vue
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/components/docs.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/components/header.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/components/hero.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/components/mailchimp.py
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/components/mailchimp.vue
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/components/markdown.py
+-rw-r--r--   0        0        0     6867 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/components/notebook.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/components/sidebar.py
+-rw-r--r--   0        0        0    31602 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/__init__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/doc_use_download.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/docutils.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/apps/__init__.py
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/apps/jupyter-dashboard-1.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/apps/layout-demo.py
+-rw-r--r--   0        0        0     5432 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/apps/scatter.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/apps/scrolling.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/apps/tutorial-streamlit.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/apps/authorization/__init__.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/apps/authorization/admin.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/apps/authorization/users.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/apps/multipage/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/apps/multipage/page1.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/apps/multipage/page2.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/changelog/__init__.py
+-rw-r--r--   0        0        0    13865 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/changelog/changelog.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/contact/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/contact/contact.md
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/__init__.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/00-overview.md
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/10-howto/00-overview.md
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/10-howto/10-multipage.md
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/10-howto/20-layout.md
+-rw-r--r--   0        0        0    19197 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/10-howto/30-testing.md
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/10-howto/31-debugging.md
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/10-howto/40-embed.md
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/10-howto/50-ipywidget_libraries.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/00-overview.md
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/40-static_files.md
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/41-asset-files.md
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/60-static-site-generation.md
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/70-search.md
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/80-reloading.md
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/90-notebook-support.md
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/95-caching.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/00-introduction.md
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/05-ipywidgets.md
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/06-ipyvuetify.md
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/10-reacton.md
+-rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/12-reacton-basics.md
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/15-anatomy.md
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/17-rules-of-hooks.md
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/18-containers.md
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/20-solara.md
+-rw-r--r--   0        0        0     9669 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/40-routing.md
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/50-solara-server.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/60-voila.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/30-enterprise/00-overview.md
+-rw-r--r--   0        0        0     9095 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/30-enterprise/10-oauth.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/40-development/00-overview.md
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/40-development/01-contribute.md
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/40-development/10-setup.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/cross_filter/__init__.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/cross_filter/cross_filter_dataframe.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/cross_filter/cross_filter_report.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/cross_filter/cross_filter_select.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/cross_filter/cross_filter_slider.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_cross_filter.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_dark_effective.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_effect.md
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_effect.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_exception.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_memo.md
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_memo.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_previous.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_reactive.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_state.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_state_or_update.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_thread.md
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_thread.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_trait_observe.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/routing/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/routing/generate_routes.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/routing/generate_routes_directory.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/routing/resolve_path.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/routing/route.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/routing/use_route.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/routing/use_router.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/utilities/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/utilities/component_vue.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/utilities/computed.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/utilities/display.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/utilities/get_kernel_id.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/utilities/get_session_id.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/utilities/memoize.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/utilities/on_kernel_start.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/utilities/reactive.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/api/utilities/widget.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/__init__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/common.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/advanced/__init__.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/advanced/link.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/advanced/meta.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/advanced/style.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/data/__init__.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/data/dataframe.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/data/pivot_table.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/enterprise/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/enterprise/avatar.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/enterprise/avatar_menu.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/input/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/input/button.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/input/checkbox.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/input/file_browser.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/input/file_drop.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/input/input.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/input/select.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/input/slider.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/input/switch.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/input/togglebuttons.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/lab/__init__.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/lab/chat.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/lab/confirmation_dialog.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/lab/cookies_headers.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/lab/input_date.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/lab/menu.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/lab/tab.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/lab/tabs.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/lab/task.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/lab/theming.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/lab/use_task.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/app_bar.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/app_bar_title.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/app_layout.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/card.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/card_actions.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/column.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/columns.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/columns_responsive.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/griddraggable.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/gridfixed.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/hbox.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/row.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/sidebar.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/layout/vbox.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/output/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/output/file_download.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/output/html.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/output/image.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/output/markdown.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/output/markdown_editor.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/output/sql_code.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/output/tooltip.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/page/__init__.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/page/head.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/page/title.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/status/__init__.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/status/error.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/status/info.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/status/progress.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/status/spinner.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/status/success.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/status/warning.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/viz/__init__.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/viz/altair.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/viz/echarts.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/viz/matplotlib.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/viz/plotly.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/components/viz/plotly_express.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/__init__.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/ipycanvas.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/ai/__init__.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/ai/chatbot.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/ai/tokenizer.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/basics/__init__.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/basics/sine.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/fullscreen/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/fullscreen/authorization.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/fullscreen/layout_demo.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/fullscreen/multipage.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/fullscreen/scatter.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/fullscreen/scrolling.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/fullscreen/tutorial_streamlit.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/general/__init__.py
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/general/custom_storage.py
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/general/deploy_model.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/general/live_update.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/general/login_oauth.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/general/mycard.vue
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/general/pokemon_search.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/general/vue_component.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/libraries/__init__.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/libraries/altair.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/libraries/bqplot.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/libraries/ipyleaflet.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/libraries/ipyleaflet_advanced.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/utilities/__init__.py
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/utilities/calculator.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/utilities/countdown_timer.py
+-rw-r--r--   0        0        0     6480 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/utilities/todo.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/visualization/__init__.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/visualization/annotator.py
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/visualization/linked_views.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/examples/visualization/plotly.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/faq/__init__.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/faq/content/99-faq.md
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/__init__.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/00-quickstart.md
+-rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/01-introduction.md
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/02-installing.md
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/80-what-is-lab.md
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/90-troubleshoot.md
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/00-overview.md
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/10_data_science.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/20-web-app.md
+-rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/30-ipywidgets.md
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/40-streamlit.md
+-rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/50-dash.md
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/60-jupyter-dashboard-part1.py
+-rw-r--r--   0        0        0   575276 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/SF_crime_sample.csv.gz
+-rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/_data_science.ipynb
+-rw-r--r--   0        0        0    57417 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/_jupyter_dashboard_1.ipynb
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/05-fundamentals/00-overview.md
+-rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/05-fundamentals/10-components.md
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/05-fundamentals/50-state-management.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/07-deploying/00-overview.md
+-rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/07-deploying/10-self-hosted.md
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/07-deploying/20-cloud-hosted.md
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/showcase/__init__.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/showcase/domino_code_assist.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/showcase/planeto_tessa.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/showcase/solara_dev.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/showcase/solarathon_2023_team_2.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/showcase/solarathon_2023_team_4.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/showcase/solarathon_2023_team_5.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/showcase/solarathon_2023_team_6.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/pages/showcase/wanderlust.py
+-rw-r--r--   0        0        0    37437 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/public/beach.jpeg
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/public/logo.svg
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/public/success.html
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/public/social/discord.svg
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/public/social/github.svg
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/public/social/twitter.svg
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/website/templates/index.html.j2
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/widgets/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/widgets/widgets.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/widgets/vue/gridlayout.vue
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/widgets/vue/html.vue
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/widgets/vue/navigator.vue
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 solara_ui-1.32.2/solara/widgets/vue/vegalite.vue
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/__init__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/conftest.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/docs/docs_howto_event_with_future_test.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/docs/docs_howto_event_with_polling_test.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/docs/docs_howto_no_browser_api_find_testing_test.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/docs/docs_howto_no_browser_testing_test.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/docs/docs_howto_no_browser_threaded_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/__init__.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/api_test.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/app_widget.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/assets_test.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/async_test.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/cdn_test.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/cmdline_test.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/create_test.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/error_test.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/esm_test.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/file_download_test.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/flask_test.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/input_date_test.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/latex_test.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/lifecycle_test.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/markdown_test.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/menu_test.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/popout_test.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/reconnect_test.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/router_test.py
+-rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/server_test.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/ssg_test.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/starlette_test.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/test.vue
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/testapp.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/widget_test.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/assets/assets1/common.js
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/assets/assets1/unique1.js
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/assets/assets2/common.js
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/assets/assets2/custom.css
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/assets/assets2/custom.js
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/assets/assets2/unique2.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/enterprise/__init__.py
+-rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/enterprise/oauth_test.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/integration/reload/apps.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-7-changed-reference.png
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-7-reference.png
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-8-changed-reference.png
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-8-reference.png
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-7-reference.png
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-8-reference.png
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-7-reference.png
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-8-reference.png
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-7-reference.png
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-8-reference.png
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-7-reference.png
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-8-reference.png
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-7-reference.png
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-8-reference.png
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_lab-chromium-linux-reference.png
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_notebook-chromium-linux-reference.png
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-solara-chromium-linux-reference.png
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-voila-chromium-linux-reference.png
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-starlette-solara-chromium-linux-reference.png
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-ipyvuetify3-reference.png
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-reference.png
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-ipyvuetify3-reference.png
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-reference.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/app_test.py
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/applayout_test.py
+-rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/autorouting_test.py
+-rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/cache_test.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/cdn_helper_test.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/chat_test.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/checkbox_test.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/common.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/component_frontend_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/component_vue_test.vue
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/confirmation_dialog_test.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/conftest.py
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/cross_filter_component_test.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/cross_filter_test.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/dataframe_test.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/datatable_test.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/display_test.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/express_test.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/file_browser_test.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/file_download_test.py
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/hooks_test.py
+-rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/input_date_test.py
+-rw-r--r--   0        0        0     8001 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/input_test.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/kernel_test.py
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/lifecycle_test.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/matplotlib_test.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/no_solara_test.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/output_widget_test.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/patch_test.py
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/pivottable_test.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/reload_test.py
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/router_test.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/select_test.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/settings_test.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/shell_test.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/slider_test.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/switch_test.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/tabs_test.py
+-rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/task_test.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/telemetry_tests.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/toestand_computed_reload.py
+-rw-r--r--   0        0        0    38498 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/toestand_test.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/toggle_button_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/lab/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/kernel_start.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/notebookapp_component.ipynb
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/notebookapp_element.ipynb
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/notebookapp_widget.ipynb
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/single_file.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/single_file_multiple_routes.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/single_file_routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/food/__init__.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/food/food.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/food/index.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage/01-home.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage/02-my_fruit.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage/03-some-markdown.md
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage/05-and-notebooks.ipynb
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage/06-custom-routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage/99-some_other_python_script.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage/some_other_file.txt
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage/04-a_directory/00-another-markdown.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage/04-a_directory/01-not-an-app.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage/04-a_directory/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage/10-single-file-directory/single-file.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage-widgets/00-overview.md
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage-widgets/01-views.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage-widgets/02-likes.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage-widgets/03-volume.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 solara_ui-1.32.2/tests/unit/solara_test_apps/multipage-widgets/04-color.ipynb
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 solara_ui-1.32.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 solara_ui-1.32.2/LICENSE
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 solara_ui-1.32.2/README.md
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 solara_ui-1.32.2/pyproject.toml
+-rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 solara_ui-1.32.2/PKG-INFO
```

### Comparing `solara_ui-1.32.1/solara/__init__.py` & `solara_ui-1.32.2/solara/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Build webapps using IPywidgets"""
 
-__version__ = "1.32.1"
+__version__ = "1.32.2"
 github_url = "https://github.com/widgetti/solara"
 git_branch = "master"
 
 
 from . import comm  # noqa: F401
```

### Comparing `solara_ui-1.32.1/solara/__main__.py` & `solara_ui-1.32.2/solara/__main__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/autorouting.py` & `solara_ui-1.32.2/solara/autorouting.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/cache.py` & `solara_ui-1.32.2/solara/cache.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/checks.html` & `solara_ui-1.32.2/solara/checks.html`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/checks.py` & `solara_ui-1.32.2/solara/checks.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/comm.py` & `solara_ui-1.32.2/solara/comm.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/datatypes.py` & `solara_ui-1.32.2/solara/datatypes.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/express.py` & `solara_ui-1.32.2/solara/express.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/layout.py` & `solara_ui-1.32.2/solara/layout.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/lifecycle.py` & `solara_ui-1.32.2/solara/lifecycle.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/minisettings.py` & `solara_ui-1.32.2/solara/minisettings.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/reactive.py` & `solara_ui-1.32.2/solara/reactive.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/routing.py` & `solara_ui-1.32.2/solara/routing.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/settings.py` & `solara_ui-1.32.2/solara/settings.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/tasks.py` & `solara_ui-1.32.2/solara/tasks.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/toestand.py` & `solara_ui-1.32.2/solara/toestand.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/util.py` & `solara_ui-1.32.2/solara/util.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/__init__.py` & `solara_ui-1.32.2/solara/components/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/alert.py` & `solara_ui-1.32.2/solara/components/alert.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/applayout.py` & `solara_ui-1.32.2/solara/components/applayout.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/button.py` & `solara_ui-1.32.2/solara/components/button.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/card.py` & `solara_ui-1.32.2/solara/components/card.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/checkbox.py` & `solara_ui-1.32.2/solara/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/code_highlight_css.vue` & `solara_ui-1.32.2/solara/components/code_highlight_css.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/columns.py` & `solara_ui-1.32.2/solara/components/columns.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/component_vue.py` & `solara_ui-1.32.2/solara/components/component_vue.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/cross_filter.py` & `solara_ui-1.32.2/solara/components/cross_filter.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/dataframe.py` & `solara_ui-1.32.2/solara/components/dataframe.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/datatable.py` & `solara_ui-1.32.2/solara/components/datatable.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/datatable.vue` & `solara_ui-1.32.2/solara/components/datatable.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/details.py` & `solara_ui-1.32.2/solara/components/details.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/download.vue` & `solara_ui-1.32.2/solara/components/download.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/echarts.py` & `solara_ui-1.32.2/solara/components/echarts.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/echarts.vue` & `solara_ui-1.32.2/solara/components/echarts.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/figure_altair.py` & `solara_ui-1.32.2/solara/components/figure_altair.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/file_browser.py` & `solara_ui-1.32.2/solara/components/file_browser.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/file_download.py` & `solara_ui-1.32.2/solara/components/file_download.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/file_drop.py` & `solara_ui-1.32.2/solara/components/file_drop.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/file_drop.vue` & `solara_ui-1.32.2/solara/components/file_drop.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/file_list_widget.vue` & `solara_ui-1.32.2/solara/components/file_list_widget.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/head.py` & `solara_ui-1.32.2/solara/components/head.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/head_tag.py` & `solara_ui-1.32.2/solara/components/head_tag.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/head_tag.vue` & `solara_ui-1.32.2/solara/components/head_tag.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/image.py` & `solara_ui-1.32.2/solara/components/image.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/input.py` & `solara_ui-1.32.2/solara/components/input.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/link.py` & `solara_ui-1.32.2/solara/components/link.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/markdown.py` & `solara_ui-1.32.2/solara/components/markdown.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/markdown_editor.py` & `solara_ui-1.32.2/solara/components/markdown_editor.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/markdown_editor.vue` & `solara_ui-1.32.2/solara/components/markdown_editor.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/matplotlib.py` & `solara_ui-1.32.2/solara/components/matplotlib.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/meta.py` & `solara_ui-1.32.2/solara/components/meta.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/misc.py` & `solara_ui-1.32.2/solara/components/misc.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/pivot_table.py` & `solara_ui-1.32.2/solara/components/pivot_table.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/pivot_table.vue` & `solara_ui-1.32.2/solara/components/pivot_table.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/progress.py` & `solara_ui-1.32.2/solara/components/progress.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/select.py` & `solara_ui-1.32.2/solara/components/select.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/select.vue` & `solara_ui-1.32.2/solara/components/select.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/slider.py` & `solara_ui-1.32.2/solara/components/slider.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/slider_date.vue` & `solara_ui-1.32.2/solara/components/slider_date.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/spinner-solara.vue` & `solara_ui-1.32.2/solara/components/spinner-solara.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/spinner.py` & `solara_ui-1.32.2/solara/components/spinner.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/sql_code.py` & `solara_ui-1.32.2/solara/components/sql_code.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/sql_code.vue` & `solara_ui-1.32.2/solara/components/sql_code.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/style.py` & `solara_ui-1.32.2/solara/components/style.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/switch.py` & `solara_ui-1.32.2/solara/components/switch.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/tab_navigation.py` & `solara_ui-1.32.2/solara/components/tab_navigation.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/title.py` & `solara_ui-1.32.2/solara/components/title.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/title.vue` & `solara_ui-1.32.2/solara/components/title.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/togglebuttons.py` & `solara_ui-1.32.2/solara/components/togglebuttons.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/components/tooltip.py` & `solara_ui-1.32.2/solara/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/hooks/dataframe.py` & `solara_ui-1.32.2/solara/hooks/dataframe.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/hooks/misc.py` & `solara_ui-1.32.2/solara/hooks/misc.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/hooks/use_reactive.py` & `solara_ui-1.32.2/solara/hooks/use_reactive.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/hooks/use_thread.py` & `solara_ui-1.32.2/solara/hooks/use_thread.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/lab/__init__.py` & `solara_ui-1.32.2/solara/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/lab/components/chat.py` & `solara_ui-1.32.2/solara/lab/components/chat.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/lab/components/confirmation_dialog.py` & `solara_ui-1.32.2/solara/lab/components/confirmation_dialog.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/lab/components/input_date.py` & `solara_ui-1.32.2/solara/lab/components/input_date.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/lab/components/menu.py` & `solara_ui-1.32.2/solara/lab/components/menu.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/lab/components/menu.vue` & `solara_ui-1.32.2/solara/lab/components/menu.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/lab/components/tabs.py` & `solara_ui-1.32.2/solara/lab/components/tabs.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/lab/components/theming.py` & `solara_ui-1.32.2/solara/lab/components/theming.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/lab/components/theming.vue` & `solara_ui-1.32.2/solara/lab/components/theming.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/lab/utils/dataframe.py` & `solara_ui-1.32.2/solara/lab/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/scope/__init__.py` & `solara_ui-1.32.2/solara/scope/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/scope/types.py` & `solara_ui-1.32.2/solara/scope/types.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/app.py` & `solara_ui-1.32.2/solara/server/app.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/cdn_helper.py` & `solara_ui-1.32.2/solara/server/cdn_helper.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/esm.py` & `solara_ui-1.32.2/solara/server/esm.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/flask.py` & `solara_ui-1.32.2/solara/server/flask.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/jupytertools.py` & `solara_ui-1.32.2/solara/server/jupytertools.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/kernel.py` & `solara_ui-1.32.2/solara/server/kernel.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/kernel_context.py` & `solara_ui-1.32.2/solara/server/kernel_context.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/patch.py` & `solara_ui-1.32.2/solara/server/patch.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/reload.py` & `solara_ui-1.32.2/solara/server/reload.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/server.py` & `solara_ui-1.32.2/solara/server/server.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/settings.py` & `solara_ui-1.32.2/solara/server/settings.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/shell.py` & `solara_ui-1.32.2/solara/server/shell.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/starlette.py` & `solara_ui-1.32.2/solara/server/starlette.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/telemetry.py` & `solara_ui-1.32.2/solara/server/telemetry.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/threaded.py` & `solara_ui-1.32.2/solara/server/threaded.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/utils.py` & `solara_ui-1.32.2/solara/server/utils.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/websocket.py` & `solara_ui-1.32.2/solara/server/websocket.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/assets/favicon.png` & `solara_ui-1.32.2/solara/server/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/assets/favicon.svg` & `solara_ui-1.32.2/solara/server/assets/favicon.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/assets/style.css` & `solara_ui-1.32.2/solara/server/assets/style.css`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/assets/theme-dark.css` & `solara_ui-1.32.2/solara/server/assets/theme-dark.css`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/assets/theme-light.css` & `solara_ui-1.32.2/solara/server/assets/theme-light.css`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/jupyter/cdn_handler.py` & `solara_ui-1.32.2/solara/server/jupyter/cdn_handler.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/jupyter/server_extension.py` & `solara_ui-1.32.2/solara/server/jupyter/server_extension.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/static/ansi.js` & `solara_ui-1.32.2/solara/server/static/ansi.js`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/static/highlight-dark.css` & `solara_ui-1.32.2/solara/server/static/highlight-dark.css`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/static/highlight.css` & `solara_ui-1.32.2/solara/server/static/highlight.css`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/static/main-vuetify.js` & `solara_ui-1.32.2/solara/server/static/main-vuetify.js`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/static/main.js` & `solara_ui-1.32.2/solara/server/static/main.js`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/static/solara_bootstrap.py` & `solara_ui-1.32.2/solara/server/static/solara_bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         "altair",
         "vega_datasets",
         "plotly",
         "ipycanvas",
     ]
     for dep in requirements:
         await micropip.install(dep, keep_going=True)
-    await micropip.install("/wheels/solara-1.32.1-py2.py3-none-any.whl", keep_going=True)
+    await micropip.install("/wheels/solara-1.32.2-py2.py3-none-any.whl", keep_going=True)
     import solara
 
     el = solara.Warning("lala")
     import solara
 
     solara.render_fixed(el)
     return el
```

### Comparing `solara_ui-1.32.1/solara/server/static/sun.svg` & `solara_ui-1.32.2/solara/server/static/sun.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/static/webworker.js` & `solara_ui-1.32.2/solara/server/static/webworker.js`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/templates/loader-plain.html` & `solara_ui-1.32.2/solara/server/templates/loader-plain.html`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/templates/loader-solara.css` & `solara_ui-1.32.2/solara/server/templates/loader-solara.css`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/templates/loader-solara.html` & `solara_ui-1.32.2/solara/server/templates/loader-solara.html`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/templates/plain.html` & `solara_ui-1.32.2/solara/server/templates/plain.html`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/server/templates/solara.html.j2` & `solara_ui-1.32.2/solara/server/templates/solara.html.j2`

 * *Files 0% similar despite different names*

```diff
@@ -343,19 +343,19 @@
                             console.log('this.autoRefreshCount!', this.autoRefreshCount)
                             this.autoRefreshCount = this.autoRefreshCount - 1;
                         }, 1000);
                     }
                 },
                 '$vuetify.theme.dark': function (value) {
                     if ( value ) {
-                        this.changeThemeCSS('dark');
+                        changeThemeCSS('dark');
                         appContainer.classList.remove('theme--light');
                         appContainer.classList.add('theme--dark');
                     } else {
-                        this.changeThemeCSS('light');
+                        changeThemeCSS('light');
                         appContainer.classList.remove('theme--dark');
                         appContainer.classList.add('theme--light');
                     }
                 }
             },
             data() {
                 return {
```

### Comparing `solara_ui-1.32.1/solara/template/markdown.py` & `solara_ui-1.32.2/solara/template/markdown.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/template/portal/.pre-commit-config.yaml` & `solara_ui-1.32.2/solara/template/portal/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/template/portal/LICENSE` & `solara_ui-1.32.2/solara/template/portal/LICENSE`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/template/portal/solara_portal/data.py` & `solara_ui-1.32.2/solara/template/portal/solara_portal/data.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/template/portal/solara_portal/components/article.py` & `solara_ui-1.32.2/solara/template/portal/solara_portal/components/article.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/template/portal/solara_portal/components/data.py` & `solara_ui-1.32.2/solara/template/portal/solara_portal/components/data.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/template/portal/solara_portal/content/articles/equis-in-vidi.md` & `solara_ui-1.32.2/solara/template/portal/solara_portal/content/articles/equis-in-vidi.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/template/portal/solara_portal/content/articles/substiterat-vati.md` & `solara_ui-1.32.2/solara/template/portal/solara_portal/content/articles/substiterat-vati.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/template/portal/solara_portal/pages/__init__.py` & `solara_ui-1.32.2/solara/template/portal/solara_portal/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/template/portal/solara_portal/pages/tabular.py` & `solara_ui-1.32.2/solara/template/portal/solara_portal/pages/tabular.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/template/portal/solara_portal/pages/article/__init__.py` & `solara_ui-1.32.2/solara/template/portal/solara_portal/pages/article/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/template/portal/solara_portal/pages/viz/__init__.py` & `solara_ui-1.32.2/solara/template/portal/solara_portal/pages/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/test/pytest_plugin.py` & `solara_ui-1.32.2/solara/test/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/utils.py` & `solara_ui-1.32.2/solara/website/utils.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/assets/custom.css` & `solara_ui-1.32.2/solara/website/assets/custom.css`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/assets/images/logo-small.png` & `solara_ui-1.32.2/solara/website/assets/images/logo-small.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/assets/images/logo.svg` & `solara_ui-1.32.2/solara/website/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/assets/images/logo_white.svg` & `solara_ui-1.32.2/solara/website/assets/images/logo_white.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/components/algolia_api.vue` & `solara_ui-1.32.2/solara/website/components/algolia_api.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/components/docs.py` & `solara_ui-1.32.2/solara/website/components/docs.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/components/header.py` & `solara_ui-1.32.2/solara/website/components/header.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/components/hero.py` & `solara_ui-1.32.2/solara/website/components/hero.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/components/mailchimp.vue` & `solara_ui-1.32.2/solara/website/components/mailchimp.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/components/markdown.py` & `solara_ui-1.32.2/solara/website/components/markdown.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/components/notebook.py` & `solara_ui-1.32.2/solara/website/components/notebook.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/components/sidebar.py` & `solara_ui-1.32.2/solara/website/components/sidebar.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/__init__.py` & `solara_ui-1.32.2/solara/website/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/doc_use_download.py` & `solara_ui-1.32.2/solara/website/pages/doc_use_download.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/docutils.py` & `solara_ui-1.32.2/solara/website/pages/docutils.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/apps/jupyter-dashboard-1.py` & `solara_ui-1.32.2/solara/website/pages/apps/jupyter-dashboard-1.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/apps/layout-demo.py` & `solara_ui-1.32.2/solara/website/pages/apps/layout-demo.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/apps/scatter.py` & `solara_ui-1.32.2/solara/website/pages/apps/scatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import solara.express as solara_px  # similar to plotly express, but comes with cross filters
 import solara.lab
 from solara.components.columns import Columns
 from solara.components.file_drop import FileDrop
 
 github_url = solara.util.github_url(__file__)
 if sys.platform != "emscripten":
-    pycafe_url = solara.util.pycafe_url(path=pathlib.Path(__file__), requirements=["solara", "pandas", "plotly"])
+    pycafe_url = solara.util.pycafe_url(path=pathlib.Path(__file__), requirements=["pandas", "plotly"])
 else:
     pycafe_url = None
 df_sample = pd.read_csv("https://raw.githubusercontent.com/plotly/datasets/master/gapminderDataFiveYear.csv")
 
 
 class State:
     size_max = solara.reactive(40.0)
```

### Comparing `solara_ui-1.32.1/solara/website/pages/apps/scrolling.py` & `solara_ui-1.32.2/solara/website/pages/apps/scrolling.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/apps/authorization/__init__.py` & `solara_ui-1.32.2/solara/website/pages/apps/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/apps/multipage/__init__.py` & `solara_ui-1.32.2/solara/website/pages/apps/multipage/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/apps/multipage/page1.py` & `solara_ui-1.32.2/solara/website/pages/apps/multipage/page1.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/apps/multipage/page2.py` & `solara_ui-1.32.2/solara/website/pages/apps/multipage/page2.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/changelog/changelog.md` & `solara_ui-1.32.2/solara/website/pages/changelog/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 # Solara Changelog
 
 
+## Version 1.32.1
+
+### Details
+
+   * Bug Fix: `solara.display` not working when running a solara server in production mode, or when running a Solara app with flask. [#622](https://github.com/widgetti/solara/pull/622)
+   * Bug Fix: `solara.Markdown` would raise a `NameError` if `pymdown-extensions` was not installed. [#621](https://github.com/widgetti/solara/pull/621)
+
+
 ## Version 1.32.0
 
 ### Details
 
    * Feature: Support for multiple custom asset locations. [#602](https://github.com/widgetti/solara/pull/602)
    * Refactor: Improve API for working with third-party dataframes. [#600](https://github.com/widgetti/solara/pull/600)
    * Bug Fix: Give task results more unique keys. [#609](https://github.com/widgetti/solara/pull/609)
```

### Comparing `solara_ui-1.32.1/solara/website/pages/contact/contact.md` & `solara_ui-1.32.2/solara/website/pages/contact/contact.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/__init__.py` & `solara_ui-1.32.2/solara/website/pages/documentation/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/10-howto/10-multipage.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/10-howto/10-multipage.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/10-howto/20-layout.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/10-howto/20-layout.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/10-howto/30-testing.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/10-howto/30-testing.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/10-howto/31-debugging.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/10-howto/31-debugging.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/10-howto/40-embed.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/10-howto/40-embed.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/10-howto/50-ipywidget_libraries.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/10-howto/50-ipywidget_libraries.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/40-static_files.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/40-static_files.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/41-asset-files.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/41-asset-files.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/60-static-site-generation.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/60-static-site-generation.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/70-search.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/70-search.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/80-reloading.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/80-reloading.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/15-reference/95-caching.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/15-reference/95-caching.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/00-introduction.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/00-introduction.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/05-ipywidgets.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/05-ipywidgets.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/06-ipyvuetify.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/06-ipyvuetify.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/10-reacton.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/10-reacton.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/12-reacton-basics.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/12-reacton-basics.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/15-anatomy.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/15-anatomy.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/18-containers.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/18-containers.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/20-solara.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/20-solara.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/40-routing.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/40-routing.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/50-solara-server.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/50-solara-server.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/20-understanding/60-voila.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/20-understanding/60-voila.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/30-enterprise/10-oauth.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/30-enterprise/10-oauth.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/40-development/01-contribute.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/40-development/01-contribute.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/advanced/content/40-development/10-setup.md` & `solara_ui-1.32.2/solara/website/pages/documentation/advanced/content/40-development/10-setup.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_cross_filter.py` & `solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_cross_filter.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_effect.md` & `solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_effect.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_exception.py` & `solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_exception.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_memo.md` & `solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_memo.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_previous.py` & `solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_previous.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_state_or_update.py` & `solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_state_or_update.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_thread.md` & `solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_thread.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/hooks/use_thread.py` & `solara_ui-1.32.2/solara/website/pages/documentation/api/hooks/use_thread.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/routing/resolve_path.py` & `solara_ui-1.32.2/solara/website/pages/documentation/api/routing/resolve_path.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/routing/route.py` & `solara_ui-1.32.2/solara/website/pages/documentation/api/routing/route.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/routing/use_route.py` & `solara_ui-1.32.2/solara/website/pages/documentation/api/routing/use_route.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/utilities/memoize.py` & `solara_ui-1.32.2/solara/website/pages/documentation/api/utilities/memoize.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/utilities/on_kernel_start.py` & `solara_ui-1.32.2/solara/website/pages/documentation/api/utilities/on_kernel_start.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/api/utilities/widget.py` & `solara_ui-1.32.2/solara/website/pages/documentation/api/utilities/widget.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/advanced/link.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/advanced/link.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/advanced/meta.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/advanced/meta.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/advanced/style.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/advanced/style.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/data/dataframe.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/data/dataframe.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/data/pivot_table.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/data/pivot_table.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/input/file_browser.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/input/file_browser.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/input/file_drop.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/input/file_drop.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/input/slider.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/input/slider.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/lab/chat.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/lab/chat.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/lab/confirmation_dialog.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/lab/confirmation_dialog.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/lab/cookies_headers.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/lab/cookies_headers.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/lab/tab.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/lab/tab.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/lab/tabs.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/lab/tabs.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/lab/theming.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/lab/theming.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/layout/column.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/layout/column.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/layout/columns.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/layout/columns.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/layout/columns_responsive.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/layout/columns_responsive.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/layout/griddraggable.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/layout/griddraggable.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/layout/row.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/layout/row.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/layout/sidebar.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/layout/sidebar.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/output/markdown.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/output/markdown.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/output/markdown_editor.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/output/markdown_editor.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/output/sql_code.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/output/sql_code.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/page/title.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/page/title.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/status/error.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/status/error.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/status/info.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/status/info.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/status/success.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/status/success.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/status/warning.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/status/warning.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/viz/altair.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/viz/altair.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/viz/echarts.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/viz/echarts.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/viz/matplotlib.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/viz/matplotlib.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/viz/plotly.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/viz/plotly.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/components/viz/plotly_express.py` & `solara_ui-1.32.2/solara/website/pages/documentation/components/viz/plotly_express.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/__init__.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/ipycanvas.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/ipycanvas.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/ai/chatbot.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/ai/chatbot.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/ai/tokenizer.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/ai/tokenizer.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/basics/sine.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/basics/sine.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/general/custom_storage.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/general/custom_storage.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/general/deploy_model.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/general/deploy_model.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/general/live_update.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/general/live_update.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/general/login_oauth.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/general/login_oauth.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/general/mycard.vue` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/general/mycard.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/general/pokemon_search.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/general/pokemon_search.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/general/vue_component.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/general/vue_component.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/libraries/altair.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/libraries/altair.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/libraries/bqplot.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/libraries/bqplot.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/libraries/ipyleaflet.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/libraries/ipyleaflet.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/libraries/ipyleaflet_advanced.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/libraries/ipyleaflet_advanced.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/utilities/calculator.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/utilities/calculator.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/utilities/countdown_timer.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/utilities/countdown_timer.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/utilities/todo.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/utilities/todo.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/visualization/annotator.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/visualization/annotator.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/visualization/linked_views.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/visualization/linked_views.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/examples/visualization/plotly.py` & `solara_ui-1.32.2/solara/website/pages/documentation/examples/visualization/plotly.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/faq/content/99-faq.md` & `solara_ui-1.32.2/solara/website/pages/documentation/faq/content/99-faq.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/00-quickstart.md` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/00-quickstart.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/01-introduction.md` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/01-introduction.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/02-installing.md` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/02-installing.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/90-troubleshoot.md` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/90-troubleshoot.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/00-overview.md` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/00-overview.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/20-web-app.md` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/20-web-app.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/30-ipywidgets.md` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/30-ipywidgets.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/40-streamlit.md` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/40-streamlit.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/50-dash.md` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/50-dash.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/60-jupyter-dashboard-part1.py` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/60-jupyter-dashboard-part1.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/SF_crime_sample.csv.gz` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/SF_crime_sample.csv.gz`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/_data_science.ipynb` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/_data_science.ipynb`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/04-tutorials/_jupyter_dashboard_1.ipynb` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/04-tutorials/_jupyter_dashboard_1.ipynb`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/05-fundamentals/10-components.md` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/05-fundamentals/10-components.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/05-fundamentals/50-state-management.md` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/05-fundamentals/50-state-management.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/07-deploying/10-self-hosted.md` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/07-deploying/10-self-hosted.md`

 * *Files 4% similar despite different names*

```diff
@@ -249,28 +249,42 @@
     # }
 }
 ```
 
 An alternative to using the `X-Script-Name` header with uvicorn, would be to pass the `--root-path` flag, e.g.:
 
 ```
-$ SOLARA_APP=sol.py uvicorn --workers 1 --root-path /solara -b 0.0.0.0:8765 solara.server.flask:app
+$ SOLARA_APP=sol.py uvicorn --workers 1 --root-path /solara -b 0.0.0.0:8765 solara.server.starlette:app
 ```
 
 In the case of an [OAuth setup](https://solara.dev/documentation/advanced/enterprise/oauth) it is important to make sure that the `X-Forwarded-Proto` and `Host` headers are forwarded correctly.
 If you are running uvicorn (the default if you use `solara run ...`) you will need to configure uvicorn to accept these headers using e.g.:
 
 ```bash
 export UVICORN_PROXY_HEADERS=1
 export FORWARDED_ALLOW_IPS = "127.0.0.1"  # If your solara-server can *only* be reached by the proxy, you can set it to "*", otherwise put in the IP of the reverse proxy
 ```
 
 Make sure you replace the IP with the correct IP of the reverse proxy server (instead of `127.0.0.1`). If you are sure that only the reverse proxy can reach the solara server, you can consider
 setting `FORWARDED_ALLOW_IPS="*"`.
 
+## HTTPS
+
+Solara does not support running in HTTPS (secure) mode directly. You can use a reverse proxy like Nginx, Traefik or Caddy to handle HTTPS for you.
+
+However, when running solara via uvicorn, it is possible to run uvicorn with HTTPS enabled. For more information, see the uvicorn documentation:
+ https://www.uvicorn.org/deployment/#running-with-https
+
+
+An example command would be:
+
+```
+$ SOLARA_APP=sol.py uvicorn --host 0.0.0.0 --port 8765 solara.server.starlette:app --ssl-keyfile=./key.pem --ssl-certfile=./cert.pem
+```
+
 ## Docker
 
 There is nothing special about running Solara in Docker. The only things you probably need to change is the interface the server binds to.
 Solara by default binds to localhost, so that it is not accessible from the outside world. Apart from that localhost (or `::1` in case of IPv6)
 might not be available, you probably want the outside world to see your Solara app. For that, you can use `--host=0.0.0.0` or `--host=::` option to bind to all interfaces.
 
 Your Dockerfile could look like:
```

### Comparing `solara_ui-1.32.1/solara/website/pages/documentation/getting_started/content/07-deploying/20-cloud-hosted.md` & `solara_ui-1.32.2/solara/website/pages/documentation/getting_started/content/07-deploying/20-cloud-hosted.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/showcase/__init__.py` & `solara_ui-1.32.2/solara/website/pages/showcase/__init__.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/showcase/domino_code_assist.py` & `solara_ui-1.32.2/solara/website/pages/showcase/domino_code_assist.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/showcase/planeto_tessa.py` & `solara_ui-1.32.2/solara/website/pages/showcase/planeto_tessa.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/showcase/solara_dev.py` & `solara_ui-1.32.2/solara/website/pages/showcase/solara_dev.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/showcase/solarathon_2023_team_2.py` & `solara_ui-1.32.2/solara/website/pages/showcase/solarathon_2023_team_2.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/showcase/solarathon_2023_team_4.py` & `solara_ui-1.32.2/solara/website/pages/showcase/solarathon_2023_team_4.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/showcase/solarathon_2023_team_5.py` & `solara_ui-1.32.2/solara/website/pages/showcase/solarathon_2023_team_5.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/showcase/solarathon_2023_team_6.py` & `solara_ui-1.32.2/solara/website/pages/showcase/solarathon_2023_team_6.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/pages/showcase/wanderlust.py` & `solara_ui-1.32.2/solara/website/pages/showcase/wanderlust.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/public/beach.jpeg` & `solara_ui-1.32.2/solara/website/public/beach.jpeg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/public/logo.svg` & `solara_ui-1.32.2/solara/website/public/logo.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/public/success.html` & `solara_ui-1.32.2/solara/website/public/success.html`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/public/social/discord.svg` & `solara_ui-1.32.2/solara/website/public/social/discord.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/public/social/github.svg` & `solara_ui-1.32.2/solara/website/public/social/github.svg`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/website/templates/index.html.j2` & `solara_ui-1.32.2/solara/website/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/widgets/widgets.py` & `solara_ui-1.32.2/solara/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/widgets/vue/gridlayout.vue` & `solara_ui-1.32.2/solara/widgets/vue/gridlayout.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/widgets/vue/navigator.vue` & `solara_ui-1.32.2/solara/widgets/vue/navigator.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/solara/widgets/vue/vegalite.vue` & `solara_ui-1.32.2/solara/widgets/vue/vegalite.vue`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/conftest.py` & `solara_ui-1.32.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/docs/docs_howto_event_with_future_test.py` & `solara_ui-1.32.2/tests/docs/docs_howto_event_with_future_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/docs/docs_howto_event_with_polling_test.py` & `solara_ui-1.32.2/tests/docs/docs_howto_event_with_polling_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/docs/docs_howto_no_browser_api_find_testing_test.py` & `solara_ui-1.32.2/tests/docs/docs_howto_no_browser_api_find_testing_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/docs/docs_howto_no_browser_testing_test.py` & `solara_ui-1.32.2/tests/docs/docs_howto_no_browser_testing_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/docs/docs_howto_no_browser_threaded_test.py` & `solara_ui-1.32.2/tests/docs/docs_howto_no_browser_threaded_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/api_test.py` & `solara_ui-1.32.2/tests/integration/api_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/assets_test.py` & `solara_ui-1.32.2/tests/integration/assets_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/async_test.py` & `solara_ui-1.32.2/tests/integration/async_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/cdn_test.py` & `solara_ui-1.32.2/tests/integration/cdn_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/cmdline_test.py` & `solara_ui-1.32.2/tests/integration/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/conftest.py` & `solara_ui-1.32.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/create_test.py` & `solara_ui-1.32.2/tests/integration/create_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/esm_test.py` & `solara_ui-1.32.2/tests/integration/esm_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/file_download_test.py` & `solara_ui-1.32.2/tests/integration/file_download_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/flask_test.py` & `solara_ui-1.32.2/tests/integration/flask_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/input_date_test.py` & `solara_ui-1.32.2/tests/integration/input_date_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/latex_test.py` & `solara_ui-1.32.2/tests/integration/latex_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/lifecycle_test.py` & `solara_ui-1.32.2/tests/integration/lifecycle_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/markdown_test.py` & `solara_ui-1.32.2/tests/integration/markdown_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/menu_test.py` & `solara_ui-1.32.2/tests/integration/menu_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/popout_test.py` & `solara_ui-1.32.2/tests/integration/popout_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/reconnect_test.py` & `solara_ui-1.32.2/tests/integration/reconnect_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/router_test.py` & `solara_ui-1.32.2/tests/integration/router_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/server_test.py` & `solara_ui-1.32.2/tests/integration/server_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/ssg_test.py` & `solara_ui-1.32.2/tests/integration/ssg_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/starlette_test.py` & `solara_ui-1.32.2/tests/integration/starlette_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/testapp.py` & `solara_ui-1.32.2/tests/integration/testapp.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/widget_test.py` & `solara_ui-1.32.2/tests/integration/widget_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/integration/enterprise/oauth_test.py` & `solara_ui-1.32.2/tests/integration/enterprise/oauth_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-7-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-7-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-8-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/latex_test.py/test_widget_latex_solara-flask-chromium-linux-ipywidgets-8-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-7-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-7-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-8-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_lab-chromium-linux-ipywidgets-8-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-7-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-7-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-8-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-jupyter_notebook-chromium-linux-ipywidgets-8-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-7-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-7-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-8-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-solara-chromium-linux-ipywidgets-8-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-7-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-7-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-8-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-flask-voila-chromium-linux-ipywidgets-8-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-7-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-7-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-8-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_slider_all-starlette-solara-chromium-linux-ipywidgets-8-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_lab-chromium-linux-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_lab-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_notebook-chromium-linux-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-jupyter_notebook-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-solara-chromium-linux-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-solara-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-voila-chromium-linux-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-flask-voila-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-starlette-solara-chromium-linux-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_solara_button_all-starlette-solara-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-ipyvuetify3-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-ipyvuetify3-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-flask-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-ipyvuetify3-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-ipyvuetify3-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-reference.png` & `solara_ui-1.32.2/tests/ui/snapshots/tests/integration/widget_test.py/test_widget_button_solara-starlette-chromium-linux-reference.png`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/app_test.py` & `solara_ui-1.32.2/tests/unit/app_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/applayout_test.py` & `solara_ui-1.32.2/tests/unit/applayout_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/autorouting_test.py` & `solara_ui-1.32.2/tests/unit/autorouting_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/cache_test.py` & `solara_ui-1.32.2/tests/unit/cache_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/cdn_helper_test.py` & `solara_ui-1.32.2/tests/unit/cdn_helper_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/chat_test.py` & `solara_ui-1.32.2/tests/unit/chat_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/checkbox_test.py` & `solara_ui-1.32.2/tests/unit/checkbox_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/common.py` & `solara_ui-1.32.2/tests/unit/common.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/component_frontend_test.py` & `solara_ui-1.32.2/tests/unit/component_frontend_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/confirmation_dialog_test.py` & `solara_ui-1.32.2/tests/unit/confirmation_dialog_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/conftest.py` & `solara_ui-1.32.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/cross_filter_component_test.py` & `solara_ui-1.32.2/tests/unit/cross_filter_component_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/cross_filter_test.py` & `solara_ui-1.32.2/tests/unit/cross_filter_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/dataframe_test.py` & `solara_ui-1.32.2/tests/unit/dataframe_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/datatable_test.py` & `solara_ui-1.32.2/tests/unit/datatable_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/display_test.py` & `solara_ui-1.32.2/tests/unit/display_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/express_test.py` & `solara_ui-1.32.2/tests/unit/express_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/file_browser_test.py` & `solara_ui-1.32.2/tests/unit/file_browser_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/file_download_test.py` & `solara_ui-1.32.2/tests/unit/file_download_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/hooks_test.py` & `solara_ui-1.32.2/tests/unit/hooks_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/input_date_test.py` & `solara_ui-1.32.2/tests/unit/input_date_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/input_test.py` & `solara_ui-1.32.2/tests/unit/input_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/kernel_test.py` & `solara_ui-1.32.2/tests/unit/kernel_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/lifecycle_test.py` & `solara_ui-1.32.2/tests/unit/lifecycle_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/matplotlib_test.py` & `solara_ui-1.32.2/tests/unit/matplotlib_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/output_widget_test.py` & `solara_ui-1.32.2/tests/unit/output_widget_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/patch_test.py` & `solara_ui-1.32.2/tests/unit/patch_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/pivottable_test.py` & `solara_ui-1.32.2/tests/unit/pivottable_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/reload_test.py` & `solara_ui-1.32.2/tests/unit/reload_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/router_test.py` & `solara_ui-1.32.2/tests/unit/router_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/select_test.py` & `solara_ui-1.32.2/tests/unit/select_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/settings_test.py` & `solara_ui-1.32.2/tests/unit/settings_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/shell_test.py` & `solara_ui-1.32.2/tests/unit/shell_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/slider_test.py` & `solara_ui-1.32.2/tests/unit/slider_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/tabs_test.py` & `solara_ui-1.32.2/tests/unit/tabs_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/task_test.py` & `solara_ui-1.32.2/tests/unit/task_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/telemetry_tests.py` & `solara_ui-1.32.2/tests/unit/telemetry_tests.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/toestand_test.py` & `solara_ui-1.32.2/tests/unit/toestand_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/toggle_button_test.py` & `solara_ui-1.32.2/tests/unit/toggle_button_test.py`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/solara_test_apps/notebookapp_component.ipynb` & `solara_ui-1.32.2/tests/unit/solara_test_apps/notebookapp_component.ipynb`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/solara_test_apps/notebookapp_element.ipynb` & `solara_ui-1.32.2/tests/unit/solara_test_apps/notebookapp_element.ipynb`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/solara_test_apps/notebookapp_widget.ipynb` & `solara_ui-1.32.2/tests/unit/solara_test_apps/notebookapp_widget.ipynb`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/solara_test_apps/multipage/03-some-markdown.md` & `solara_ui-1.32.2/tests/unit/solara_test_apps/multipage/03-some-markdown.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/tests/unit/solara_test_apps/multipage-widgets/04-color.ipynb` & `solara_ui-1.32.2/tests/unit/solara_test_apps/multipage-widgets/04-color.ipynb`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/.gitignore` & `solara_ui-1.32.2/.gitignore`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/LICENSE` & `solara_ui-1.32.2/LICENSE`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/README.md` & `solara_ui-1.32.2/README.md`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/pyproject.toml` & `solara_ui-1.32.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `solara_ui-1.32.1/PKG-INFO` & `solara_ui-1.32.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: solara-ui
-Version: 1.32.1
+Version: 1.32.2
 Dynamic: Summary
 Project-URL: Home, https://www.github.com/widgetti/solara
 Project-URL: Documentation, https://solara.dev
 Author-email: "Maarten A. Breddels" <maartenbreddels@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Maarten A. Breddels
```

