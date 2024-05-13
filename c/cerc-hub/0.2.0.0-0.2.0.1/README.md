# Comparing `tmp/cerc_hub-0.2.0.0.tar.gz` & `tmp/cerc_hub-0.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerc_hub-0.2.0.0.tar", last modified: Mon Apr 29 04:10:22 2024, max compression
+gzip compressed data, was "cerc_hub-0.2.0.1.tar", last modified: Mon May 13 05:43:19 2024, max compression
```

## Comparing `cerc_hub-0.2.0.0.tar` & `cerc_hub-0.2.0.1.tar`

### file list

```diff
@@ -1,367 +1,367 @@
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.941336 cerc_hub-0.2.0.0/
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1539 2024-04-29 04:10:22.941336 cerc_hub-0.2.0.0/PKG-INFO
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.941336 cerc_hub-0.2.0.0/cerc_hub.egg-info/
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1539 2024-04-29 04:10:22.000000 cerc_hub-0.2.0.0/cerc_hub.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (103) jenkins    (111)    14300 2024-04-29 04:10:22.000000 cerc_hub-0.2.0.0/cerc_hub.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)        1 2024-04-29 04:10:22.000000 cerc_hub-0.2.0.0/cerc_hub.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)      280 2024-04-29 04:10:22.000000 cerc_hub-0.2.0.0/cerc_hub.egg-info/requires.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)        4 2024-04-29 04:10:22.000000 cerc_hub-0.2.0.0/cerc_hub.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.885335 cerc_hub-0.2.0.0/hub/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/__init__.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.889335 cerc_hub-0.2.0.0/hub/catalog_factories/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      870 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/catalog.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.889335 cerc_hub-0.2.0.0/hub/catalog_factories/construction/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/construction/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1701 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/construction/construction_helper.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    10216 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/construction/eilat_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    10333 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/construction/nrcan_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    10384 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/construction/nrel_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1507 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/construction_catalog_factory.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.889335 cerc_hub-0.2.0.0/hub/catalog_factories/cost/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/cost/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     8566 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/cost/montreal_custom_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1044 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/costs_catalog_factory.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.889335 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/__init__.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.889335 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4634 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/archetype.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2057 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/construction.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1370 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/content.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1298 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/layer.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3187 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/material.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1728 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/window.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.889335 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3180 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/archetype.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1801 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/capital_cost.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1320 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/chapter.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      951 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/content.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1926 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/fuel.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2189 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/income.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2612 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/item_description.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2132 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/operational_cost.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.889335 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1128 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/archetype.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1459 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/content.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4734 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/distribution_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3106 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/electrical_storage_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1449 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/emission_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1694 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/energy_storage_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2421 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/generation_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    10831 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/non_pv_generation_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2116 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/performance_curves.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5367 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/pv_generation_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2866 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3442 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/thermal_storage_system.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.889335 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/greenery/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/greenery/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1164 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/greenery/content.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2912 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/greenery/plant.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1494 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/greenery/plant_percentage.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3584 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/greenery/soil.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5825 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/greenery/vegetation.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.893335 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2063 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/appliances.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      873 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/content.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1879 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/domestic_hot_water.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2053 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/lighting.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2547 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/occupancy.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2225 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/schedule.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3578 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/thermal_control.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4090 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/usage.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.893335 cerc_hub-0.2.0.0/hub/catalog_factories/energy_systems/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/energy_systems/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    12126 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/energy_systems/montreal_custom_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    29316 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/energy_systems/montreal_future_system_catalogue.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1461 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/energy_systems_catalog_factory.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.893335 cerc_hub-0.2.0.0/hub/catalog_factories/greenery/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/greenery/__init__.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.893335 cerc_hub-0.2.0.0/hub/catalog_factories/greenery/ecore_greenery/
--rw-r--r--   0 jenkins    (103) jenkins    (111)    19314 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.ecore
--rw-r--r--   0 jenkins    (103) jenkins    (111)    12388 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    18684 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog_no_quantities.ecore
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4564 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/greenery/greenery_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1107 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/greenery_catalog_factory.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.893335 cerc_hub-0.2.0.0/hub/catalog_factories/usage/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/usage/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    10095 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/usage/comnet_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    10022 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/usage/eilat_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    10213 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/usage/nrcan_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4425 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/usage/usage_helper.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1516 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/catalog_factories/usage_catalog_factory.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.893335 cerc_hub-0.2.0.0/hub/city_model_structure/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/__init__.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.893335 cerc_hub-0.2.0.0/hub/city_model_structure/attributes/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/attributes/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      935 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/attributes/edge.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1194 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/attributes/node.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1929 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/attributes/plane.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      843 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/attributes/point.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    13218 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/attributes/polygon.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     6590 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/attributes/polyhedron.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      763 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/attributes/record.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2922 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/attributes/schedule.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      770 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/attributes/time_series.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    28635 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.897335 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2359 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/appliances.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2939 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/construction.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2052 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/domestic_hot_water.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      650 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/household.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3009 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/internal_gain.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4156 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/internal_zone.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4493 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/layer.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2349 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/lighting.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2865 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/occupancy.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3178 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/storey.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    11254 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/surface.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3502 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/thermal_archetype.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    11103 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/thermal_boundary.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4563 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/thermal_control.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5277 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/thermal_opening.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    25615 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/thermal_zone.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     7852 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/usage.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      957 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/buildings_cluster.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    16188 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/city.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     8085 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/city_object.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1638 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/city_objects_cluster.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.897335 cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      570 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/control_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4706 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/distribution_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2495 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/electrical_storage_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1275 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/emission_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2532 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/energy_storage_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3666 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/energy_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3216 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/generation_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    11977 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/non_pv_generation_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3288 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/performance_curve.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5202 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/pv_generation_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2072 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/thermal_storage_system.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.897335 cerc_hub-0.2.0.0/hub/city_model_structure/greenery/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/greenery/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2304 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/greenery/plant.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3288 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/greenery/soil.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1630 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/greenery/vegetation.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.897335 cerc_hub-0.2.0.0/hub/city_model_structure/iot/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/iot/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1503 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/iot/sensor.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      867 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/iot/sensor_measure.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      462 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/iot/sensor_type.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      943 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/iot/station.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2502 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/level_of_detail.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1195 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/network.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      974 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/city_model_structure/parts_consisting_building.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.897335 cerc_hub-0.2.0.0/hub/config/
--rw-r--r--   0 jenkins    (103) jenkins    (111)      629 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/config/configuration.ini
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.885335 cerc_hub-0.2.0.0/hub/data/
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.901335 cerc_hub-0.2.0.0/hub/data/construction/
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3280 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/construction/eilat_archetypes.json
--rw-r--r--   0 jenkins    (103) jenkins    (111)    73899 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/construction/eilat_constructions.json
--rw-r--r--   0 jenkins    (103) jenkins    (111)  1894214 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/construction/nrcan_archetypes.json
--rw-r--r--   0 jenkins    (103) jenkins    (111)   274471 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/construction/nrcan_constructions.json
--rw-r--r--   0 jenkins    (103) jenkins    (111)    44638 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/construction/us_archetypes.xml
--rw-r--r--   0 jenkins    (103) jenkins    (111)    32891 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/construction/us_constructions.xml
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.901335 cerc_hub-0.2.0.0/hub/data/costs/
--rw-r--r--   0 jenkins    (103) jenkins    (111)    11017 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/costs/montreal_costs.xml
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.901335 cerc_hub-0.2.0.0/hub/data/customized_imports/
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3228 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/customized_imports/ashrae_archetypes.xml
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.901335 cerc_hub-0.2.0.0/hub/data/energy_systems/
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.905335 cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/
--rw-r--r--   0 jenkins    (103) jenkins    (111)   105875 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/air_source.xlsx
--rw-r--r--   0 jenkins    (103) jenkins    (111)    11051 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/as_parallel.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)    10802 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/as_series.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)      446 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/constants.yaml
--rw-r--r--   0 jenkins    (103) jenkins    (111)  1040664 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/demand.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)    10820 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/w2w_parallel.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)    10411 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/w2w_series.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)    73906 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/water_to_water.xlsx
--rw-r--r--   0 jenkins    (103) jenkins    (111)   257760 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/wt_hourly3.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)    20817 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/energy_systems/montreal_custom_systems.xml
--rw-r--r--   0 jenkins    (103) jenkins    (111)    50129 2024-04-29 04:08:59.000000 cerc_hub-0.2.0.0/hub/data/energy_systems/montreal_future_systems.xml
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.909335 cerc_hub-0.2.0.0/hub/data/geolocation/
--rw-r--r--   0 jenkins    (103) jenkins    (111)  2219196 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/data/geolocation/admin2Codes.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)  6284352 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/data/geolocation/cities15000.txt
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.917335 cerc_hub-0.2.0.0/hub/data/greenery/
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5044 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/data/greenery/ecore_greenery_catalog.xml
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.917335 cerc_hub-0.2.0.0/hub/data/usage/
--rw-r--r--   0 jenkins    (103) jenkins    (111)   299386 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/data/usage/comnet_archetypes.xlsx
--rw-r--r--   0 jenkins    (103) jenkins    (111)   348793 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/data/usage/comnet_schedules_archetypes.xlsx
--rw-r--r--   0 jenkins    (103) jenkins    (111)    15170 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/data/usage/eilat_archetypes.xlsx
--rw-r--r--   0 jenkins    (103) jenkins    (111)    78312 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/data/usage/eilat_schedules_archetypes.xlsx
--rw-r--r--   0 jenkins    (103) jenkins    (111)   186345 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/data/usage/nrcan_schedules.json
--rw-r--r--   0 jenkins    (103) jenkins    (111)   150910 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/data/usage/nrcan_space_compliance_2015.json
--rw-r--r--   0 jenkins    (103) jenkins    (111)  1314444 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/data/usage/nrcan_space_types.json
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.885335 cerc_hub-0.2.0.0/hub/data/weather/
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.921336 cerc_hub-0.2.0.0/hub/data/weather/epw/
--rw-r--r--   0 jenkins    (103) jenkins    (111)  1588401 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/data/weather/epw/CAN_PQ_Montreal.Intl.AP.716270_CWEC.epw
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.921336 cerc_hub-0.2.0.0/hub/exports/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/__init__.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.921336 cerc_hub-0.2.0.0/hub/exports/building_energy/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/building_energy/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    17080 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/building_energy/energy_ade.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    36308 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/building_energy/idf.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.929335 cerc_hub-0.2.0.0/hub/exports/building_energy/idf_files/
--rw-r--r--   0 jenkins    (103) jenkins    (111)  4625243 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/building_energy/idf_files/Energy+.idd
--rw-r--r--   0 jenkins    (103) jenkins    (111)  4241609 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/building_energy/idf_files/Energy+9.5.idd
--rw-r--r--   0 jenkins    (103) jenkins    (111)     7206 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/building_energy/idf_files/Minimal.idf
--rw-r--r--   0 jenkins    (103) jenkins    (111)     7428 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/building_energy/idf_files/Minimal9.5.idf
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.929335 cerc_hub-0.2.0.0/hub/exports/building_energy/insel/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/building_energy/insel/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    13598 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/building_energy/insel/insel_monthly_energy_balance.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2814 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/energy_building_exports_factory.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.929335 cerc_hub-0.2.0.0/hub/exports/energy_systems/
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2379 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/energy_systems/air_source_hp_export.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    12750 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/energy_systems/heat_pump_export.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2228 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/energy_systems/water_to_water_hp_export.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2238 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/energy_systems_factory.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2396 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/exports_factory.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.929335 cerc_hub-0.2.0.0/hub/exports/formats/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/formats/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5418 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/formats/cesiumjs_tileset.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3808 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/formats/geojson.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1503 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/formats/glb.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3410 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/formats/obj.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4889 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/formats/simplified_radiosity_algorithm.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      398 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/formats/stl.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1069 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/exports/formats/triangular.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.933336 cerc_hub-0.2.0.0/hub/helpers/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      766 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/auth.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4765 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/configuration_helper.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    10588 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/constants.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.933336 cerc_hub-0.2.0.0/hub/helpers/data/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     9183 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/alkis_function_to_hub_function.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      694 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/eilat_function_to_hub_function.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1039 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/hft_function_to_hub_function.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      762 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/hub_function_to_eilat_construction_function.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3318 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/hub_function_to_montreal_custom_costs_function.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3032 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/hub_function_to_nrcan_construction_function.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3058 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/hub_function_to_nrel_construction_function.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3265 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/hub_usage_to_comnet_usage.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      682 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/hub_usage_to_eilat_usage.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3230 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/hub_usage_to_hft_usage.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3280 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/hub_usage_to_nrcan_usage.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      635 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/montreal_custom_fuel_to_hub_fuel.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      813 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/montreal_demand_type_to_hub_energy_demand_type.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    32830 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/montreal_function_to_hub_function.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      829 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/montreal_generation_system_to_hub_energy_generation_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2155 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/montreal_system_to_hub_energy_generation_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      705 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/north_america_custom_fuel_to_hub_fuel.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      817 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/north_america_demand_type_to_hub_energy_demand_type.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      701 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/north_america_storage_system_to_hub_storage.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1001 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/north_america_system_to_hub_energy_generation_system.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     6408 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/data/pluto_function_to_hub_function.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     7155 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/dictionaries.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    12443 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/geometry_helper.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1279 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/location.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1238 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/monthly_values.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.933336 cerc_hub-0.2.0.0/hub/helpers/peak_calculation/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/peak_calculation/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     6305 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/peak_calculation/loads_calculation.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4873 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/peak_loads.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1674 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/thermal_zones_creation.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      916 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/helpers/utils.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.933336 cerc_hub-0.2.0.0/hub/imports/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/__init__.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.933336 cerc_hub-0.2.0.0/hub/imports/construction/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/construction/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5784 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/construction/eilat_physics_parameters.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.933336 cerc_hub-0.2.0.0/hub/imports/construction/helpers/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/construction/helpers/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2878 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/construction/helpers/construction_helper.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     7447 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/construction/helpers/storeys_generation.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5424 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/construction/nrcan_physics_parameters.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5706 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/construction/nrel_physics_parameters.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1916 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/construction_factory.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.937336 cerc_hub-0.2.0.0/hub/imports/energy_systems/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/energy_systems/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     7338 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/energy_systems/montreal_custom_energy_system_parameters.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    11766 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/energy_systems/montreal_future_energy_systems_parameters.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     7818 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/energy_systems/north_america_custom_energy_system_parameters.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2322 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/energy_systems_factory.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.937336 cerc_hub-0.2.0.0/hub/imports/geometry/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/geometry/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     8013 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/geometry/citygml.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.937336 cerc_hub-0.2.0.0/hub/imports/geometry/citygml_classes/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/geometry/citygml_classes/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      792 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/geometry/citygml_classes/citygml_base.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2358 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/geometry/citygml_classes/citygml_lod1.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3516 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/geometry/citygml_classes/citygml_lod2.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    14585 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/geometry/geojson.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.937336 cerc_hub-0.2.0.0/hub/imports/geometry/helpers/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/geometry/helpers/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3259 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/geometry/helpers/geometry_helper.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2936 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/geometry/obj.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2355 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/geometry_factory.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.937336 cerc_hub-0.2.0.0/hub/imports/results/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/results/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5199 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/results/energy_plus.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4999 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/results/energy_plus_single_building.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4279 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/results/ep_multiple_buildings.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5165 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/results/insel_monthly_energry_balance.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1828 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/results/simplified_radiosity_algorithm.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2345 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/results_factory.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.937336 cerc_hub-0.2.0.0/hub/imports/usage/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/usage/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    10879 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/usage/comnet_usage_parameters.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    10867 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/usage/eilat_usage_parameters.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     9287 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/usage/nrcan_usage_parameters.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1894 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/usage_factory.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.937336 cerc_hub-0.2.0.0/hub/imports/weather/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/weather/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     9033 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/weather/epw_weather_parameters.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.937336 cerc_hub-0.2.0.0/hub/imports/weather/helpers/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/weather/helpers/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4385 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/weather/helpers/weather.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1179 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/imports/weather_factory.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.937336 cerc_hub-0.2.0.0/hub/persistence/
--rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1941 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/configuration.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     9684 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/db_control.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2942 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/db_setup.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.937336 cerc_hub-0.2.0.0/hub/persistence/models/
--rw-r--r--   0 jenkins    (103) jenkins    (111)      203 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/models/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1040 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/models/application.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1275 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/models/city.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3086 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/models/city_object.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1217 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/models/simulation_results.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1129 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/models/user.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.937336 cerc_hub-0.2.0.0/hub/persistence/repositories/
--rw-r--r--   0 jenkins    (103) jenkins    (111)       29 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/repositories/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3778 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/repositories/application.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4659 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/repositories/city.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     8660 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/repositories/city_object.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     7260 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/repositories/simulation_results.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5410 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/repositories/user.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      695 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/persistence/repository.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)       51 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/hub/version.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      164 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/pyproject.toml
--rw-r--r--   0 jenkins    (103) jenkins    (111)      268 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/requirements.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)       38 2024-04-29 04:10:22.941336 cerc_hub-0.2.0.0/setup.cfg
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5279 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/setup.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-29 04:10:22.941336 cerc_hub-0.2.0.0/tests/
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4919 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_city_merge.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2734 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_construction_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    16963 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_construction_factory.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      938 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_costs_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     7097 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_custom_insel_block.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    13805 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_db_factory.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     6907 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_db_retrieve.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     7488 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_enrichement.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     6042 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_exports.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     9910 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_geometry_factory.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1339 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_greenery_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3225 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_greenery_in_idf.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     6967 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_insel_exports.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     6620 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_results_import.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2189 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_systems_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     6670 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_systems_factory.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      819 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_usage_catalog.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)    11500 2024-04-29 04:09:00.000000 cerc_hub-0.2.0.0/tests/test_usage_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.977058 cerc_hub-0.2.0.1/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1539 2024-05-13 05:43:19.977058 cerc_hub-0.2.0.1/PKG-INFO
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.977058 cerc_hub-0.2.0.1/cerc_hub.egg-info/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1539 2024-05-13 05:43:19.000000 cerc_hub-0.2.0.1/cerc_hub.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    14300 2024-05-13 05:43:19.000000 cerc_hub-0.2.0.1/cerc_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        1 2024-05-13 05:43:19.000000 cerc_hub-0.2.0.1/cerc_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      280 2024-05-13 05:43:19.000000 cerc_hub-0.2.0.1/cerc_hub.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        4 2024-05-13 05:43:19.000000 cerc_hub-0.2.0.1/cerc_hub.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.921057 cerc_hub-0.2.0.1/hub/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/__init__.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.921057 cerc_hub-0.2.0.1/hub/catalog_factories/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      870 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/catalog.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.921057 cerc_hub-0.2.0.1/hub/catalog_factories/construction/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/construction/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1701 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/construction/construction_helper.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    10216 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/construction/eilat_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    10333 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/construction/nrcan_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    10384 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/construction/nrel_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1507 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/construction_catalog_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.921057 cerc_hub-0.2.0.1/hub/catalog_factories/cost/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/cost/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     8566 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/cost/montreal_custom_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1044 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/costs_catalog_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.921057 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/__init__.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.925057 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4634 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/archetype.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2057 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/construction.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1370 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/content.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1298 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/layer.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3187 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/material.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1728 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/window.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.925057 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3180 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/archetype.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1801 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/capital_cost.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1320 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/chapter.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      951 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/content.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1926 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/fuel.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2189 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/income.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2612 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/item_description.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2132 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/operational_cost.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.925057 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1128 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/archetype.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1459 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/content.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4734 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/distribution_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3106 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/electrical_storage_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1449 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/emission_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1694 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/energy_storage_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2421 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/generation_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    10831 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/non_pv_generation_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2116 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/performance_curves.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5367 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/pv_generation_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2866 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3442 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/thermal_storage_system.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.925057 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/greenery/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/greenery/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1164 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/greenery/content.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2912 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/greenery/plant.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1494 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/greenery/plant_percentage.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3584 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/greenery/soil.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5825 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/greenery/vegetation.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.925057 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2063 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/appliances.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      873 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/content.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1879 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/domestic_hot_water.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2053 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/lighting.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2547 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/occupancy.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2225 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/schedule.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3578 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/thermal_control.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4090 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/usage.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.925057 cerc_hub-0.2.0.1/hub/catalog_factories/energy_systems/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/energy_systems/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    12126 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/energy_systems/montreal_custom_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    29316 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/energy_systems/montreal_future_system_catalogue.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1461 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/energy_systems_catalog_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.929057 cerc_hub-0.2.0.1/hub/catalog_factories/greenery/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/greenery/__init__.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.929057 cerc_hub-0.2.0.1/hub/catalog_factories/greenery/ecore_greenery/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    19314 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.ecore
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    12388 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    18684 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog_no_quantities.ecore
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4564 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/greenery/greenery_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1107 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/greenery_catalog_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.929057 cerc_hub-0.2.0.1/hub/catalog_factories/usage/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/usage/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    10095 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/usage/comnet_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    10022 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/usage/eilat_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    10213 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/usage/nrcan_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4425 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/usage/usage_helper.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1516 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/catalog_factories/usage_catalog_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.929057 cerc_hub-0.2.0.1/hub/city_model_structure/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/__init__.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.929057 cerc_hub-0.2.0.1/hub/city_model_structure/attributes/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/attributes/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      935 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/attributes/edge.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1194 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/attributes/node.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1929 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/attributes/plane.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      843 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/attributes/point.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    13218 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/attributes/polygon.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     6590 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/attributes/polyhedron.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      763 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/attributes/record.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2922 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/attributes/schedule.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      770 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/attributes/time_series.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    28635 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.933057 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2359 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/appliances.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2939 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/construction.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2052 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/domestic_hot_water.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      650 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/household.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3009 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/internal_gain.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4156 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/internal_zone.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4493 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/layer.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2349 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/lighting.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2865 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/occupancy.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3178 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/storey.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    11254 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/surface.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3502 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/thermal_archetype.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    11103 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/thermal_boundary.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4563 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/thermal_control.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5277 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/thermal_opening.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    25615 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/thermal_zone.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     7852 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/usage.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      957 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/buildings_cluster.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    16188 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/city.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     8085 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/city_object.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1638 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/city_objects_cluster.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.933057 cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      570 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/control_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4706 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/distribution_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2495 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/electrical_storage_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1275 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/emission_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2532 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/energy_storage_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3666 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/energy_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3216 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/generation_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    11977 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/non_pv_generation_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3288 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/performance_curve.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5202 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/pv_generation_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2072 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/thermal_storage_system.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.933057 cerc_hub-0.2.0.1/hub/city_model_structure/greenery/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/greenery/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2304 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/greenery/plant.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3288 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/greenery/soil.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1630 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/greenery/vegetation.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.933057 cerc_hub-0.2.0.1/hub/city_model_structure/iot/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/iot/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1503 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/iot/sensor.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      867 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/iot/sensor_measure.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      462 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/iot/sensor_type.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      943 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/iot/station.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2502 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/level_of_detail.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1195 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/network.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      974 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/city_model_structure/parts_consisting_building.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.933057 cerc_hub-0.2.0.1/hub/config/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      629 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/config/configuration.ini
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.921057 cerc_hub-0.2.0.1/hub/data/
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.937057 cerc_hub-0.2.0.1/hub/data/construction/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3280 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/construction/eilat_archetypes.json
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    73899 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/construction/eilat_constructions.json
+-rw-r--r--   0 jenkins    (103) jenkins    (111)  1894214 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/construction/nrcan_archetypes.json
+-rw-r--r--   0 jenkins    (103) jenkins    (111)   274471 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/construction/nrcan_constructions.json
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    44638 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/construction/us_archetypes.xml
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    32891 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/construction/us_constructions.xml
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.937057 cerc_hub-0.2.0.1/hub/data/costs/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    11017 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/costs/montreal_costs.xml
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.937057 cerc_hub-0.2.0.1/hub/data/customized_imports/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3228 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/customized_imports/ashrae_archetypes.xml
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.937057 cerc_hub-0.2.0.1/hub/data/energy_systems/
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.941057 cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)   105875 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/air_source.xlsx
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    11051 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/as_parallel.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    10802 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/as_series.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      446 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/constants.yaml
+-rw-r--r--   0 jenkins    (103) jenkins    (111)  1040664 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/demand.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    10820 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/w2w_parallel.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    10411 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/w2w_series.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    73906 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/water_to_water.xlsx
+-rw-r--r--   0 jenkins    (103) jenkins    (111)   257760 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/wt_hourly3.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    20817 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/energy_systems/montreal_custom_systems.xml
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    50129 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/energy_systems/montreal_future_systems.xml
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.945057 cerc_hub-0.2.0.1/hub/data/geolocation/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)  2219196 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/geolocation/admin2Codes.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)  6284352 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/geolocation/cities15000.txt
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.949057 cerc_hub-0.2.0.1/hub/data/greenery/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5044 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/greenery/ecore_greenery_catalog.xml
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.953057 cerc_hub-0.2.0.1/hub/data/usage/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)   299386 2024-05-13 05:41:54.000000 cerc_hub-0.2.0.1/hub/data/usage/comnet_archetypes.xlsx
+-rw-r--r--   0 jenkins    (103) jenkins    (111)   348793 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/data/usage/comnet_schedules_archetypes.xlsx
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    15170 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/data/usage/eilat_archetypes.xlsx
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    78312 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/data/usage/eilat_schedules_archetypes.xlsx
+-rw-r--r--   0 jenkins    (103) jenkins    (111)   186345 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/data/usage/nrcan_schedules.json
+-rw-r--r--   0 jenkins    (103) jenkins    (111)   150910 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/data/usage/nrcan_space_compliance_2015.json
+-rw-r--r--   0 jenkins    (103) jenkins    (111)  1314444 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/data/usage/nrcan_space_types.json
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.921057 cerc_hub-0.2.0.1/hub/data/weather/
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.957058 cerc_hub-0.2.0.1/hub/data/weather/epw/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)  1588401 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/data/weather/epw/CAN_PQ_Montreal.Intl.AP.716270_CWEC.epw
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.957058 cerc_hub-0.2.0.1/hub/exports/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/__init__.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.957058 cerc_hub-0.2.0.1/hub/exports/building_energy/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/building_energy/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    17080 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/building_energy/energy_ade.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    36308 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/building_energy/idf.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.965057 cerc_hub-0.2.0.1/hub/exports/building_energy/idf_files/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)  4625243 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/building_energy/idf_files/Energy+.idd
+-rw-r--r--   0 jenkins    (103) jenkins    (111)  4241609 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/building_energy/idf_files/Energy+9.5.idd
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     7206 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/building_energy/idf_files/Minimal.idf
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     7428 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/building_energy/idf_files/Minimal9.5.idf
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.965057 cerc_hub-0.2.0.1/hub/exports/building_energy/insel/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/building_energy/insel/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    13598 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/building_energy/insel/insel_monthly_energy_balance.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2814 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/energy_building_exports_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.965057 cerc_hub-0.2.0.1/hub/exports/energy_systems/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2379 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/energy_systems/air_source_hp_export.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    12750 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/energy_systems/heat_pump_export.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2228 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/energy_systems/water_to_water_hp_export.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2238 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/energy_systems_factory.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2396 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/exports_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.965057 cerc_hub-0.2.0.1/hub/exports/formats/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/formats/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5418 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/formats/cesiumjs_tileset.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3808 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/formats/geojson.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1503 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/formats/glb.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3410 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/formats/obj.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4889 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/formats/simplified_radiosity_algorithm.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      398 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/formats/stl.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1069 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/exports/formats/triangular.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.969058 cerc_hub-0.2.0.1/hub/helpers/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      766 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/auth.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4765 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/configuration_helper.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    10588 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/constants.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.969058 cerc_hub-0.2.0.1/hub/helpers/data/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     9183 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/alkis_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      694 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/eilat_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1039 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/hft_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      762 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/hub_function_to_eilat_construction_function.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3318 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/hub_function_to_montreal_custom_costs_function.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3032 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/hub_function_to_nrcan_construction_function.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3058 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/hub_function_to_nrel_construction_function.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3265 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/hub_usage_to_comnet_usage.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      682 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/hub_usage_to_eilat_usage.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3230 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/hub_usage_to_hft_usage.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3280 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/hub_usage_to_nrcan_usage.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      635 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/montreal_custom_fuel_to_hub_fuel.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      813 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/montreal_demand_type_to_hub_energy_demand_type.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    32830 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/montreal_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      829 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/montreal_generation_system_to_hub_energy_generation_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2155 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/montreal_system_to_hub_energy_generation_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      705 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/north_america_custom_fuel_to_hub_fuel.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      817 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/north_america_demand_type_to_hub_energy_demand_type.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      701 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/north_america_storage_system_to_hub_storage.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1001 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/north_america_system_to_hub_energy_generation_system.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     6408 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/data/pluto_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     7155 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/dictionaries.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    12443 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/geometry_helper.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1279 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/location.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1238 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/monthly_values.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.969058 cerc_hub-0.2.0.1/hub/helpers/peak_calculation/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/peak_calculation/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     6305 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/peak_calculation/loads_calculation.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4873 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/peak_loads.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1674 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/thermal_zones_creation.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      916 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/helpers/utils.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.969058 cerc_hub-0.2.0.1/hub/imports/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/__init__.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.969058 cerc_hub-0.2.0.1/hub/imports/construction/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/construction/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5784 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/construction/eilat_physics_parameters.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.969058 cerc_hub-0.2.0.1/hub/imports/construction/helpers/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/construction/helpers/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2878 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/construction/helpers/construction_helper.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     7447 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/construction/helpers/storeys_generation.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5424 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/construction/nrcan_physics_parameters.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5706 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/construction/nrel_physics_parameters.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1916 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/construction_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.973058 cerc_hub-0.2.0.1/hub/imports/energy_systems/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/energy_systems/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     7731 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/energy_systems/montreal_custom_energy_system_parameters.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    11766 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/energy_systems/montreal_future_energy_systems_parameters.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     7818 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/energy_systems/north_america_custom_energy_system_parameters.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2322 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/energy_systems_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.973058 cerc_hub-0.2.0.1/hub/imports/geometry/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/geometry/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     8013 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/geometry/citygml.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.973058 cerc_hub-0.2.0.1/hub/imports/geometry/citygml_classes/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/geometry/citygml_classes/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      792 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/geometry/citygml_classes/citygml_base.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2358 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/geometry/citygml_classes/citygml_lod1.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3516 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/geometry/citygml_classes/citygml_lod2.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    14585 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/geometry/geojson.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.973058 cerc_hub-0.2.0.1/hub/imports/geometry/helpers/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/geometry/helpers/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3259 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/geometry/helpers/geometry_helper.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2936 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/geometry/obj.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2355 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/geometry_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.973058 cerc_hub-0.2.0.1/hub/imports/results/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/results/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5199 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/results/energy_plus.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4999 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/results/energy_plus_single_building.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4279 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/results/ep_multiple_buildings.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5165 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/results/insel_monthly_energry_balance.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1828 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/results/simplified_radiosity_algorithm.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2345 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/results_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.973058 cerc_hub-0.2.0.1/hub/imports/usage/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/usage/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    10879 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/usage/comnet_usage_parameters.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    10867 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/usage/eilat_usage_parameters.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     9287 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/usage/nrcan_usage_parameters.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1894 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/usage_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.973058 cerc_hub-0.2.0.1/hub/imports/weather/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/weather/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     9033 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/weather/epw_weather_parameters.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.973058 cerc_hub-0.2.0.1/hub/imports/weather/helpers/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/weather/helpers/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4385 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/weather/helpers/weather.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1179 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/imports/weather_factory.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.973058 cerc_hub-0.2.0.1/hub/persistence/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1941 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/configuration.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     9684 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/db_control.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2942 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/db_setup.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.973058 cerc_hub-0.2.0.1/hub/persistence/models/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      203 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/models/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1040 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/models/application.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1275 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/models/city.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3086 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/models/city_object.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1217 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/models/simulation_results.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1129 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/models/user.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.973058 cerc_hub-0.2.0.1/hub/persistence/repositories/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)       29 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/repositories/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3778 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/repositories/application.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4659 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/repositories/city.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     8660 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/repositories/city_object.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     7260 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/repositories/simulation_results.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5410 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/repositories/user.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      695 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/persistence/repository.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)       51 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/hub/version.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      164 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/pyproject.toml
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      268 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/requirements.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)       38 2024-05-13 05:43:19.977058 cerc_hub-0.2.0.1/setup.cfg
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5279 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/setup.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-05-13 05:43:19.977058 cerc_hub-0.2.0.1/tests/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4919 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_city_merge.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2734 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_construction_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    16963 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_construction_factory.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      938 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_costs_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     7097 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_custom_insel_block.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    13805 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_db_factory.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     6907 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_db_retrieve.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     7488 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_enrichement.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     6042 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_exports.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     9910 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_geometry_factory.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1339 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_greenery_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3225 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_greenery_in_idf.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     6967 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_insel_exports.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     6620 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_results_import.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2189 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_systems_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     6670 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_systems_factory.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      819 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_usage_catalog.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)    11500 2024-05-13 05:41:55.000000 cerc_hub-0.2.0.1/tests/test_usage_factory.py
```

### Comparing `cerc_hub-0.2.0.0/PKG-INFO` & `cerc_hub-0.2.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-hub
-Version: 0.2.0.0
+Version: 0.2.0.1
 Summary: CERC Hub consist of a set of classes (Central data model), importers and exporters to help researchers to create better and more sustainable cities
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: xmltodict
 Requires-Dist: numpy
 Requires-Dist: trimesh[all]
```

### Comparing `cerc_hub-0.2.0.0/cerc_hub.egg-info/PKG-INFO` & `cerc_hub-0.2.0.1/cerc_hub.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-hub
-Version: 0.2.0.0
+Version: 0.2.0.1
 Summary: CERC Hub consist of a set of classes (Central data model), importers and exporters to help researchers to create better and more sustainable cities
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: xmltodict
 Requires-Dist: numpy
 Requires-Dist: trimesh[all]
```

### Comparing `cerc_hub-0.2.0.0/cerc_hub.egg-info/SOURCES.txt` & `cerc_hub-0.2.0.1/cerc_hub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/catalog.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/construction/construction_helper.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/construction/construction_helper.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/construction/eilat_catalog.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/construction/eilat_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/construction/nrcan_catalog.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/construction/nrcan_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/construction/nrel_catalog.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/construction/nrel_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/construction_catalog_factory.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/construction_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/cost/montreal_custom_catalog.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/cost/montreal_custom_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/costs_catalog_factory.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/costs_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/archetype.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/archetype.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/construction.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/construction.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/content.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/content.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/layer.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/layer.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/material.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/material.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/construction/window.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/construction/window.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/archetype.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/archetype.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/capital_cost.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/capital_cost.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/chapter.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/chapter.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/content.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/content.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/fuel.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/fuel.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/income.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/income.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/item_description.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/item_description.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/cost/operational_cost.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/cost/operational_cost.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/archetype.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/archetype.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/content.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/content.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/distribution_system.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/distribution_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/electrical_storage_system.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/electrical_storage_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/emission_system.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/emission_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/energy_storage_system.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/energy_storage_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/generation_system.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/non_pv_generation_system.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/non_pv_generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/performance_curves.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/performance_curves.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/pv_generation_system.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/pv_generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/system.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/energy_systems/thermal_storage_system.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/energy_systems/thermal_storage_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/greenery/content.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/greenery/content.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/greenery/plant.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/greenery/plant.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/greenery/plant_percentage.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/greenery/plant_percentage.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/greenery/soil.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/greenery/soil.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/greenery/vegetation.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/greenery/vegetation.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/appliances.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/appliances.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/content.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/content.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/domestic_hot_water.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/domestic_hot_water.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/lighting.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/lighting.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/occupancy.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/occupancy.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/schedule.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/schedule.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/thermal_control.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/thermal_control.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/data_models/usages/usage.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/data_models/usages/usage.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/energy_systems/montreal_custom_catalog.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/energy_systems/montreal_custom_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/energy_systems/montreal_future_system_catalogue.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/energy_systems/montreal_future_system_catalogue.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/energy_systems_catalog_factory.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/energy_systems_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.ecore` & `cerc_hub-0.2.0.1/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.ecore`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog_no_quantities.ecore` & `cerc_hub-0.2.0.1/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog_no_quantities.ecore`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/greenery/greenery_catalog.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/greenery/greenery_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/greenery_catalog_factory.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/greenery_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/usage/comnet_catalog.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/usage/comnet_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/usage/eilat_catalog.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/usage/eilat_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/usage/nrcan_catalog.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/usage/nrcan_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/usage/usage_helper.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/usage/usage_helper.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/catalog_factories/usage_catalog_factory.py` & `cerc_hub-0.2.0.1/hub/catalog_factories/usage_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/attributes/edge.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/attributes/edge.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/attributes/node.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/attributes/node.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/attributes/plane.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/attributes/plane.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/attributes/point.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/attributes/point.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/attributes/polygon.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/attributes/polygon.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/attributes/polyhedron.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/attributes/polyhedron.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/attributes/record.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/attributes/record.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/attributes/schedule.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/attributes/schedule.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/attributes/time_series.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/attributes/time_series.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/appliances.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/appliances.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/construction.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/construction.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/domestic_hot_water.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/domestic_hot_water.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/household.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/household.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/internal_gain.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/internal_gain.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/internal_zone.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/internal_zone.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/layer.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/layer.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/lighting.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/lighting.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/occupancy.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/occupancy.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/storey.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/storey.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/surface.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/surface.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/thermal_archetype.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/thermal_archetype.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/thermal_boundary.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/thermal_boundary.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/thermal_control.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/thermal_control.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/thermal_opening.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/thermal_opening.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/thermal_zone.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/thermal_zone.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/building_demand/usage.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/building_demand/usage.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/buildings_cluster.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/buildings_cluster.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/city.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/city.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/city_object.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/city_object.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/city_objects_cluster.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/city_objects_cluster.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/control_system.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/control_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/distribution_system.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/distribution_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/electrical_storage_system.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/electrical_storage_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/emission_system.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/emission_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/energy_storage_system.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/energy_storage_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/energy_system.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/energy_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/generation_system.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/non_pv_generation_system.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/non_pv_generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/performance_curve.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/performance_curve.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/pv_generation_system.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/pv_generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/energy_systems/thermal_storage_system.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/energy_systems/thermal_storage_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/greenery/plant.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/greenery/plant.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/greenery/soil.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/greenery/soil.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/greenery/vegetation.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/greenery/vegetation.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/iot/sensor.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/iot/sensor.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/iot/sensor_measure.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/iot/sensor_measure.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/iot/station.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/iot/station.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/level_of_detail.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/level_of_detail.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/network.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/network.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/city_model_structure/parts_consisting_building.py` & `cerc_hub-0.2.0.1/hub/city_model_structure/parts_consisting_building.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/config/configuration.ini` & `cerc_hub-0.2.0.1/hub/config/configuration.ini`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/construction/eilat_archetypes.json` & `cerc_hub-0.2.0.1/hub/data/construction/eilat_archetypes.json`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/construction/eilat_constructions.json` & `cerc_hub-0.2.0.1/hub/data/construction/eilat_constructions.json`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/construction/nrcan_archetypes.json` & `cerc_hub-0.2.0.1/hub/data/construction/nrcan_archetypes.json`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/construction/nrcan_constructions.json` & `cerc_hub-0.2.0.1/hub/data/construction/nrcan_constructions.json`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/construction/us_archetypes.xml` & `cerc_hub-0.2.0.1/hub/data/construction/us_archetypes.xml`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/construction/us_constructions.xml` & `cerc_hub-0.2.0.1/hub/data/construction/us_constructions.xml`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/costs/montreal_costs.xml` & `cerc_hub-0.2.0.1/hub/data/costs/montreal_costs.xml`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/customized_imports/ashrae_archetypes.xml` & `cerc_hub-0.2.0.1/hub/data/customized_imports/ashrae_archetypes.xml`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/air_source.xlsx` & `cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/air_source.xlsx`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/as_parallel.txt` & `cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/as_parallel.txt`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/as_series.txt` & `cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/as_series.txt`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/demand.txt` & `cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/demand.txt`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/w2w_parallel.txt` & `cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/w2w_parallel.txt`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/w2w_series.txt` & `cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/w2w_series.txt`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/water_to_water.xlsx` & `cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/water_to_water.xlsx`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/energy_systems/heat_pumps/wt_hourly3.txt` & `cerc_hub-0.2.0.1/hub/data/energy_systems/heat_pumps/wt_hourly3.txt`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/energy_systems/montreal_custom_systems.xml` & `cerc_hub-0.2.0.1/hub/data/energy_systems/montreal_custom_systems.xml`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/energy_systems/montreal_future_systems.xml` & `cerc_hub-0.2.0.1/hub/data/energy_systems/montreal_future_systems.xml`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/geolocation/admin2Codes.txt` & `cerc_hub-0.2.0.1/hub/data/geolocation/admin2Codes.txt`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/geolocation/cities15000.txt` & `cerc_hub-0.2.0.1/hub/data/geolocation/cities15000.txt`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/greenery/ecore_greenery_catalog.xml` & `cerc_hub-0.2.0.1/hub/data/greenery/ecore_greenery_catalog.xml`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/usage/comnet_archetypes.xlsx` & `cerc_hub-0.2.0.1/hub/data/usage/comnet_archetypes.xlsx`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/usage/comnet_schedules_archetypes.xlsx` & `cerc_hub-0.2.0.1/hub/data/usage/comnet_schedules_archetypes.xlsx`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/usage/eilat_archetypes.xlsx` & `cerc_hub-0.2.0.1/hub/data/usage/eilat_archetypes.xlsx`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/usage/eilat_schedules_archetypes.xlsx` & `cerc_hub-0.2.0.1/hub/data/usage/eilat_schedules_archetypes.xlsx`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/usage/nrcan_schedules.json` & `cerc_hub-0.2.0.1/hub/data/usage/nrcan_schedules.json`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/usage/nrcan_space_compliance_2015.json` & `cerc_hub-0.2.0.1/hub/data/usage/nrcan_space_compliance_2015.json`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/usage/nrcan_space_types.json` & `cerc_hub-0.2.0.1/hub/data/usage/nrcan_space_types.json`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/data/weather/epw/CAN_PQ_Montreal.Intl.AP.716270_CWEC.epw` & `cerc_hub-0.2.0.1/hub/data/weather/epw/CAN_PQ_Montreal.Intl.AP.716270_CWEC.epw`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/building_energy/energy_ade.py` & `cerc_hub-0.2.0.1/hub/exports/building_energy/energy_ade.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/building_energy/idf.py` & `cerc_hub-0.2.0.1/hub/exports/building_energy/idf.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/building_energy/idf_files/Energy+.idd` & `cerc_hub-0.2.0.1/hub/exports/building_energy/idf_files/Energy+.idd`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/building_energy/idf_files/Energy+9.5.idd` & `cerc_hub-0.2.0.1/hub/exports/building_energy/idf_files/Energy+9.5.idd`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/building_energy/idf_files/Minimal.idf` & `cerc_hub-0.2.0.1/hub/exports/building_energy/idf_files/Minimal.idf`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/building_energy/idf_files/Minimal9.5.idf` & `cerc_hub-0.2.0.1/hub/exports/building_energy/idf_files/Minimal9.5.idf`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/building_energy/insel/insel_monthly_energy_balance.py` & `cerc_hub-0.2.0.1/hub/exports/building_energy/insel/insel_monthly_energy_balance.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/energy_building_exports_factory.py` & `cerc_hub-0.2.0.1/hub/exports/energy_building_exports_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/energy_systems/air_source_hp_export.py` & `cerc_hub-0.2.0.1/hub/exports/energy_systems/air_source_hp_export.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/energy_systems/heat_pump_export.py` & `cerc_hub-0.2.0.1/hub/exports/energy_systems/heat_pump_export.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/energy_systems/water_to_water_hp_export.py` & `cerc_hub-0.2.0.1/hub/exports/energy_systems/water_to_water_hp_export.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/energy_systems_factory.py` & `cerc_hub-0.2.0.1/hub/exports/energy_systems_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/exports_factory.py` & `cerc_hub-0.2.0.1/hub/exports/exports_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/formats/cesiumjs_tileset.py` & `cerc_hub-0.2.0.1/hub/exports/formats/cesiumjs_tileset.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/formats/geojson.py` & `cerc_hub-0.2.0.1/hub/exports/formats/geojson.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/formats/glb.py` & `cerc_hub-0.2.0.1/hub/exports/formats/glb.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/formats/obj.py` & `cerc_hub-0.2.0.1/hub/exports/formats/obj.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/formats/simplified_radiosity_algorithm.py` & `cerc_hub-0.2.0.1/hub/exports/formats/simplified_radiosity_algorithm.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/exports/formats/triangular.py` & `cerc_hub-0.2.0.1/hub/exports/formats/triangular.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/auth.py` & `cerc_hub-0.2.0.1/hub/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/configuration_helper.py` & `cerc_hub-0.2.0.1/hub/helpers/configuration_helper.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/constants.py` & `cerc_hub-0.2.0.1/hub/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/alkis_function_to_hub_function.py` & `cerc_hub-0.2.0.1/hub/helpers/data/alkis_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/eilat_function_to_hub_function.py` & `cerc_hub-0.2.0.1/hub/helpers/data/eilat_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/hft_function_to_hub_function.py` & `cerc_hub-0.2.0.1/hub/helpers/data/hft_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/hub_function_to_eilat_construction_function.py` & `cerc_hub-0.2.0.1/hub/helpers/data/hub_function_to_eilat_construction_function.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/hub_function_to_montreal_custom_costs_function.py` & `cerc_hub-0.2.0.1/hub/helpers/data/hub_function_to_montreal_custom_costs_function.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/hub_function_to_nrcan_construction_function.py` & `cerc_hub-0.2.0.1/hub/helpers/data/hub_function_to_nrcan_construction_function.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/hub_function_to_nrel_construction_function.py` & `cerc_hub-0.2.0.1/hub/helpers/data/hub_function_to_nrel_construction_function.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/hub_usage_to_comnet_usage.py` & `cerc_hub-0.2.0.1/hub/helpers/data/hub_usage_to_comnet_usage.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/hub_usage_to_eilat_usage.py` & `cerc_hub-0.2.0.1/hub/helpers/data/hub_usage_to_eilat_usage.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/hub_usage_to_hft_usage.py` & `cerc_hub-0.2.0.1/hub/helpers/data/hub_usage_to_hft_usage.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/hub_usage_to_nrcan_usage.py` & `cerc_hub-0.2.0.1/hub/helpers/data/hub_usage_to_nrcan_usage.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/montreal_custom_fuel_to_hub_fuel.py` & `cerc_hub-0.2.0.1/hub/helpers/data/montreal_custom_fuel_to_hub_fuel.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/montreal_demand_type_to_hub_energy_demand_type.py` & `cerc_hub-0.2.0.1/hub/helpers/data/montreal_demand_type_to_hub_energy_demand_type.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/montreal_function_to_hub_function.py` & `cerc_hub-0.2.0.1/hub/helpers/data/montreal_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/montreal_generation_system_to_hub_energy_generation_system.py` & `cerc_hub-0.2.0.1/hub/helpers/data/montreal_generation_system_to_hub_energy_generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/montreal_system_to_hub_energy_generation_system.py` & `cerc_hub-0.2.0.1/hub/helpers/data/montreal_system_to_hub_energy_generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/north_america_custom_fuel_to_hub_fuel.py` & `cerc_hub-0.2.0.1/hub/helpers/data/north_america_custom_fuel_to_hub_fuel.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/north_america_demand_type_to_hub_energy_demand_type.py` & `cerc_hub-0.2.0.1/hub/helpers/data/north_america_demand_type_to_hub_energy_demand_type.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/north_america_storage_system_to_hub_storage.py` & `cerc_hub-0.2.0.1/hub/helpers/data/north_america_storage_system_to_hub_storage.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/north_america_system_to_hub_energy_generation_system.py` & `cerc_hub-0.2.0.1/hub/helpers/data/north_america_system_to_hub_energy_generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/data/pluto_function_to_hub_function.py` & `cerc_hub-0.2.0.1/hub/helpers/data/pluto_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/dictionaries.py` & `cerc_hub-0.2.0.1/hub/helpers/dictionaries.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/geometry_helper.py` & `cerc_hub-0.2.0.1/hub/helpers/geometry_helper.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/location.py` & `cerc_hub-0.2.0.1/hub/helpers/location.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/monthly_values.py` & `cerc_hub-0.2.0.1/hub/helpers/monthly_values.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/peak_calculation/loads_calculation.py` & `cerc_hub-0.2.0.1/hub/helpers/peak_calculation/loads_calculation.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/peak_loads.py` & `cerc_hub-0.2.0.1/hub/helpers/peak_loads.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/thermal_zones_creation.py` & `cerc_hub-0.2.0.1/hub/helpers/thermal_zones_creation.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/helpers/utils.py` & `cerc_hub-0.2.0.1/hub/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/construction/eilat_physics_parameters.py` & `cerc_hub-0.2.0.1/hub/imports/construction/eilat_physics_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/construction/helpers/construction_helper.py` & `cerc_hub-0.2.0.1/hub/imports/construction/helpers/construction_helper.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/construction/helpers/storeys_generation.py` & `cerc_hub-0.2.0.1/hub/imports/construction/helpers/storeys_generation.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/construction/nrcan_physics_parameters.py` & `cerc_hub-0.2.0.1/hub/imports/construction/nrcan_physics_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/construction/nrel_physics_parameters.py` & `cerc_hub-0.2.0.1/hub/imports/construction/nrel_physics_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/construction_factory.py` & `cerc_hub-0.2.0.1/hub/imports/construction_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/energy_systems/montreal_custom_energy_system_parameters.py` & `cerc_hub-0.2.0.1/hub/imports/energy_systems/montreal_custom_energy_system_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,21 +103,27 @@
         _generation_system.fuel_type = _fuel_type
         _generation_system.source_types = archetype_generation_system.source_medium
         _generation_system.heat_efficiency = archetype_generation_system.heat_efficiency
         _generation_system.cooling_efficiency = archetype_generation_system.cooling_efficiency
         _generation_system.electricity_efficiency = archetype_generation_system.electricity_efficiency
         _generic_storage_system = None
         if archetype_generation_system.energy_storage_systems is not None:
-          if archetype_generation_system.energy_storage_systems.type_energy_stored == 'electrical':
-            _generic_storage_system = ElectricalStorageSystem()
-            _generic_storage_system.type_energy_stored = 'electrical'
-          else:
-            _generic_storage_system = ThermalStorageSystem()
-            _generic_storage_system.type_energy_stored = 'thermal'
-        _generation_system.energy_storage_systems = [_generic_storage_system]
+          _storage_systems = []
+          for storage_system in archetype_generation_system.energy_storage_systems:
+            if storage_system.type_energy_stored == 'electrical':
+              _generic_storage_system = ElectricalStorageSystem()
+              _generic_storage_system.type_energy_stored = 'electrical'
+            else:
+              _generic_storage_system = ThermalStorageSystem()
+              _generic_storage_system.type_energy_stored = storage_system.type_energy_stored
+              _generic_storage_system.height = storage_system.height
+              _generic_storage_system.layers = storage_system.layers
+              _generic_storage_system.storage_medium = storage_system.storage_medium
+            _storage_systems.append(_generic_storage_system)
+          _generation_system.energy_storage_systems = _storage_systems
       _generation_systems.append(_generation_system)
     return _generation_systems
 
   @staticmethod
   def _create_distribution_systems(archetype_system):
     _distribution_systems = []
     for archetype_distribution_system in archetype_system.distribution_systems:
```

### Comparing `cerc_hub-0.2.0.0/hub/imports/energy_systems/montreal_future_energy_systems_parameters.py` & `cerc_hub-0.2.0.1/hub/imports/energy_systems/montreal_future_energy_systems_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/energy_systems/north_america_custom_energy_system_parameters.py` & `cerc_hub-0.2.0.1/hub/imports/energy_systems/north_america_custom_energy_system_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/energy_systems_factory.py` & `cerc_hub-0.2.0.1/hub/imports/energy_systems_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/geometry/citygml.py` & `cerc_hub-0.2.0.1/hub/imports/geometry/citygml.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/geometry/citygml_classes/citygml_base.py` & `cerc_hub-0.2.0.1/hub/imports/geometry/citygml_classes/citygml_base.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/geometry/citygml_classes/citygml_lod1.py` & `cerc_hub-0.2.0.1/hub/imports/geometry/citygml_classes/citygml_lod1.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/geometry/citygml_classes/citygml_lod2.py` & `cerc_hub-0.2.0.1/hub/imports/geometry/citygml_classes/citygml_lod2.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/geometry/geojson.py` & `cerc_hub-0.2.0.1/hub/imports/geometry/geojson.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/geometry/helpers/geometry_helper.py` & `cerc_hub-0.2.0.1/hub/imports/geometry/helpers/geometry_helper.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/geometry/obj.py` & `cerc_hub-0.2.0.1/hub/imports/geometry/obj.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/geometry_factory.py` & `cerc_hub-0.2.0.1/hub/imports/geometry_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/results/energy_plus.py` & `cerc_hub-0.2.0.1/hub/imports/results/energy_plus.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/results/energy_plus_single_building.py` & `cerc_hub-0.2.0.1/hub/imports/results/energy_plus_single_building.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/results/ep_multiple_buildings.py` & `cerc_hub-0.2.0.1/hub/imports/results/ep_multiple_buildings.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/results/insel_monthly_energry_balance.py` & `cerc_hub-0.2.0.1/hub/imports/results/insel_monthly_energry_balance.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/results/simplified_radiosity_algorithm.py` & `cerc_hub-0.2.0.1/hub/imports/results/simplified_radiosity_algorithm.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/results_factory.py` & `cerc_hub-0.2.0.1/hub/imports/results_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/usage/comnet_usage_parameters.py` & `cerc_hub-0.2.0.1/hub/imports/usage/comnet_usage_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/usage/eilat_usage_parameters.py` & `cerc_hub-0.2.0.1/hub/imports/usage/eilat_usage_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/usage/nrcan_usage_parameters.py` & `cerc_hub-0.2.0.1/hub/imports/usage/nrcan_usage_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/usage_factory.py` & `cerc_hub-0.2.0.1/hub/imports/usage_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/weather/epw_weather_parameters.py` & `cerc_hub-0.2.0.1/hub/imports/weather/epw_weather_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/weather/helpers/weather.py` & `cerc_hub-0.2.0.1/hub/imports/weather/helpers/weather.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/imports/weather_factory.py` & `cerc_hub-0.2.0.1/hub/imports/weather_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/configuration.py` & `cerc_hub-0.2.0.1/hub/persistence/configuration.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/db_control.py` & `cerc_hub-0.2.0.1/hub/persistence/db_control.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/db_setup.py` & `cerc_hub-0.2.0.1/hub/persistence/db_setup.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/models/application.py` & `cerc_hub-0.2.0.1/hub/persistence/models/application.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/models/city.py` & `cerc_hub-0.2.0.1/hub/persistence/models/city.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/models/city_object.py` & `cerc_hub-0.2.0.1/hub/persistence/models/city_object.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/models/simulation_results.py` & `cerc_hub-0.2.0.1/hub/persistence/models/simulation_results.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/models/user.py` & `cerc_hub-0.2.0.1/hub/persistence/models/user.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/repositories/application.py` & `cerc_hub-0.2.0.1/hub/persistence/repositories/application.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/repositories/city.py` & `cerc_hub-0.2.0.1/hub/persistence/repositories/city.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/repositories/city_object.py` & `cerc_hub-0.2.0.1/hub/persistence/repositories/city_object.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/repositories/simulation_results.py` & `cerc_hub-0.2.0.1/hub/persistence/repositories/simulation_results.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/repositories/user.py` & `cerc_hub-0.2.0.1/hub/persistence/repositories/user.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/hub/persistence/repository.py` & `cerc_hub-0.2.0.1/hub/persistence/repository.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/setup.py` & `cerc_hub-0.2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_city_merge.py` & `cerc_hub-0.2.0.1/tests/test_city_merge.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_construction_catalog.py` & `cerc_hub-0.2.0.1/tests/test_construction_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_construction_factory.py` & `cerc_hub-0.2.0.1/tests/test_construction_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_costs_catalog.py` & `cerc_hub-0.2.0.1/tests/test_costs_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_custom_insel_block.py` & `cerc_hub-0.2.0.1/tests/test_custom_insel_block.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_db_factory.py` & `cerc_hub-0.2.0.1/tests/test_db_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_db_retrieve.py` & `cerc_hub-0.2.0.1/tests/test_db_retrieve.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_enrichement.py` & `cerc_hub-0.2.0.1/tests/test_enrichement.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_exports.py` & `cerc_hub-0.2.0.1/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_geometry_factory.py` & `cerc_hub-0.2.0.1/tests/test_geometry_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_greenery_catalog.py` & `cerc_hub-0.2.0.1/tests/test_greenery_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_greenery_in_idf.py` & `cerc_hub-0.2.0.1/tests/test_greenery_in_idf.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_insel_exports.py` & `cerc_hub-0.2.0.1/tests/test_insel_exports.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_results_import.py` & `cerc_hub-0.2.0.1/tests/test_results_import.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_systems_catalog.py` & `cerc_hub-0.2.0.1/tests/test_systems_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_systems_factory.py` & `cerc_hub-0.2.0.1/tests/test_systems_factory.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_usage_catalog.py` & `cerc_hub-0.2.0.1/tests/test_usage_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc_hub-0.2.0.0/tests/test_usage_factory.py` & `cerc_hub-0.2.0.1/tests/test_usage_factory.py`

 * *Files identical despite different names*
