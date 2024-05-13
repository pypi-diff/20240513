# Comparing `tmp/cognite_neat-0.76.3.tar.gz` & `tmp/cognite_neat-0.77.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.76.3.tar", max compression
+gzip compressed data, was "cognite_neat-0.77.0.tar", max compression
```

## Comparing `cognite_neat-0.76.3.tar` & `cognite_neat-0.77.0.tar`

### file list

```diff
@@ -1,277 +1,277 @@
--rw-r--r--   0        0        0    11351 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/LICENSE
--rw-r--r--   0        0        0     6775 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/README.md
--rw-r--r--   0        0        0       61 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4232 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     1675 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      585 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3523 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4597 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13686 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     8121 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12393 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0    10756 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
--rw-r--r--   0        0        0     8374 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
--rw-r--r--   0        0        0     5333 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
--rw-r--r--   0        0        0      629 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-05-10 13:52:00.040956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-05-10 13:52:00.040956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-05-10 13:52:00.040956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-05-10 13:52:00.040956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-05-10 13:52:00.040956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1423717 2024-05-10 13:52:00.044956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
--rw-r--r--   0        0        0     2667 2024-05-10 13:52:00.044956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
--rw-r--r--   0        0        0  6282875 2024-05-10 13:52:00.072956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
--rw-r--r--   0        0        0   240334 2024-05-10 13:52:00.072956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     6145 2024-05-10 13:52:00.080956 cognite_neat-0.76.3/cognite/neat/config.py
--rw-r--r--   0        0        0     1300 2024-05-10 13:52:00.080956 cognite_neat-0.76.3/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-05-10 13:52:00.080956 cognite_neat-0.76.3/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-05-10 13:52:00.080956 cognite_neat-0.76.3/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-10 13:52:00.084956 cognite_neat-0.76.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-10 13:52:00.084956 cognite_neat-0.76.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-10 13:52:00.084956 cognite_neat-0.76.3/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14961 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      149 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    13473 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/legacy/__init__.py
--rw-r--r--   0        0        0       73 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/legacy/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/__init__.py
--rw-r--r--   0        0        0      363 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_base.py
--rw-r--r--   0        0        0    11734 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_dexpi.py
--rw-r--r--   0        0        0    17695 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14908 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      701 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/__init__.py
--rw-r--r--   0        0        0    23823 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/_asset_loader.py
--rw-r--r--   0        0        0     2383 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/_base.py
--rw-r--r--   0        0        0     2835 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/_exceptions.py
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/__init__.py
--rw-r--r--   0        0        0     2321 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/labels.py
--rw-r--r--   0        0        0     5023 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/models.py
--rw-r--r--   0        0        0    40464 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22707 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12979 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
--rw-r--r--   0        0        0     3328 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/validator.py
--rw-r--r--   0        0        0      149 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/__init__.py
--rw-r--r--   0        0        0    14289 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/__init__.py
--rw-r--r--   0        0        0     4765 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
--rw-r--r--   0        0        0    18719 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
--rw-r--r--   0        0        0    14737 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/transformer.py
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/__init__.py
--rw-r--r--   0        0        0     8610 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/__init__.py
--rw-r--r--   0        0        0     2598 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5567 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_base.py
--rw-r--r--   0        0        0      102 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_core/__init__.py
--rw-r--r--   0        0        0      771 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
--rw-r--r--   0        0        0    36813 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     8312 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0     6251 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2graphql.py
--rw-r--r--   0        0        0    18458 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0    28805 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3881 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2rules.py
--rw-r--r--   0        0        0     1085 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2triples.py
--rw-r--r--   0        0        0     5767 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/__init__.py
--rw-r--r--   0        0        0     2273 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_base.py
--rw-r--r--   0        0        0     6476 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_dict2rules.py
--rw-r--r--   0        0        0     7697 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0    12093 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_json2rules.py
--rw-r--r--   0        0        0       63 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9407 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10557 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1502 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0      421 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_xsd2rules.py
--rw-r--r--   0        0        0     1601 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      127 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/_base.py
--rw-r--r--   0        0        0    12382 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7351 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51091 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/tables.py
--rw-r--r--   0        0        0     4402 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/value_types.py
--rw-r--r--   0        0        0     1898 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0      170 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0      115 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/rules/analysis/__init__.py
--rw-r--r--   0        0        0      669 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/rules/analysis/_base.py
--rw-r--r--   0        0        0    19584 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/analysis/_information_rules.py
--rw-r--r--   0        0        0      374 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0    65934 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      413 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1511 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1976 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    13529 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0    14934 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    20120 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3026 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4078 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      408 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4274 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0    16891 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12663 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6717 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11897 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7591 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7786 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7437 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     6925 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    11882 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4275 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     6438 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    22035 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     5748 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3385 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0    12288 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13936 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0      782 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/__init__.py
--rw-r--r--   0        0        0    10876 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/_base.py
--rw-r--r--   0        0        0    11030 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/_rdfpath.py
--rw-r--r--   0        0        0      305 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/_types/__init__.py
--rw-r--r--   0        0        0      929 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/_types/_base.py
--rw-r--r--   0        0        0     3197 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/_types/_field.py
--rw-r--r--   0        0        0     6078 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/data_types.py
--rw-r--r--   0        0        0      491 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/__init__.py
--rw-r--r--   0        0        0     5706 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_converter.py
--rw-r--r--   0        0        0    18908 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_exporter.py
--rw-r--r--   0        0        0    15599 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_rules.py
--rw-r--r--   0        0        0    13620 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_rules_input.py
--rw-r--r--   0        0        0    37463 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_schema.py
--rw-r--r--   0        0        0     6668 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_serializer.py
--rw-r--r--   0        0        0    14290 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_validation.py
--rw-r--r--   0        0        0     2993 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/domain.py
--rw-r--r--   0        0        0    16395 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/entities.py
--rw-r--r--   0        0        0      195 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/rules/models/information/__init__.py
--rw-r--r--   0        0        0     7964 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/rules/models/information/_converter.py
--rw-r--r--   0        0        0    15546 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/rules/models/information/_rules.py
--rw-r--r--   0        0        0     6154 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/rules/models/wrapped_entities.py
--rw-r--r--   0        0        0       68 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11336 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6303 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2714 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12818 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26800 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0    14102 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6570 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     3009 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0        0 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0      225 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/graph_loader.py
--rw-r--r--   0        0        0     6295 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/graph_store.py
--rw-r--r--   0        0        0    22898 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/rules_exporter.py
--rw-r--r--   0        0        0    10338 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/rules_importer.py
--rw-r--r--   0        0        0     4729 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/rules_validator.py
--rw-r--r--   0        0        0       32 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/io/__init__.py
--rw-r--r--   0        0        0    16874 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/io/io_steps.py
--rw-r--r--   0        0        0      274 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/__init__.py
--rw-r--r--   0        0        0     3919 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
--rw-r--r--   0        0        0    29357 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
--rw-r--r--   0        0        0    27265 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
--rw-r--r--   0        0        0    12704 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_store.py
--rw-r--r--   0        0        0     2351 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
--rw-r--r--   0        0        0    20462 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
--rw-r--r--   0        0        0    28065 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
--rw-r--r--   0        0        0     2943 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    11007 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4591 2024-05-10 13:52:00.492955 cognite_neat-0.76.3/pyproject.toml
--rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.76.3/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/LICENSE
+-rw-r--r--   0        0        0     6775 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/README.md
+-rw-r--r--   0        0        0       61 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4232 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     1675 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      585 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3523 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4597 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13686 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     8121 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12393 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0    10756 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
+-rw-r--r--   0        0        0     8374 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
+-rw-r--r--   0        0        0     5333 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
+-rw-r--r--   0        0        0      629 2024-05-13 12:04:56.620933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-05-13 12:04:56.624934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-05-13 12:04:56.624934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-13 12:04:56.624934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-05-13 12:04:56.624934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-05-13 12:04:56.624934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1423717 2024-05-13 12:04:56.628934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
+-rw-r--r--   0        0        0     2667 2024-05-13 12:04:56.628934 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
+-rw-r--r--   0        0        0  6282875 2024-05-13 12:04:56.652933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
+-rw-r--r--   0        0        0   240334 2024-05-13 12:04:56.656933 cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     6145 2024-05-13 12:04:56.664934 cognite_neat-0.77.0/cognite/neat/config.py
+-rw-r--r--   0        0        0     1300 2024-05-13 12:04:56.664934 cognite_neat-0.77.0/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-05-13 12:04:56.664934 cognite_neat-0.77.0/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-05-13 12:04:56.664934 cognite_neat-0.77.0/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-13 12:04:56.664934 cognite_neat-0.77.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-13 12:04:56.668933 cognite_neat-0.77.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-13 12:04:56.668933 cognite_neat-0.77.0/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-13 12:04:56.668933 cognite_neat-0.77.0/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-05-13 12:04:56.668933 cognite_neat-0.77.0/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14961 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      149 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    13473 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/legacy/__init__.py
+-rw-r--r--   0        0        0       73 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/legacy/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-13 12:04:56.672933 cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      363 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_base.py
+-rw-r--r--   0        0        0    11734 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_dexpi.py
+-rw-r--r--   0        0        0    17695 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14908 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      701 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/__init__.py
+-rw-r--r--   0        0        0    23823 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/_asset_loader.py
+-rw-r--r--   0        0        0     2383 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/_base.py
+-rw-r--r--   0        0        0     2835 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2321 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5023 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    40464 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22707 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12979 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
+-rw-r--r--   0        0        0     3328 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/validator.py
+-rw-r--r--   0        0        0      149 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14289 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/__init__.py
+-rw-r--r--   0        0        0     4765 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0    18719 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    14737 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/__init__.py
+-rw-r--r--   0        0        0     8610 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-05-13 12:04:56.676934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_base.py
+-rw-r--r--   0        0        0      102 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_core/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
+-rw-r--r--   0        0        0    36813 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     8312 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0     6251 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2graphql.py
+-rw-r--r--   0        0        0    18458 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0    28805 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3881 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2rules.py
+-rw-r--r--   0        0        0     1085 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2triples.py
+-rw-r--r--   0        0        0     5767 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/__init__.py
+-rw-r--r--   0        0        0     2273 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_base.py
+-rw-r--r--   0        0        0     6476 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_dict2rules.py
+-rw-r--r--   0        0        0     7697 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0    12093 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9407 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10557 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1502 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      421 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_xsd2rules.py
+-rw-r--r--   0        0        0     1601 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      127 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/_base.py
+-rw-r--r--   0        0        0    12382 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7351 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51091 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/tables.py
+-rw-r--r--   0        0        0     4402 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/rules/models/value_types.py
+-rw-r--r--   0        0        0     1898 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0      170 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0      115 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/rules/analysis/__init__.py
+-rw-r--r--   0        0        0      669 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/rules/analysis/_base.py
+-rw-r--r--   0        0        0    19584 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/rules/analysis/_information_rules.py
+-rw-r--r--   0        0        0      374 2024-05-13 12:04:56.680934 cognite_neat-0.77.0/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    65934 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      413 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1511 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1976 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    13530 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    14934 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    20120 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3026 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4078 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      408 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4274 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    18317 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12663 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6717 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11897 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7591 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7786 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7437 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     6925 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    11882 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4275 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6438 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    22035 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     5748 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3385 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0    12288 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13936 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0      782 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/__init__.py
+-rw-r--r--   0        0        0    10876 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/_base.py
+-rw-r--r--   0        0        0    11030 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/_rdfpath.py
+-rw-r--r--   0        0        0      305 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/_types/__init__.py
+-rw-r--r--   0        0        0      929 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/_types/_base.py
+-rw-r--r--   0        0        0     3197 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/_types/_field.py
+-rw-r--r--   0        0        0     6078 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/data_types.py
+-rw-r--r--   0        0        0      491 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/__init__.py
+-rw-r--r--   0        0        0     5706 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_converter.py
+-rw-r--r--   0        0        0    18809 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_exporter.py
+-rw-r--r--   0        0        0    15545 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_rules.py
+-rw-r--r--   0        0        0    13620 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_rules_input.py
+-rw-r--r--   0        0        0    41719 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_schema.py
+-rw-r--r--   0        0        0     6668 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_serializer.py
+-rw-r--r--   0        0        0    14273 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/dms/_validation.py
+-rw-r--r--   0        0        0     2993 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/domain.py
+-rw-r--r--   0        0        0    16395 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/entities.py
+-rw-r--r--   0        0        0      195 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/information/__init__.py
+-rw-r--r--   0        0        0     7964 2024-05-13 12:04:56.684934 cognite_neat-0.77.0/cognite/neat/rules/models/information/_converter.py
+-rw-r--r--   0        0        0    15546 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/rules/models/information/_rules.py
+-rw-r--r--   0        0        0     6154 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/rules/models/wrapped_entities.py
+-rw-r--r--   0        0        0       68 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11336 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6303 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2714 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12818 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26800 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0    14102 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6570 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     3009 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/graph_loader.py
+-rw-r--r--   0        0        0     6295 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/graph_store.py
+-rw-r--r--   0        0        0    22898 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/rules_exporter.py
+-rw-r--r--   0        0        0    10338 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/rules_importer.py
+-rw-r--r--   0        0        0     4729 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/rules_validator.py
+-rw-r--r--   0        0        0       32 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/io/__init__.py
+-rw-r--r--   0        0        0    16874 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/io/io_steps.py
+-rw-r--r--   0        0        0      274 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/__init__.py
+-rw-r--r--   0        0        0     3919 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
+-rw-r--r--   0        0        0    29357 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
+-rw-r--r--   0        0        0    27265 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
+-rw-r--r--   0        0        0    12704 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_store.py
+-rw-r--r--   0        0        0     2351 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
+-rw-r--r--   0        0        0    20462 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
+-rw-r--r--   0        0        0    28065 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
+-rw-r--r--   0        0        0     2943 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    11007 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-05-13 12:04:56.688933 cognite_neat-0.77.0/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4591 2024-05-13 12:04:57.080934 cognite_neat-0.77.0/pyproject.toml
+-rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.77.0/PKG-INFO
```

### Comparing `cognite_neat-0.76.3/LICENSE` & `cognite_neat-0.77.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/README.md` & `cognite_neat-0.77.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/api/configuration.py` & `cognite_neat-0.77.0/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.77.0/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/api/explorer.py` & `cognite_neat-0.77.0/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.77.0/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.77.0/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.77.0/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.77.0/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.77.0/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.77.0/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.77.0/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.77.0/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.77.0/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.77.0/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg` & `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg` & `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg` & `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js` & `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt` & `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map` & `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.77.0/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/config.py` & `cognite_neat-0.77.0/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/constants.py` & `cognite_neat-0.77.0/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/exceptions.py` & `cognite_neat-0.77.0/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.77.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.77.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.77.0/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/graph/exceptions.py` & `cognite_neat-0.77.0/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.77.0/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.77.0/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.77.0/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.77.0/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.77.0/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.77.0/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.77.0/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.77.0/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/exceptions.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_dexpi.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/__init__.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/_asset_loader.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/_base.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/_exceptions.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/labels.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/models.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/rdf_to_dms.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/validator.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/__init__.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_base.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_graphdb_store.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_memory_store.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_oxigraph_store.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_oxrdflib.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/entity_matcher.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/query_generator/sparql.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/transformer.py` & `cognite_neat-0.77.0/cognite/neat/legacy/graph/transformations/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/analysis.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/__init__.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/power-grid-model.yaml` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/rules-template.xlsx` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/skos-rules.xlsx` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/wind-energy.owl` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/exceptions.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/__init__.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_base.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_core/rules2labels.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2dms.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2excel.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2graphql.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2ontology.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2rules.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2triples.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_validation.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/__init__.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_base.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_dict2rules.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_dms2rules.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_graph2rules.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_json2rules.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_yaml2rules.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/models/_base.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/models/raw_rules.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/models/rdfpath.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/models/rules.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/rules/models/value_types.py` & `cognite_neat-0.77.0/cognite/neat/legacy/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/analysis/_base.py` & `cognite_neat-0.77.0/cognite/neat/rules/analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/analysis/_information_rules.py` & `cognite_neat-0.77.0/cognite/neat/rules/analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.77.0/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/exceptions.py` & `cognite_neat-0.77.0/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.77.0/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.77.0/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import warnings
 from collections.abc import Collection, Iterable
 from pathlib import Path
 from typing import Literal, TypeAlias, cast
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes._base import CogniteResource, CogniteResourceList
-from cognite.client.data_classes.data_modeling import DataModelApply, DataModelId
+from cognite.client.data_classes.data_modeling import DataModelApply, DataModelApplyList, DataModelId
 from cognite.client.exceptions import CogniteAPIError
 
 from cognite.neat.rules import issues
 from cognite.neat.rules._shared import Rules
 from cognite.neat.rules.issues import IssueList
 from cognite.neat.rules.models import InformationRules
 from cognite.neat.rules.models.dms import DMSRules, DMSSchema, PipelineSchema
@@ -110,17 +110,15 @@
     def export(self, rules: Rules) -> DMSSchema:
         if isinstance(rules, DMSRules):
             dms_rules = rules
         elif isinstance(rules, InformationRules):
             dms_rules = rules.as_dms_architect_rules()
         else:
             raise ValueError(f"{type(rules).__name__} cannot be exported to DMS")
-        return dms_rules.as_schema(
-            include_ref=True, include_pipeline=self.export_pipeline, instance_space=self.instance_space
-        )
+        return dms_rules.as_schema(include_pipeline=self.export_pipeline, instance_space=self.instance_space)
 
     def delete_from_cdf(self, rules: Rules, client: CogniteClient, dry_run: bool = False) -> Iterable[UploadResult]:
         schema, to_export = self._prepare_schema_and_exporters(rules, client)
 
         # we need to reverse order in which we are picking up the items to delete
         # as they are sorted in the order of creation and we need to delete them in reverse order
         for all_items, loader in reversed(to_export):
@@ -268,15 +266,15 @@
         if self.export_components.intersection({"all", "spaces"}):
             to_export.append((schema.spaces, SpaceLoader(client)))
         if self.export_components.intersection({"all", "containers"}):
             to_export.append((schema.containers, ContainerLoader(client)))
         if self.export_components.intersection({"all", "views"}):
             to_export.append((schema.views, ViewLoader(client, self.existing_handling)))
         if self.export_components.intersection({"all", "data_models"}):
-            to_export.append((schema.data_models, DataModelLoader(client)))
+            to_export.append((DataModelApplyList([schema.data_model]), DataModelLoader(client)))
         if isinstance(schema, PipelineSchema):
             to_export.append((schema.databases, RawDatabaseLoader(client)))
             to_export.append((schema.raw_tables, RawTableLoader(client)))
             to_export.append((schema.transformations, TransformationLoader(client)))
         return schema, to_export
 
     def _validate(self, loader: ResourceLoader, items: list[CogniteResource]) -> IssueList:
```

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.77.0/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.77.0/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.77.0/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.77.0/cognite/neat/rules/importers/_dms2rules.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections.abc import Sequence
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Literal, cast, overload
 
 from cognite.client import CogniteClient
 from cognite.client import data_modeling as dm
-from cognite.client.data_classes.data_modeling import DataModelIdentifier
+from cognite.client.data_classes.data_modeling import DataModelId, DataModelIdentifier
 from cognite.client.data_classes.data_modeling.containers import BTreeIndex, InvertedIndex
 from cognite.client.data_classes.data_modeling.views import (
     MultiEdgeConnectionApply,
     MultiReverseDirectRelationApply,
     SingleEdgeConnectionApply,
     SingleReverseDirectRelationApply,
     ViewPropertyApply,
@@ -35,86 +35,123 @@
     DMSMetadata,
     DMSProperty,
     DMSView,
 )
 from cognite.neat.rules.models.entities import (
     ClassEntity,
     ContainerEntity,
-    DataModelEntity,
     DMSUnknownEntity,
     ViewEntity,
     ViewPropertyEntity,
 )
 
 
 class DMSImporter(BaseImporter):
     def __init__(
         self,
         schema: DMSSchema,
         read_issues: Sequence[ValidationIssue] | None = None,
         metadata: DMSMetadata | None = None,
+        ref_metadata: DMSMetadata | None = None,
     ):
         # Calling this root schema to distinguish it from
         # * User Schema
         # * Reference Schema
         self.root_schema = schema
         self.metadata = metadata
+        self.ref_metadata = ref_metadata
         self.issue_list = IssueList(read_issues)
         self._all_containers_by_id = {container.as_id(): container for container in schema.containers}
         if self.root_schema.reference:
             self._all_containers_by_id.update(
                 {container.as_id(): container for container in self.root_schema.reference.containers}
             )
 
     @classmethod
-    def from_data_model_id(cls, client: CogniteClient, data_model_id: DataModelIdentifier) -> "DMSImporter":
+    def from_data_model_id(
+        cls,
+        client: CogniteClient,
+        data_model_id: DataModelIdentifier,
+        reference_model_id: DataModelIdentifier | None = None,
+    ) -> "DMSImporter":
         """Create a DMSImporter ready to convert the given data model to rules.
 
         Args:
             client: Instantiated CogniteClient to retrieve data model.
+            reference_model_id: The reference data model to retrieve. This is the data model that
+                the given data model is built on top of, typically, an enterprise data model.
             data_model_id: Data Model to retrieve.
 
         Returns:
             DMSImporter: DMSImporter instance
         """
-        data_models = client.data_modeling.data_models.retrieve(data_model_id, inline_views=True)
-        if len(data_models) == 0:
+        data_model_ids = [data_model_id, reference_model_id] if reference_model_id else [data_model_id]
+        data_models = client.data_modeling.data_models.retrieve(data_model_ids, inline_views=True)
+
+        user_models = cls._find_model_in_list(data_models, data_model_id)
+        if len(user_models) == 0:
             return cls(DMSSchema(), [issues.importing.NoDataModelError(f"Data model {data_model_id} not found")])
-        data_model = data_models.latest_version()
+        user_model = user_models.latest_version()
+
+        if reference_model_id:
+            ref_models = cls._find_model_in_list(data_models, reference_model_id)
+            if len(ref_models) == 0:
+                return cls(
+                    DMSSchema(), [issues.importing.NoDataModelError(f"Data model {reference_model_id} not found")]
+                )
+            ref_model: dm.DataModel[dm.View] | None = ref_models.latest_version()
+        else:
+            ref_model = None
 
         try:
-            schema = DMSSchema.from_data_model(client, data_model)
+            schema = DMSSchema.from_data_model(client, user_model, ref_model)
         except Exception as e:
             return cls(DMSSchema(), [issues.importing.APIError(str(e))])
 
-        created = ms_to_datetime(data_model.created_time)
-        updated = ms_to_datetime(data_model.last_updated_time)
+        metadata = cls._create_metadata_from_model(user_model)
+        ref_metadata = cls._create_metadata_from_model(ref_model) if ref_model else None
 
-        metadata = cls._create_metadata_from_model(data_model, created, updated)
+        return cls(schema, [], metadata, ref_metadata)
 
-        return cls(schema, [], metadata)
+    @classmethod
+    def _find_model_in_list(
+        cls, data_models: dm.DataModelList[dm.View], model_id: DataModelIdentifier
+    ) -> dm.DataModelList[dm.View]:
+        identifier = DataModelId.load(model_id)
+        return dm.DataModelList[dm.View](
+            [
+                model
+                for model in data_models
+                if (model.space, model.external_id) == (identifier.space, identifier.external_id)
+            ]
+        )
 
     @classmethod
     def _create_metadata_from_model(
         cls,
         model: dm.DataModel[dm.View] | dm.DataModelApply,
-        created: datetime | None = None,
-        updated: datetime | None = None,
     ) -> DMSMetadata:
         description, creator = DMSMetadata._get_description_and_creator(model.description)
-        now = datetime.now().replace(microsecond=0)
+
+        if isinstance(model, dm.DataModel):
+            created = ms_to_datetime(model.created_time)
+            updated = ms_to_datetime(model.last_updated_time)
+        else:
+            now = datetime.now().replace(microsecond=0)
+            created = now
+            updated = now
         return DMSMetadata(
             schema_=SchemaCompleteness.complete,
             extension=ExtensionCategory.addition,
             space=model.space,
             external_id=model.external_id,
             name=model.name or model.external_id,
             version=model.version or "0.1.0",
-            updated=updated or now,
-            created=created or now,
+            updated=updated,
+            created=created,
             creator=creator,
             description=description,
         )
 
     @classmethod
     def from_directory(cls, directory: str | Path) -> "DMSImporter":
         issue_list = IssueList()
@@ -143,61 +180,57 @@
     def to_rules(
         self, errors: Literal["raise", "continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList] | Rules:
         if self.issue_list.has_errors:
             # In case there were errors during the import, the to_rules method will return None
             return self._return_or_raise(self.issue_list, errors)
 
-        if len(self.root_schema.data_models) == 0:
+        if not self.root_schema.data_model:
             self.issue_list.append(issues.importing.NoDataModelError("No data model found."))
             return self._return_or_raise(self.issue_list, errors)
-
+        model = self.root_schema.data_model
         with _handle_issues(
             self.issue_list,
         ) as future:
             schema_completeness = SchemaCompleteness.complete
             data_model_type = DataModelType.enterprise
             reference: DMSRules | None = None
-            if ref_schema := self.root_schema.reference:
+            if (ref_schema := self.root_schema.reference) and (ref_model := ref_schema.data_model):
                 # Reference should always be an enterprise model.
                 reference = DMSRules(
                     **self._create_rule_components(
-                        ref_schema, self._create_default_metadata(ref_schema.views), DataModelType.enterprise
+                        ref_model,
+                        ref_schema,
+                        self.ref_metadata or self._create_default_metadata(ref_schema.views),
+                        DataModelType.enterprise,
                     )
                 )
                 schema_completeness = SchemaCompleteness.extended
                 data_model_type = DataModelType.solution
 
             user_rules = DMSRules(
-                **self._create_rule_components(self.root_schema, self.metadata, data_model_type, schema_completeness),
+                **self._create_rule_components(
+                    model, self.root_schema, self.metadata, data_model_type, schema_completeness
+                ),
                 reference=reference,
             )
 
         if future.result == "failure" or self.issue_list.has_errors:
             return self._return_or_raise(self.issue_list, errors)
 
         return self._to_output(user_rules, self.issue_list, errors, role)
 
     def _create_rule_components(
         self,
+        data_model: dm.DataModelApply,
         schema: DMSSchema,
         metadata: DMSMetadata | None = None,
         data_model_type: DataModelType | None = None,
         schema_completeness: SchemaCompleteness | None = None,
     ) -> dict[str, Any]:
-        if len(schema.data_models) > 2:
-            # Creating a DataModelEntity to convert the data model id to a string.
-            self.issue_list.append(
-                issues.importing.MultipleDataModelsWarning(
-                    [str(DataModelEntity.from_id(model.as_id())) for model in schema.data_models]
-                )
-            )
-
-        data_model = schema.data_models[0]
-
         properties = SheetList[DMSProperty]()
         for view in schema.views:
             view_id = view.as_id()
             view_entity = ViewEntity.from_id(view_id)
             class_entity = view_entity.as_class()
             for prop_id, prop in (view.properties or {}).items():
                 dms_property = self._create_dms_property(prop_id, prop, view_entity, class_entity)
```

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.77.0/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.77.0/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.77.0/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.77.0/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.77.0/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/issues/base.py` & `cognite_neat-0.77.0/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.77.0/cognite/neat/rules/issues/dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.77.0/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.77.0/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.77.0/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.77.0/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.77.0/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/__init__.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/_base.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/_rdfpath.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/_rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/_types/_base.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/_types/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/_types/_field.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/data_types.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_converter.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_exporter.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,17 @@
             raw tables and transformations necessary to populate the data model.
         instance_space (str): The space to use for the instance. Defaults to None,`Rules.metadata.space` will be used
     """
 
     def __init__(
         self,
         rules: DMSRules,
-        include_ref: bool = True,
         include_pipeline: bool = False,
         instance_space: str | None = None,
     ):
-        self.include_ref = include_ref
         self.include_pipeline = include_pipeline
         self.instance_space = instance_space
         self.rules = rules
         self._ref_schema = rules.reference.as_schema() if rules.reference else None
         if self._ref_schema:
             # We skip version as that will always be missing in the reference
             self._ref_views_by_id = {dm.ViewId(view.space, view.external_id): view for view in self._ref_schema.views}
@@ -71,15 +69,15 @@
             key=lambda v: v.as_tuple(),  # type: ignore[union-attr]
         )
 
         spaces = self._create_spaces(rules.metadata, containers, views, data_model)
 
         output = DMSSchema(
             spaces=spaces,
-            data_models=dm.DataModelApplyList([data_model]),
+            data_model=data_model,
             views=views,
             containers=containers,
             node_types=node_types,
         )
         if self.include_pipeline:
             return PipelineSchema.from_dms(output, self.instance_space)
```

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_rules.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,20 +341,18 @@
     ) -> dict[str, Any]:
         from ._serializer import _DMSRulesSerializer
 
         dumped = cast(dict[str, Any], handler(self, info))
         space, version = self.metadata.space, self.metadata.version
         return _DMSRulesSerializer(info, space, version).clean(dumped)
 
-    def as_schema(
-        self, include_ref: bool = False, include_pipeline: bool = False, instance_space: str | None = None
-    ) -> DMSSchema:
+    def as_schema(self, include_pipeline: bool = False, instance_space: str | None = None) -> DMSSchema:
         from ._exporter import _DMSExporter
 
-        return _DMSExporter(self, include_ref, include_pipeline, instance_space).to_schema()
+        return _DMSExporter(self, include_pipeline, instance_space).to_schema()
 
     def as_information_architect_rules(self) -> "InformationRules":
         from ._converter import _DMSRulesConverter
 
         return _DMSRulesConverter(self).as_information_architect_rules()
 
     def as_domain_expert_rules(self) -> DomainRules:
```

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_rules_input.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_rules_input.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_schema.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import sys
 import warnings
 import zipfile
 from collections import Counter, defaultdict
+from collections.abc import Sequence
 from dataclasses import Field, dataclass, field, fields
 from pathlib import Path
 from typing import Any, ClassVar, cast
 
 import yaml
 from cognite.client import CogniteClient
 from cognite.client import data_modeling as dm
@@ -39,29 +40,29 @@
     from typing import Self
 else:
     from typing_extensions import Self
 
 
 @dataclass
 class DMSSchema:
-    data_models: dm.DataModelApplyList = field(default_factory=lambda: dm.DataModelApplyList([]))
+    data_model: dm.DataModelApply | None = None
     spaces: dm.SpaceApplyList = field(default_factory=lambda: dm.SpaceApplyList([]))
     views: dm.ViewApplyList = field(default_factory=lambda: dm.ViewApplyList([]))
     containers: dm.ContainerApplyList = field(default_factory=lambda: dm.ContainerApplyList([]))
     node_types: dm.NodeApplyList = field(default_factory=lambda: dm.NodeApplyList([]))
-    # The last schema is the previous version of the data model. In the case, extension=additio, this
+    # The last schema is the previous version of the data model. In the case, extension=addition, this
     # should not be modified.
     last: "DMSSchema | None" = None
     # Reference is typically the Enterprise model, while this is the solution model.
     reference: "DMSSchema | None" = None
 
     _FIELD_NAME_BY_RESOURCE_TYPE: ClassVar[dict[str, str]] = {
         "container": "containers",
         "view": "views",
-        "datamodel": "data_models",
+        "datamodel": "data_model",
         "space": "spaces",
         "node": "node_types",
     }
 
     def _get_mapped_container_from_view(self, view_id: dm.ViewId) -> set[dm.ContainerId]:
         # index all views, including ones from reference
         indexed_views = {
@@ -91,45 +92,106 @@
         data_models = client.data_modeling.data_models.retrieve(data_model_id, inline_views=True)
         if len(data_models) == 0:
             raise ValueError(f"Data model {data_model_id} not found")
         data_model = data_models.latest_version()
         return cls.from_data_model(client, data_model)
 
     @classmethod
-    def from_data_model(cls, client: CogniteClient, data_model: dm.DataModel) -> "DMSSchema":
+    def from_data_model(
+        cls,
+        client: CogniteClient,
+        data_model: dm.DataModel[dm.View],
+        reference_model: dm.DataModel[dm.View] | None = None,
+    ) -> "DMSSchema":
+        """Create a schema from a data model.
+
+        If a reference model is provided, the schema will include a reference schema. To determine which views,
+        and containers to put in the reference schema, the following rule is applied:
+
+            If a view or container space is different from the data model space,
+            it will be included in the reference schema.*
+
+        *One exception to this rule is if a view is directly referenced by the data model. In this case, the view will
+        be included in the data model schema, even if the space is different.
+
+        Args:
+            client: The Cognite client used for retrieving components referenced by the data model.
+            data_model: The data model to create the schema from.
+            reference_model: (Optional) The reference model to include in the schema.
+                This is typically the Enterprise model.
+
+        Returns:
+            DMSSchema: The schema created from the data model.
+        """
         views = dm.ViewList(data_model.views)
+
+        data_model_write = data_model.as_write()
+        data_model_write.views = list(views.as_ids())
+
+        if reference_model:
+            views.extend(reference_model.views)
+
         container_ids = views.referenced_containers()
         containers = client.data_modeling.containers.retrieve(list(container_ids))
         cls._append_referenced_containers(client, containers)
 
-        space_read = client.data_modeling.spaces.retrieve(data_model.space)
-        if space_read is None:
-            raise ValueError(f"Space {data_model.space} not found")
-        space = space_read.as_write()
-        data_model_write = data_model.as_write()
-        data_model_write.views = list(views.as_write())
+        space_ids = [data_model.space, reference_model.space] if reference_model else [data_model.space]
+        space_read = client.data_modeling.spaces.retrieve(space_ids)
+        if len(space_read) != len(space_ids):
+            raise ValueError(f"Space(s) {space_read} not found")
+        space_write = space_read.as_write()
 
         view_loader = ViewLoader(client)
         # We need to include parent views in the schema to make sure that the schema is valid.
         existing_view_ids = set(views.as_ids())
         parent_view_ids = {parent for view in views for parent in view.implements or []}
         parents = view_loader.retrieve_all_parents(list(parent_view_ids - existing_view_ids))
         views.extend([parent for parent in parents if parent.as_id() not in existing_view_ids])
 
         # Converting views from read to write format requires to account for parents (implements)
         # as the read format contains all properties from all parents, while the write formate should not contain
         # properties from any parents.
         # The ViewLoader as_write method looks up parents and remove properties from them.
         view_write = dm.ViewApplyList([view_loader.as_write(view) for view in views])
 
+        container_write = containers.as_write()
+        user_space = data_model.space
+        if reference_model:
+            user_model_view_ids = set(data_model_write.views)
+            ref_model_write = reference_model.as_write()
+            ref_model_write.views = [view.as_id() for view in reference_model.views]
+
+            ref_views = dm.ViewApplyList(
+                [view for view in view_write if (view.space != user_space) or (view.as_id() not in user_model_view_ids)]
+            )
+            view_write = dm.ViewApplyList(
+                [view for view in view_write if view.space == user_space or view.as_id() in user_model_view_ids]
+            )
+
+            ref_containers = dm.ContainerApplyList(
+                [container for container in container_write if container.space != user_space]
+            )
+            container_write = dm.ContainerApplyList(
+                [container for container in container_write if container.space == user_space]
+            )
+
+            ref_schema: DMSSchema | None = cls(
+                spaces=dm.SpaceApplyList([s for s in space_write if s.space != user_space]),
+                data_model=ref_model_write,
+                views=ref_views,
+                containers=ref_containers,
+            )
+        else:
+            ref_schema = None
         return cls(
-            spaces=dm.SpaceApplyList([space]),
-            data_models=dm.DataModelApplyList([data_model_write]),
+            spaces=dm.SpaceApplyList([s for s in space_write if s.space == user_space]),
+            data_model=data_model_write,
             views=view_write,
-            containers=containers.as_write(),
+            containers=container_write,
+            reference=ref_schema,
         )
 
     @classmethod
     def from_directory(cls, directory: str | Path) -> Self:
         """Load a schema from a directory containing YAML files.
 
         The directory is expected to follow the Cognite-Toolkit convention
@@ -183,19 +245,18 @@
         data_models = path_dir / "data_models"
         data_models.mkdir(parents=True, exist_ok=True)
         if "spaces" not in exclude_set:
             for space in self.spaces:
                 (data_models / f"{space.space}.space.yaml").write_text(
                     space.dump_yaml(), newline=new_line, encoding=encoding
                 )
-        if "data_models" not in exclude_set:
-            for model in self.data_models:
-                (data_models / f"{model.external_id}.datamodel.yaml").write_text(
-                    model.dump_yaml(), newline=new_line, encoding=encoding
-                )
+        if "data_models" not in exclude_set and self.data_model:
+            (data_models / f"{self.data_model.external_id}.datamodel.yaml").write_text(
+                self.data_model.dump_yaml(), newline=new_line, encoding=encoding
+            )
         if "views" not in exclude_set and self.views:
             view_dir = data_models / "views"
             view_dir.mkdir(parents=True, exist_ok=True)
             for view in self.views:
                 (view_dir / f"{view.external_id}.view.yaml").write_text(
                     view.dump_yaml(), newline=new_line, encoding=encoding
                 )
@@ -261,17 +322,18 @@
             exclude (set[str]): A set of attributes to exclude from the output.
         """
         exclude_set = exclude or set()
         with zipfile.ZipFile(zip_file, "w") as zip_ref:
             if "spaces" not in exclude_set:
                 for space in self.spaces:
                     zip_ref.writestr(f"data_models/{space.space}.space.yaml", space.dump_yaml())
-            if "data_models" not in exclude_set:
-                for model in self.data_models:
-                    zip_ref.writestr(f"data_models/{model.external_id}.datamodel.yaml", model.dump_yaml())
+            if "data_models" not in exclude_set and self.data_model:
+                zip_ref.writestr(
+                    f"data_models/{self.data_model.external_id}.datamodel.yaml", self.data_model.dump_yaml()
+                )
             if "views" not in exclude_set:
                 for view in self.views:
                     zip_ref.writestr(f"data_models/views/{view.external_id}.view.yaml", view.dump_yaml())
             if "containers" not in exclude_set:
                 for container in self.containers:
                     zip_ref.writestr(
                         f"data_models/containers{container.external_id}.container.yaml", container.dump_yaml()
@@ -304,18 +366,38 @@
                     "dict[str, list[Any]]", f"Invalid data structure: {type(data)}"
                 ).as_exception() from None
         else:
             data_dict = data
         loaded: dict[str, Any] = {}
         for attr in fields(cls):
             if items := data_dict.get(attr.name) or data_dict.get(to_camel(attr.name)):
-                try:
-                    loaded[attr.name] = attr.type.load(items)
-                except Exception as e:
-                    loaded[attr.name] = cls._load_individual_resources(items, attr, str(e), context.get(attr.name, []))
+                if attr.name == "data_model":
+                    if isinstance(items, list) and len(items) > 1:
+                        warnings.warn(
+                            issues.importing.MultipleDataModelsWarning(
+                                [item.get("externalId", "Unknown") for item in items]
+                            ),
+                            stacklevel=2,
+                        )
+                    item = items[0] if isinstance(items, list) else items
+                    try:
+                        loaded[attr.name] = dm.DataModelApply.load(item)
+                    except Exception as e:
+                        data_model_file = context.get(attr.name, [Path("UNKNOWN")])[0]
+                        warnings.warn(
+                            issues.fileread.FailedLoadWarning(data_model_file, dm.DataModelApply.__name__, str(e)),
+                            stacklevel=2,
+                        )
+                else:
+                    try:
+                        loaded[attr.name] = attr.type.load(items)
+                    except Exception as e:
+                        loaded[attr.name] = cls._load_individual_resources(
+                            items, attr, str(e), context.get(attr.name, [])
+                        )
         return cls(**loaded)
 
     @classmethod
     def _load_individual_resources(cls, items: list, attr: Field, trigger_error: str, resource_context) -> list[Any]:
         resources = attr.type([])
         if not hasattr(attr.type, "_RESOURCE"):
             warnings.warn(
@@ -349,17 +431,20 @@
         Returns:
             dict: The schema as a dictionary.
         """
         output: dict[str, Any] = {}
         cls_fields = sorted(fields(self), key=lambda f: f.name) if sort else fields(self)
         for attr in cls_fields:
             if items := getattr(self, attr.name):
-                items = sorted(items, key=self._to_sortable_identifier) if sort else items
                 key = to_camel(attr.name) if camel_case else attr.name
-                output[key] = [item.dump(camel_case=camel_case) for item in items]
+                if isinstance(items, Sequence):
+                    items = sorted(items, key=self._to_sortable_identifier) if sort else items
+                    output[key] = [item.dump(camel_case=camel_case) for item in items]
+                else:
+                    output[key] = items.dump(camel_case=camel_case)
         return output
 
     @classmethod
     def _to_sortable_identifier(cls, item: Any) -> str | tuple[str, str] | tuple[str, str, str]:
         if isinstance(item, dm.ContainerApply | dm.ViewApply | dm.DataModelApply | dm.NodeApply | RawTableWrite):
             identifier = item.as_id().as_tuple()
             if len(identifier) == 3 and identifier[2] is None:
@@ -454,15 +539,16 @@
                         ContainerPropertyUsedMultipleTimesError(
                             container=container_id,
                             property=container_property_identifier,
                             referred_by=frozenset({(view_id, prop_name) for prop_name in view_properties}),
                         )
                     )
 
-        for model in self.data_models:
+        if self.data_model:
+            model = self.data_model
             if model.space not in defined_spaces:
                 errors.add(MissingSpaceError(space=model.space, referred_by=model.as_id()))
 
             view_counts: dict[dm.ViewId, int] = defaultdict(int)
             for view_id_or_class in model.views or []:
                 view_id = view_id_or_class if isinstance(view_id_or_class, dm.ViewId) else view_id_or_class.as_id()
                 if view_id not in defined_views:
@@ -502,24 +588,33 @@
                 "The maximum number of iterations was reached while resolving referenced containers."
                 "There might be referenced containers that are not included in the list of containers.",
                 RuntimeWarning,
                 stacklevel=2,
             )
         return None
 
-    def referenced_spaces(self) -> set[str]:
-        referenced_spaces = {container.space for container in self.containers}
-        referenced_spaces |= {view.space for view in self.views}
-        referenced_spaces |= {container.space for view in self.views for container in view.referenced_containers()}
-        referenced_spaces |= {parent.space for view in self.views for parent in view.implements or []}
+    def referenced_spaces(self, include_indirect_references: bool = True) -> set[str]:
+        """Get the spaces referenced by the schema.
+
+        Args:
+            include_indirect_references (bool): If True, the spaces referenced by as view.implements, and
+                view.referenced_containers will be included in the output.
+        Returns:
+            set[str]: The spaces referenced by the schema.
+        """
+        referenced_spaces = {view.space for view in self.views}
+        referenced_spaces |= {container.space for container in self.containers}
+        if include_indirect_references:
+            referenced_spaces |= {container.space for view in self.views for container in view.referenced_containers()}
+            referenced_spaces |= {parent.space for view in self.views for parent in view.implements or []}
         referenced_spaces |= {node.space for node in self.node_types}
-        referenced_spaces |= {model.space for model in self.data_models}
-        referenced_spaces |= {view.space for model in self.data_models for view in model.views or []}
+        if self.data_model:
+            referenced_spaces |= {self.data_model.space}
+            referenced_spaces |= {view.space for view in self.data_model.views or []}
         referenced_spaces |= {s.space for s in self.spaces}
-
         return referenced_spaces
 
 
 @dataclass
 class PipelineSchema(DMSSchema):
     transformations: TransformationWriteList = field(default_factory=lambda: TransformationWriteList([]))
     databases: DatabaseWriteList = field(default_factory=lambda: DatabaseWriteList([]))
@@ -621,17 +716,17 @@
                         else:
                             data[attr_name].append(loaded)
                             context[attr_name].append(filepath)
         return data, context
 
     @classmethod
     def from_dms(cls, schema: DMSSchema, instance_space: str | None = None) -> "PipelineSchema":
-        if not schema.data_models:
+        if not schema.data_model:
             raise ValueError("PipelineSchema must contain at least one data model")
-        first_data_model = schema.data_models[0]
+        first_data_model = schema.data_model
         # The database name is limited to 32 characters
         database_name = first_data_model.external_id[:32]
         instance_space = instance_space or first_data_model.space
         database = DatabaseWrite(name=database_name)
         parent_views = {parent for view in schema.views for parent in view.implements or []}
         container_by_id = {container.as_id(): container for container in schema.containers}
 
@@ -662,15 +757,15 @@
                 view_table = RawTableWrite(name=f"{view.external_id}.{prop_name}Edge", database=database_name)
                 raw_tables.append(view_table)
                 transformation = cls._create_edge_transformation(connection_property, view, view_table, instance_space)
                 transformations.append(transformation)
 
         return cls(
             spaces=schema.spaces,
-            data_models=schema.data_models,
+            data_model=schema.data_model,
             views=schema.views,
             containers=schema.containers,
             transformations=transformations,
             databases=DatabaseWriteList([database]),
             raw_tables=raw_tables,
         )
```

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_serializer.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_serializer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_validation.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/dms/_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         is_solution = self.metadata.space != self.rules.reference.metadata.space
         if is_solution:
             return None
         if self.metadata.extension is ExtensionCategory.rebuild:
             # Everything is allowed
             return None
         # Is an extension of an existing model.
-        user_schema = self.rules.as_schema(include_ref=False)
+        user_schema = self.rules.as_schema()
         ref_schema = self.rules.reference.as_schema()
         new_containers = {container.as_id(): container for container in user_schema.containers}
         existing_containers = {container.as_id(): container for container in ref_schema.containers}
 
         for container_id, container in new_containers.items():
             existing_container = existing_containers.get(container_id)
             if not existing_container or existing_container == container:
```

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/domain.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/domain.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/entities.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/entities.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/information/_converter.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/information/_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/information/_rules.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/information/_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/rules/models/wrapped_entities.py` & `cognite_neat-0.77.0/cognite/neat/rules/models/wrapped_entities.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/utils/cdf.py` & `cognite_neat-0.77.0/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.77.0/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/utils/exceptions.py` & `cognite_neat-0.77.0/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.77.0/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/utils/text.py` & `cognite_neat-0.77.0/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/utils/utils.py` & `cognite_neat-0.77.0/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/utils/xml.py` & `cognite_neat-0.77.0/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.77.0/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/base.py` & `cognite_neat-0.77.0/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.77.0/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.77.0/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/manager.py` & `cognite_neat-0.77.0/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.77.0/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.77.0/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/model.py` & `cognite_neat-0.77.0/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/graph_extractor.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/graph_loader.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/graph_store.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/rules_exporter.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/rules_importer.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/rules_validator.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/current/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/io/io_steps.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/io/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_loader.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_store.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/rules_importer.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/lib/legacy/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.77.0/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/tasks.py` & `cognite_neat-0.77.0/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/cognite/neat/workflows/triggers.py` & `cognite_neat-0.77.0/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.3/pyproject.toml` & `cognite_neat-0.77.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.76.3"
+version = "0.77.0"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.76.3/PKG-INFO` & `cognite_neat-0.77.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.76.3
+Version: 0.77.0
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

