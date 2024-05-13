# Comparing `tmp/cimsparql-3.3.1.tar.gz` & `tmp/cimsparql-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cimsparql-3.3.1.tar", max compression
+gzip compressed data, was "cimsparql-4.0.0.tar", max compression
```

## Comparing `cimsparql-3.3.1.tar` & `cimsparql-4.0.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1065 2024-05-10 12:53:02.992521 cimsparql-3.3.1/LICENSE
--rw-r--r--   0        0        0     5195 2024-05-10 12:53:02.992521 cimsparql-3.3.1/README.md
--rw-r--r--   0        0        0       60 2024-05-10 12:53:16.472606 cimsparql-3.3.1/cimsparql/__init__.py
--rw-r--r--   0        0        0     4744 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/adaptions.py
--rw-r--r--   0        0        0     1642 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/constants.py
--rw-r--r--   0        0        0     9739 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/data_models.py
--rw-r--r--   0        0        0    16044 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/graphdb.py
--rw-r--r--   0        0        0    28376 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/model.py
--rw-r--r--   0        0        0     5202 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/ac_lines.sparql
--rw-r--r--   0        0        0      221 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/add_mrid.sparql
--rw-r--r--   0        0        0     1761 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/borders.sparql
--rw-r--r--   0        0        0     2073 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/branch_node_withdraw.sparql
--rw-r--r--   0        0        0     1795 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/bus.sparql
--rw-r--r--   0        0        0      984 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/connections.sparql
--rw-r--r--   0        0        0     1291 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/connectivity_nodes.sparql
--rw-r--r--   0        0        0      737 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/converter_hvdc_bidzones.sparql
--rw-r--r--   0        0        0     2614 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/converters.sparql
--rw-r--r--   0        0        0      588 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/coordinates.sparql
--rw-r--r--   0        0        0     2521 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/dc_active_power_flow.sparql
--rw-r--r--   0        0        0      242 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/disconnected.sparql
--rw-r--r--   0        0        0     3063 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/exchange.sparql
--rw-r--r--   0        0        0      792 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/full_model.sparql
--rw-r--r--   0        0        0     2813 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/loads.sparql
--rw-r--r--   0        0        0      287 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/market_dates.sparql
--rw-r--r--   0        0        0      523 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/power_flow.sparql
--rw-r--r--   0        0        0      397 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/ras_equipment.sparql
--rw-r--r--   0        0        0      573 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/regions.sparql
--rw-r--r--   0        0        0     3655 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/series_compensators.sparql
--rw-r--r--   0        0        0      426 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/station_group_code_and_names.sparql
--rw-r--r--   0        0        0      645 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/substation_voltage_level.sparql
--rw-r--r--   0        0        0     2877 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/sv_branch.sparql
--rw-r--r--   0        0        0      245 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/sv_injection.sparql
--rw-r--r--   0        0        0      781 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/switches.sparql
--rw-r--r--   0        0        0     3285 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/synchronous_machines.sparql
--rw-r--r--   0        0        0      318 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/test_configuration_modifications/add_zero_sv_power.sparql
--rw-r--r--   0        0        0     3102 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/three_winding.sparql
--rw-r--r--   0        0        0     1953 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/three_winding_dummy_nodes.sparql
--rw-r--r--   0        0        0     1583 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/three_winding_loss.sparql
--rw-r--r--   0        0        0      363 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/transformer_windings.sparql
--rw-r--r--   0        0        0     1269 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/transformers.sparql
--rw-r--r--   0        0        0     1844 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/transformers_connected_to_converter.sparql
--rw-r--r--   0        0        0     4520 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/two_winding_transformer.sparql
--rw-r--r--   0        0        0     1049 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/two_winding_transformer_angle.sparql
--rw-r--r--   0        0        0      461 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/type_mapper.sparql
--rw-r--r--   0        0        0      814 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/wind_generating_units.sparql
--rw-r--r--   0        0        0      944 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/winding.sparql
--rw-r--r--   0        0        0     2298 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql_result_json.py
--rw-r--r--   0        0        0     3193 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/templates.py
--rw-r--r--   0        0        0     5650 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/type_mapper.py
--rw-r--r--   0        0        0      768 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/url.py
--rw-r--r--   0        0        0      616 2024-05-10 12:53:02.996521 cimsparql-3.3.1/cimsparql/value_mapper.py
--rw-r--r--   0        0        0      459 2024-05-10 12:53:03.004521 cimsparql-3.3.1/pkg_data/blazegraph_repo_config.xml
--rw-r--r--   0        0        0      676 2024-05-10 12:53:03.004521 cimsparql-3.3.1/pkg_data/namespaces.json
--rw-r--r--   0        0        0      805 2024-05-10 12:53:03.004521 cimsparql-3.3.1/pkg_data/native_store_config_template.ttl
--rw-r--r--   0        0        0     4219 2024-05-10 12:53:16.472606 cimsparql-3.3.1/pyproject.toml
--rw-r--r--   0        0        0     5969 1970-01-01 00:00:00.000000 cimsparql-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-13 13:08:10.129235 cimsparql-4.0.0/LICENSE
+-rw-r--r--   0        0        0     5195 2024-05-13 13:08:10.129235 cimsparql-4.0.0/README.md
+-rw-r--r--   0        0        0       60 2024-05-13 13:08:24.753188 cimsparql-4.0.0/cimsparql/__init__.py
+-rw-r--r--   0        0        0     4744 2024-05-13 13:08:10.129235 cimsparql-4.0.0/cimsparql/adaptions.py
+-rw-r--r--   0        0        0     1642 2024-05-13 13:08:10.129235 cimsparql-4.0.0/cimsparql/constants.py
+-rw-r--r--   0        0        0     9739 2024-05-13 13:08:10.129235 cimsparql-4.0.0/cimsparql/data_models.py
+-rw-r--r--   0        0        0    16044 2024-05-13 13:08:10.129235 cimsparql-4.0.0/cimsparql/graphdb.py
+-rw-r--r--   0        0        0    28744 2024-05-13 13:08:10.129235 cimsparql-4.0.0/cimsparql/model.py
+-rw-r--r--   0        0        0     5202 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/ac_lines.sparql
+-rw-r--r--   0        0        0      221 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/add_mrid.sparql
+-rw-r--r--   0        0        0     1761 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/borders.sparql
+-rw-r--r--   0        0        0     2073 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/branch_node_withdraw.sparql
+-rw-r--r--   0        0        0     1795 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/bus.sparql
+-rw-r--r--   0        0        0      984 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/connections.sparql
+-rw-r--r--   0        0        0     1291 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/connectivity_nodes.sparql
+-rw-r--r--   0        0        0      737 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/converter_hvdc_bidzones.sparql
+-rw-r--r--   0        0        0     2614 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/converters.sparql
+-rw-r--r--   0        0        0      588 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/coordinates.sparql
+-rw-r--r--   0        0        0     2521 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/dc_active_power_flow.sparql
+-rw-r--r--   0        0        0      242 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/disconnected.sparql
+-rw-r--r--   0        0        0     3063 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/exchange.sparql
+-rw-r--r--   0        0        0      792 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/full_model.sparql
+-rw-r--r--   0        0        0     2813 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/loads.sparql
+-rw-r--r--   0        0        0      287 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/market_dates.sparql
+-rw-r--r--   0        0        0      523 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/power_flow.sparql
+-rw-r--r--   0        0        0      397 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/ras_equipment.sparql
+-rw-r--r--   0        0        0      573 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/regions.sparql
+-rw-r--r--   0        0        0     3655 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/series_compensators.sparql
+-rw-r--r--   0        0        0      426 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/station_group_code_and_names.sparql
+-rw-r--r--   0        0        0      645 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/substation_voltage_level.sparql
+-rw-r--r--   0        0        0     2877 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/sv_branch.sparql
+-rw-r--r--   0        0        0      245 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/sv_injection.sparql
+-rw-r--r--   0        0        0      781 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/switches.sparql
+-rw-r--r--   0        0        0     3285 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/synchronous_machines.sparql
+-rw-r--r--   0        0        0      318 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/test_configuration_modifications/add_zero_sv_power.sparql
+-rw-r--r--   0        0        0     3461 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/transformer_branches.sparql
+-rw-r--r--   0        0        0     1461 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/transformer_center_nodes.sparql
+-rw-r--r--   0        0        0      363 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/transformer_windings.sparql
+-rw-r--r--   0        0        0     1269 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/transformers.sparql
+-rw-r--r--   0        0        0     1844 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/transformers_connected_to_converter.sparql
+-rw-r--r--   0        0        0     4520 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/two_winding_transformer.sparql
+-rw-r--r--   0        0        0      880 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/two_winding_transformer_angle.sparql
+-rw-r--r--   0        0        0      461 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/type_mapper.sparql
+-rw-r--r--   0        0        0      814 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/wind_generating_units.sparql
+-rw-r--r--   0        0        0      944 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/winding.sparql
+-rw-r--r--   0        0        0     1277 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql/winding_loss.sparql
+-rw-r--r--   0        0        0     2298 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/sparql_result_json.py
+-rw-r--r--   0        0        0     3193 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/templates.py
+-rw-r--r--   0        0        0     5650 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/type_mapper.py
+-rw-r--r--   0        0        0      768 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/url.py
+-rw-r--r--   0        0        0      616 2024-05-13 13:08:10.133235 cimsparql-4.0.0/cimsparql/value_mapper.py
+-rw-r--r--   0        0        0      459 2024-05-13 13:08:10.141235 cimsparql-4.0.0/pkg_data/blazegraph_repo_config.xml
+-rw-r--r--   0        0        0      676 2024-05-13 13:08:10.141235 cimsparql-4.0.0/pkg_data/namespaces.json
+-rw-r--r--   0        0        0      805 2024-05-13 13:08:10.141235 cimsparql-4.0.0/pkg_data/native_store_config_template.ttl
+-rw-r--r--   0        0        0     4219 2024-05-13 13:08:24.753188 cimsparql-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5969 1970-01-01 00:00:00.000000 cimsparql-4.0.0/PKG-INFO
```

### Comparing `cimsparql-3.3.1/LICENSE` & `cimsparql-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/README.md` & `cimsparql-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/adaptions.py` & `cimsparql-4.0.0/cimsparql/adaptions.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/constants.py` & `cimsparql-4.0.0/cimsparql/constants.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/data_models.py` & `cimsparql-4.0.0/cimsparql/data_models.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/graphdb.py` & `cimsparql-4.0.0/cimsparql/graphdb.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/model.py` & `cimsparql-4.0.0/cimsparql/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,28 +221,28 @@
         df = self.get_table_and_convert(self.market_dates_query, index="mrid")
         return MarketDatesDataFrame(df)
 
     def bus_data_query(self, region: str | None = None) -> str:
         substitutes = {"region": region or ".*"}
         return self.template_to_query(templates.BUS_DATA_QUERY, substitutes)
 
-    def three_winding_dummy_nodes_query(self, region: str | None = None) -> str:
+    def transformer_center_nodes_query(self, region: str | None = None) -> str:
         substitutes = {"region": region or ".*"}
-        return self.template_to_query(templates.THREE_WINDING_DUMMY_NODES_QUERY, substitutes)
+        return self.template_to_query(templates.TRANSFORMER_CENTER_NODES_QUERY, substitutes)
 
     @time_it
     def bus_data(self, region: str | None = None) -> BusDataFrame:
         """Query name of topological nodes (TP query).
 
         Args:
            region: Limit to region (use None to get all)
         """
         dfs = [
             self.get_table_and_convert(self.bus_data_query(region), index="node"),
-            self.get_table_and_convert(self.three_winding_dummy_nodes_query(region), index="node"),
+            self.get_table_and_convert(self.transformer_center_nodes_query(region), index="node"),
         ]
         df = pd.concat(dfs)
         return BusDataFrame(df)
 
     def loads_query(self, region: str | None = None) -> str:
         substitutes = {"region": region or ".*"}
         return self.template_to_query(templates.LOADS_QUERY, substitutes)
@@ -470,41 +470,54 @@
             data["angle"] += angle.reindex(index=data.index, fill_value=0.0).squeeze()
         return TransformerWindingDataFrame(data)
 
     @property
     def winding_query(self) -> str:
         return self.template_to_query(templates.WINDING)
 
-    def three_winding_loss_query(self, region: str | None = None) -> str:
+    def winding_loss_query(self, region: str | None = None) -> str:
         substitutes = {"region": region or ".*"}
-        return self.template_to_query(templates.THREE_WINDING_LOSS_QUERY, substitutes)
+        return self.template_to_query(templates.WINDING_LOSS_QUERY, substitutes)
 
-    def three_winding_transformers_query(
-        self, region: str | None = None, rate: str | None = None
-    ) -> str:
+    def transformer_branches_query(self, region: str | None = None, rate: str | None = None) -> str:
         substitutes = {"region": region or ".*", "rate": rate or "Normal@20"}
-        return self.template_to_query(templates.THREE_WINDING_QUERY, substitutes)
+        return self.template_to_query(templates.TRANSFORMER_BRANCHES_QUERY, substitutes)
 
     @time_it
-    def three_winding_transformers(
+    def transformer_branches(
         self, region: str | None = None, rate: str | None = None
     ) -> TransformerWindingDataFrame:
-        """Query three-winding transformer. Return as three two-winding transformers.
+        """Query transformer branches. For two winding transformers will
+        give two "branches" (x are nodes, o is the fictisous center node)
+
+        x --- o ---- x
+
+        Three winding transformers
+
+            x
+            |
+        x - o - x
+
+
 
         Example:
             >>> from cimsparql.model import get_single_client_model
             >>> server_url = "127.0.0.1:7200"
             >>> model = get_single_client_model(server_url, "LATEST")
-            >>> model.two_winding_transformers()
+            >>> model.transformer_branches()
         """
-        query = self.three_winding_transformers_query(region, rate)
+        query = self.transformer_branches_query(region, rate)
         data = self.get_table_and_convert(query, index="mrid")
-        query_loss = self.three_winding_loss_query(region)
+        query_loss = self.winding_loss_query(region)
         loss = self.get_table_and_convert(query_loss, index="mrid")
         df = pd.concat([data.assign(ploss_1=0.0), loss.loc[data.index]], axis=1)
+        query_angle = self.two_winding_angle_query(region)
+        angle = self.get_table_and_convert(query_angle, index="mrid")
+        if not angle.empty:
+            data["angle"] += angle.reindex(index=data.index, fill_value=0.0).squeeze()
         return TransformerWindingDataFrame(df)
 
     @property
     def substation_voltage_level_query(self) -> str:
         return self.template_to_query(templates.SUBSTATION_VOLTAGE_LEVEL_QUERY)
 
     def substation_voltage_level(self) -> SubstationVoltageDataFrame:
@@ -755,18 +768,18 @@
         "DC Active Power Flow",
         "Full model",
         "Series compensators",
         "SV branch",
         "Power flow",
         "SvInjection",
         "Switches",
-        "Three winding",
-        "Three winding loss",
-        "Three winding with dummy nodes",
+        "Transformer branches",
+        "Transformer branches loss",
+        "Transformer center nodes",
         "Two winding transformer",
-        "Two winding transformer angle",
         "Synchronous machines",
         "Windings",
+        "Winding transformer angle",
     )
     for query in exec_from_tpssvssh:
         clients[query] = tpsvssh_client
     return Model(clients, model_cfg, mapper)
```

### Comparing `cimsparql-3.3.1/cimsparql/sparql/ac_lines.sparql` & `cimsparql-4.0.0/cimsparql/sparql/ac_lines.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/borders.sparql` & `cimsparql-4.0.0/cimsparql/sparql/borders.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/branch_node_withdraw.sparql` & `cimsparql-4.0.0/cimsparql/sparql/branch_node_withdraw.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/bus.sparql` & `cimsparql-4.0.0/cimsparql/sparql/bus.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/connections.sparql` & `cimsparql-4.0.0/cimsparql/sparql/connections.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/connectivity_nodes.sparql` & `cimsparql-4.0.0/cimsparql/sparql/connectivity_nodes.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/converter_hvdc_bidzones.sparql` & `cimsparql-4.0.0/cimsparql/sparql/converter_hvdc_bidzones.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/converters.sparql` & `cimsparql-4.0.0/cimsparql/sparql/converters.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/coordinates.sparql` & `cimsparql-4.0.0/cimsparql/sparql/coordinates.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/dc_active_power_flow.sparql` & `cimsparql-4.0.0/cimsparql/sparql/dc_active_power_flow.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/exchange.sparql` & `cimsparql-4.0.0/cimsparql/sparql/exchange.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/full_model.sparql` & `cimsparql-4.0.0/cimsparql/sparql/full_model.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/loads.sparql` & `cimsparql-4.0.0/cimsparql/sparql/loads.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/power_flow.sparql` & `cimsparql-4.0.0/cimsparql/sparql/power_flow.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/regions.sparql` & `cimsparql-4.0.0/cimsparql/sparql/regions.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/series_compensators.sparql` & `cimsparql-4.0.0/cimsparql/sparql/series_compensators.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/substation_voltage_level.sparql` & `cimsparql-4.0.0/cimsparql/sparql/substation_voltage_level.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/sv_branch.sparql` & `cimsparql-4.0.0/cimsparql/sparql/sv_branch.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/switches.sparql` & `cimsparql-4.0.0/cimsparql/sparql/switches.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/synchronous_machines.sparql` & `cimsparql-4.0.0/cimsparql/sparql/synchronous_machines.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/three_winding.sparql` & `cimsparql-4.0.0/cimsparql/sparql/two_winding_transformer.sparql`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,82 @@
-# Name: Three winding
+# Name: Two winding transformer
 PREFIX cim: <${cim}>
 PREFIX SN: <${SN}>
 PREFIX xsd: <${xsd}>
-select ?node_1 ?node_2 ?status ?name ?mrid ?un ?r ?x ?b ?g ?rate (?bidzone as ?bidzone_1) (?bidzone as ?bidzone_2) ?angle ?ratio ?connectivity_node_1 (?node_2 as ?connectivity_node_2)
-where {
-  ?con_node cim:ConnectivityNode.TopologicalNode/cim:IdentifiedObject.mRID ?node_1 .
-  ?terminal cim:ACDCTerminal.connected ?connected .
-  optional {?winding ^cim:SvStatus.ConductingEquipment/cim:SvStatus.inService ?in_service} .
 
-  ?_eq_subject <http://entsoe.eu/CIM/EquipmentCore/3/1> ?eq_repo .
-  service ?eq_repo {
-     # Extract three winding transformers
-    {
-      select  ?p_transformer
-      where {
-        ?p_transformer ^cim:PowerTransformerEnd.PowerTransformer/cim:TransformerEnd.endNumber ?nr
-      }
-      group by ?p_transformer
-      having (count(*) > 2)
+select ?mrid ?name ?bidzone_1 ?bidzone_2 ?node_1 ?node_2 ?ploss_1 ?ploss_2 ?r ?rate ?status (?un_1 as ?un) ?x ?b ?g ?angle ?ratio ?connectivity_node_1 ?connectivity_node_2
+where
+{
+    # Collect properties for terminal_1
+    ?terminal_1 cim:ACDCTerminal.connected ?connected_1;
+                ^cim:SvPowerFlow.Terminal/cim:SvPowerFlow.p ?p_1 ;
+                cim:Terminal.TopologicalNode/cim:IdentifiedObject.mRID ?node_1 .
+    # Collect properties from terminal_2
+    ?terminal_2 cim:ACDCTerminal.connected ?connected_2;
+                ^cim:SvPowerFlow.Terminal/cim:SvPowerFlow.p ?p_2 ;
+                cim:Terminal.TopologicalNode/cim:IdentifiedObject.mRID ?node_2 .
+    optional {?p_transformer ^cim:SvStatus.ConductingEquipment/cim:SvStatus.inService ?in_service }.
+    ?_eq_subject <http://entsoe.eu/CIM/EquipmentCore/3/1> ?eq_repo .
+    service ?eq_repo {
+        # Extract two winding transformers
+        {
+            select ?p_transformer where {
+                ?p_transformer a cim:PowerTransformer;
+                               ^cim:PowerTransformerEnd.PowerTransformer ?power_transformer_end
+            }
+            group by ?p_transformer
+            having (count(*) = 2)
+        } .
+        ?p_transformer cim:IdentifiedObject.name ?name ;
+                       cim:Equipment.EquipmentContainer ?substation;
+                       cim:Equipment.EquipmentContainer/cim:Substation.Region/cim:SubGeographicalRegion.Region/cim:IdentifiedObject.name ?area .
+        filter(regex(?area, '${region}'))
+        optional {?substation SN:Substation.MarketDeliveryPoint/SN:MarketDeliveryPoint.BiddingArea/SN:BiddingArea.marketCode ?bidzone }.
+        optional {
+            ?p_transformer SN:Equipment.networkAnalysisEnable ?_network_analysis
+        }
+        bind(coalesce(?_network_analysis, True) as ?network_analysis)
+        # Extract for winding_1
+        ?winding_1 cim:PowerTransformerEnd.PowerTransformer ?p_transformer;
+                   cim:TransformerEnd.Terminal ?terminal_1;
+                   cim:PowerTransformerEnd.ratedU ?ubase_1 ;
+                   cim:TransformerEnd.endNumber 1;
+                   cim:PowerTransformerEnd.r ?r;
+                   cim:PowerTransformerEnd.x ?x;
+                   cim:PowerTransformerEnd.b ?b;
+                   cim:PowerTransformerEnd.g ?g;
+                   cim:IdentifiedObject.mRID ?mrid .
+        ?terminal_1 cim:Terminal.ConnectivityNode ?con_node_1.
+        ?con_node_1 cim:ConnectivityNode.ConnectivityNodeContainer/cim:VoltageLevel.BaseVoltage/cim:BaseVoltage.nominalVoltage ?un_1;
+            cim:IdentifiedObject.mRID ?connectivity_node_1 .
+        optional {
+            ?p_lim cim:OperationalLimit.OperationalLimitSet/cim:OperationalLimitSet.Terminal ?terminal_1;
+                                                           a cim:ActivePowerLimit;
+                                                           cim:IdentifiedObject.name '${rate}';
+                                                           cim:ActivePowerLimit.value ?rate
+        } .
+        # Extract for winding_2
+        ?winding_2 cim:PowerTransformerEnd.PowerTransformer ?p_transformer;
+                   cim:TransformerEnd.Terminal ?terminal_2;
+                   cim:PowerTransformerEnd.ratedU ?ubase_2 ;
+                   cim:TransformerEnd.endNumber 2 .
+        ?terminal_2 cim:Terminal.ConnectivityNode ?con_node_2 .
+        ?con_node_2 cim:ConnectivityNode.ConnectivityNodeContainer/cim:VoltageLevel.BaseVoltage/cim:BaseVoltage.nominalVoltage ?un_2 ;
+             cim:IdentifiedObject.mRID ?connectivity_node_2 .
+        optional{
+            ?winding_2 cim:PowerTransformerEnd.phaseAngleClock ?aclock .
+        }
+        bind(coalesce(?aclock, 0.0) as ?angleclock)
+        bind(xsd:double(30.0) * ?angleclock as ?angle)
     } .
-
-    # Use mrid of transformer as dummy node
-    ?p_transformer cim:IdentifiedObject.mRID ?node_2;
-            cim:Equipment.EquipmentContainer ?Substation;
-            cim:IdentifiedObject.name ?name .
-    ?Substation cim:Substation.Region/cim:SubGeographicalRegion.Region/cim:IdentifiedObject.name ?area .
-    filter(regex(?area, '${region}'))
-
-    # Extract properties for the windings associated with p_transformer
-    ?winding cim:TransformerEnd.Terminal ?terminal;
-          cim:IdentifiedObject.mRID ?mrid;
-          cim:PowerTransformerEnd.PowerTransformer ?p_transformer;
-          cim:PowerTransformerEnd.ratedU ?ubase;
-          cim:PowerTransformerEnd.r ?r;
-          cim:PowerTransformerEnd.x ?x;
-          cim:PowerTransformerEnd.b ?b;
-          cim:PowerTransformerEnd.g ?g .
-    optional{?winding cim:PowerTransformerEnd.phaseAngleClock ?aclock .}
-    bind(coalesce(?aclock, 0.0) as ?angleclock)
-
-    # Extract the connectivity node for each termina, and find the nominal voltage from the connectivity node
-    ?terminal cim:Terminal.ConnectivityNode ?con_node .
-    ?con_node cim:ConnectivityNode.ConnectivityNodeContainer/cim:VoltageLevel.BaseVoltage/cim:BaseVoltage.nominalVoltage ?un ;
-      cim:IdentifiedObject.mRID ?connectivity_node_1 .
-
-    # Optionally extract bidzone for substations
-    optional {?Substation SN:Substation.MarketDeliveryPoint/SN:MarketDeliveryPoint.BiddingArea/SN:BiddingArea.marketCode ?bidzone} .
-
-    # Optionally extract active power limits
+    # Aggregate results
     optional {
-      ?_lim a cim:ActivePowerLimit;
-            cim:OperationalLimit.OperationalLimitSet/cim:OperationalLimitSet.Terminal ?terminal;
-            cim:IdentifiedObject.name '${rate}';
-            cim:ActivePowerLimit.value ?rate .
+        bind((xsd:double(str(?p_1)) + xsd:double(str(?p_2))) as ?pl)
+        bind(if (xsd:double(str(?p_1)) > xsd:double(str(?p_2)), ?pl, xsd:double(0.0)) as ?ploss_2)
+        bind(if (xsd:double(str(?p_1)) < xsd:double(str(?p_2)), ?pl, xsd:double(0.0)) as ?ploss_1)
     }
-    optional {?p_transformer SN:Equipment.networkAnalysisEnable ?_network_analysis}
-  }
-
-  bind(coalesce(?_network_analysis, True) as ?network_analysis)
-  filter(?network_analysis)
-
-  # Assign status flag to the transformer. The first that exists is used
-  # 1) in_service flag on the transformer
-  # 2) Connected flag for the terminal
-  bind(coalesce(?in_service, ?connected) as ?status)
-  bind(xsd:double(str(?un)) / xsd:double(str(?ubase)) as ?ratio)
-  bind(xsd:double(30.0) * ?angleclock as ?angle)
+    bind(coalesce(?in_service, ?connected_1 && ?connected_2) as ?status)
+    #  ratio: n = Us / Up (secondary (2) / primary (1))
+    bind((xsd:double(str(?ubase_2)) / xsd:double(str(?un_2))) / (xsd:double(str(?ubase_1)) / xsd:double(str(?un_1))) as ?ratio)
+    bind(?bidzone as ?bidzone_1)
+    bind(?bidzone as ?bidzone_2)
 }
```

### Comparing `cimsparql-3.3.1/cimsparql/sparql/three_winding_dummy_nodes.sparql` & `cimsparql-4.0.0/cimsparql/sparql/transformer_center_nodes.sparql`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,21 @@
-# Name: Three winding with dummy nodes
+# Name: Transformer center nodes
 PREFIX cim:<${cim}>
 PREFIX SN:<${SN}>
 select ?node ?busname (?container_name as ?substation) ?un (?container_mrid as ?substation_mrid) ?bidzone ?island (False as ?is_swing_bus) ?connectivity_node
 where
 {
   optional{
     ?con_node cim:ConnectivityNode.TopologicalNode ?top_node .
     ?top_node ^cim:TopologicalIsland.TopologicalNodes/cim:IdentifiedObject.name ?island_name
   }.
 
 
   ?_eq_subject <http://entsoe.eu/CIM/EquipmentCore/3/1> ?eq_repo .
   service ?eq_repo {
-    # Select all three winding transformerss
-    {
-      select  ?p_transformer
-      where {
-        ?p_transformer a cim:PowerTransformer;
-          cim:Equipment.EquipmentContainer/cim:Substation.Region/cim:SubGeographicalRegion.Region/cim:IdentifiedObject.name ?area;
-                      ^cim:PowerTransformerEnd.PowerTransformer/cim:TransformerEnd.endNumber ?nr.
-        filter(regex(?area, '${region}'))
-      }
-      group by ?p_transformer
-      having (count(*) > 2)
-    } .
     ?p_transformer cim:IdentifiedObject.mRID ?node;
       cim:IdentifiedObject.name ?busname;
                   cim:Equipment.EquipmentContainer ?container.
     ?winding cim:TransformerEnd.endNumber 1;
             cim:PowerTransformerEnd.ratedU ?un;
             cim:PowerTransformerEnd.PowerTransformer ?p_transformer;
             cim:TransformerEnd.Terminal ?terminal .
```

### Comparing `cimsparql-3.3.1/cimsparql/sparql/three_winding_loss.sparql` & `cimsparql-4.0.0/cimsparql/sparql/winding_loss.sparql`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Name: Three winding loss
+# Name: Transformer branches loss
 PREFIX cim: <${cim}>
 PREFIX SN: <${SN}>
 PREFIX xsd: <${xsd}>
 
 select ?mrid (sum(xsd:double(str(?sv_p)))/sum(?in_service) as ?ploss_2)
 where {
   ?terminal cim:ACDCTerminal.connected ?connected .
@@ -12,23 +12,14 @@
   ?_eq_subject <http://entsoe.eu/CIM/EquipmentCore/3/1> ?eq_repo .
   service ?eq_repo {
     # Extract mRID and area for each power transformer
     ?p_transformer a cim:PowerTransformer;
             ^cim:PowerTransformerEnd.PowerTransformer/cim:IdentifiedObject.mRID ?mrid;
             cim:Equipment.EquipmentContainer/cim:Substation.Region/cim:SubGeographicalRegion.Region/cim:IdentifiedObject.name ?area .
     filter(regex(?area, '.*'))
-    {
-      # Select all three winding transformers
-      select  ?p_transformer (count(distinct ?nr) as ?winding_count)
-      where {
-        ?p_transformer ^cim:PowerTransformerEnd.PowerTransformer/cim:TransformerEnd.endNumber ?nr .
-      }
-      group by ?p_transformer
-      having (?winding_count > 2)
-    }
     ?winding cim:PowerTransformerEnd.PowerTransformer ?p_transformer;
     		     cim:TransformerEnd.Terminal ?terminal .
     optional {?p_transformer SN:Equipment.networkAnalysisEnable ?_network_analysis}
   }
 
   bind(if(coalesce(?_in_service, ?connected), 1, 0) as ?in_service) .
   bind(coalesce(?_sv_p, xsd:double(0.0)) as ?sv_p)
```

### Comparing `cimsparql-3.3.1/cimsparql/sparql/transformers.sparql` & `cimsparql-4.0.0/cimsparql/sparql/transformers.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/transformers_connected_to_converter.sparql` & `cimsparql-4.0.0/cimsparql/sparql/transformers_connected_to_converter.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/two_winding_transformer_angle.sparql` & `cimsparql-4.0.0/cimsparql/sparql/two_winding_transformer_angle.sparql`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-# Name: Two winding transformer angle
+# Name: Winding transformer angle
 PREFIX cim: <${cim}>
 PREFIX rdf: <${rdf}>
 PREFIX xsd: <${xsd}>
 select ?mrid ?angle
 where {
   ?tap_changer cim:TapChanger.step ?ssh_position .
   optional{ ?tap_changer ^cim:SvTapStep.TapChanger/cim:SvTapStep.position ?sv_position } .
 
   ?_eq_subject <http://entsoe.eu/CIM/EquipmentCore/3/1> ?eq_repo .
   service ?eq_repo {
-    ?winding1 cim:PowerTransformerEnd.PowerTransformer ?p_transformer;
-              cim:IdentifiedObject.mRID ?mrid;
-              cim:TransformerEnd.endNumber 1 .
-    ?winding2 cim:PowerTransformerEnd.PowerTransformer ?p_transformer;
-              cim:TransformerEnd.endNumber 2 .
+    ?winding cim:PowerTransformerEnd.PowerTransformer ?p_transformer;
+              cim:IdentifiedObject.mRID ?mrid .
     ?tap_changer cim:PhaseTapChangerLinear.stepPhaseShiftIncrement ?inc;
                 cim:TapChanger.normalStep ?normalstep;
                 ^cim:PhaseTapChanger.TransformerEnd/cim:PowerTransformerEnd.PowerTransformer ?p_transformer .
   }
 
   bind(coalesce(?sv_position, ?ssh_position) as ?position)
   bind((xsd:double(str(?position)) - xsd:double(str(?normalstep))) * xsd:double(str(?inc)) as ?angle)
```

### Comparing `cimsparql-3.3.1/cimsparql/sparql/wind_generating_units.sparql` & `cimsparql-4.0.0/cimsparql/sparql/wind_generating_units.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql/winding.sparql` & `cimsparql-4.0.0/cimsparql/sparql/winding.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/sparql_result_json.py` & `cimsparql-4.0.0/cimsparql/sparql_result_json.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/templates.py` & `cimsparql-4.0.0/cimsparql/templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,20 +33,20 @@
     sparql_folder / "station_group_code_and_names.sparql"
 )
 SUBSTATION_VOLTAGE_LEVEL_QUERY = _read_template(sparql_folder / "substation_voltage_level.sparql")
 SV_BRANCH_QUERY = _read_template(sparql_folder / "sv_branch.sparql")
 SV_INJECTION_QUERY = _read_template(sparql_folder / "sv_injection.sparql")
 SYNCHRONOUS_MACHINES_QUERY = _read_template(sparql_folder / "synchronous_machines.sparql")
 SWITCHES_QUERY = _read_template(sparql_folder / "switches.sparql")
-THREE_WINDING_DUMMY_NODES_QUERY = _read_template(sparql_folder / "three_winding_dummy_nodes.sparql")
-THREE_WINDING_LOSS_QUERY = _read_template(sparql_folder / "three_winding_loss.sparql")
-THREE_WINDING_QUERY = _read_template(sparql_folder / "three_winding.sparql")
+TRANSFORMER_BRANCHES_QUERY = _read_template(sparql_folder / "transformer_branches.sparql")
+TRANSFORMER_CENTER_NODES_QUERY = _read_template(sparql_folder / "transformer_center_nodes.sparql")
 TRANSFORMERS_QUERY = _read_template(sparql_folder / "transformers.sparql")
 TRANSFORMERS_CONNECTED_TO_CONVERTER_QUERY = _read_template(
     sparql_folder / "transformers_connected_to_converter.sparql"
 )
 TWO_WINDING_ANGLE_QUERY = _read_template(sparql_folder / "two_winding_transformer_angle.sparql")
 TWO_WINDING_QUERY = _read_template(sparql_folder / "two_winding_transformer.sparql")
 TYPE_MAPPER_QUERY = _read_template(sparql_folder / "type_mapper.sparql")
 WIND_GENERATING_UNITS_QUERY = _read_template(sparql_folder / "wind_generating_units.sparql")
 TRANSFORMER_WINDINGS_QUERY = _read_template(sparql_folder / "transformer_windings.sparql")
 WINDING = _read_template(sparql_folder / "winding.sparql")
+WINDING_LOSS_QUERY = _read_template(sparql_folder / "winding_loss.sparql")
```

### Comparing `cimsparql-3.3.1/cimsparql/type_mapper.py` & `cimsparql-4.0.0/cimsparql/type_mapper.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/url.py` & `cimsparql-4.0.0/cimsparql/url.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/cimsparql/value_mapper.py` & `cimsparql-4.0.0/cimsparql/value_mapper.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/pkg_data/namespaces.json` & `cimsparql-4.0.0/pkg_data/namespaces.json`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/pkg_data/native_store_config_template.ttl` & `cimsparql-4.0.0/pkg_data/native_store_config_template.ttl`

 * *Files identical despite different names*

### Comparing `cimsparql-3.3.1/pyproject.toml` & `cimsparql-4.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cimsparql"
-version = "3.3.1"
+version = "4.0.0"
 description = "CIM query utilities"
 readme = "README.md"
 authors = ["Statnett Datascience <Datascience.Drift@Statnett.no>"]
 repository = "https://github.com/statnett/cimsparql.git"
 include = ["pkg_data/*"]
 exclude = ["tests/*"]
```

### Comparing `cimsparql-3.3.1/PKG-INFO` & `cimsparql-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cimsparql
-Version: 3.3.1
+Version: 4.0.0
 Summary: CIM query utilities
 Home-page: https://github.com/statnett/cimsparql.git
 Author: Statnett Datascience
 Author-email: Datascience.Drift@Statnett.no
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

