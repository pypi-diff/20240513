# Comparing `tmp/grafana_foundation_sdk-1715089318!10.1.0.tar.gz` & `tmp/grafana_foundation_sdk-1715605824!10.1.0.tar.gz`

## Comparing `grafana_foundation_sdk-1715089318!10.1.0.tar` & `grafana_foundation_sdk-1715605824!10.1.0.tar`

### file list

```diff
@@ -1,105 +1,109 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/__init__.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/accesspolicy.py
--rw-r--r--   0        0        0    16488 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/alertgroups.py
--rw-r--r--   0        0        0    18475 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/annotationslist.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/azuremonitor.py
--rw-r--r--   0        0        0    36550 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/barchart.py
--rw-r--r--   0        0        0    18213 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/bargauge.py
--rw-r--r--   0        0        0    46386 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/candlestick.py
--rw-r--r--   0        0        0    16550 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/canvas.py
--rw-r--r--   0        0        0    29609 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/cloudwatch.py
--rw-r--r--   0        0        0    48403 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/common.py
--rw-r--r--   0        0        0    71911 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/dashboard.py
--rw-r--r--   0        0        0    18357 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/dashboardlist.py
--rw-r--r--   0        0        0    15646 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/datagrid.py
--rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/debug.py
--rw-r--r--   0        0        0    62126 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/elasticsearch.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/folder.py
--rw-r--r--   0        0        0    17170 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/gauge.py
--rw-r--r--   0        0        0    17061 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/geomap.py
--rw-r--r--   0        0        0    22978 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/grafanapyroscope.py
--rw-r--r--   0        0        0    23184 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/heatmap.py
--rw-r--r--   0        0        0    29881 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/histogram.py
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/librarypanel.py
--rw-r--r--   0        0        0    18024 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/logs.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/loki.py
--rw-r--r--   0        0        0    15917 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/news.py
--rw-r--r--   0        0        0    15866 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/nodegraph.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/parca.py
--rw-r--r--   0        0        0    18907 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/piechart.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/playlist.py
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/preferences.py
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/prometheus.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/publicdashboard.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/role.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/rolebinding.py
--rw-r--r--   0        0        0    17809 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/stat.py
--rw-r--r--   0        0        0    21233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/statetimeline.py
--rw-r--r--   0        0        0    20932 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/statushistory.py
--rw-r--r--   0        0        0    17923 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/table.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/team.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/tempo.py
--rw-r--r--   0        0        0    11092 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/testdata.py
--rw-r--r--   0        0        0    16131 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/text.py
--rw-r--r--   0        0        0    44391 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/timeseries.py
--rw-r--r--   0        0        0    44124 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/trend.py
--rw-r--r--   0        0        0    34002 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/xychart.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/cog/__init__.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/cog/builder.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/cog/encoder.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/cog/plugins.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/cog/runtime.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/cog/variants.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/__init__.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/accesspolicy.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/alertgroups.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/annotationslist.py
--rw-r--r--   0        0        0    39886 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/azuremonitor.py
--rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/barchart.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/bargauge.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/candlestick.py
--rw-r--r--   0        0        0    13569 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/canvas.py
--rw-r--r--   0        0        0    39994 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/cloudwatch.py
--rw-r--r--   0        0        0    84419 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/common.py
--rw-r--r--   0        0        0    87863 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/dashboard.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/dashboardlist.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/datagrid.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/debug.py
--rw-r--r--   0        0        0    90822 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/elasticsearch.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/folder.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/gauge.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/geomap.py
--rw-r--r--   0        0        0    32434 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/grafanapyroscope.py
--rw-r--r--   0        0        0    20031 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/heatmap.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/histogram.py
--rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/librarypanel.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/logs.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/loki.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/news.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/nodegraph.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/parca.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/piechart.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/playlist.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/preferences.py
--rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/prometheus.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/publicdashboard.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/role.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/rolebinding.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/stat.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/statetimeline.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/statushistory.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/table.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/team.py
--rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/tempo.py
--rw-r--r--   0        0        0    20019 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/testdata.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/text.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/timeseries.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/trend.py
--rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/xychart.py
--rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/LICENSE.md
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/README.md
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/pyproject.toml
--rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715089318!10.1.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/accesspolicy.py
+-rw-r--r--   0        0        0    18780 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/alertgroups.py
+-rw-r--r--   0        0        0    19381 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/alerting.py
+-rw-r--r--   0        0        0    20767 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/annotationslist.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/azuremonitor.py
+-rw-r--r--   0        0        0    38842 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/barchart.py
+-rw-r--r--   0        0        0    20505 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/bargauge.py
+-rw-r--r--   0        0        0    48678 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/candlestick.py
+-rw-r--r--   0        0        0    18842 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/canvas.py
+-rw-r--r--   0        0        0    29609 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/cloudwatch.py
+-rw-r--r--   0        0        0    48403 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/common.py
+-rw-r--r--   0        0        0    76059 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/dashboard.py
+-rw-r--r--   0        0        0    20649 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/dashboardlist.py
+-rw-r--r--   0        0        0    17938 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/datagrid.py
+-rw-r--r--   0        0        0    18133 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/debug.py
+-rw-r--r--   0        0        0    63427 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/elasticsearch.py
+-rw-r--r--   0        0        0    49166 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/expr.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/folder.py
+-rw-r--r--   0        0        0    19462 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/gauge.py
+-rw-r--r--   0        0        0    19353 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/geomap.py
+-rw-r--r--   0        0        0    22904 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/grafanapyroscope.py
+-rw-r--r--   0        0        0    25476 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/heatmap.py
+-rw-r--r--   0        0        0    32173 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/histogram.py
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/librarypanel.py
+-rw-r--r--   0        0        0    20316 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/logs.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/loki.py
+-rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/news.py
+-rw-r--r--   0        0        0    18158 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/nodegraph.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/parca.py
+-rw-r--r--   0        0        0    21199 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/piechart.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/playlist.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/preferences.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/prometheus.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/publicdashboard.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/role.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/rolebinding.py
+-rw-r--r--   0        0        0    20101 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/stat.py
+-rw-r--r--   0        0        0    23525 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/statetimeline.py
+-rw-r--r--   0        0        0    23224 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/statushistory.py
+-rw-r--r--   0        0        0    20215 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/table.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/team.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/tempo.py
+-rw-r--r--   0        0        0    12183 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/testdata.py
+-rw-r--r--   0        0        0    18423 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/text.py
+-rw-r--r--   0        0        0    46683 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/timeseries.py
+-rw-r--r--   0        0        0    46416 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/trend.py
+-rw-r--r--   0        0        0    36294 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/xychart.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/cog/__init__.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/cog/builder.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/cog/encoder.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/cog/plugins.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/cog/runtime.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/cog/variants.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/__init__.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/accesspolicy.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/alertgroups.py
+-rw-r--r--   0        0        0    27377 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/alerting.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/annotationslist.py
+-rw-r--r--   0        0        0    39886 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/azuremonitor.py
+-rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/barchart.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/bargauge.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/candlestick.py
+-rw-r--r--   0        0        0    13569 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/canvas.py
+-rw-r--r--   0        0        0    39994 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/cloudwatch.py
+-rw-r--r--   0        0        0    84419 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/common.py
+-rw-r--r--   0        0        0    87863 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/dashboard.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/dashboardlist.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/datagrid.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/debug.py
+-rw-r--r--   0        0        0    91792 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/elasticsearch.py
+-rw-r--r--   0        0        0    64441 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/expr.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/folder.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/gauge.py
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/geomap.py
+-rw-r--r--   0        0        0    32298 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/grafanapyroscope.py
+-rw-r--r--   0        0        0    20031 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/heatmap.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/histogram.py
+-rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/librarypanel.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/logs.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/loki.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/news.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/nodegraph.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/parca.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/piechart.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/playlist.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/preferences.py
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/prometheus.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/publicdashboard.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/role.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/rolebinding.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/stat.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/statetimeline.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/statushistory.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/table.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/team.py
+-rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/tempo.py
+-rw-r--r--   0        0        0    20919 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/testdata.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/text.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/timeseries.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/trend.py
+-rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/xychart.py
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/LICENSE.md
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/README.md
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605824!10.1.0/PKG-INFO
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/accesspolicy.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/accesspolicy.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
     def __init__(self):
         self._internal = accesspolicy.AccessRule()
 
     def build(self) -> accesspolicy.AccessRule:
         return self._internal    
     
-    def kind(self, kind: typing.Union[typing.Literal["*"]]) -> typing.Self:    
+    def kind(self, kind: str) -> typing.Self:    
         """
         The kind this rule applies to (dashboards, alert, etc)
         """
             
         self._internal.kind = kind
     
         return self
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/alertgroups.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/alertgroups.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -147,14 +157,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -356,14 +377,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -375,14 +416,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/annotationslist.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/annotationslist.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -147,14 +157,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -356,14 +377,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -375,14 +416,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/azuremonitor.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/azuremonitor.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/barchart.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/barchart.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/bargauge.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/bargauge.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/candlestick.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/candlestick.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/canvas.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/canvas.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -147,14 +157,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -356,14 +377,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -375,14 +416,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/cloudwatch.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/common.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/common.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/dashboard.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,14 +274,29 @@
             if self.__current_x >= 24:
                 self.__current_x = 0
                 self.__current_y += self.__last_panel_height
                 self.__last_panel_height = 0
     
         return self
     
+    def variables(self, list_val: list[cogbuilder.Builder[dashboard.VariableModel]]) -> typing.Self:    
+        """
+        Configured template variables
+        """
+            
+        if self._internal.templating is None:
+            self._internal.templating = dashboard.DashboardDashboardTemplating()
+        
+        assert isinstance(self._internal.templating, dashboard.DashboardDashboardTemplating)
+        
+        list_val_resources = [r1.build() for r1 in list_val]
+        self._internal.templating.list_val = list_val_resources
+    
+        return self
+    
     def with_variable(self, list_val: cogbuilder.Builder[dashboard.VariableModel]) -> typing.Self:    
         """
         Configured template variables
         """
             
         if self._internal.templating is None:
             self._internal.templating = dashboard.DashboardDashboardTemplating()
@@ -292,14 +307,32 @@
             self._internal.templating.list_val = []
         
         list_val_resource = list_val.build()
         self._internal.templating.list_val.append(list_val_resource)
     
         return self
     
+    def annotations(self, list_val: list[cogbuilder.Builder[dashboard.AnnotationQuery]]) -> typing.Self:    
+        """
+        Contains the list of annotations that are associated with the dashboard.
+        Annotations are used to overlay event markers and overlay event tags on graphs.
+        Grafana comes with a native annotation store and the ability to add annotation events directly from the graph panel or via the HTTP API.
+        See https://grafana.com/docs/grafana/latest/dashboards/build-dashboards/annotate-visualizations/
+        """
+            
+        if self._internal.annotations is None:
+            self._internal.annotations = dashboard.AnnotationContainer()
+        
+        assert isinstance(self._internal.annotations, dashboard.AnnotationContainer)
+        
+        list_val_resources = [r1.build() for r1 in list_val]
+        self._internal.annotations.list_val = list_val_resources
+    
+        return self
+    
     def annotation(self, list_val: cogbuilder.Builder[dashboard.AnnotationQuery]) -> typing.Self:    
         """
         Contains the list of annotations that are associated with the dashboard.
         Annotations are used to overlay event markers and overlay event tags on graphs.
         Grafana comes with a native annotation store and the ability to add annotation events directly from the graph panel or via the HTTP API.
         See https://grafana.com/docs/grafana/latest/dashboards/build-dashboards/annotate-visualizations/
         """
@@ -313,14 +346,24 @@
             self._internal.annotations.list_val = []
         
         list_val_resource = list_val.build()
         self._internal.annotations.list_val.append(list_val_resource)
     
         return self
     
+    def links(self, links: list[cogbuilder.Builder[dashboard.DashboardLink]]) -> typing.Self:    
+        """
+        Links with references to other dashboards or external websites.
+        """
+            
+        links_resources = [r1.build() for r1 in links]
+        self._internal.links = links_resources
+    
+        return self
+    
     def link(self, links: cogbuilder.Builder[dashboard.DashboardLink]) -> typing.Self:    
         """
         Links with references to other dashboards or external websites.
         """
             
         if self._internal.links is None:
             self._internal.links = []
@@ -938,14 +981,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -1059,14 +1112,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -1268,14 +1332,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -1287,14 +1371,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/dashboardlist.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/dashboardlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -147,14 +157,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -356,14 +377,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -375,14 +416,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/datagrid.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/datagrid.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -147,14 +157,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -356,14 +377,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -375,14 +416,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/debug.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/debug.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -147,14 +157,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -356,14 +377,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -375,14 +416,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/elasticsearch.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/elasticsearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1379,55 +1379,99 @@
 
     def __init__(self):
         self._internal = elasticsearch.Dataquery()
 
     def build(self) -> elasticsearch.Dataquery:
         return self._internal    
     
-    def alias(self, alias: str) -> typing.Self:        
+    def alias(self, alias: str) -> typing.Self:    
+        """
+        Alias pattern
+        """
+            
         self._internal.alias = alias
     
         return self
     
-    def query(self, query: str) -> typing.Self:        
+    def query(self, query: str) -> typing.Self:    
+        """
+        Lucene query
+        """
+            
         self._internal.query = query
     
         return self
     
-    def time_field(self, time_field: str) -> typing.Self:        
+    def time_field(self, time_field: str) -> typing.Self:    
+        """
+        Name of time field
+        """
+            
         self._internal.time_field = time_field
     
         return self
     
-    def bucket_aggs(self, bucket_aggs: list[elasticsearch.BucketAggregation]) -> typing.Self:        
+    def bucket_aggs(self, bucket_aggs: list[elasticsearch.BucketAggregation]) -> typing.Self:    
+        """
+        List of bucket aggregations
+        """
+            
         self._internal.bucket_aggs = bucket_aggs
     
         return self
     
-    def metrics(self, metrics: list[elasticsearch.MetricAggregation]) -> typing.Self:        
+    def metrics(self, metrics: list[elasticsearch.MetricAggregation]) -> typing.Self:    
+        """
+        List of metric aggregations
+        """
+            
         self._internal.metrics = metrics
     
         return self
     
-    def ref_id(self, ref_id: str) -> typing.Self:        
+    def ref_id(self, ref_id: str) -> typing.Self:    
+        """
+        A unique identifier for the query within the list of targets.
+        In server side expressions, the refId is used as a variable name to identify results.
+        By default, the UI will assign A->Z; however setting meaningful names may be useful.
+        """
+            
         self._internal.ref_id = ref_id
     
         return self
     
-    def hide(self, hide: bool) -> typing.Self:        
+    def hide(self, hide: bool) -> typing.Self:    
+        """
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
+        """
+            
         self._internal.hide = hide
     
         return self
     
-    def query_type(self, query_type: str) -> typing.Self:        
+    def query_type(self, query_type: str) -> typing.Self:    
+        """
+        Specify the query flavor
+        TODO make this required and give it a default
+        """
+            
         self._internal.query_type = query_type
     
         return self
     
-    def datasource(self, datasource: object) -> typing.Self:        
+    def datasource(self, datasource: object) -> typing.Self:    
+        """
+        For mixed data sources the selected datasource is on the query level.
+        For non mixed scenarios this is undefined.
+        TODO find a better way to do this ^ that's friendly to schema
+        TODO this shouldn't be unknown but DataSourceRef | null
+        """
+            
         self._internal.datasource = datasource
     
         return self
     
 
 class ElasticsearchDateHistogramSettings(cogbuilder.Builder[elasticsearch.ElasticsearchDateHistogramSettings]):    
     _internal: elasticsearch.ElasticsearchDateHistogramSettings
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/folder.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/folder.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/gauge.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
-from ..models import gauge
+from ..models import text
 from ..cog import variants as cogvariants
-from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "gauge"
+        self._internal.type_val = "text"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +157,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +377,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,14 +416,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -396,59 +451,37 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def show_threshold_labels(self, show_threshold_labels: bool) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        
-        assert isinstance(self._internal.options, gauge.Options)
-        
-        self._internal.options.show_threshold_labels = show_threshold_labels
-    
-        return self
-    
-    def reduce_options(self, reduce_options: cogbuilder.Builder[common.ReduceDataOptions]) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        
-        assert isinstance(self._internal.options, gauge.Options)
-        
-        reduce_options_resource = reduce_options.build()
-        self._internal.options.reduce_options = reduce_options_resource
-    
-        return self
-    
-    def text(self, text: cogbuilder.Builder[common.VizTextDisplayOptions]) -> typing.Self:        
+    def mode(self, mode: text.TextMode) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
+            self._internal.options = text.Options()
         
-        assert isinstance(self._internal.options, gauge.Options)
+        assert isinstance(self._internal.options, text.Options)
         
-        text_resource = text.build()
-        self._internal.options.text = text_resource
+        self._internal.options.mode = mode
     
         return self
     
-    def show_threshold_markers(self, show_threshold_markers: bool) -> typing.Self:        
+    def code(self, code: text.CodeOptions) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
+            self._internal.options = text.Options()
         
-        assert isinstance(self._internal.options, gauge.Options)
+        assert isinstance(self._internal.options, text.Options)
         
-        self._internal.options.show_threshold_markers = show_threshold_markers
+        self._internal.options.code = code
     
         return self
     
-    def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
+    def content(self, content: str) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
+            self._internal.options = text.Options()
         
-        assert isinstance(self._internal.options, gauge.Options)
+        assert isinstance(self._internal.options, text.Options)
         
-        self._internal.options.orientation = orientation
+        self._internal.options.content = content
     
         return self
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/geomap.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/nodegraph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
-from ..models import geomap
+from ..models import nodegraph
 from ..cog import variants as cogvariants
-from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "geomap"
+        self._internal.type_val = "nodeGraph"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +157,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,98 +377,101 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
-    def no_value(self, no_value: str) -> typing.Self:    
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
         """
-        Alternative to empty string
+        Panel color configuration
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
-        self._internal.field_config.defaults.no_value = no_value
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
     
         return self
     
-    def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
+    def no_value(self, no_value: str) -> typing.Self:    
         """
-        Overrides are the options applied to specific fields overriding the defaults.
+        Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         
-        if self._internal.field_config.overrides is None:
-            self._internal.field_config.overrides = []
-        
-        self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
-            matcher=matcher,
-            properties=properties,
-        ))
-    
-        return self
-    
-    def view(self, view: geomap.MapViewConfig) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = geomap.Options()
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
         
-        assert isinstance(self._internal.options, geomap.Options)
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
-        self._internal.options.view = view
+        self._internal.field_config.defaults.no_value = no_value
     
         return self
     
-    def controls(self, controls: geomap.ControlsOptions) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = geomap.Options()
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
         
-        assert isinstance(self._internal.options, geomap.Options)
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         
-        self._internal.options.controls = controls
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
     
         return self
     
-    def basemap(self, basemap: cogbuilder.Builder[common.MapLayerOptions]) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = geomap.Options()
+    def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
         
-        assert isinstance(self._internal.options, geomap.Options)
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         
-        basemap_resource = basemap.build()
-        self._internal.options.basemap = basemap_resource
+        if self._internal.field_config.overrides is None:
+            self._internal.field_config.overrides = []
+        
+        self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
+            matcher=matcher,
+            properties=properties,
+        ))
     
         return self
     
-    def layers(self, layers: list[cogbuilder.Builder[common.MapLayerOptions]]) -> typing.Self:        
+    def nodes(self, nodes: nodegraph.NodeOptions) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = geomap.Options()
+            self._internal.options = nodegraph.Options()
         
-        assert isinstance(self._internal.options, geomap.Options)
+        assert isinstance(self._internal.options, nodegraph.Options)
         
-        layers_resources = [r1.build() for r1 in layers]
-        self._internal.options.layers = layers_resources
+        self._internal.options.nodes = nodes
     
         return self
     
-    def tooltip(self, tooltip: geomap.TooltipOptions) -> typing.Self:        
+    def edges(self, edges: nodegraph.EdgeOptions) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = geomap.Options()
+            self._internal.options = nodegraph.Options()
         
-        assert isinstance(self._internal.options, geomap.Options)
+        assert isinstance(self._internal.options, nodegraph.Options)
         
-        self._internal.options.tooltip = tooltip
+        self._internal.options.edges = edges
     
         return self
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,15 +416,15 @@
         MQL query to be executed.
         """
             
         self._internal.query = query
     
         return self
     
-    def graph_period(self, graph_period: typing.Union[typing.Literal["disabled"]]) -> typing.Self:    
+    def graph_period(self, graph_period: str) -> typing.Self:    
         """
         To disable the graphPeriod, it should explictly be set to 'disabled'.
         """
             
         self._internal.graph_period = graph_period
     
         return self
@@ -649,15 +649,15 @@
         Preprocessor is not part of the API, but is used to store the preprocessor and not affect the UI for the rest of parameters
         """
             
         self._internal.preprocessor = preprocessor
     
         return self
     
-    def graph_period(self, graph_period: typing.Union[typing.Literal["disabled"]]) -> typing.Self:    
+    def graph_period(self, graph_period: str) -> typing.Self:    
         """
         To disable the graphPeriod, it should explictly be set to 'disabled'.
         """
             
         self._internal.graph_period = graph_period
     
         return self
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/heatmap.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/histogram.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/histogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/librarypanel.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/librarypanel.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/logs.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/loki.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/parca.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,78 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
-from ..models import loki
+from ..models import parca
 
 
-class Dataquery(cogbuilder.Builder[loki.Dataquery]):    
-    _internal: loki.Dataquery
+class Dataquery(cogbuilder.Builder[parca.Dataquery]):    
+    _internal: parca.Dataquery
 
     def __init__(self):
-        self._internal = loki.Dataquery()
+        self._internal = parca.Dataquery()
 
-    def build(self) -> loki.Dataquery:
+    def build(self) -> parca.Dataquery:
         return self._internal    
     
-    def expr(self, expr: str) -> typing.Self:        
-        self._internal.expr = expr
+    def label_selector(self, label_selector: str) -> typing.Self:    
+        """
+        Specifies the query label selectors.
+        """
+            
+        self._internal.label_selector = label_selector
     
         return self
     
-    def legend_format(self, legend_format: str) -> typing.Self:        
-        self._internal.legend_format = legend_format
+    def profile_type_id(self, profile_type_id: str) -> typing.Self:    
+        """
+        Specifies the type of profile to query.
+        """
+            
+        self._internal.profile_type_id = profile_type_id
     
         return self
     
-    def max_lines(self, max_lines: int) -> typing.Self:        
-        self._internal.max_lines = max_lines
-    
-        return self
-    
-    def resolution(self, resolution: int) -> typing.Self:        
-        self._internal.resolution = resolution
-    
-        return self
-    
-    def editor_mode(self, editor_mode: loki.QueryEditorMode) -> typing.Self:        
-        self._internal.editor_mode = editor_mode
-    
-        return self
-    
-    def range_val(self, range_val: bool) -> typing.Self:        
-        self._internal.range_val = range_val
-    
-        return self
-    
-    def instant(self, instant: bool) -> typing.Self:        
-        self._internal.instant = instant
-    
-        return self
-    
-    def step(self, step: str) -> typing.Self:        
-        self._internal.step = step
-    
-        return self
-    
-    def ref_id(self, ref_id: str) -> typing.Self:        
+    def ref_id(self, ref_id: str) -> typing.Self:    
+        """
+        A unique identifier for the query within the list of targets.
+        In server side expressions, the refId is used as a variable name to identify results.
+        By default, the UI will assign A->Z; however setting meaningful names may be useful.
+        """
+            
         self._internal.ref_id = ref_id
     
         return self
     
-    def hide(self, hide: bool) -> typing.Self:        
+    def hide(self, hide: bool) -> typing.Self:    
+        """
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
+        """
+            
         self._internal.hide = hide
     
         return self
     
-    def query_type(self, query_type: str) -> typing.Self:        
+    def query_type(self, query_type: str) -> typing.Self:    
+        """
+        Specify the query flavor
+        TODO make this required and give it a default
+        """
+            
         self._internal.query_type = query_type
     
         return self
     
-    def datasource(self, datasource: object) -> typing.Self:        
+    def datasource(self, datasource: object) -> typing.Self:    
+        """
+        For mixed data sources the selected datasource is on the query level.
+        For non mixed scenarios this is undefined.
+        TODO find a better way to do this ^ that's friendly to schema
+        TODO this shouldn't be unknown but DataSourceRef | null
+        """
+            
         self._internal.datasource = datasource
     
         return self
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/news.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/news.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -147,14 +157,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -356,14 +377,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -375,14 +416,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/nodegraph.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/gauge.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
-from ..models import nodegraph
+from ..models import gauge
 from ..cog import variants as cogvariants
+from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "nodeGraph"
+        self._internal.type_val = "gauge"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -147,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -356,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -375,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -395,27 +452,59 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def nodes(self, nodes: nodegraph.NodeOptions) -> typing.Self:        
+    def show_threshold_labels(self, show_threshold_labels: bool) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = gauge.Options()
+        
+        assert isinstance(self._internal.options, gauge.Options)
+        
+        self._internal.options.show_threshold_labels = show_threshold_labels
+    
+        return self
+    
+    def reduce_options(self, reduce_options: cogbuilder.Builder[common.ReduceDataOptions]) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = gauge.Options()
+        
+        assert isinstance(self._internal.options, gauge.Options)
+        
+        reduce_options_resource = reduce_options.build()
+        self._internal.options.reduce_options = reduce_options_resource
+    
+        return self
+    
+    def text(self, text: cogbuilder.Builder[common.VizTextDisplayOptions]) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = gauge.Options()
+        
+        assert isinstance(self._internal.options, gauge.Options)
+        
+        text_resource = text.build()
+        self._internal.options.text = text_resource
+    
+        return self
+    
+    def show_threshold_markers(self, show_threshold_markers: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = nodegraph.Options()
+            self._internal.options = gauge.Options()
         
-        assert isinstance(self._internal.options, nodegraph.Options)
+        assert isinstance(self._internal.options, gauge.Options)
         
-        self._internal.options.nodes = nodes
+        self._internal.options.show_threshold_markers = show_threshold_markers
     
         return self
     
-    def edges(self, edges: nodegraph.EdgeOptions) -> typing.Self:        
+    def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = nodegraph.Options()
+            self._internal.options = gauge.Options()
         
-        assert isinstance(self._internal.options, nodegraph.Options)
+        assert isinstance(self._internal.options, gauge.Options)
         
-        self._internal.options.edges = edges
+        self._internal.options.orientation = orientation
     
         return self
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/piechart.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/piechart.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/playlist.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/playlist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/preferences.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/preferences.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/publicdashboard.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/role.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/role.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         Role description
         """
             
         self._internal.description = description
     
         return self
     
-    def hidden(self, hidden: typing.Union[bool]) -> typing.Self:    
+    def hidden(self, hidden: bool) -> typing.Self:    
         """
         Do not show this role
         """
             
         self._internal.hidden = hidden
     
         return self
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/rolebinding.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/stat.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/stat.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/statetimeline.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/statushistory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
-from ..models import statetimeline
+from ..models import statushistory
 from ..cog import variants as cogvariants
 from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "state-timeline"
+        self._internal.type_val = "status-history"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,121 +417,126 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
-    def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         
-        if self._internal.field_config.overrides is None:
-            self._internal.field_config.overrides = []
-        
-        self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
-            matcher=matcher,
-            properties=properties,
-        ))
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
     
         return self
     
-    def show_value(self, show_value: common.VisibilityMode) -> typing.Self:    
+    def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
-        Show timeline values on chart
+        Overrides are the options applied to specific fields overriding the defaults.
         """
             
-        if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
         
-        assert isinstance(self._internal.options, statetimeline.Options)
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         
-        self._internal.options.show_value = show_value
+        if self._internal.field_config.overrides is None:
+            self._internal.field_config.overrides = []
+        
+        self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
+            matcher=matcher,
+            properties=properties,
+        ))
     
         return self
     
     def row_height(self, row_height: float) -> typing.Self:    
         """
-        Controls the row height
+        Set the height of the rows
         """
             
+        if not row_height >= 0:
+            raise ValueError("row_height must be >= 0")
         if not row_height <= 1:
             raise ValueError("row_height must be <= 1")
         if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
+            self._internal.options = statushistory.Options()
         
-        assert isinstance(self._internal.options, statetimeline.Options)
+        assert isinstance(self._internal.options, statushistory.Options)
         
         self._internal.options.row_height = row_height
     
         return self
     
-    def merge_values(self, merge_values: bool) -> typing.Self:    
+    def show_value(self, show_value: common.VisibilityMode) -> typing.Self:    
         """
-        Merge equal consecutive values
+        Show values on the columns
         """
             
         if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
+            self._internal.options = statushistory.Options()
         
-        assert isinstance(self._internal.options, statetimeline.Options)
+        assert isinstance(self._internal.options, statushistory.Options)
         
-        self._internal.options.merge_values = merge_values
+        self._internal.options.show_value = show_value
     
         return self
     
     def legend(self, legend: cogbuilder.Builder[common.VizLegendOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
+            self._internal.options = statushistory.Options()
         
-        assert isinstance(self._internal.options, statetimeline.Options)
+        assert isinstance(self._internal.options, statushistory.Options)
         
         legend_resource = legend.build()
         self._internal.options.legend = legend_resource
     
         return self
     
     def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
+            self._internal.options = statushistory.Options()
         
-        assert isinstance(self._internal.options, statetimeline.Options)
+        assert isinstance(self._internal.options, statushistory.Options)
         
         tooltip_resource = tooltip.build()
         self._internal.options.tooltip = tooltip_resource
     
         return self
     
     def timezone(self, timezone: list[common.TimeZone]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
+            self._internal.options = statushistory.Options()
         
-        assert isinstance(self._internal.options, statetimeline.Options)
+        assert isinstance(self._internal.options, statushistory.Options)
         
         self._internal.options.timezone = timezone
     
         return self
     
-    def align_value(self, align_value: common.TimelineValueAlignment) -> typing.Self:    
+    def col_width(self, col_width: float) -> typing.Self:    
         """
-        Controls value alignment on the timelines
+        Controls the column width
         """
             
+        if not col_width <= 1:
+            raise ValueError("col_width must be <= 1")
         if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
+            self._internal.options = statushistory.Options()
         
-        assert isinstance(self._internal.options, statetimeline.Options)
+        assert isinstance(self._internal.options, statushistory.Options)
         
-        self._internal.options.align_value = align_value
+        self._internal.options.col_width = col_width
     
         return self
     
     def line_width(self, line_width: int) -> typing.Self:        
         if not line_width <= 10:
             raise ValueError("line_width must be <= 10")
         if self._internal.field_config is None:
@@ -500,17 +546,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = statetimeline.FieldConfig()
+            self._internal.field_config.defaults.custom = statushistory.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, statetimeline.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, statushistory.FieldConfig)
         
         self._internal.field_config.defaults.custom.line_width = line_width
     
         return self
     
     def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
         if self._internal.field_config is None:
@@ -520,17 +566,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = statetimeline.FieldConfig()
+            self._internal.field_config.defaults.custom = statushistory.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, statetimeline.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, statushistory.FieldConfig)
         
         hide_from_resource = hide_from.build()
         self._internal.field_config.defaults.custom.hide_from = hide_from_resource
     
         return self
     
     def fill_opacity(self, fill_opacity: int) -> typing.Self:        
@@ -543,15 +589,15 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = statetimeline.FieldConfig()
+            self._internal.field_config.defaults.custom = statushistory.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, statetimeline.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, statushistory.FieldConfig)
         
         self._internal.field_config.defaults.custom.fill_opacity = fill_opacity
     
         return self
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/statushistory.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
-from ..models import statushistory
+from ..models import table
 from ..cog import variants as cogvariants
 from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "status-history"
+        self._internal.type_val = "table"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -396,152 +452,93 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def row_height(self, row_height: float) -> typing.Self:    
+    def frame_index(self, frame_index: float) -> typing.Self:    
         """
-        Set the height of the rows
+        Represents the index of the selected frame
         """
             
-        if not row_height >= 0:
-            raise ValueError("row_height must be >= 0")
-        if not row_height <= 1:
-            raise ValueError("row_height must be <= 1")
         if self._internal.options is None:
-            self._internal.options = statushistory.Options()
+            self._internal.options = table.Options()
         
-        assert isinstance(self._internal.options, statushistory.Options)
+        assert isinstance(self._internal.options, table.Options)
         
-        self._internal.options.row_height = row_height
+        self._internal.options.frame_index = frame_index
     
         return self
     
-    def show_value(self, show_value: common.VisibilityMode) -> typing.Self:    
+    def show_header(self, show_header: bool) -> typing.Self:    
         """
-        Show values on the columns
+        Controls whether the panel should show the header
         """
             
         if self._internal.options is None:
-            self._internal.options = statushistory.Options()
+            self._internal.options = table.Options()
         
-        assert isinstance(self._internal.options, statushistory.Options)
+        assert isinstance(self._internal.options, table.Options)
         
-        self._internal.options.show_value = show_value
+        self._internal.options.show_header = show_header
     
         return self
     
-    def legend(self, legend: cogbuilder.Builder[common.VizLegendOptions]) -> typing.Self:        
+    def show_type_icons(self, show_type_icons: bool) -> typing.Self:    
+        """
+        Controls whether the header should show icons for the column types
+        """
+            
         if self._internal.options is None:
-            self._internal.options = statushistory.Options()
+            self._internal.options = table.Options()
         
-        assert isinstance(self._internal.options, statushistory.Options)
+        assert isinstance(self._internal.options, table.Options)
         
-        legend_resource = legend.build()
-        self._internal.options.legend = legend_resource
+        self._internal.options.show_type_icons = show_type_icons
     
         return self
     
-    def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
+    def sort_by(self, sort_by: list[cogbuilder.Builder[common.TableSortByFieldState]]) -> typing.Self:    
+        """
+        Used to control row sorting
+        """
+            
         if self._internal.options is None:
-            self._internal.options = statushistory.Options()
+            self._internal.options = table.Options()
         
-        assert isinstance(self._internal.options, statushistory.Options)
+        assert isinstance(self._internal.options, table.Options)
         
-        tooltip_resource = tooltip.build()
-        self._internal.options.tooltip = tooltip_resource
+        sort_by_resources = [r1.build() for r1 in sort_by]
+        self._internal.options.sort_by = sort_by_resources
     
         return self
     
-    def timezone(self, timezone: list[common.TimeZone]) -> typing.Self:        
+    def footer(self, footer: cogbuilder.Builder[common.TableFooterOptions]) -> typing.Self:    
+        """
+        Controls footer options
+        """
+            
         if self._internal.options is None:
-            self._internal.options = statushistory.Options()
+            self._internal.options = table.Options()
         
-        assert isinstance(self._internal.options, statushistory.Options)
+        assert isinstance(self._internal.options, table.Options)
         
-        self._internal.options.timezone = timezone
+        footer_resource = footer.build()
+        self._internal.options.footer = footer_resource
     
         return self
     
-    def col_width(self, col_width: float) -> typing.Self:    
+    def cell_height(self, cell_height: common.TableCellHeight) -> typing.Self:    
         """
-        Controls the column width
+        Controls the height of the rows
         """
             
-        if not col_width <= 1:
-            raise ValueError("col_width must be <= 1")
         if self._internal.options is None:
-            self._internal.options = statushistory.Options()
-        
-        assert isinstance(self._internal.options, statushistory.Options)
-        
-        self._internal.options.col_width = col_width
-    
-        return self
-    
-    def line_width(self, line_width: int) -> typing.Self:        
-        if not line_width <= 10:
-            raise ValueError("line_width must be <= 10")
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = statushistory.FieldConfig()
-        
-        assert isinstance(self._internal.field_config.defaults.custom, statushistory.FieldConfig)
-        
-        self._internal.field_config.defaults.custom.line_width = line_width
-    
-        return self
-    
-    def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = statushistory.FieldConfig()
-        
-        assert isinstance(self._internal.field_config.defaults.custom, statushistory.FieldConfig)
-        
-        hide_from_resource = hide_from.build()
-        self._internal.field_config.defaults.custom.hide_from = hide_from_resource
-    
-        return self
-    
-    def fill_opacity(self, fill_opacity: int) -> typing.Self:        
-        if not fill_opacity <= 100:
-            raise ValueError("fill_opacity must be <= 100")
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = statushistory.FieldConfig()
+            self._internal.options = table.Options()
         
-        assert isinstance(self._internal.field_config.defaults.custom, statushistory.FieldConfig)
+        assert isinstance(self._internal.options, table.Options)
         
-        self._internal.field_config.defaults.custom.fill_opacity = fill_opacity
+        self._internal.options.cell_height = cell_height
     
         return self
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/table.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/geomap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
-from ..models import table
+from ..models import geomap
 from ..cog import variants as cogvariants
 from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "table"
+        self._internal.type_val = "geomap"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,132 +378,133 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
-    def no_value(self, no_value: str) -> typing.Self:    
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
         """
-        Alternative to empty string
+        Panel color configuration
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
-        self._internal.field_config.defaults.no_value = no_value
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
     
         return self
     
-    def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
+    def no_value(self, no_value: str) -> typing.Self:    
         """
-        Overrides are the options applied to specific fields overriding the defaults.
+        Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         
-        if self._internal.field_config.overrides is None:
-            self._internal.field_config.overrides = []
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
         
-        self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
-            matcher=matcher,
-            properties=properties,
-        ))
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        self._internal.field_config.defaults.no_value = no_value
     
         return self
     
-    def frame_index(self, frame_index: float) -> typing.Self:    
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
         """
-        Represents the index of the selected frame
+        Overrides are the options applied to specific fields overriding the defaults.
         """
             
-        if self._internal.options is None:
-            self._internal.options = table.Options()
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
         
-        assert isinstance(self._internal.options, table.Options)
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         
-        self._internal.options.frame_index = frame_index
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
     
         return self
     
-    def show_header(self, show_header: bool) -> typing.Self:    
+    def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
-        Controls whether the panel should show the header
+        Overrides are the options applied to specific fields overriding the defaults.
         """
             
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.overrides is None:
+            self._internal.field_config.overrides = []
+        
+        self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
+            matcher=matcher,
+            properties=properties,
+        ))
+    
+        return self
+    
+    def view(self, view: geomap.MapViewConfig) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = table.Options()
+            self._internal.options = geomap.Options()
         
-        assert isinstance(self._internal.options, table.Options)
+        assert isinstance(self._internal.options, geomap.Options)
         
-        self._internal.options.show_header = show_header
+        self._internal.options.view = view
     
         return self
     
-    def show_type_icons(self, show_type_icons: bool) -> typing.Self:    
-        """
-        Controls whether the header should show icons for the column types
-        """
-            
+    def controls(self, controls: geomap.ControlsOptions) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = table.Options()
+            self._internal.options = geomap.Options()
         
-        assert isinstance(self._internal.options, table.Options)
+        assert isinstance(self._internal.options, geomap.Options)
         
-        self._internal.options.show_type_icons = show_type_icons
+        self._internal.options.controls = controls
     
         return self
     
-    def sort_by(self, sort_by: list[cogbuilder.Builder[common.TableSortByFieldState]]) -> typing.Self:    
-        """
-        Used to control row sorting
-        """
-            
+    def basemap(self, basemap: cogbuilder.Builder[common.MapLayerOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = table.Options()
+            self._internal.options = geomap.Options()
         
-        assert isinstance(self._internal.options, table.Options)
+        assert isinstance(self._internal.options, geomap.Options)
         
-        sort_by_resources = [r1.build() for r1 in sort_by]
-        self._internal.options.sort_by = sort_by_resources
+        basemap_resource = basemap.build()
+        self._internal.options.basemap = basemap_resource
     
         return self
     
-    def footer(self, footer: cogbuilder.Builder[common.TableFooterOptions]) -> typing.Self:    
-        """
-        Controls footer options
-        """
-            
+    def layers(self, layers: list[cogbuilder.Builder[common.MapLayerOptions]]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = table.Options()
+            self._internal.options = geomap.Options()
         
-        assert isinstance(self._internal.options, table.Options)
+        assert isinstance(self._internal.options, geomap.Options)
         
-        footer_resource = footer.build()
-        self._internal.options.footer = footer_resource
+        layers_resources = [r1.build() for r1 in layers]
+        self._internal.options.layers = layers_resources
     
         return self
     
-    def cell_height(self, cell_height: common.TableCellHeight) -> typing.Self:    
-        """
-        Controls the height of the rows
-        """
-            
+    def tooltip(self, tooltip: geomap.TooltipOptions) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = table.Options()
+            self._internal.options = geomap.Options()
         
-        assert isinstance(self._internal.options, table.Options)
+        assert isinstance(self._internal.options, geomap.Options)
         
-        self._internal.options.cell_height = cell_height
+        self._internal.options.tooltip = tooltip
     
         return self
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/team.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/tempo.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/tempo.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/testdata.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/testdata.py`

 * *Files 11% similar despite different names*

```diff
@@ -341,35 +341,63 @@
         return self
     
     def points(self, points: list[list[typing.Union[str, int]]]) -> typing.Self:        
         self._internal.points = points
     
         return self
     
-    def drop_percent(self, drop_percent: float) -> typing.Self:        
+    def drop_percent(self, drop_percent: float) -> typing.Self:    
+        """
+        Drop percentage (the chance we will lose a point 0-100)
+        """
+            
         self._internal.drop_percent = drop_percent
     
         return self
     
-    def ref_id(self, ref_id: str) -> typing.Self:        
+    def ref_id(self, ref_id: str) -> typing.Self:    
+        """
+        A unique identifier for the query within the list of targets.
+        In server side expressions, the refId is used as a variable name to identify results.
+        By default, the UI will assign A->Z; however setting meaningful names may be useful.
+        """
+            
         self._internal.ref_id = ref_id
     
         return self
     
-    def hide(self, hide: bool) -> typing.Self:        
+    def hide(self, hide: bool) -> typing.Self:    
+        """
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
+        """
+            
         self._internal.hide = hide
     
         return self
     
-    def query_type(self, query_type: str) -> typing.Self:        
+    def query_type(self, query_type: str) -> typing.Self:    
+        """
+        Specify the query flavor
+        TODO make this required and give it a default
+        """
+            
         self._internal.query_type = query_type
     
         return self
     
-    def datasource(self, datasource: object) -> typing.Self:        
+    def datasource(self, datasource: object) -> typing.Self:    
+        """
+        For mixed data sources the selected datasource is on the query level.
+        For non mixed scenarios this is undefined.
+        TODO find a better way to do this ^ that's friendly to schema
+        TODO this shouldn't be unknown but DataSourceRef | null
+        """
+            
         self._internal.datasource = datasource
     
         return self
     
 
 class Key(cogbuilder.Builder[testdata.Key]):    
     _internal: testdata.Key
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/text.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/statetimeline.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
-from ..models import text
+from ..models import statetimeline
 from ..cog import variants as cogvariants
+from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "text"
+        self._internal.type_val = "state-timeline"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -147,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -356,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -375,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -395,37 +452,162 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def mode(self, mode: text.TextMode) -> typing.Self:        
+    def show_value(self, show_value: common.VisibilityMode) -> typing.Self:    
+        """
+        Show timeline values on chart
+        """
+            
         if self._internal.options is None:
-            self._internal.options = text.Options()
+            self._internal.options = statetimeline.Options()
         
-        assert isinstance(self._internal.options, text.Options)
+        assert isinstance(self._internal.options, statetimeline.Options)
         
-        self._internal.options.mode = mode
+        self._internal.options.show_value = show_value
     
         return self
     
-    def code(self, code: text.CodeOptions) -> typing.Self:        
+    def row_height(self, row_height: float) -> typing.Self:    
+        """
+        Controls the row height
+        """
+            
+        if not row_height <= 1:
+            raise ValueError("row_height must be <= 1")
         if self._internal.options is None:
-            self._internal.options = text.Options()
+            self._internal.options = statetimeline.Options()
         
-        assert isinstance(self._internal.options, text.Options)
+        assert isinstance(self._internal.options, statetimeline.Options)
         
-        self._internal.options.code = code
+        self._internal.options.row_height = row_height
     
         return self
     
-    def content(self, content: str) -> typing.Self:        
+    def merge_values(self, merge_values: bool) -> typing.Self:    
+        """
+        Merge equal consecutive values
+        """
+            
         if self._internal.options is None:
-            self._internal.options = text.Options()
+            self._internal.options = statetimeline.Options()
+        
+        assert isinstance(self._internal.options, statetimeline.Options)
+        
+        self._internal.options.merge_values = merge_values
+    
+        return self
+    
+    def legend(self, legend: cogbuilder.Builder[common.VizLegendOptions]) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = statetimeline.Options()
+        
+        assert isinstance(self._internal.options, statetimeline.Options)
+        
+        legend_resource = legend.build()
+        self._internal.options.legend = legend_resource
+    
+        return self
+    
+    def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = statetimeline.Options()
+        
+        assert isinstance(self._internal.options, statetimeline.Options)
+        
+        tooltip_resource = tooltip.build()
+        self._internal.options.tooltip = tooltip_resource
+    
+        return self
+    
+    def timezone(self, timezone: list[common.TimeZone]) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = statetimeline.Options()
+        
+        assert isinstance(self._internal.options, statetimeline.Options)
+        
+        self._internal.options.timezone = timezone
+    
+        return self
+    
+    def align_value(self, align_value: common.TimelineValueAlignment) -> typing.Self:    
+        """
+        Controls value alignment on the timelines
+        """
+            
+        if self._internal.options is None:
+            self._internal.options = statetimeline.Options()
+        
+        assert isinstance(self._internal.options, statetimeline.Options)
+        
+        self._internal.options.align_value = align_value
+    
+        return self
+    
+    def line_width(self, line_width: int) -> typing.Self:        
+        if not line_width <= 10:
+            raise ValueError("line_width must be <= 10")
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = statetimeline.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults.custom, statetimeline.FieldConfig)
+        
+        self._internal.field_config.defaults.custom.line_width = line_width
+    
+        return self
+    
+    def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = statetimeline.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults.custom, statetimeline.FieldConfig)
+        
+        hide_from_resource = hide_from.build()
+        self._internal.field_config.defaults.custom.hide_from = hide_from_resource
+    
+        return self
+    
+    def fill_opacity(self, fill_opacity: int) -> typing.Self:        
+        if not fill_opacity <= 100:
+            raise ValueError("fill_opacity must be <= 100")
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = statetimeline.FieldConfig()
         
-        assert isinstance(self._internal.options, text.Options)
+        assert isinstance(self._internal.field_config.defaults.custom, statetimeline.FieldConfig)
         
-        self._internal.options.content = content
+        self._internal.field_config.defaults.custom.fill_opacity = fill_opacity
     
         return self
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/timeseries.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/trend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
-from ..models import timeseries
+from ..models import trend
 from ..cog import variants as cogvariants
 from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "timeseries"
+        self._internal.type_val = "trend"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -396,61 +452,65 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def timezone(self, timezone: list[common.TimeZone]) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = timeseries.Options()
-        
-        assert isinstance(self._internal.options, timeseries.Options)
-        
-        self._internal.options.timezone = timezone
-    
-        return self
-    
     def legend(self, legend: cogbuilder.Builder[common.VizLegendOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = timeseries.Options()
+            self._internal.options = trend.Options()
         
-        assert isinstance(self._internal.options, timeseries.Options)
+        assert isinstance(self._internal.options, trend.Options)
         
         legend_resource = legend.build()
         self._internal.options.legend = legend_resource
     
         return self
     
     def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = timeseries.Options()
+            self._internal.options = trend.Options()
         
-        assert isinstance(self._internal.options, timeseries.Options)
+        assert isinstance(self._internal.options, trend.Options)
         
         tooltip_resource = tooltip.build()
         self._internal.options.tooltip = tooltip_resource
     
         return self
     
+    def x_field(self, x_field: str) -> typing.Self:    
+        """
+        Name of the x field to use (defaults to first number)
+        """
+            
+        if self._internal.options is None:
+            self._internal.options = trend.Options()
+        
+        assert isinstance(self._internal.options, trend.Options)
+        
+        self._internal.options.x_field = x_field
+    
+        return self
+    
     def draw_style(self, draw_style: common.GraphDrawStyle) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.draw_style = draw_style
     
         return self
     
     def gradient_mode(self, gradient_mode: common.GraphGradientMode) -> typing.Self:        
         if self._internal.field_config is None:
@@ -460,17 +520,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.gradient_mode = gradient_mode
     
         return self
     
     def thresholds_style(self, thresholds_style: cogbuilder.Builder[common.GraphThresholdsStyleConfig]) -> typing.Self:        
         if self._internal.field_config is None:
@@ -480,17 +540,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         thresholds_style_resource = thresholds_style.build()
         self._internal.field_config.defaults.custom.thresholds_style = thresholds_style_resource
     
         return self
     
     def line_color(self, line_color: str) -> typing.Self:        
@@ -501,17 +561,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.line_color = line_color
     
         return self
     
     def line_width(self, line_width: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -521,17 +581,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.line_width = line_width
     
         return self
     
     def line_interpolation(self, line_interpolation: common.LineInterpolation) -> typing.Self:        
         if self._internal.field_config is None:
@@ -541,17 +601,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.line_interpolation = line_interpolation
     
         return self
     
     def line_style(self, line_style: cogbuilder.Builder[common.LineStyle]) -> typing.Self:        
         if self._internal.field_config is None:
@@ -561,17 +621,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         line_style_resource = line_style.build()
         self._internal.field_config.defaults.custom.line_style = line_style_resource
     
         return self
     
     def fill_color(self, fill_color: str) -> typing.Self:        
@@ -582,17 +642,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.fill_color = fill_color
     
         return self
     
     def fill_opacity(self, fill_opacity: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -602,17 +662,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.fill_opacity = fill_opacity
     
         return self
     
     def show_points(self, show_points: common.VisibilityMode) -> typing.Self:        
         if self._internal.field_config is None:
@@ -622,17 +682,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.show_points = show_points
     
         return self
     
     def point_size(self, point_size: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -642,17 +702,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.point_size = point_size
     
         return self
     
     def point_color(self, point_color: str) -> typing.Self:        
         if self._internal.field_config is None:
@@ -662,17 +722,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.point_color = point_color
     
         return self
     
     def axis_placement(self, axis_placement: common.AxisPlacement) -> typing.Self:        
         if self._internal.field_config is None:
@@ -682,17 +742,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_placement = axis_placement
     
         return self
     
     def axis_color_mode(self, axis_color_mode: common.AxisColorMode) -> typing.Self:        
         if self._internal.field_config is None:
@@ -702,17 +762,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_color_mode = axis_color_mode
     
         return self
     
     def axis_label(self, axis_label: str) -> typing.Self:        
         if self._internal.field_config is None:
@@ -722,17 +782,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_label = axis_label
     
         return self
     
     def axis_width(self, axis_width: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -742,17 +802,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_width = axis_width
     
         return self
     
     def axis_soft_min(self, axis_soft_min: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -762,17 +822,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_soft_min = axis_soft_min
     
         return self
     
     def axis_soft_max(self, axis_soft_max: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -782,17 +842,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_soft_max = axis_soft_max
     
         return self
     
     def axis_grid_show(self, axis_grid_show: bool) -> typing.Self:        
         if self._internal.field_config is None:
@@ -802,17 +862,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_grid_show = axis_grid_show
     
         return self
     
     def scale_distribution(self, scale_distribution: cogbuilder.Builder[common.ScaleDistributionConfig]) -> typing.Self:        
         if self._internal.field_config is None:
@@ -822,17 +882,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         scale_distribution_resource = scale_distribution.build()
         self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
     
         return self
     
     def bar_alignment(self, bar_alignment: common.BarAlignment) -> typing.Self:        
@@ -843,17 +903,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.bar_alignment = bar_alignment
     
         return self
     
     def bar_width_factor(self, bar_width_factor: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -863,17 +923,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.bar_width_factor = bar_width_factor
     
         return self
     
     def stacking(self, stacking: cogbuilder.Builder[common.StackingConfig]) -> typing.Self:        
         if self._internal.field_config is None:
@@ -883,17 +943,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         stacking_resource = stacking.build()
         self._internal.field_config.defaults.custom.stacking = stacking_resource
     
         return self
     
     def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
@@ -904,17 +964,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         hide_from_resource = hide_from.build()
         self._internal.field_config.defaults.custom.hide_from = hide_from_resource
     
         return self
     
     def transform(self, transform: common.GraphTransform) -> typing.Self:        
@@ -925,17 +985,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.transform = transform
     
         return self
     
     def span_nulls(self, span_nulls: typing.Union[bool, float]) -> typing.Self:    
         """
@@ -951,17 +1011,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.span_nulls = span_nulls
     
         return self
     
     def fill_below_to(self, fill_below_to: str) -> typing.Self:        
         if self._internal.field_config is None:
@@ -971,17 +1031,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.fill_below_to = fill_below_to
     
         return self
     
     def point_symbol(self, point_symbol: str) -> typing.Self:        
         if self._internal.field_config is None:
@@ -991,17 +1051,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.point_symbol = point_symbol
     
         return self
     
     def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
         if self._internal.field_config is None:
@@ -1011,17 +1071,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
     
         return self
     
     def bar_max_width(self, bar_max_width: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -1031,15 +1091,15 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         
         self._internal.field_config.defaults.custom.bar_max_width = bar_max_width
     
         return self
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/trend.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/timeseries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
-from ..models import trend
+from ..models import timeseries
 from ..cog import variants as cogvariants
 from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "trend"
+        self._internal.type_val = "timeseries"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -396,47 +452,43 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def legend(self, legend: cogbuilder.Builder[common.VizLegendOptions]) -> typing.Self:        
+    def timezone(self, timezone: list[common.TimeZone]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = trend.Options()
+            self._internal.options = timeseries.Options()
         
-        assert isinstance(self._internal.options, trend.Options)
+        assert isinstance(self._internal.options, timeseries.Options)
         
-        legend_resource = legend.build()
-        self._internal.options.legend = legend_resource
+        self._internal.options.timezone = timezone
     
         return self
     
-    def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
+    def legend(self, legend: cogbuilder.Builder[common.VizLegendOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = trend.Options()
+            self._internal.options = timeseries.Options()
         
-        assert isinstance(self._internal.options, trend.Options)
+        assert isinstance(self._internal.options, timeseries.Options)
         
-        tooltip_resource = tooltip.build()
-        self._internal.options.tooltip = tooltip_resource
+        legend_resource = legend.build()
+        self._internal.options.legend = legend_resource
     
         return self
     
-    def x_field(self, x_field: str) -> typing.Self:    
-        """
-        Name of the x field to use (defaults to first number)
-        """
-            
+    def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = trend.Options()
+            self._internal.options = timeseries.Options()
         
-        assert isinstance(self._internal.options, trend.Options)
+        assert isinstance(self._internal.options, timeseries.Options)
         
-        self._internal.options.x_field = x_field
+        tooltip_resource = tooltip.build()
+        self._internal.options.tooltip = tooltip_resource
     
         return self
     
     def draw_style(self, draw_style: common.GraphDrawStyle) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         
@@ -444,17 +496,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.draw_style = draw_style
     
         return self
     
     def gradient_mode(self, gradient_mode: common.GraphGradientMode) -> typing.Self:        
         if self._internal.field_config is None:
@@ -464,17 +516,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.gradient_mode = gradient_mode
     
         return self
     
     def thresholds_style(self, thresholds_style: cogbuilder.Builder[common.GraphThresholdsStyleConfig]) -> typing.Self:        
         if self._internal.field_config is None:
@@ -484,17 +536,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         thresholds_style_resource = thresholds_style.build()
         self._internal.field_config.defaults.custom.thresholds_style = thresholds_style_resource
     
         return self
     
     def line_color(self, line_color: str) -> typing.Self:        
@@ -505,17 +557,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.line_color = line_color
     
         return self
     
     def line_width(self, line_width: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -525,17 +577,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.line_width = line_width
     
         return self
     
     def line_interpolation(self, line_interpolation: common.LineInterpolation) -> typing.Self:        
         if self._internal.field_config is None:
@@ -545,17 +597,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.line_interpolation = line_interpolation
     
         return self
     
     def line_style(self, line_style: cogbuilder.Builder[common.LineStyle]) -> typing.Self:        
         if self._internal.field_config is None:
@@ -565,17 +617,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         line_style_resource = line_style.build()
         self._internal.field_config.defaults.custom.line_style = line_style_resource
     
         return self
     
     def fill_color(self, fill_color: str) -> typing.Self:        
@@ -586,17 +638,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.fill_color = fill_color
     
         return self
     
     def fill_opacity(self, fill_opacity: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -606,17 +658,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.fill_opacity = fill_opacity
     
         return self
     
     def show_points(self, show_points: common.VisibilityMode) -> typing.Self:        
         if self._internal.field_config is None:
@@ -626,17 +678,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.show_points = show_points
     
         return self
     
     def point_size(self, point_size: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -646,17 +698,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.point_size = point_size
     
         return self
     
     def point_color(self, point_color: str) -> typing.Self:        
         if self._internal.field_config is None:
@@ -666,17 +718,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.point_color = point_color
     
         return self
     
     def axis_placement(self, axis_placement: common.AxisPlacement) -> typing.Self:        
         if self._internal.field_config is None:
@@ -686,17 +738,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_placement = axis_placement
     
         return self
     
     def axis_color_mode(self, axis_color_mode: common.AxisColorMode) -> typing.Self:        
         if self._internal.field_config is None:
@@ -706,17 +758,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_color_mode = axis_color_mode
     
         return self
     
     def axis_label(self, axis_label: str) -> typing.Self:        
         if self._internal.field_config is None:
@@ -726,17 +778,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_label = axis_label
     
         return self
     
     def axis_width(self, axis_width: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -746,17 +798,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_width = axis_width
     
         return self
     
     def axis_soft_min(self, axis_soft_min: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -766,17 +818,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_soft_min = axis_soft_min
     
         return self
     
     def axis_soft_max(self, axis_soft_max: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -786,17 +838,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_soft_max = axis_soft_max
     
         return self
     
     def axis_grid_show(self, axis_grid_show: bool) -> typing.Self:        
         if self._internal.field_config is None:
@@ -806,17 +858,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_grid_show = axis_grid_show
     
         return self
     
     def scale_distribution(self, scale_distribution: cogbuilder.Builder[common.ScaleDistributionConfig]) -> typing.Self:        
         if self._internal.field_config is None:
@@ -826,17 +878,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         scale_distribution_resource = scale_distribution.build()
         self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
     
         return self
     
     def bar_alignment(self, bar_alignment: common.BarAlignment) -> typing.Self:        
@@ -847,17 +899,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.bar_alignment = bar_alignment
     
         return self
     
     def bar_width_factor(self, bar_width_factor: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -867,17 +919,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.bar_width_factor = bar_width_factor
     
         return self
     
     def stacking(self, stacking: cogbuilder.Builder[common.StackingConfig]) -> typing.Self:        
         if self._internal.field_config is None:
@@ -887,17 +939,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         stacking_resource = stacking.build()
         self._internal.field_config.defaults.custom.stacking = stacking_resource
     
         return self
     
     def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
@@ -908,17 +960,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         hide_from_resource = hide_from.build()
         self._internal.field_config.defaults.custom.hide_from = hide_from_resource
     
         return self
     
     def transform(self, transform: common.GraphTransform) -> typing.Self:        
@@ -929,17 +981,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.transform = transform
     
         return self
     
     def span_nulls(self, span_nulls: typing.Union[bool, float]) -> typing.Self:    
         """
@@ -955,17 +1007,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.span_nulls = span_nulls
     
         return self
     
     def fill_below_to(self, fill_below_to: str) -> typing.Self:        
         if self._internal.field_config is None:
@@ -975,17 +1027,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.fill_below_to = fill_below_to
     
         return self
     
     def point_symbol(self, point_symbol: str) -> typing.Self:        
         if self._internal.field_config is None:
@@ -995,17 +1047,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.point_symbol = point_symbol
     
         return self
     
     def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
         if self._internal.field_config is None:
@@ -1015,17 +1067,17 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
     
         return self
     
     def bar_max_width(self, bar_max_width: float) -> typing.Self:        
         if self._internal.field_config is None:
@@ -1035,15 +1087,15 @@
         
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         
         self._internal.field_config.defaults.custom.bar_max_width = bar_max_width
     
         return self
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/builders/xychart.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/builders/xychart.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,24 @@
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
         """
             
         self._internal.id_val = id_val
     
         return self
     
+    def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
+        """
+        Depends on the panel plugin. See the plugin documentation for details.
+        """
+            
+        targets_resources = [r1.build() for r1 in targets]
+        self._internal.targets = targets_resources
+    
+        return self
+    
     def with_target(self, targets: cogbuilder.Builder[cogvariants.Dataquery]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         if self._internal.targets is None:
             self._internal.targets = []
@@ -148,14 +158,25 @@
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
         return self
     
+    def transformations(self, transformations: list[dashboard.DataTransformerConfig]) -> typing.Self:    
+        """
+        List of transformations that are applied to the panel data before rendering.
+        When there are multiple transformations, Grafana applies them in the order they are listed.
+        Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
+        """
+            
+        self._internal.transformations = transformations
+    
+        return self
+    
     def with_transformation(self, transformations: dashboard.DataTransformerConfig) -> typing.Self:    
         """
         List of transformations that are applied to the panel data before rendering.
         When there are multiple transformations, Grafana applies them in the order they are listed.
         Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
         """
             
@@ -357,14 +378,34 @@
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         thresholds_resource = thresholds.build()
         self._internal.field_config.defaults.thresholds = thresholds_resource
     
         return self
     
+    def color_scheme(self, color: cogbuilder.Builder[dashboard.FieldColor]) -> typing.Self:    
+        """
+        Panel color configuration
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        
+        color_resource = color.build()
+        self._internal.field_config.defaults.color = color_resource
+    
+        return self
+    
     def no_value(self, no_value: str) -> typing.Self:    
         """
         Alternative to empty string
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -376,14 +417,29 @@
         
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         
         self._internal.field_config.defaults.no_value = no_value
     
         return self
     
+    def overrides(self, overrides: list[cogbuilder.Builder[dashboard.DashboardFieldConfigSourceOverrides]]) -> typing.Self:    
+        """
+        Overrides are the options applied to specific fields overriding the defaults.
+        """
+            
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        
+        overrides_resources = [r1.build() for r1 in overrides]
+        self._internal.field_config.overrides = overrides_resources
+    
+        return self
+    
     def with_override(self, matcher: dashboard.MatcherConfig, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:    
         """
         Overrides are the options applied to specific fields overriding the defaults.
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/cog/plugins.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/cog/plugins.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
-from ..models import debug
+from ..models import annotationslist
+from ..models import cloudwatch
+from ..models import geomap
 from ..models import logs
-from ..models import loki
+from ..models import news
+from ..models import nodegraph
 from ..models import datagrid
-from ..models import bargauge
-from ..models import cloudwatch
-from ..models import statushistory
-from ..models import xychart
-from ..models import alertgroups
+from ..models import gauge
+from ..models import googlecloudmonitoring
+from ..models import prometheus
+from ..models import timeseries
+from ..models import azuremonitor
+from ..models import elasticsearch
+from ..models import loki
+from ..models import testdata
+from ..models import text
 from ..models import dashboardlist
-from ..models import statetimeline
-from ..models import heatmap
+from ..models import debug
+from ..models import histogram
 from ..models import tempo
-from ..models import grafanapyroscope
-from ..models import nodegraph
-from ..models import piechart
-from ..models import timeseries
-from ..models import trend
-from ..models import annotationslist
-from ..models import geomap
 from ..models import candlestick
-from ..models import googlecloudmonitoring
-from ..models import histogram
-from ..models import parca
 from ..models import canvas
-from ..models import gauge
-from ..models import prometheus
 from ..models import stat
-from ..models import barchart
-from ..models import elasticsearch
-from ..models import news
 from ..models import table
-from ..models import testdata
-from ..models import text
-from ..models import azuremonitor
+from ..models import trend
+from ..models import bargauge
+from ..models import parca
+from ..models import piechart
+from ..models import xychart
+from ..models import statetimeline
+from ..models import statushistory
+from ..models import alertgroups
+from ..models import barchart
+from ..models import heatmap
+from ..models import grafanapyroscope
 from . import runtime as cogruntime
 
 
 def register_default_plugins():
     # Panelcfg variants
     cogruntime.register_panelcfg_variant(alertgroups.variant_config())
     cogruntime.register_panelcfg_variant(annotationslist.variant_config())
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/cog/runtime.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/cog/runtime.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/accesspolicy.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/accesspolicy.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,22 +98,22 @@
             args["name"] = data["name"]        
 
         return cls(**args)
 
 
 class AccessRule:
     # The kind this rule applies to (dashboards, alert, etc)
-    kind: typing.Union[typing.Literal["*"]]
+    kind: str
     # READ, WRITE, CREATE, DELETE, ...
     # should move to k8s style verbs like: "get", "list", "watch", "create", "update", "patch", "delete"
     verb: typing.Union[typing.Literal["*"]]
     # Specific sub-elements like "alert.rules" or "dashboard.permissions"????
     target: typing.Optional[str]
 
-    def __init__(self, kind: typing.Union[typing.Literal["*"]] = "*", verb: typing.Union[typing.Literal["*"]] = "*", target: typing.Optional[str] = None):
+    def __init__(self, kind: str = "*", verb: typing.Union[typing.Literal["*"]] = "*", target: typing.Optional[str] = None):
         self.kind = kind
         self.verb = verb
         self.target = target
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "kind": self.kind,
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/alertgroups.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/alertgroups.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/annotationslist.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/annotationslist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/azuremonitor.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/azuremonitor.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/barchart.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/barchart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/bargauge.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/bargauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/candlestick.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/candlestick.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/canvas.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/canvas.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/cloudwatch.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/common.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/common.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/dashboard.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/dashboardlist.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/dashboardlist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/datagrid.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/datagrid.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/debug.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/debug.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/elasticsearch.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/elasticsearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1896,22 +1896,39 @@
 PipelineMetricAggregation: typing.TypeAlias = typing.Union['MovingAverage', 'Derivative', 'CumulativeSum', 'BucketScript']
 
 
 MetricAggregationWithSettings: typing.TypeAlias = typing.Union['BucketScript', 'CumulativeSum', 'Derivative', 'SerialDiff', 'RawData', 'RawDocument', 'UniqueCount', 'Percentiles', 'ExtendedStats', 'Min', 'Max', 'Sum', 'Average', 'MovingAverage', 'MovingFunction', 'Logs', 'Rate', 'TopMetrics']
 
 
 class Dataquery(cogvariants.Dataquery):
+    # Alias pattern
     alias: typing.Optional[str]
+    # Lucene query
     query: typing.Optional[str]
+    # Name of time field
     time_field: typing.Optional[str]
+    # List of bucket aggregations
     bucket_aggs: typing.Optional[list['BucketAggregation']]
+    # List of metric aggregations
     metrics: typing.Optional[list['MetricAggregation']]
+    # A unique identifier for the query within the list of targets.
+    # In server side expressions, the refId is used as a variable name to identify results.
+    # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: typing.Optional[str]
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
+    # Specify the query flavor
+    # TODO make this required and give it a default
     query_type: typing.Optional[str]
+    # For mixed data sources the selected datasource is on the query level.
+    # For non mixed scenarios this is undefined.
+    # TODO find a better way to do this ^ that's friendly to schema
+    # TODO this shouldn't be unknown but DataSourceRef | null
     datasource: typing.Optional[object]
 
     def __init__(self, alias: typing.Optional[str] = None, query: typing.Optional[str] = None, time_field: typing.Optional[str] = None, bucket_aggs: typing.Optional[list['BucketAggregation']] = None, metrics: typing.Optional[list['MetricAggregation']] = None, ref_id: typing.Optional[str] = None, hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
         self.alias = alias
         self.query = query
         self.time_field = time_field
         self.bucket_aggs = bucket_aggs
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/folder.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/folder.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/gauge.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/gauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/geomap.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/geomap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/googlecloudmonitoring.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/googlecloudmonitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,17 +363,17 @@
     """
 
     # GCP project to execute the query against.
     project_name: str
     # MQL query to be executed.
     query: str
     # To disable the graphPeriod, it should explictly be set to 'disabled'.
-    graph_period: typing.Optional[typing.Union[typing.Literal["disabled"]]]
+    graph_period: typing.Optional[str]
 
-    def __init__(self, project_name: str = "", query: str = "", graph_period: typing.Optional[typing.Union[typing.Literal["disabled"]]] = None):
+    def __init__(self, project_name: str = "", query: str = "", graph_period: typing.Optional[str] = "disabled"):
         self.project_name = project_name
         self.query = query
         self.graph_period = graph_period
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "projectName": self.project_name,
@@ -507,17 +507,17 @@
     value_type: typing.Optional[str]
     view: typing.Optional[str]
     # MQL query to be executed.
     query: str
     # Preprocessor is not part of the API, but is used to store the preprocessor and not affect the UI for the rest of parameters
     preprocessor: typing.Optional['PreprocessorType']
     # To disable the graphPeriod, it should explictly be set to 'disabled'.
-    graph_period: typing.Optional[typing.Union[typing.Literal["disabled"]]]
+    graph_period: typing.Optional[str]
 
-    def __init__(self, project_name: str = "", per_series_aligner: typing.Optional[str] = None, alignment_period: typing.Optional[str] = None, alias_by: typing.Optional[str] = None, editor_mode: str = "", metric_type: str = "", cross_series_reducer: str = "", group_bys: typing.Optional[list[str]] = None, filters: typing.Optional[list[str]] = None, metric_kind: typing.Optional['MetricKind'] = None, value_type: typing.Optional[str] = None, view: typing.Optional[str] = None, query: str = "", preprocessor: typing.Optional['PreprocessorType'] = None, graph_period: typing.Optional[typing.Union[typing.Literal["disabled"]]] = None):
+    def __init__(self, project_name: str = "", per_series_aligner: typing.Optional[str] = None, alignment_period: typing.Optional[str] = None, alias_by: typing.Optional[str] = None, editor_mode: str = "", metric_type: str = "", cross_series_reducer: str = "", group_bys: typing.Optional[list[str]] = None, filters: typing.Optional[list[str]] = None, metric_kind: typing.Optional['MetricKind'] = None, value_type: typing.Optional[str] = None, view: typing.Optional[str] = None, query: str = "", preprocessor: typing.Optional['PreprocessorType'] = None, graph_period: typing.Optional[str] = "disabled"):
         self.project_name = project_name
         self.per_series_aligner = per_series_aligner
         self.alignment_period = alignment_period
         self.alias_by = alias_by
         self.editor_mode = editor_mode
         self.metric_type = metric_type
         self.cross_series_reducer = cross_series_reducer
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/heatmap.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/heatmap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/histogram.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/histogram.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/librarypanel.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/librarypanel.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/logs.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/logs.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/loki.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/preferences.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,127 +1,132 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
-import enum
-from ..cog import variants as cogvariants
 import typing
-from ..cog import runtime as cogruntime
 
 
-class QueryEditorMode(enum.StrEnum):
-    CODE = "code"
-    BUILDER = "builder"
-
-
-class LokiQueryType(enum.StrEnum):
-    RANGE = "range"
-    INSTANT = "instant"
-    STREAM = "stream"
-
-
-class SupportingQueryType(enum.StrEnum):
-    LOGS_VOLUME = "logsVolume"
-    LOGS_SAMPLE = "logsSample"
-    DATA_SAMPLE = "dataSample"
-
-
-class LokiQueryDirection(enum.StrEnum):
-    FORWARD = "forward"
-    BACKWARD = "backward"
-
-
-class Dataquery(cogvariants.Dataquery):
-    expr: typing.Optional[str]
-    legend_format: typing.Optional[str]
-    max_lines: typing.Optional[int]
-    resolution: typing.Optional[int]
-    editor_mode: typing.Optional['QueryEditorMode']
-    range_val: typing.Optional[bool]
-    instant: typing.Optional[bool]
-    step: typing.Optional[str]
-    ref_id: typing.Optional[str]
-    hide: typing.Optional[bool]
-    query_type: typing.Optional[str]
-    datasource: typing.Optional[object]
-
-    def __init__(self, expr: typing.Optional[str] = None, legend_format: typing.Optional[str] = None, max_lines: typing.Optional[int] = None, resolution: typing.Optional[int] = None, editor_mode: typing.Optional['QueryEditorMode'] = None, range_val: typing.Optional[bool] = None, instant: typing.Optional[bool] = None, step: typing.Optional[str] = None, ref_id: typing.Optional[str] = None, hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
-        self.expr = expr
-        self.legend_format = legend_format
-        self.max_lines = max_lines
-        self.resolution = resolution
-        self.editor_mode = editor_mode
-        self.range_val = range_val
-        self.instant = instant
-        self.step = step
-        self.ref_id = ref_id
-        self.hide = hide
-        self.query_type = query_type
-        self.datasource = datasource
+class Preferences:
+    # UID for the home dashboard
+    home_dashboard_uid: typing.Optional[str]
+    # The timezone selection
+    # TODO: this should use the timezone defined in common
+    timezone: typing.Optional[str]
+    # day of the week (sunday, monday, etc)
+    week_start: typing.Optional[str]
+    # light, dark, empty is default
+    theme: typing.Optional[str]
+    # Selected language (beta)
+    language: typing.Optional[str]
+    # Explore query history preferences
+    query_history: typing.Optional['QueryHistoryPreference']
+    # Cookie preferences
+    cookie_preferences: typing.Optional['CookiePreferences']
+
+    def __init__(self, home_dashboard_uid: typing.Optional[str] = None, timezone: typing.Optional[str] = None, week_start: typing.Optional[str] = None, theme: typing.Optional[str] = None, language: typing.Optional[str] = None, query_history: typing.Optional['QueryHistoryPreference'] = None, cookie_preferences: typing.Optional['CookiePreferences'] = None):
+        self.home_dashboard_uid = home_dashboard_uid
+        self.timezone = timezone
+        self.week_start = week_start
+        self.theme = theme
+        self.language = language
+        self.query_history = query_history
+        self.cookie_preferences = cookie_preferences
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
-        if self.expr is not None:
-            payload["expr"] = self.expr
-        if self.legend_format is not None:
-            payload["legendFormat"] = self.legend_format
-        if self.max_lines is not None:
-            payload["maxLines"] = self.max_lines
-        if self.resolution is not None:
-            payload["resolution"] = self.resolution
-        if self.editor_mode is not None:
-            payload["editorMode"] = self.editor_mode
-        if self.range_val is not None:
-            payload["range"] = self.range_val
-        if self.instant is not None:
-            payload["instant"] = self.instant
-        if self.step is not None:
-            payload["step"] = self.step
-        if self.ref_id is not None:
-            payload["refId"] = self.ref_id
-        if self.hide is not None:
-            payload["hide"] = self.hide
-        if self.query_type is not None:
-            payload["queryType"] = self.query_type
-        if self.datasource is not None:
-            payload["datasource"] = self.datasource
+        if self.home_dashboard_uid is not None:
+            payload["homeDashboardUID"] = self.home_dashboard_uid
+        if self.timezone is not None:
+            payload["timezone"] = self.timezone
+        if self.week_start is not None:
+            payload["weekStart"] = self.week_start
+        if self.theme is not None:
+            payload["theme"] = self.theme
+        if self.language is not None:
+            payload["language"] = self.language
+        if self.query_history is not None:
+            payload["queryHistory"] = self.query_history
+        if self.cookie_preferences is not None:
+            payload["cookiePreferences"] = self.cookie_preferences
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "expr" in data:
-            args["expr"] = data["expr"]
-        if "legendFormat" in data:
-            args["legend_format"] = data["legendFormat"]
-        if "maxLines" in data:
-            args["max_lines"] = data["maxLines"]
-        if "resolution" in data:
-            args["resolution"] = data["resolution"]
-        if "editorMode" in data:
-            args["editor_mode"] = data["editorMode"]
-        if "range" in data:
-            args["range_val"] = data["range"]
-        if "instant" in data:
-            args["instant"] = data["instant"]
-        if "step" in data:
-            args["step"] = data["step"]
-        if "refId" in data:
-            args["ref_id"] = data["refId"]
-        if "hide" in data:
-            args["hide"] = data["hide"]
-        if "queryType" in data:
-            args["query_type"] = data["queryType"]
-        if "datasource" in data:
-            args["datasource"] = data["datasource"]        
+        if "homeDashboardUID" in data:
+            args["home_dashboard_uid"] = data["homeDashboardUID"]
+        if "timezone" in data:
+            args["timezone"] = data["timezone"]
+        if "weekStart" in data:
+            args["week_start"] = data["weekStart"]
+        if "theme" in data:
+            args["theme"] = data["theme"]
+        if "language" in data:
+            args["language"] = data["language"]
+        if "queryHistory" in data:
+            args["query_history"] = QueryHistoryPreference.from_json(data["queryHistory"])
+        if "cookiePreferences" in data:
+            args["cookie_preferences"] = CookiePreferences.from_json(data["cookiePreferences"])        
 
         return cls(**args)
 
 
-def variant_config() -> cogruntime.DataqueryConfig:
-    return cogruntime.DataqueryConfig(
-        identifier="loki",
-        from_json_hook=Dataquery.from_json,
-    )
+class QueryHistoryPreference:
+    # one of: '' | 'query' | 'starred';
+    home_tab: typing.Optional[str]
+
+    def __init__(self, home_tab: typing.Optional[str] = None):
+        self.home_tab = home_tab
+
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+        }
+        if self.home_tab is not None:
+            payload["homeTab"] = self.home_tab
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        
+        if "homeTab" in data:
+            args["home_tab"] = data["homeTab"]        
+
+        return cls(**args)
+
+
+class CookiePreferences:
+    analytics: typing.Optional[object]
+    performance: typing.Optional[object]
+    functional: typing.Optional[object]
+
+    def __init__(self, analytics: typing.Optional[object] = None, performance: typing.Optional[object] = None, functional: typing.Optional[object] = None):
+        self.analytics = analytics
+        self.performance = performance
+        self.functional = functional
+
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+        }
+        if self.analytics is not None:
+            payload["analytics"] = self.analytics
+        if self.performance is not None:
+            payload["performance"] = self.performance
+        if self.functional is not None:
+            payload["functional"] = self.functional
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        
+        if "analytics" in data:
+            args["analytics"] = data["analytics"]
+        if "performance" in data:
+            args["performance"] = data["performance"]
+        if "functional" in data:
+            args["functional"] = data["functional"]        
+
+        return cls(**args)
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/news.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/news.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/nodegraph.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/nodegraph.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/parca.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/table.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,70 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
-import enum
-from ..cog import variants as cogvariants
 import typing
+from ..models import common
 from ..cog import runtime as cogruntime
 
 
-class ParcaQueryType(enum.StrEnum):
-    METRICS = "metrics"
-    PROFILE = "profile"
-    BOTH = "both"
-
-
-class Dataquery(cogvariants.Dataquery):
-    label_selector: typing.Optional[str]
-    profile_type_id: typing.Optional[str]
-    ref_id: typing.Optional[str]
-    hide: typing.Optional[bool]
-    query_type: typing.Optional[str]
-    datasource: typing.Optional[object]
-
-    def __init__(self, label_selector: typing.Optional[str] = "{}", profile_type_id: typing.Optional[str] = None, ref_id: typing.Optional[str] = None, hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
-        self.label_selector = label_selector
-        self.profile_type_id = profile_type_id
-        self.ref_id = ref_id
-        self.hide = hide
-        self.query_type = query_type
-        self.datasource = datasource
+class Options:
+    # Represents the index of the selected frame
+    frame_index: float
+    # Controls whether the panel should show the header
+    show_header: bool
+    # Controls whether the header should show icons for the column types
+    show_type_icons: typing.Optional[bool]
+    # Used to control row sorting
+    sort_by: typing.Optional[list[common.TableSortByFieldState]]
+    # Controls footer options
+    footer: typing.Optional[common.TableFooterOptions]
+    # Controls the height of the rows
+    cell_height: typing.Optional[common.TableCellHeight]
+
+    def __init__(self, frame_index: float = 0, show_header: bool = True, show_type_icons: typing.Optional[bool] = False, sort_by: typing.Optional[list[common.TableSortByFieldState]] = None, footer: typing.Optional[common.TableFooterOptions] = None, cell_height: typing.Optional[common.TableCellHeight] = None):
+        self.frame_index = frame_index
+        self.show_header = show_header
+        self.show_type_icons = show_type_icons
+        self.sort_by = sort_by
+        self.footer = footer if footer is not None else common.TableFooterOptions(count_rows=False, reducer=None, show=False)
+        self.cell_height = cell_height if cell_height is not None else common.TableCellHeight.SM
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
+            "frameIndex": self.frame_index,
+            "showHeader": self.show_header,
         }
-        if self.label_selector is not None:
-            payload["labelSelector"] = self.label_selector
-        if self.profile_type_id is not None:
-            payload["profileTypeId"] = self.profile_type_id
-        if self.ref_id is not None:
-            payload["refId"] = self.ref_id
-        if self.hide is not None:
-            payload["hide"] = self.hide
-        if self.query_type is not None:
-            payload["queryType"] = self.query_type
-        if self.datasource is not None:
-            payload["datasource"] = self.datasource
+        if self.show_type_icons is not None:
+            payload["showTypeIcons"] = self.show_type_icons
+        if self.sort_by is not None:
+            payload["sortBy"] = self.sort_by
+        if self.footer is not None:
+            payload["footer"] = self.footer
+        if self.cell_height is not None:
+            payload["cellHeight"] = self.cell_height
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "labelSelector" in data:
-            args["label_selector"] = data["labelSelector"]
-        if "profileTypeId" in data:
-            args["profile_type_id"] = data["profileTypeId"]
-        if "refId" in data:
-            args["ref_id"] = data["refId"]
-        if "hide" in data:
-            args["hide"] = data["hide"]
-        if "queryType" in data:
-            args["query_type"] = data["queryType"]
-        if "datasource" in data:
-            args["datasource"] = data["datasource"]        
+        if "frameIndex" in data:
+            args["frame_index"] = data["frameIndex"]
+        if "showHeader" in data:
+            args["show_header"] = data["showHeader"]
+        if "showTypeIcons" in data:
+            args["show_type_icons"] = data["showTypeIcons"]
+        if "sortBy" in data:
+            args["sort_by"] = data["sortBy"]
+        if "footer" in data:
+            args["footer"] = common.TableFooterOptions.from_json(data["footer"])
+        if "cellHeight" in data:
+            args["cell_height"] = data["cellHeight"]        
 
         return cls(**args)
 
 
-def variant_config() -> cogruntime.DataqueryConfig:
-    return cogruntime.DataqueryConfig(
-        identifier="parca",
-        from_json_hook=Dataquery.from_json,
+def variant_config():
+    return cogruntime.PanelCfgConfig(
+        identifier="table",
+        options_from_json_hook=Options.from_json,
+        field_config_from_json_hook=None,
     )
-
-
-
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/piechart.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/piechart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/playlist.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/playlist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/publicdashboard.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/role.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/role.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     # Optional display
     display_name: typing.Optional[str]
     # Name of the team.
     group_name: typing.Optional[str]
     # Role description
     description: typing.Optional[str]
     # Do not show this role
-    hidden: typing.Union[bool]
+    hidden: bool
 
-    def __init__(self, name: str = "", display_name: typing.Optional[str] = None, group_name: typing.Optional[str] = None, description: typing.Optional[str] = None, hidden: typing.Union[bool] = False):
+    def __init__(self, name: str = "", display_name: typing.Optional[str] = None, group_name: typing.Optional[str] = None, description: typing.Optional[str] = None, hidden: bool = False):
         self.name = name
         self.display_name = display_name
         self.group_name = group_name
         self.description = description
         self.hidden = hidden
 
     def to_json(self) -> dict[str, object]:
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/rolebinding.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/stat.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/stat.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/statetimeline.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/statetimeline.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/statushistory.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/statushistory.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/team.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/tempo.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/tempo.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/testdata.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/testdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -350,18 +350,31 @@
     csv_content: typing.Optional[str]
     raw_frame_content: typing.Optional[str]
     series_count: typing.Optional[int]
     usa: typing.Optional['USAQuery']
     error_type: typing.Optional[typing.Literal["server_panic", "frontend_exception", "frontend_observable"]]
     span_count: typing.Optional[int]
     points: typing.Optional[list[list[typing.Union[str, int]]]]
+    # Drop percentage (the chance we will lose a point 0-100)
     drop_percent: typing.Optional[float]
+    # A unique identifier for the query within the list of targets.
+    # In server side expressions, the refId is used as a variable name to identify results.
+    # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: typing.Optional[str]
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
+    # Specify the query flavor
+    # TODO make this required and give it a default
     query_type: typing.Optional[str]
+    # For mixed data sources the selected datasource is on the query level.
+    # For non mixed scenarios this is undefined.
+    # TODO find a better way to do this ^ that's friendly to schema
+    # TODO this shouldn't be unknown but DataSourceRef | null
     datasource: typing.Optional[object]
 
     def __init__(self, alias: typing.Optional[str] = None, scenario_id: typing.Optional['TestDataQueryType'] = None, string_input: typing.Optional[str] = None, stream: typing.Optional['StreamingQuery'] = None, pulse_wave: typing.Optional['PulseWaveQuery'] = None, sim: typing.Optional['SimulationQuery'] = None, csv_wave: typing.Optional[list['CSVWave']] = None, labels: typing.Optional[str] = None, lines: typing.Optional[int] = None, level_column: typing.Optional[bool] = None, channel: typing.Optional[str] = None, nodes: typing.Optional['NodesQuery'] = None, csv_file_name: typing.Optional[str] = None, csv_content: typing.Optional[str] = None, raw_frame_content: typing.Optional[str] = None, series_count: typing.Optional[int] = None, usa: typing.Optional['USAQuery'] = None, error_type: typing.Optional[typing.Literal["server_panic", "frontend_exception", "frontend_observable"]] = None, span_count: typing.Optional[int] = None, points: typing.Optional[list[list[typing.Union[str, int]]]] = None, drop_percent: typing.Optional[float] = None, ref_id: typing.Optional[str] = None, hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
         self.alias = alias
         self.scenario_id = scenario_id if scenario_id is not None else TestDataQueryType.RANDOM_WALK
         self.string_input = string_input
         self.stream = stream
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/text.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/text.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/timeseries.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/timeseries.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/trend.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/trend.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/grafana_foundation_sdk/models/xychart.py` & `grafana_foundation_sdk-1715605824!10.1.0/grafana_foundation_sdk/models/xychart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/LICENSE.md` & `grafana_foundation_sdk-1715605824!10.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/README.md` & `grafana_foundation_sdk-1715605824!10.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 > [!NOTE]
 > This branch contains **types and builders generated for Grafana v10.1.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1715089318!10.1.0'
+python3 -m pip install 'grafana_foundation_sdk==1715605824!10.1.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/pyproject.toml` & `grafana_foundation_sdk-1715605824!10.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "observability",
     "sdk",
     "grafana",
     "logs",
     "traces",
     "metrics"
 ]
-version = "1715089318!10.1.0"
+version = "1715605824!10.1.0"
 dependencies = []
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `grafana_foundation_sdk-1715089318!10.1.0/PKG-INFO` & `grafana_foundation_sdk-1715605824!10.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grafana_foundation_sdk
-Version: 1715089318!10.1.0
+Version: 1715605824!10.1.0
 Summary: A set of tools, types and libraries for building and manipulating Grafana objects.
 Project-URL: Homepage, https://github.com/grafana/grafana-foundation-sdk
 Project-URL: Repository, https://github.com/grafana/grafana-foundation-sdk.git
 Project-URL: Issues, https://github.com/grafana/grafana-foundation-sdk/issues
 Author: Grafana Labs
 License-File: LICENSE.md
 Keywords: grafana,logs,metrics,observability,sdk,traces
@@ -27,15 +27,15 @@
 > [!NOTE]
 > This branch contains **types and builders generated for Grafana v10.1.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1715089318!10.1.0'
+python3 -m pip install 'grafana_foundation_sdk==1715605824!10.1.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```

