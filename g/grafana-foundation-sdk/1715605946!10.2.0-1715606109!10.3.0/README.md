# Comparing `tmp/grafana_foundation_sdk-1715605946!10.2.0.tar.gz` & `tmp/grafana_foundation_sdk-1715606109!10.3.0.tar.gz`

## Comparing `grafana_foundation_sdk-1715605946!10.2.0.tar` & `grafana_foundation_sdk-1715606109!10.3.0.tar`

### file list

```diff
@@ -1,107 +1,105 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/accesspolicy.py
--rw-r--r--   0        0        0    19379 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/alertgroups.py
--rw-r--r--   0        0        0    19721 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/alerting.py
--rw-r--r--   0        0        0    21366 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/annotationslist.py
--rw-r--r--   0        0        0    27683 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/azuremonitor.py
--rw-r--r--   0        0        0    40353 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/barchart.py
--rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/bargauge.py
--rw-r--r--   0        0        0    50195 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/candlestick.py
--rw-r--r--   0        0        0    19441 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/canvas.py
--rw-r--r--   0        0        0    29609 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/cloudwatch.py
--rw-r--r--   0        0        0    49050 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/common.py
--rw-r--r--   0        0        0    71463 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/dashboard.py
--rw-r--r--   0        0        0    21699 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/dashboardlist.py
--rw-r--r--   0        0        0    18537 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/datagrid.py
--rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/debug.py
--rw-r--r--   0        0        0    63427 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/elasticsearch.py
--rw-r--r--   0        0        0    49166 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/expr.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/folder.py
--rw-r--r--   0        0        0    21081 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/gauge.py
--rw-r--r--   0        0        0    19952 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/geomap.py
--rw-r--r--   0        0        0    19922 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/grafanapyroscope.py
--rw-r--r--   0        0        0    26075 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/heatmap.py
--rw-r--r--   0        0        0    33686 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/histogram.py
--rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/librarypanel.py
--rw-r--r--   0        0        0    20915 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/logs.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/loki.py
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/news.py
--rw-r--r--   0        0        0    18757 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/nodegraph.py
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/parca.py
--rw-r--r--   0        0        0    21798 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/piechart.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/preferences.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/prometheus.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/publicdashboard.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/role.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/rolebinding.py
--rw-r--r--   0        0        0    21033 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/stat.py
--rw-r--r--   0        0        0    24124 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/statetimeline.py
--rw-r--r--   0        0        0    23823 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/statushistory.py
--rw-r--r--   0        0        0    29069 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/table.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/team.py
--rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/tempo.py
--rw-r--r--   0        0        0    12347 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/testdata.py
--rw-r--r--   0        0        0    19022 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/text.py
--rw-r--r--   0        0        0    48198 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/timeseries.py
--rw-r--r--   0        0        0    47921 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/trend.py
--rw-r--r--   0        0        0    37803 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/xychart.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/cog/__init__.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/cog/builder.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/cog/encoder.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/cog/plugins.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/cog/runtime.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/cog/variants.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/__init__.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/accesspolicy.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/alertgroups.py
--rw-r--r--   0        0        0    27221 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/alerting.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/annotationslist.py
--rw-r--r--   0        0        0    40767 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/azuremonitor.py
--rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/barchart.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/bargauge.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/candlestick.py
--rw-r--r--   0        0        0    13660 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/canvas.py
--rw-r--r--   0        0        0    39994 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/cloudwatch.py
--rw-r--r--   0        0        0    86075 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/common.py
--rw-r--r--   0        0        0    85133 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/dashboard.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/dashboardlist.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/datagrid.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/debug.py
--rw-r--r--   0        0        0    91792 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/elasticsearch.py
--rw-r--r--   0        0        0    64441 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/expr.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/folder.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/gauge.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/geomap.py
--rw-r--r--   0        0        0    27647 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/grafanapyroscope.py
--rw-r--r--   0        0        0    20787 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/heatmap.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/histogram.py
--rw-r--r--   0        0        0    15800 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/librarypanel.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/logs.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/loki.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/news.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/nodegraph.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/parca.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/piechart.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/preferences.py
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/prometheus.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/publicdashboard.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/role.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/rolebinding.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/stat.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/statetimeline.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/statushistory.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/table.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/team.py
--rw-r--r--   0        0        0    10653 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/tempo.py
--rw-r--r--   0        0        0    21260 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/testdata.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/text.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/timeseries.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/trend.py
--rw-r--r--   0        0        0    17916 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/xychart.py
--rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/LICENSE.md
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/README.md
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/pyproject.toml
--rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715605946!10.2.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/accesspolicy.py
+-rw-r--r--   0        0        0    19379 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/alertgroups.py
+-rw-r--r--   0        0        0    19721 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/alerting.py
+-rw-r--r--   0        0        0    21366 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/annotationslist.py
+-rw-r--r--   0        0        0    27683 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/azuremonitor.py
+-rw-r--r--   0        0        0    40353 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/barchart.py
+-rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/bargauge.py
+-rw-r--r--   0        0        0    50195 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/candlestick.py
+-rw-r--r--   0        0        0    19827 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/canvas.py
+-rw-r--r--   0        0        0    29609 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/cloudwatch.py
+-rw-r--r--   0        0        0    49050 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/common.py
+-rw-r--r--   0        0        0    69424 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/dashboard.py
+-rw-r--r--   0        0        0    21699 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/dashboardlist.py
+-rw-r--r--   0        0        0    18537 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/datagrid.py
+-rw-r--r--   0        0        0    18732 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/debug.py
+-rw-r--r--   0        0        0    63427 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/elasticsearch.py
+-rw-r--r--   0        0        0    49166 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/expr.py
+-rw-r--r--   0        0        0    21081 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/gauge.py
+-rw-r--r--   0        0        0    19952 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/geomap.py
+-rw-r--r--   0        0        0    19922 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/grafanapyroscope.py
+-rw-r--r--   0        0        0    26075 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/heatmap.py
+-rw-r--r--   0        0        0    33686 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/histogram.py
+-rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/librarypanel.py
+-rw-r--r--   0        0        0    20915 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/logs.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/loki.py
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/news.py
+-rw-r--r--   0        0        0    18757 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/nodegraph.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/parca.py
+-rw-r--r--   0        0        0    21798 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/piechart.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/preferences.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/prometheus.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/publicdashboard.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/role.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/rolebinding.py
+-rw-r--r--   0        0        0    21398 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/stat.py
+-rw-r--r--   0        0        0    24124 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/statetimeline.py
+-rw-r--r--   0        0        0    23823 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/statushistory.py
+-rw-r--r--   0        0        0    29069 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/table.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/team.py
+-rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/tempo.py
+-rw-r--r--   0        0        0    12347 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/testdata.py
+-rw-r--r--   0        0        0    19022 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/text.py
+-rw-r--r--   0        0        0    48198 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/timeseries.py
+-rw-r--r--   0        0        0    47921 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/trend.py
+-rw-r--r--   0        0        0    37915 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/xychart.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/cog/__init__.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/cog/builder.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/cog/encoder.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/cog/plugins.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/cog/runtime.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/cog/variants.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/__init__.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/accesspolicy.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/alertgroups.py
+-rw-r--r--   0        0        0    27221 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/alerting.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/annotationslist.py
+-rw-r--r--   0        0        0    40767 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/azuremonitor.py
+-rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/barchart.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/bargauge.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/candlestick.py
+-rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/canvas.py
+-rw-r--r--   0        0        0    39994 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/cloudwatch.py
+-rw-r--r--   0        0        0    86326 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/common.py
+-rw-r--r--   0        0        0    84422 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/dashboard.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/dashboardlist.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/datagrid.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/debug.py
+-rw-r--r--   0        0        0    91792 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/elasticsearch.py
+-rw-r--r--   0        0        0    64441 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/expr.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/gauge.py
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/geomap.py
+-rw-r--r--   0        0        0    27647 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/grafanapyroscope.py
+-rw-r--r--   0        0        0    20904 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/heatmap.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/histogram.py
+-rw-r--r--   0        0        0    15800 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/librarypanel.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/logs.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/loki.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/news.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/nodegraph.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/parca.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/piechart.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/preferences.py
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/prometheus.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/publicdashboard.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/role.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/rolebinding.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/stat.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/statetimeline.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/statushistory.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/table.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/team.py
+-rw-r--r--   0        0        0    10653 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/tempo.py
+-rw-r--r--   0        0        0    21260 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/testdata.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/text.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/timeseries.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/trend.py
+-rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/xychart.py
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/LICENSE.md
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/README.md
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715606109!10.3.0/PKG-INFO
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/accesspolicy.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/accesspolicy.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/alertgroups.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/alertgroups.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/alerting.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/alerting.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/annotationslist.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/annotationslist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/azuremonitor.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/azuremonitor.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/barchart.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/barchart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/bargauge.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/bargauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/candlestick.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/candlestick.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/canvas.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -498,14 +498,28 @@
         
         assert isinstance(self._internal.options, canvas.Options)
         
         self._internal.options.show_advanced_types = show_advanced_types
     
         return self
     
+    def pan_zoom(self, pan_zoom: bool) -> typing.Self:    
+        """
+        Enable pan and zoom
+        """
+            
+        if self._internal.options is None:
+            self._internal.options = canvas.Options()
+        
+        assert isinstance(self._internal.options, canvas.Options)
+        
+        self._internal.options.pan_zoom = pan_zoom
+    
+        return self
+    
     def root(self, root: canvas.CanvasOptionsRoot) -> typing.Self:    
         """
         The root element of canvas (frame), where all canvas elements are nested
         TODO: Figure out how to define a default value for this
         """
             
         if self._internal.options is None:
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/cloudwatch.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/common.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/common.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/dashboard.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1770,60 +1770,28 @@
         Options that can be selected for a variable.
         """
             
         self._internal.options = options
     
         return self
     
-    def refresh(self, refresh: dashboard.VariableRefresh) -> typing.Self:    
-        """
-        Options to config when to refresh a variable
-        """
-            
+    def refresh(self, refresh: dashboard.VariableRefresh) -> typing.Self:        
         self._internal.refresh = refresh
     
         return self
     
     def sort(self, sort: dashboard.VariableSort) -> typing.Self:    
         """
         Options sort order
         """
             
         self._internal.sort = sort
     
         return self
     
-    def include_all(self, include_all: bool) -> typing.Self:    
-        """
-        Whether all value option is available or not
-        """
-            
-        self._internal.include_all = include_all
-    
-        return self
-    
-    def all_value(self, all_value: str) -> typing.Self:    
-        """
-        Custom all value
-        """
-            
-        self._internal.all_value = all_value
-    
-        return self
-    
-    def regex(self, regex: str) -> typing.Self:    
-        """
-        Optional field, if you want to extract part of a series name or metric node segment.
-        Named capture groups can be used to separate the display text and value.
-        """
-            
-        self._internal.regex = regex
-    
-        return self
-    
 
 class AdHocVariable(cogbuilder.Builder[dashboard.VariableModel]):    
     """
     A variable is a placeholder for a value. You can use variables in metric queries and in panel titles.
     """
     
     _internal: dashboard.VariableModel
@@ -2008,42 +1976,14 @@
         Whether multiple values can be selected or not from variable value list
         """
             
         self._internal.multi = multi
     
         return self
     
-    def include_all(self, include_all: bool) -> typing.Self:    
-        """
-        Whether all value option is available or not
-        """
-            
-        self._internal.include_all = include_all
-    
-        return self
-    
-    def all_value(self, all_value: str) -> typing.Self:    
-        """
-        Custom all value
-        """
-            
-        self._internal.all_value = all_value
-    
-        return self
-    
-    def regex(self, regex: str) -> typing.Self:    
-        """
-        Optional field, if you want to extract part of a series name or metric node segment.
-        Named capture groups can be used to separate the display text and value.
-        """
-            
-        self._internal.regex = regex
-    
-        return self
-    
 
 class IntervalVariable(cogbuilder.Builder[dashboard.VariableModel]):    
     """
     A variable is a placeholder for a value. You can use variables in metric queries and in panel titles.
     """
     
     _internal: dashboard.VariableModel
@@ -2281,26 +2221,8 @@
         """
         Options that can be selected for a variable.
         """
             
         self._internal.options = options
     
         return self
-    
-    def include_all(self, include_all: bool) -> typing.Self:    
-        """
-        Whether all value option is available or not
-        """
-            
-        self._internal.include_all = include_all
-    
-        return self
-    
-    def all_value(self, all_value: str) -> typing.Self:    
-        """
-        Custom all value
-        """
-            
-        self._internal.all_value = all_value
-    
-        return self
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/dashboardlist.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/dashboardlist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/datagrid.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/datagrid.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/debug.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/debug.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/elasticsearch.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/expr.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/expr.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/gauge.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/gauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/geomap.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/geomap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/grafanapyroscope.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/grafanapyroscope.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/heatmap.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/heatmap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/histogram.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/histogram.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/librarypanel.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/librarypanel.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/logs.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/logs.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/loki.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/loki.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/news.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/news.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/nodegraph.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/nodegraph.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/parca.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/parca.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/piechart.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/piechart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/preferences.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/preferences.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/prometheus.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/prometheus.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/publicdashboard.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/role.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/role.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/rolebinding.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/stat.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/stat.py`

 * *Files 3% similar despite different names*

```diff
@@ -511,14 +511,24 @@
         
         assert isinstance(self._internal.options, stat.Options)
         
         self._internal.options.text_mode = text_mode
     
         return self
     
+    def wide_layout(self, wide_layout: bool) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = stat.Options()
+        
+        assert isinstance(self._internal.options, stat.Options)
+        
+        self._internal.options.wide_layout = wide_layout
+    
+        return self
+    
     def reduce_options(self, reduce_options: cogbuilder.Builder[common.ReduceDataOptions]) -> typing.Self:        
         if self._internal.options is None:
             self._internal.options = stat.Options()
         
         assert isinstance(self._internal.options, stat.Options)
         
         reduce_options_resource = reduce_options.build()
@@ -533,21 +543,21 @@
         assert isinstance(self._internal.options, stat.Options)
         
         text_resource = text.build()
         self._internal.options.text = text_resource
     
         return self
     
-    def wide_layout(self, wide_layout: bool) -> typing.Self:        
+    def show_percent_change(self, show_percent_change: bool) -> typing.Self:        
         if self._internal.options is None:
             self._internal.options = stat.Options()
         
         assert isinstance(self._internal.options, stat.Options)
         
-        self._internal.options.wide_layout = wide_layout
+        self._internal.options.show_percent_change = show_percent_change
     
         return self
     
     def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
         if self._internal.options is None:
             self._internal.options = stat.Options()
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/statetimeline.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/statetimeline.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/statushistory.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/statushistory.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/table.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/table.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/team.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/tempo.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/tempo.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/testdata.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/testdata.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/text.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/text.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/timeseries.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/timeseries.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/trend.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/trend.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/builders/xychart.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/builders/xychart.py`

 * *Files 0% similar despite different names*

```diff
@@ -870,15 +870,19 @@
         
         assert isinstance(self._internal.options, xychart.Options)
         
         self._internal.options.series_mapping = series_mapping
     
         return self
     
-    def dims(self, dims: xychart.XYDimensionConfig) -> typing.Self:        
+    def dims(self, dims: xychart.XYDimensionConfig) -> typing.Self:    
+        """
+        Table Mode (auto)
+        """
+            
         if self._internal.options is None:
             self._internal.options = xychart.Options()
         
         assert isinstance(self._internal.options, xychart.Options)
         
         self._internal.options.dims = dims
     
@@ -902,15 +906,19 @@
         assert isinstance(self._internal.options, xychart.Options)
         
         tooltip_resource = tooltip.build()
         self._internal.options.tooltip = tooltip_resource
     
         return self
     
-    def series(self, series: list[xychart.ScatterSeriesConfig]) -> typing.Self:        
+    def series(self, series: list[xychart.ScatterSeriesConfig]) -> typing.Self:    
+        """
+        Manual Mode
+        """
+            
         if self._internal.options is None:
             self._internal.options = xychart.Options()
         
         assert isinstance(self._internal.options, xychart.Options)
         
         self._internal.options.series = series
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/cog/plugins.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/cog/plugins.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
-from ..models import trend
+from ..models import azuremonitor
 from ..models import cloudwatch
+from ..models import gauge
+from ..models import googlecloudmonitoring
+from ..models import statushistory
+from ..models import dashboardlist
 from ..models import datagrid
 from ..models import debug
+from ..models import elasticsearch
 from ..models import grafanapyroscope
-from ..models import nodegraph
+from ..models import news
 from ..models import piechart
-from ..models import prometheus
-from ..models import xychart
-from ..models import annotationslist
-from ..models import bargauge
-from ..models import dashboardlist
-from ..models import heatmap
-from ..models import canvas
-from ..models import parca
-from ..models import tempo
-from ..models import logs
-from ..models import statushistory
+from ..models import barchart
+from ..models import text
 from ..models import timeseries
-from ..models import azuremonitor
-from ..models import geomap
-from ..models import googlecloudmonitoring
+from ..models import testdata
+from ..models import annotationslist
 from ..models import histogram
+from ..models import loki
+from ..models import prometheus
 from ..models import statetimeline
-from ..models import table
-from ..models import testdata
 from ..models import alertgroups
-from ..models import elasticsearch
-from ..models import gauge
-from ..models import loki
-from ..models import news
-from ..models import barchart
 from ..models import candlestick
+from ..models import logs
+from ..models import parca
 from ..models import stat
-from ..models import text
+from ..models import table
+from ..models import xychart
+from ..models import nodegraph
+from ..models import bargauge
+from ..models import canvas
+from ..models import heatmap
+from ..models import trend
+from ..models import tempo
+from ..models import geomap
 from . import runtime as cogruntime
 
 
 def register_default_plugins():
     # Panelcfg variants
     cogruntime.register_panelcfg_variant(alertgroups.variant_config())
     cogruntime.register_panelcfg_variant(annotationslist.variant_config())
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/cog/runtime.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/cog/runtime.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/accesspolicy.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/accesspolicy.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/alertgroups.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/alertgroups.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/alerting.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/alerting.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/annotationslist.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/annotationslist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/azuremonitor.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/azuremonitor.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/barchart.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/barchart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/bargauge.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/bargauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/candlestick.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/candlestick.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/canvas.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/canvas.py`

 * *Files 4% similar despite different names*

```diff
@@ -328,39 +328,45 @@
 
 
 class Options:
     # Enable inline editing
     inline_editing: bool
     # Show all available element types
     show_advanced_types: bool
+    # Enable pan and zoom
+    pan_zoom: bool
     # The root element of canvas (frame), where all canvas elements are nested
     # TODO: Figure out how to define a default value for this
     root: 'CanvasOptionsRoot'
 
-    def __init__(self, inline_editing: bool = True, show_advanced_types: bool = True, root: typing.Optional['CanvasOptionsRoot'] = None):
+    def __init__(self, inline_editing: bool = True, show_advanced_types: bool = True, pan_zoom: bool = True, root: typing.Optional['CanvasOptionsRoot'] = None):
         self.inline_editing = inline_editing
         self.show_advanced_types = show_advanced_types
+        self.pan_zoom = pan_zoom
         self.root = root if root is not None else CanvasOptionsRoot()
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "inlineEditing": self.inline_editing,
             "showAdvancedTypes": self.show_advanced_types,
+            "panZoom": self.pan_zoom,
             "root": self.root,
         }
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "inlineEditing" in data:
             args["inline_editing"] = data["inlineEditing"]
         if "showAdvancedTypes" in data:
             args["show_advanced_types"] = data["showAdvancedTypes"]
+        if "panZoom" in data:
+            args["pan_zoom"] = data["panZoom"]
         if "root" in data:
             args["root"] = CanvasOptionsRoot.from_json(data["root"])        
 
         return cls(**args)
 
 
 class CanvasOptionsRoot:
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/cloudwatch.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/cloudwatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -896,15 +896,15 @@
         return cls(**args)
 
 
 CloudWatchQuery: typing.TypeAlias = typing.Union['CloudWatchMetricsQuery', 'CloudWatchLogsQuery', 'CloudWatchAnnotationQuery']
 
 
 def variant_config() -> cogruntime.DataqueryConfig:
-    decoding_map: dict[str, typing.Union[typing.Type[CloudWatchMetricsQuery], typing.Type[CloudWatchLogsQuery], typing.Type[CloudWatchAnnotationQuery]]] = {"Metrics": CloudWatchMetricsQuery, "Logs": CloudWatchLogsQuery, "Annotations": CloudWatchAnnotationQuery}
+    decoding_map: dict[str, typing.Union[typing.Type[CloudWatchLogsQuery], typing.Type[CloudWatchAnnotationQuery], typing.Type[CloudWatchMetricsQuery]]] = {"Logs": CloudWatchLogsQuery, "Annotations": CloudWatchAnnotationQuery, "Metrics": CloudWatchMetricsQuery}
     return cogruntime.DataqueryConfig(
         identifier="cloudwatch",
         from_json_hook=lambda data: decoding_map[data["queryMode"]].from_json(data),
     )
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/common.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
+import enum
 import typing
 from ..cog import variants as cogvariants
 from ..cog import runtime as cogruntime
-import enum
+
+
+class DataTopic(enum.StrEnum):
+    """
+    A topic is attached to DataFrame metadata in query results.
+    This specifies where the data should be used.
+    """
+
+    SERIES = "series"
+    ANNOTATIONS = "annotations"
+    ALERT_STATES = "alertStates"
 
 
 class DataSourceJsonData:
     """
     TODO docs
     """
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/dashboard.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,43 +408,32 @@
     datasource: typing.Optional['DataSourceRef']
     # Shows current selected variable text/value on the dashboard
     current: typing.Optional['VariableOption']
     # Whether multiple values can be selected or not from variable value list
     multi: typing.Optional[bool]
     # Options that can be selected for a variable.
     options: typing.Optional[list['VariableOption']]
-    # Options to config when to refresh a variable
     refresh: typing.Optional['VariableRefresh']
     # Options sort order
     sort: typing.Optional['VariableSort']
-    # Whether all value option is available or not
-    include_all: typing.Optional[bool]
-    # Custom all value
-    all_value: typing.Optional[str]
-    # Optional field, if you want to extract part of a series name or metric node segment.
-    # Named capture groups can be used to separate the display text and value.
-    regex: typing.Optional[str]
 
-    def __init__(self, type_val: typing.Optional['VariableType'] = None, name: str = "", label: typing.Optional[str] = None, hide: typing.Optional['VariableHide'] = None, skip_url_sync: typing.Optional[bool] = False, description: typing.Optional[str] = None, query: typing.Optional[typing.Union[str, object]] = None, datasource: typing.Optional['DataSourceRef'] = None, current: typing.Optional['VariableOption'] = None, multi: typing.Optional[bool] = False, options: typing.Optional[list['VariableOption']] = None, refresh: typing.Optional['VariableRefresh'] = None, sort: typing.Optional['VariableSort'] = None, include_all: typing.Optional[bool] = False, all_value: typing.Optional[str] = None, regex: typing.Optional[str] = None):
+    def __init__(self, type_val: typing.Optional['VariableType'] = None, name: str = "", label: typing.Optional[str] = None, hide: typing.Optional['VariableHide'] = None, skip_url_sync: typing.Optional[bool] = False, description: typing.Optional[str] = None, query: typing.Optional[typing.Union[str, object]] = None, datasource: typing.Optional['DataSourceRef'] = None, current: typing.Optional['VariableOption'] = None, multi: typing.Optional[bool] = False, options: typing.Optional[list['VariableOption']] = None, refresh: typing.Optional['VariableRefresh'] = None, sort: typing.Optional['VariableSort'] = None):
         self.type_val = type_val if type_val is not None else VariableType.QUERY
         self.name = name
         self.label = label
         self.hide = hide
         self.skip_url_sync = skip_url_sync
         self.description = description
         self.query = query
         self.datasource = datasource
         self.current = current
         self.multi = multi
         self.options = options
         self.refresh = refresh
         self.sort = sort
-        self.include_all = include_all
-        self.all_value = all_value
-        self.regex = regex
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "type": self.type_val,
             "name": self.name,
         }
         if self.label is not None:
@@ -465,20 +454,14 @@
             payload["multi"] = self.multi
         if self.options is not None:
             payload["options"] = self.options
         if self.refresh is not None:
             payload["refresh"] = self.refresh
         if self.sort is not None:
             payload["sort"] = self.sort
-        if self.include_all is not None:
-            payload["includeAll"] = self.include_all
-        if self.all_value is not None:
-            payload["allValue"] = self.all_value
-        if self.regex is not None:
-            payload["regex"] = self.regex
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "type" in data:
@@ -502,21 +485,15 @@
         if "multi" in data:
             args["multi"] = data["multi"]
         if "options" in data:
             args["options"] = data["options"]
         if "refresh" in data:
             args["refresh"] = data["refresh"]
         if "sort" in data:
-            args["sort"] = data["sort"]
-        if "includeAll" in data:
-            args["include_all"] = data["includeAll"]
-        if "allValue" in data:
-            args["all_value"] = data["allValue"]
-        if "regex" in data:
-            args["regex"] = data["regex"]        
+            args["sort"] = data["sort"]        
 
         return cls(**args)
 
 
 class VariableOption:
     """
     Option to be selected in a variable.
@@ -1189,45 +1166,52 @@
 
     # Unique identifier of transformer
     id_val: str
     # Disabled transformations are skipped
     disabled: typing.Optional[bool]
     # Optional frame matcher. When missing it will be applied to all results
     filter_val: typing.Optional['MatcherConfig']
+    # Where to pull DataFrames from as input to transformation
+    topic: typing.Optional[typing.Literal["series", "annotations", "alertStates"]]
     # Options to be passed to the transformer
     # Valid options depend on the transformer id
     options: object
 
-    def __init__(self, id_val: str = "", disabled: typing.Optional[bool] = None, filter_val: typing.Optional['MatcherConfig'] = None, options: object = None):
+    def __init__(self, id_val: str = "", disabled: typing.Optional[bool] = None, filter_val: typing.Optional['MatcherConfig'] = None, topic: typing.Optional[typing.Literal["series", "annotations", "alertStates"]] = None, options: object = None):
         self.id_val = id_val
         self.disabled = disabled
         self.filter_val = filter_val
+        self.topic = topic
         self.options = options
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "id": self.id_val,
             "options": self.options,
         }
         if self.disabled is not None:
             payload["disabled"] = self.disabled
         if self.filter_val is not None:
             payload["filter"] = self.filter_val
+        if self.topic is not None:
+            payload["topic"] = self.topic
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "id" in data:
             args["id_val"] = data["id"]
         if "disabled" in data:
             args["disabled"] = data["disabled"]
         if "filter" in data:
             args["filter_val"] = MatcherConfig.from_json(data["filter"])
+        if "topic" in data:
+            args["topic"] = data["topic"]
         if "options" in data:
             args["options"] = data["options"]        
 
         return cls(**args)
 
 
 class TimePickerConfig:
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/dashboardlist.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/dashboardlist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/datagrid.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/datagrid.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/debug.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/debug.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/elasticsearch.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/expr.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..cog import variants as cogvariants
 
 
 Expr: typing.TypeAlias = typing.Union['TypeMath', 'TypeReduce', 'TypeResample', 'TypeClassicConditions', 'TypeThreshold', 'TypeSql']
 
 
 def variant_config() -> cogruntime.DataqueryConfig:
-    decoding_map: dict[str, typing.Union[typing.Type[TypeReduce], typing.Type[TypeResample], typing.Type[TypeClassicConditions], typing.Type[TypeThreshold], typing.Type[TypeSql], typing.Type[TypeMath]]] = {"reduce": TypeReduce, "resample": TypeResample, "classic_conditions": TypeClassicConditions, "threshold": TypeThreshold, "sql": TypeSql, "math": TypeMath}
+    decoding_map: dict[str, typing.Union[typing.Type[TypeThreshold], typing.Type[TypeSql], typing.Type[TypeMath], typing.Type[TypeReduce], typing.Type[TypeResample], typing.Type[TypeClassicConditions]]] = {"threshold": TypeThreshold, "sql": TypeSql, "math": TypeMath, "reduce": TypeReduce, "resample": TypeResample, "classic_conditions": TypeClassicConditions}
     return cogruntime.DataqueryConfig(
         identifier="__expr__",
         from_json_hook=lambda data: decoding_map[data["type"]].from_json(data),
     )
 
 
 class TypeMath(cogvariants.Dataquery):
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/folder.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/role.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 
 
-class Folder:
-    """
-    TODO:
-    common metadata will soon support setting the parent folder in the metadata
-    """
-
-    # Unique folder id. (will be k8s name)
-    uid: str
-    # Folder title
-    title: str
-    # Description of the folder.
+class Role:
+    # The role identifier `managed:builtins:editor:permissions`
+    name: str
+    # Optional display
+    display_name: typing.Optional[str]
+    # Name of the team.
+    group_name: typing.Optional[str]
+    # Role description
     description: typing.Optional[str]
+    # Do not show this role
+    hidden: bool
 
-    def __init__(self, uid: str = "", title: str = "", description: typing.Optional[str] = None):
-        self.uid = uid
-        self.title = title
+    def __init__(self, name: str = "", display_name: typing.Optional[str] = None, group_name: typing.Optional[str] = None, description: typing.Optional[str] = None, hidden: bool = False):
+        self.name = name
+        self.display_name = display_name
+        self.group_name = group_name
         self.description = description
+        self.hidden = hidden
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "uid": self.uid,
-            "title": self.title,
+            "name": self.name,
+            "hidden": self.hidden,
         }
+        if self.display_name is not None:
+            payload["displayName"] = self.display_name
+        if self.group_name is not None:
+            payload["groupName"] = self.group_name
         if self.description is not None:
             payload["description"] = self.description
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "uid" in data:
-            args["uid"] = data["uid"]
-        if "title" in data:
-            args["title"] = data["title"]
+        if "name" in data:
+            args["name"] = data["name"]
+        if "displayName" in data:
+            args["display_name"] = data["displayName"]
+        if "groupName" in data:
+            args["group_name"] = data["groupName"]
         if "description" in data:
-            args["description"] = data["description"]        
+            args["description"] = data["description"]
+        if "hidden" in data:
+            args["hidden"] = data["hidden"]        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/gauge.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/gauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/geomap.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/geomap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/googlecloudmonitoring.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/googlecloudmonitoring.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/grafanapyroscope.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/grafanapyroscope.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/heatmap.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/heatmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -290,42 +290,42 @@
 
 
 class HeatmapTooltip:
     """
     Controls tooltip options
     """
 
-    # Controls if the tooltip is shown
-    show: bool
+    # Controls how the tooltip is shown
+    mode: common.TooltipDisplayMode
     # Controls if the tooltip shows a histogram of the y-axis values
     y_histogram: typing.Optional[bool]
     # Controls if the tooltip shows a color scale in header
     show_color_scale: typing.Optional[bool]
 
-    def __init__(self, show: bool = False, y_histogram: typing.Optional[bool] = None, show_color_scale: typing.Optional[bool] = None):
-        self.show = show
+    def __init__(self, mode: typing.Optional[common.TooltipDisplayMode] = None, y_histogram: typing.Optional[bool] = None, show_color_scale: typing.Optional[bool] = None):
+        self.mode = mode if mode is not None else common.TooltipDisplayMode.SINGLE
         self.y_histogram = y_histogram
         self.show_color_scale = show_color_scale
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "show": self.show,
+            "mode": self.mode,
         }
         if self.y_histogram is not None:
             payload["yHistogram"] = self.y_histogram
         if self.show_color_scale is not None:
             payload["showColorScale"] = self.show_color_scale
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "show" in data:
-            args["show"] = data["show"]
+        if "mode" in data:
+            args["mode"] = data["mode"]
         if "yHistogram" in data:
             args["y_histogram"] = data["yHistogram"]
         if "showColorScale" in data:
             args["show_color_scale"] = data["showColorScale"]        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/histogram.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/histogram.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/librarypanel.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/librarypanel.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/logs.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/logs.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/loki.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/loki.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/news.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/news.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/nodegraph.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/nodegraph.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/parca.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/parca.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/piechart.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/piechart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/preferences.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/preferences.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/prometheus.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/prometheus.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/publicdashboard.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/role.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/trend.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
+from ..models import common
 import typing
+from ..cog import runtime as cogruntime
 
 
-class Role:
-    # The role identifier `managed:builtins:editor:permissions`
-    name: str
-    # Optional display
-    display_name: typing.Optional[str]
-    # Name of the team.
-    group_name: typing.Optional[str]
-    # Role description
-    description: typing.Optional[str]
-    # Do not show this role
-    hidden: bool
-
-    def __init__(self, name: str = "", display_name: typing.Optional[str] = None, group_name: typing.Optional[str] = None, description: typing.Optional[str] = None, hidden: bool = False):
-        self.name = name
-        self.display_name = display_name
-        self.group_name = group_name
-        self.description = description
-        self.hidden = hidden
+class Options:
+    """
+    Identical to timeseries... except it does not have timezone settings
+    """
+
+    legend: common.VizLegendOptions
+    tooltip: common.VizTooltipOptions
+    # Name of the x field to use (defaults to first number)
+    x_field: typing.Optional[str]
+
+    def __init__(self, legend: typing.Optional[common.VizLegendOptions] = None, tooltip: typing.Optional[common.VizTooltipOptions] = None, x_field: typing.Optional[str] = None):
+        self.legend = legend if legend is not None else common.VizLegendOptions()
+        self.tooltip = tooltip if tooltip is not None else common.VizTooltipOptions()
+        self.x_field = x_field
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "name": self.name,
-            "hidden": self.hidden,
+            "legend": self.legend,
+            "tooltip": self.tooltip,
         }
-        if self.display_name is not None:
-            payload["displayName"] = self.display_name
-        if self.group_name is not None:
-            payload["groupName"] = self.group_name
-        if self.description is not None:
-            payload["description"] = self.description
+        if self.x_field is not None:
+            payload["xField"] = self.x_field
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "name" in data:
-            args["name"] = data["name"]
-        if "displayName" in data:
-            args["display_name"] = data["displayName"]
-        if "groupName" in data:
-            args["group_name"] = data["groupName"]
-        if "description" in data:
-            args["description"] = data["description"]
-        if "hidden" in data:
-            args["hidden"] = data["hidden"]        
+        if "legend" in data:
+            args["legend"] = common.VizLegendOptions.from_json(data["legend"])
+        if "tooltip" in data:
+            args["tooltip"] = common.VizTooltipOptions.from_json(data["tooltip"])
+        if "xField" in data:
+            args["x_field"] = data["xField"]        
 
         return cls(**args)
+
+
+FieldConfig: typing.TypeAlias = common.GraphFieldConfig
+
+
+
+
+
+def variant_config():
+    return cogruntime.PanelCfgConfig(
+        identifier="trend",
+        options_from_json_hook=Options.from_json,
+        field_config_from_json_hook=FieldConfig.from_json,
+    )
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/rolebinding.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/stat.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/stat.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,37 +6,40 @@
 
 
 class Options:
     graph_mode: common.BigValueGraphMode
     color_mode: common.BigValueColorMode
     justify_mode: common.BigValueJustifyMode
     text_mode: common.BigValueTextMode
+    wide_layout: bool
     reduce_options: common.ReduceDataOptions
     text: typing.Optional[common.VizTextDisplayOptions]
-    wide_layout: bool
+    show_percent_change: bool
     orientation: common.VizOrientation
 
-    def __init__(self, graph_mode: typing.Optional[common.BigValueGraphMode] = None, color_mode: typing.Optional[common.BigValueColorMode] = None, justify_mode: typing.Optional[common.BigValueJustifyMode] = None, text_mode: typing.Optional[common.BigValueTextMode] = None, reduce_options: typing.Optional[common.ReduceDataOptions] = None, text: typing.Optional[common.VizTextDisplayOptions] = None, wide_layout: bool = True, orientation: typing.Optional[common.VizOrientation] = None):
+    def __init__(self, graph_mode: typing.Optional[common.BigValueGraphMode] = None, color_mode: typing.Optional[common.BigValueColorMode] = None, justify_mode: typing.Optional[common.BigValueJustifyMode] = None, text_mode: typing.Optional[common.BigValueTextMode] = None, wide_layout: bool = True, reduce_options: typing.Optional[common.ReduceDataOptions] = None, text: typing.Optional[common.VizTextDisplayOptions] = None, show_percent_change: bool = False, orientation: typing.Optional[common.VizOrientation] = None):
         self.graph_mode = graph_mode if graph_mode is not None else common.BigValueGraphMode.AREA
         self.color_mode = color_mode if color_mode is not None else common.BigValueColorMode.VALUE
         self.justify_mode = justify_mode if justify_mode is not None else common.BigValueJustifyMode.AUTO
         self.text_mode = text_mode if text_mode is not None else common.BigValueTextMode.AUTO
+        self.wide_layout = wide_layout
         self.reduce_options = reduce_options if reduce_options is not None else common.ReduceDataOptions()
         self.text = text
-        self.wide_layout = wide_layout
+        self.show_percent_change = show_percent_change
         self.orientation = orientation if orientation is not None else common.VizOrientation.AUTO
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "graphMode": self.graph_mode,
             "colorMode": self.color_mode,
             "justifyMode": self.justify_mode,
             "textMode": self.text_mode,
-            "reduceOptions": self.reduce_options,
             "wideLayout": self.wide_layout,
+            "reduceOptions": self.reduce_options,
+            "showPercentChange": self.show_percent_change,
             "orientation": self.orientation,
         }
         if self.text is not None:
             payload["text"] = self.text
         return payload
 
     @classmethod
@@ -47,20 +50,22 @@
             args["graph_mode"] = data["graphMode"]
         if "colorMode" in data:
             args["color_mode"] = data["colorMode"]
         if "justifyMode" in data:
             args["justify_mode"] = data["justifyMode"]
         if "textMode" in data:
             args["text_mode"] = data["textMode"]
+        if "wideLayout" in data:
+            args["wide_layout"] = data["wideLayout"]
         if "reduceOptions" in data:
             args["reduce_options"] = common.ReduceDataOptions.from_json(data["reduceOptions"])
         if "text" in data:
             args["text"] = common.VizTextDisplayOptions.from_json(data["text"])
-        if "wideLayout" in data:
-            args["wide_layout"] = data["wideLayout"]
+        if "showPercentChange" in data:
+            args["show_percent_change"] = data["showPercentChange"]
         if "orientation" in data:
             args["orientation"] = data["orientation"]        
 
         return cls(**args)
 
 
 def variant_config():
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/statetimeline.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/statetimeline.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/statushistory.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/statushistory.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/table.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/table.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/team.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/tempo.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/tempo.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/testdata.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/testdata.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/text.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/text.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/timeseries.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/timeseries.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/grafana_foundation_sdk/models/xychart.py` & `grafana_foundation_sdk-1715606109!10.3.0/grafana_foundation_sdk/models/xychart.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,33 @@
 import enum
 import typing
 from ..models import common
 from ..cog import runtime as cogruntime
 
 
 class SeriesMapping(enum.StrEnum):
+    """
+    Auto is "table" in the UI
+    """
+
     AUTO = "auto"
     MANUAL = "manual"
 
 
 class ScatterShow(enum.StrEnum):
     POINTS = "points"
     LINES = "lines"
     POINTS_AND_LINES = "points+lines"
 
 
 class XYDimensionConfig:
+    """
+    Configuration for the Table/Auto mode
+    """
+
     frame: int
     x: typing.Optional[str]
     exclude: typing.Optional[list[str]]
 
     def __init__(self, frame: int = 0, x: typing.Optional[str] = None, exclude: typing.Optional[list[str]] = None):
         self.frame = frame
         self.x = x
@@ -329,17 +337,19 @@
             args["axis_border_show"] = data["axisBorderShow"]        
 
         return cls(**args)
 
 
 class Options:
     series_mapping: typing.Optional['SeriesMapping']
+    # Table Mode (auto)
     dims: 'XYDimensionConfig'
     legend: common.VizLegendOptions
     tooltip: common.VizTooltipOptions
+    # Manual Mode
     series: list['ScatterSeriesConfig']
 
     def __init__(self, series_mapping: typing.Optional['SeriesMapping'] = None, dims: typing.Optional['XYDimensionConfig'] = None, legend: typing.Optional[common.VizLegendOptions] = None, tooltip: typing.Optional[common.VizTooltipOptions] = None, series: typing.Optional[list['ScatterSeriesConfig']] = None):
         self.series_mapping = series_mapping
         self.dims = dims if dims is not None else XYDimensionConfig()
         self.legend = legend if legend is not None else common.VizLegendOptions()
         self.tooltip = tooltip if tooltip is not None else common.VizTooltipOptions()
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/LICENSE.md` & `grafana_foundation_sdk-1715606109!10.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/README.md` & `grafana_foundation_sdk-1715606109!10.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Grafana Foundation SDK – Python
 
 A set of tools, types and *builder libraries* for building and manipulating Grafana objects in Python.
 
 > [!NOTE]
-> This branch contains **types and builders generated for Grafana v10.2.x.**
+> This branch contains **types and builders generated for Grafana v10.3.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1715605946!10.2.0'
+python3 -m pip install 'grafana_foundation_sdk==1715606109!10.3.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/pyproject.toml` & `grafana_foundation_sdk-1715606109!10.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "observability",
     "sdk",
     "grafana",
     "logs",
     "traces",
     "metrics"
 ]
-version = "1715605946!10.2.0"
+version = "1715606109!10.3.0"
 dependencies = []
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `grafana_foundation_sdk-1715605946!10.2.0/PKG-INFO` & `grafana_foundation_sdk-1715606109!10.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grafana_foundation_sdk
-Version: 1715605946!10.2.0
+Version: 1715606109!10.3.0
 Summary: A set of tools, types and libraries for building and manipulating Grafana objects.
 Project-URL: Homepage, https://github.com/grafana/grafana-foundation-sdk
 Project-URL: Repository, https://github.com/grafana/grafana-foundation-sdk.git
 Project-URL: Issues, https://github.com/grafana/grafana-foundation-sdk/issues
 Author: Grafana Labs
 License-File: LICENSE.md
 Keywords: grafana,logs,metrics,observability,sdk,traces
@@ -21,21 +21,21 @@
 Description-Content-Type: text/markdown
 
 # Grafana Foundation SDK – Python
 
 A set of tools, types and *builder libraries* for building and manipulating Grafana objects in Python.
 
 > [!NOTE]
-> This branch contains **types and builders generated for Grafana v10.2.x.**
+> This branch contains **types and builders generated for Grafana v10.3.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1715605946!10.2.0'
+python3 -m pip install 'grafana_foundation_sdk==1715606109!10.3.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```

