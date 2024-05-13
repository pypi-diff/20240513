# Comparing `tmp/nucliadb-3.1.0.post496-py3-none-any.whl.zip` & `tmp/nucliadb-3.1.0.post497-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,457 +1,458 @@
-Zip file size: 750778 bytes, number of entries: 455
--rw-r--r--  2.0 unx     1135 b- defN 24-May-13 13:31 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-13 13:31 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-13 13:31 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-13 13:31 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-13 13:31 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-13 13:31 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-13 13:31 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-13 13:31 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-13 13:31 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-13 13:31 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-13 13:31 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-13 13:31 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-13 13:31 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-13 13:31 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-13 13:31 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-13 13:31 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-13 13:31 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-13 13:31 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-13 13:31 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-13 13:31 nucliadb/health.py
--rw-r--r--  2.0 unx    11626 b- defN 24-May-13 13:31 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-13 13:31 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-13 13:31 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 13:31 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     5022 b- defN 24-May-13 13:31 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     4971 b- defN 24-May-13 13:31 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-13 13:31 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3790 b- defN 24-May-13 13:31 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-13 13:31 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    21672 b- defN 24-May-13 13:31 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8593 b- defN 24-May-13 13:31 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    19773 b- defN 24-May-13 13:31 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     2713 b- defN 24-May-13 13:31 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5747 b- defN 24-May-13 13:31 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-13 13:31 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12518 b- defN 24-May-13 13:31 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-13 13:31 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-13 13:31 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-13 13:31 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-13 13:31 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-13 13:31 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13707 b- defN 24-May-13 13:31 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-13 13:31 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-13 13:31 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-May-13 13:31 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-May-13 13:31 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-13 13:31 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1813 b- defN 24-May-13 13:31 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-13 13:31 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-13 13:31 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-13 13:31 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-13 13:31 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-13 13:31 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-13 13:31 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx     8719 b- defN 24-May-13 13:31 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5634 b- defN 24-May-13 13:31 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-13 13:31 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-13 13:31 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-13 13:31 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-13 13:31 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-13 13:31 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-13 13:31 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-13 13:31 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-May-13 13:31 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-13 13:31 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-13 13:31 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-13 13:31 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-May-13 13:31 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4109 b- defN 24-May-13 13:31 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-13 13:31 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-13 13:31 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-13 13:31 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-13 13:31 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-13 13:31 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-13 13:31 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-13 13:31 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19401 b- defN 24-May-13 13:31 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-13 13:31 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-13 13:31 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-13 13:31 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-13 13:31 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19541 b- defN 24-May-13 13:31 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-May-13 13:31 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3183 b- defN 24-May-13 13:31 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-13 13:31 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx    11563 b- defN 24-May-13 13:31 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12174 b- defN 24-May-13 13:31 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3788 b- defN 24-May-13 13:31 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-13 13:31 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-13 13:31 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6935 b- defN 24-May-13 13:31 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-13 13:31 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-13 13:31 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    18433 b- defN 24-May-13 13:31 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-May-13 13:31 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-13 13:31 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-13 13:31 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     5159 b- defN 24-May-13 13:31 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-13 13:31 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-13 13:31 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-13 13:31 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4531 b- defN 24-May-13 13:31 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-13 13:31 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28367 b- defN 24-May-13 13:31 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-13 13:31 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-May-13 13:31 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    17167 b- defN 24-May-13 13:31 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-13 13:31 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    60444 b- defN 24-May-13 13:31 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     1739 b- defN 24-May-13 13:31 nucliadb/ingest/orm/synonyms.py
--rw-r--r--  2.0 unx     3683 b- defN 24-May-13 13:31 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    26423 b- defN 24-May-13 13:31 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-13 13:31 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-13 13:31 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    33196 b- defN 24-May-13 13:31 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-13 13:31 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24060 b- defN 24-May-13 13:31 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-13 13:31 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-13 13:31 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2549 b- defN 24-May-13 13:31 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2591 b- defN 24-May-13 13:31 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4465 b- defN 24-May-13 13:31 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-13 13:31 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-13 13:31 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27336 b- defN 24-May-13 13:31 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-13 13:31 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-13 13:31 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     4004 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4140 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-13 13:31 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-13 13:31 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-13 13:31 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-13 13:31 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-13 13:31 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-13 13:31 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-13 13:31 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9249 b- defN 24-May-13 13:31 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-13 13:31 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-13 13:31 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-13 13:31 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-13 13:31 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-13 13:31 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-13 13:31 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-13 13:31 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-13 13:31 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-13 13:31 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-13 13:31 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-May-13 13:31 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-13 13:31 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2434 b- defN 24-May-13 13:31 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-13 13:31 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12392 b- defN 24-May-13 13:31 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6459 b- defN 24-May-13 13:31 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3641 b- defN 24-May-13 13:31 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2099 b- defN 24-May-13 13:31 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4472 b- defN 24-May-13 13:31 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13940 b- defN 24-May-13 13:31 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-13 13:31 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12399 b- defN 24-May-13 13:31 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     8155 b- defN 24-May-13 13:31 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-13 13:31 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-May-13 13:31 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-13 13:31 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-13 13:31 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-13 13:31 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-13 13:31 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-13 13:31 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-13 13:31 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-13 13:31 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-13 13:31 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    17332 b- defN 24-May-13 13:31 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-May-13 13:31 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-13 13:31 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-13 13:31 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1222 b- defN 24-May-13 13:31 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     9882 b- defN 24-May-13 13:31 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2668 b- defN 24-May-13 13:31 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8810 b- defN 24-May-13 13:31 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-13 13:31 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3047 b- defN 24-May-13 13:31 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-13 13:31 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    18337 b- defN 24-May-13 13:31 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5970 b- defN 24-May-13 13:31 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-13 13:31 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-13 13:31 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     5821 b- defN 24-May-13 13:31 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5303 b- defN 24-May-13 13:31 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-13 13:31 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9111 b- defN 24-May-13 13:31 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-13 13:31 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-13 13:31 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-13 13:31 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-13 13:31 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-13 13:31 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-13 13:31 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-13 13:31 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-13 13:31 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-13 13:31 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-13 13:31 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31127 b- defN 24-May-13 13:31 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-13 13:31 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-13 13:31 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-13 13:31 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-13 13:31 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-13 13:31 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    15401 b- defN 24-May-13 13:31 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-13 13:31 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-13 13:31 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-13 13:31 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    13101 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-13 13:31 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-13 13:31 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-13 13:31 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-13 13:31 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5309 b- defN 24-May-13 13:31 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6930 b- defN 24-May-13 13:31 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-13 13:31 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1980 b- defN 24-May-13 13:31 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1317 b- defN 24-May-13 13:31 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5415 b- defN 24-May-13 13:31 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5781 b- defN 24-May-13 13:31 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-13 13:31 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-13 13:31 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-13 13:31 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-13 13:31 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-13 13:31 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-13 13:31 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-13 13:31 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-13 13:31 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-13 13:31 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-13 13:31 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1845 b- defN 24-May-13 13:31 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1587 b- defN 24-May-13 13:31 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-13 13:31 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-13 13:31 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-13 13:31 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-13 13:31 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-13 13:31 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-13 13:31 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-13 13:31 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-13 13:31 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-13 13:31 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-13 13:31 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-13 13:31 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-13 13:31 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-13 13:31 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-13 13:31 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-13 13:31 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-13 13:31 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-13 13:31 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3662 b- defN 24-May-13 13:31 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-13 13:31 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2780 b- defN 24-May-13 13:31 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-13 13:31 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-13 13:31 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-13 13:31 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-13 13:31 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3649 b- defN 24-May-13 13:31 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    11955 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     9465 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5627 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2136 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     3093 b- defN 24-May-13 13:31 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-13 13:31 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-13 13:31 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-13 13:31 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-13 13:31 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-13 13:31 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-13 13:31 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-13 13:31 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-13 13:31 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-13 13:31 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-13 13:31 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-13 13:31 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-13 13:31 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-13 13:31 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-13 13:31 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-13 13:31 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-13 13:31 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-13 13:31 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-13 13:31 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-May-13 13:31 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-13 13:31 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-13 13:31 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-13 13:31 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-13 13:31 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-13 13:31 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-13 13:31 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-13 13:31 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-13 13:31 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-13 13:31 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-May-13 13:31 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-13 13:31 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1908 b- defN 24-May-13 13:31 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2135 b- defN 24-May-13 13:31 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-13 13:31 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-13 13:31 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-13 13:31 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-13 13:31 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-13 13:31 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-13 13:31 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-13 13:31 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-13 13:31 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-13 13:31 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-May-13 13:31 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-13 13:31 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-13 13:31 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-May-13 13:31 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-13 13:31 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-May-13 13:31 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-13 13:31 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-13 13:31 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-13 13:31 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-13 13:31 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-13 13:31 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-13 13:31 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-13 13:31 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-13 13:31 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-13 13:31 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-13 13:31 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-13 13:31 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-13 13:31 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-13 13:31 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19495 b- defN 24-May-13 13:31 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-13 13:31 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-13 13:31 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-13 13:31 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-May-13 13:31 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3074 b- defN 24-May-13 13:31 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-13 13:31 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-13 13:31 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-13 13:31 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6571 b- defN 24-May-13 13:31 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24482 b- defN 24-May-13 13:31 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5248 b- defN 24-May-13 13:31 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-13 13:31 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18893 b- defN 24-May-13 13:31 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-13 13:31 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10747 b- defN 24-May-13 13:31 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30857 b- defN 24-May-13 13:31 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-13 13:31 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-13 13:31 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-13 13:31 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-13 13:31 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16319 b- defN 24-May-13 13:31 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-13 13:31 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1152 b- defN 24-May-13 13:31 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-13 13:31 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-13 13:31 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-13 13:31 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-13 13:31 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-13 13:31 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-13 13:31 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4358 b- defN 24-May-13 13:31 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16694 b- defN 24-May-13 13:31 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-13 13:31 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-13 13:31 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-13 13:31 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-13 13:31 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-13 13:31 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-13 13:31 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-13 13:31 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-13 13:31 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-13 13:31 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-13 13:31 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-13 13:31 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-13 13:31 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4399 b- defN 24-May-13 13:32 nucliadb-3.1.0.post496.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-13 13:32 nucliadb-3.1.0.post496.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-13 13:32 nucliadb-3.1.0.post496.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-13 13:32 nucliadb-3.1.0.post496.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-13 13:32 nucliadb-3.1.0.post496.dist-info/zip-safe
--rw-rw-r--  2.0 unx    42669 b- defN 24-May-13 13:32 nucliadb-3.1.0.post496.dist-info/RECORD
-455 files, 2218280 bytes uncompressed, 682546 bytes compressed:  69.2%
+Zip file size: 752691 bytes, number of entries: 456
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-13 14:49 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-13 14:49 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-13 14:49 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-13 14:49 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-13 14:49 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-13 14:49 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-13 14:49 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-13 14:49 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-13 14:49 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-13 14:49 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-13 14:49 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-13 14:49 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-13 14:49 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-13 14:49 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-13 14:49 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-13 14:49 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-13 14:49 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-13 14:49 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx     3268 b- defN 24-May-13 14:49 migrations/0020_drain_nodes_from_cluster.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-13 14:49 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-13 14:49 nucliadb/health.py
+-rw-r--r--  2.0 unx    11626 b- defN 24-May-13 14:49 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-13 14:49 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-13 14:49 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-13 14:49 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     5022 b- defN 24-May-13 14:49 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     4971 b- defN 24-May-13 14:49 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-13 14:49 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3790 b- defN 24-May-13 14:49 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-13 14:49 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    22097 b- defN 24-May-13 14:49 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8593 b- defN 24-May-13 14:49 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    20221 b- defN 24-May-13 14:49 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     2992 b- defN 24-May-13 14:49 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5747 b- defN 24-May-13 14:49 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-13 14:49 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12518 b- defN 24-May-13 14:49 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-13 14:49 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-13 14:49 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-13 14:49 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-13 14:49 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-13 14:49 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13707 b- defN 24-May-13 14:49 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-13 14:49 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-13 14:49 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-May-13 14:49 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-May-13 14:49 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-13 14:49 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1813 b- defN 24-May-13 14:49 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-13 14:49 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-13 14:49 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-13 14:49 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-13 14:49 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-13 14:49 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-13 14:49 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx     8719 b- defN 24-May-13 14:49 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5634 b- defN 24-May-13 14:49 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-13 14:49 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-13 14:49 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-13 14:49 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-13 14:49 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-13 14:49 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-13 14:49 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-13 14:49 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-May-13 14:49 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-13 14:49 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-13 14:49 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-13 14:49 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-May-13 14:49 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4109 b- defN 24-May-13 14:49 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-13 14:49 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-13 14:49 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-13 14:49 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-13 14:49 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-13 14:49 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-13 14:49 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-13 14:49 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19401 b- defN 24-May-13 14:49 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-13 14:49 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-13 14:49 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-13 14:49 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-13 14:49 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19541 b- defN 24-May-13 14:49 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-13 14:49 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3183 b- defN 24-May-13 14:49 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-13 14:49 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx    11563 b- defN 24-May-13 14:49 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12174 b- defN 24-May-13 14:49 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3788 b- defN 24-May-13 14:49 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-13 14:49 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-13 14:49 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6935 b- defN 24-May-13 14:49 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-13 14:49 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-13 14:49 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    18433 b- defN 24-May-13 14:49 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-13 14:49 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-13 14:49 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-13 14:49 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-May-13 14:49 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-13 14:49 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-13 14:49 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-13 14:49 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4531 b- defN 24-May-13 14:49 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-13 14:49 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28367 b- defN 24-May-13 14:49 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-13 14:49 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-May-13 14:49 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    17167 b- defN 24-May-13 14:49 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-13 14:49 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    60444 b- defN 24-May-13 14:49 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     1739 b- defN 24-May-13 14:49 nucliadb/ingest/orm/synonyms.py
+-rw-r--r--  2.0 unx     3683 b- defN 24-May-13 14:49 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    26423 b- defN 24-May-13 14:49 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-13 14:49 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-13 14:49 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    33196 b- defN 24-May-13 14:49 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-13 14:49 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24060 b- defN 24-May-13 14:49 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-13 14:49 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-13 14:49 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2549 b- defN 24-May-13 14:49 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-May-13 14:49 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4465 b- defN 24-May-13 14:49 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-13 14:49 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-13 14:49 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27336 b- defN 24-May-13 14:49 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-13 14:49 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-13 14:49 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     4004 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4140 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-13 14:49 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-13 14:49 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-13 14:49 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-13 14:49 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-13 14:49 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-13 14:49 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-13 14:49 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9249 b- defN 24-May-13 14:49 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-13 14:49 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-13 14:49 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-13 14:49 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-13 14:49 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-13 14:49 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-13 14:49 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-13 14:49 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-13 14:49 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-13 14:49 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-13 14:49 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-13 14:49 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-13 14:49 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2434 b- defN 24-May-13 14:49 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-13 14:49 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12392 b- defN 24-May-13 14:49 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6459 b- defN 24-May-13 14:49 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-May-13 14:49 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-May-13 14:49 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-May-13 14:49 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13940 b- defN 24-May-13 14:49 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-13 14:49 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12399 b- defN 24-May-13 14:49 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     8155 b- defN 24-May-13 14:49 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-13 14:49 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-13 14:49 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-13 14:49 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-13 14:49 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-13 14:49 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-13 14:49 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-13 14:49 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-13 14:49 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-13 14:49 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-13 14:49 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    17332 b- defN 24-May-13 14:49 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-13 14:49 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-13 14:49 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-13 14:49 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1222 b- defN 24-May-13 14:49 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     9882 b- defN 24-May-13 14:49 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-May-13 14:49 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8810 b- defN 24-May-13 14:49 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-13 14:49 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-May-13 14:49 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-13 14:49 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    18337 b- defN 24-May-13 14:49 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-May-13 14:49 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-13 14:49 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-13 14:49 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     5821 b- defN 24-May-13 14:49 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-May-13 14:49 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-13 14:49 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9111 b- defN 24-May-13 14:49 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-13 14:49 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-13 14:49 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-13 14:49 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-13 14:49 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-13 14:49 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-13 14:49 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-13 14:49 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-13 14:49 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-13 14:49 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-13 14:49 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31127 b- defN 24-May-13 14:49 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-13 14:49 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-13 14:49 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-13 14:49 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-13 14:49 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-13 14:49 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    15401 b- defN 24-May-13 14:49 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-13 14:49 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-13 14:49 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-13 14:49 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    13101 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-13 14:49 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-13 14:49 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-13 14:49 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-13 14:49 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5309 b- defN 24-May-13 14:49 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6930 b- defN 24-May-13 14:49 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-13 14:49 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-May-13 14:49 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-May-13 14:49 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5415 b- defN 24-May-13 14:49 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5781 b- defN 24-May-13 14:49 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-13 14:49 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-13 14:49 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-13 14:49 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-13 14:49 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-13 14:49 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-13 14:49 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-13 14:49 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-13 14:49 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-13 14:49 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-13 14:49 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1845 b- defN 24-May-13 14:49 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1587 b- defN 24-May-13 14:49 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-13 14:49 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-13 14:49 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-13 14:49 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-13 14:49 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-13 14:49 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-13 14:49 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-13 14:49 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-13 14:49 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-13 14:49 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-13 14:49 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-13 14:49 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-13 14:49 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-13 14:49 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-13 14:49 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-13 14:49 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-13 14:49 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-13 14:49 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3662 b- defN 24-May-13 14:49 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-13 14:49 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-May-13 14:49 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-13 14:49 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-13 14:49 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-13 14:49 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-13 14:49 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3649 b- defN 24-May-13 14:49 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     9465 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3761 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2136 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     3093 b- defN 24-May-13 14:49 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-13 14:49 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-13 14:49 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-13 14:49 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-13 14:49 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-13 14:49 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-13 14:49 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-13 14:49 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-13 14:49 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-13 14:49 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-13 14:49 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-13 14:49 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-13 14:49 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-13 14:49 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-13 14:49 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-13 14:49 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-13 14:49 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-13 14:49 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-13 14:49 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-13 14:49 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-13 14:49 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-13 14:49 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-13 14:49 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-13 14:49 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-13 14:49 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-13 14:49 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-13 14:49 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-13 14:49 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-13 14:49 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-May-13 14:49 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-13 14:49 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-13 14:49 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-May-13 14:49 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-13 14:49 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-13 14:49 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-13 14:49 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-13 14:49 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-13 14:49 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-13 14:49 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-13 14:49 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-13 14:49 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-13 14:49 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-13 14:49 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-13 14:49 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-13 14:49 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-May-13 14:49 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-13 14:49 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-May-13 14:49 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-13 14:49 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-13 14:49 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-13 14:49 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-13 14:49 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-13 14:49 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-13 14:49 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-13 14:49 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-13 14:49 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-13 14:49 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-13 14:49 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-13 14:49 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-13 14:49 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-13 14:49 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19495 b- defN 24-May-13 14:49 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-13 14:49 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-13 14:49 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-13 14:49 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-13 14:49 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-May-13 14:49 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-13 14:49 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-13 14:49 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-13 14:49 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6571 b- defN 24-May-13 14:49 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-May-13 14:49 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-May-13 14:49 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-13 14:49 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18893 b- defN 24-May-13 14:49 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-13 14:49 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10747 b- defN 24-May-13 14:49 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30857 b- defN 24-May-13 14:49 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-13 14:49 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-13 14:49 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-13 14:49 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-13 14:49 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16319 b- defN 24-May-13 14:49 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-13 14:49 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx     1152 b- defN 24-May-13 14:49 nucliadb/writer/resource/slug.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-13 14:49 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-13 14:49 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-13 14:49 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-13 14:49 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-13 14:49 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-13 14:49 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4358 b- defN 24-May-13 14:49 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16694 b- defN 24-May-13 14:49 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-13 14:49 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-13 14:49 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-13 14:49 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-13 14:49 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-13 14:49 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-13 14:49 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-13 14:49 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-13 14:49 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-13 14:49 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-13 14:49 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-13 14:49 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-13 14:49 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4399 b- defN 24-May-13 14:50 nucliadb-3.1.0.post497.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 14:50 nucliadb-3.1.0.post497.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-13 14:50 nucliadb-3.1.0.post497.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-13 14:50 nucliadb-3.1.0.post497.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-13 14:50 nucliadb-3.1.0.post497.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    42769 b- defN 24-May-13 14:50 nucliadb-3.1.0.post497.dist-info/RECORD
+456 files, 2223085 bytes uncompressed, 684297 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -48,14 +48,17 @@
 
 Filename: migrations/0018_purge_orphan_kbslugs.py
 Comment: 
 
 Filename: migrations/0019_upgrade_to_paragraphs_v3.py
 Comment: 
 
+Filename: migrations/0020_drain_nodes_from_cluster.py
+Comment: 
+
 Filename: migrations/__init__.py
 Comment: 
 
 Filename: nucliadb/__init__.py
 Comment: 
 
 Filename: nucliadb/health.py
@@ -1341,26 +1344,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-3.1.0.post496.dist-info/METADATA
+Filename: nucliadb-3.1.0.post497.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-3.1.0.post496.dist-info/WHEEL
+Filename: nucliadb-3.1.0.post497.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-3.1.0.post496.dist-info/entry_points.txt
+Filename: nucliadb-3.1.0.post497.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-3.1.0.post496.dist-info/top_level.txt
+Filename: nucliadb-3.1.0.post497.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-3.1.0.post496.dist-info/zip-safe
+Filename: nucliadb-3.1.0.post497.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-3.1.0.post496.dist-info/RECORD
+Filename: nucliadb-3.1.0.post497.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/common/cluster/manager.py

```diff
@@ -202,15 +202,18 @@
             )
             logger.error(msg, extra={"kbid": kbid})
             raise ShardsNotFound(msg)
 
         existing_kb_nodes = [
             replica.node for shard in kb_shards.shards for replica in shard.replicas
         ]
-        nodes = sorted_primary_nodes(avoid_nodes=existing_kb_nodes)
+        nodes = sorted_primary_nodes(
+            avoid_nodes=existing_kb_nodes,
+            ignore_nodes=settings.drain_nodes,
+        )
 
         shard_uuid = uuid.uuid4().hex
         shard = writer_pb2.ShardObject(shard=shard_uuid, read_only=False)
         try:
             # Attempt to create configured number of replicas
             replicas_created = 0
             while replicas_created < settings.node_replicas:
@@ -547,16 +550,18 @@
     return selected_node, shard_replica_id
 
 
 def check_enough_nodes():
     """
     It raises an exception if it can't find enough nodes for the configured replicas.
     """
+    drain_nodes = settings.drain_nodes
     target_replicas = settings.node_replicas
     available_nodes = get_index_nodes()
+    available_nodes = [node for node in available_nodes if node.id not in drain_nodes]
     if len(available_nodes) < target_replicas:
         raise NodeClusterSmall(
             f"Not enough nodes. Total: {len(available_nodes)}, Required: {target_replicas}"
         )
     if settings.max_node_replicas >= 0:
         available_nodes = list(
             filter(
@@ -565,30 +570,38 @@
         )
         if len(available_nodes) < target_replicas:
             raise NodeClusterSmall(
                 f"Could not find enough nodes with available shards. Available: {len(available_nodes)}, Required: {target_replicas}"  # noqa
             )
 
 
-def sorted_primary_nodes(avoid_nodes: Optional[list[str]] = None) -> list[str]:
+def sorted_primary_nodes(
+    avoid_nodes: Optional[list[str]] = None,
+    ignore_nodes: Optional[list[str]] = None,
+) -> list[str]:
     """
     Returns the list of all primary node ids sorted by decreasing available
     disk space (from more to less available disk reported).
 
-    It will put the node ids in `avoid_nodes` at the tail of the list.
+    Nodes in `avoid_nodes` are placed at the tail of the list.
+    Nodes in `ignore_nodes` are ignored and never returned.
     """
     primary_nodes = get_index_nodes(include_secondary=False)
 
     # Sort by available disk
-    sorted_primary_nodes = sorted(
-        primary_nodes, key=lambda n: n.available_disk, reverse=True
-    )
-    available_node_ids = [node.id for node in sorted_primary_nodes]
+    sorted_nodes = sorted(primary_nodes, key=lambda n: n.available_disk, reverse=True)
+    available_node_ids = [node.id for node in sorted_nodes]
 
     avoid_nodes = avoid_nodes or []
-    # get preferred nodes first
+    ignore_nodes = ignore_nodes or []
+
+    # Get the non-avoided nodes first
     preferred_nodes = [nid for nid in available_node_ids if nid not in avoid_nodes]
-    # now, add to the end of the last nodes
-    preferred_node_order = preferred_nodes + [
+
+    # Add avoid_nodes to the end of the last nodes
+    result_nodes = preferred_nodes + [
         nid for nid in available_node_ids if nid not in preferred_nodes
     ]
-    return preferred_node_order
+
+    # Remove ignore_nodes from the list
+    result_nodes = [nid for nid in result_nodes if nid not in ignore_nodes]
+    return result_nodes
```

## nucliadb/common/cluster/rollover.py

```diff
@@ -59,18 +59,19 @@
 
 
 class UnexpectedRolloverError(Exception):
     pass
 
 
 async def create_rollover_shards(
-    app_context: ApplicationContext, kbid: str
+    app_context: ApplicationContext, kbid: str, drain_nodes: Optional[list[str]] = None
 ) -> writer_pb2.Shards:
     """
-    Creates shards to be used for a rollover operation
+    Creates shards to be used for a rollover operation.
+    If drain_nodes is provided, no replicas will be created on those nodes.
     """
     logger.warning("Creating rollover shards", extra={"kbid": kbid})
     sm = app_context.shard_manager
 
     async with datamanagers.with_transaction() as txn:
         existing_rollover_shards = await datamanagers.rollover.get_kb_rollover_shards(
             txn, kbid=kbid
@@ -82,23 +83,25 @@
         kb_shards = await datamanagers.cluster.get_kb_shards(txn, kbid=kbid)
         if kb_shards is None:
             raise UnexpectedRolloverError(f"No shards found for KB {kbid}")
 
         # create new shards
         created_shards = []
         try:
-            nodes = cluster_manager.sorted_primary_nodes()
+            nodes = cluster_manager.sorted_primary_nodes(ignore_nodes=drain_nodes)
             for shard in kb_shards.shards:
                 shard.ClearField("replicas")
                 # Attempt to create configured number of replicas
                 replicas_created = 0
                 while replicas_created < settings.node_replicas:
                     if len(nodes) == 0:
                         # could have multiple shards on single node
-                        nodes = cluster_manager.sorted_primary_nodes()
+                        nodes = cluster_manager.sorted_primary_nodes(
+                            ignore_nodes=drain_nodes
+                        )
                     node_id = nodes.pop(0)
 
                     node = get_index_node(node_id)
                     if node is None:
                         logger.error(f"Node {node_id} is not found or not available")
                         continue
                     is_matryoshka = len(kb_shards.model.matryoshka_dimensions) > 0
@@ -463,22 +466,27 @@
             )
             return
 
         _clear_rollover_status(kb_shards)
         await datamanagers.cluster.update_kb_shards(txn, kbid=kbid, shards=kb_shards)
 
 
-async def rollover_kb_shards(app_context: ApplicationContext, kbid: str) -> None:
+async def rollover_kb_shards(
+    app_context: ApplicationContext, kbid: str, drain_nodes: Optional[list[str]] = None
+) -> None:
     """
     Rollover a shard is the process of creating new shard replicas for every
     shard and indexing all existing resources into the replicas.
 
     Once all the data is in the new shards, cut over the registered replicas
     to the new shards and delete the old shards.
 
+    If drain_nodes is provided, no replicas will be created on those nodes. This is useful
+    for when we want to remove a set of nodes from the cluster.
+
     This is a very expensive operation and should be done with care.
 
     Process:
     - Create new shards
     - Schedule all resources to be indexed
     - Index all resources into new shards
     - Cut over replicas to new shards
@@ -492,15 +500,15 @@
         logger.warning("Waiting for index nodes to be available")
         await asyncio.sleep(1)
         node_ready_checks += 1
 
     logger.warning("Rolling over shards", extra={"kbid": kbid})
 
     async with locking.distributed_lock(locking.KB_SHARDS_LOCK.format(kbid=kbid)):
-        await create_rollover_shards(app_context, kbid)
+        await create_rollover_shards(app_context, kbid, drain_nodes=drain_nodes)
         await schedule_resource_indexing(app_context, kbid)
         await index_rollover_shards(app_context, kbid)
         await cutover_shards(app_context, kbid)
         # we need to cut over BEFORE we validate the data
         await validate_indexed_data(app_context, kbid)
         await clean_indexed_data(app_context, kbid)
         await clean_rollover_status(app_context, kbid)
```

## nucliadb/common/cluster/settings.py

```diff
@@ -66,14 +66,20 @@
     )
     max_resource_paragraphs: int = Field(
         default=50_000,
         title="Max paragraphs per resource",
         description="Maximum number of paragraphs allowed on a single resource",
     )
 
+    drain_nodes: list[str] = Field(
+        default=[],
+        title="Drain nodes",
+        description="List of node IDs to ignore when creating new shards. It is used for draining nodes from a cluster. Example: ['1bf3bfe7-e164-4a19-a4d9-41372fc15aca',]",  # noqa: E501
+    )
+
     local_reader_threads: int = 5
     local_writer_threads: int = 5
 
     cluster_discovery_mode: ClusterDiscoveryMode = ClusterDiscoveryMode.KUBERNETES
     cluster_discovery_kubernetes_namespace: str = "nucliadb"
     cluster_discovery_kubernetes_selector: str = "appType=node"
     cluster_discovery_manual_addresses: list[str] = []
```

## nucliadb/tests/unit/common/cluster/test_cluster.py

```diff
@@ -56,28 +56,37 @@
 
 def test_sorted_primary_nodes_orders_by_available_disk(available_nodes):
     with mock.patch.object(settings, "node_replicas", 2):
         nodes = manager.sorted_primary_nodes()
         assert nodes == ["node-0", "node-30", "node-40"]
 
 
-def test_sorted_primary_nodes_puts_nodes_to_avoid_at_the_end(available_nodes):
+def test_sorted_primary_nodes_avoid_nodes(available_nodes):
     with mock.patch.object(settings, "node_replicas", 2):
         excluded_node = "node-0"
         nodes = manager.sorted_primary_nodes(avoid_nodes=[excluded_node])
         assert nodes == ["node-30", "node-40", "node-0"]
 
         # even if all are used, still should find nodes
         all_nodes = list(available_nodes.keys())
         assert manager.sorted_primary_nodes(avoid_nodes=all_nodes) == [
             "node-0",
             "node-30",
             "node-40",
         ]
 
+        # check ignore_nodes are ignored while keeping avoid_nodes at the end
+        all_nodes = list(available_nodes.keys())
+        assert manager.sorted_primary_nodes(
+            avoid_nodes=["node-0"], ignore_nodes=["node-30"]
+        ) == [
+            "node-40",
+            "node-0",
+        ]
+
 
 def test_check_enough_nodes_raises_error_if_not_enough_nodes_are_found(available_nodes):
     with mock.patch.object(settings, "node_replicas", 200):
         with pytest.raises(NodeClusterSmall):
             manager.check_enough_nodes()
```

## Comparing `nucliadb-3.1.0.post496.dist-info/METADATA` & `nucliadb-3.1.0.post497.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 3.1.0.post496
+Version: 3.1.0.post497
 Home-page: https://docs.nuclia.dev/docs/guides/nucliadb/intro
 Author: NucliaDB Community
 Author-email: nucliadb@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -17,18 +17,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
-Requires-Dist: nucliadb-telemetry[all] >=3.1.0.post496
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.1.0.post496
-Requires-Dist: nucliadb-protos >=3.1.0.post496
-Requires-Dist: nucliadb-models >=3.1.0.post496
+Requires-Dist: nucliadb-telemetry[all] >=3.1.0.post497
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.1.0.post497
+Requires-Dist: nucliadb-protos >=3.1.0.post497
+Requires-Dist: nucliadb-models >=3.1.0.post497
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: pydantic-argparse
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-3.1.0.post496.dist-info/entry_points.txt` & `nucliadb-3.1.0.post497.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-3.1.0.post496.dist-info/RECORD` & `nucliadb-3.1.0.post497.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -12,32 +12,33 @@
 migrations/0013_rollover_shards.py,sha256=c3IU8zinlWeVRN8T6o5eLpvGzkQOHX_Yz5xuFVRUy5U,1024
 migrations/0014_rollover_shards.py,sha256=24yLtXAwlVvCwtHLx9Tz-VWCzeMuy-0o3M6QNESi_Iw,1382
 migrations/0015_targeted_rollover.py,sha256=7C9XM8wg-bpkNyFh0xJuaGzOcE2WqU1BfqtInKAjTkw,1462
 migrations/0016_upgrade_to_paragraphs_v2.py,sha256=pOZUwTDfGoLjcSSKiWaN6FUvMDN95XNCBoux3u0dsmQ,2506
 migrations/0017_multiple_writable_shards.py,sha256=NY38wFVxSDXglkZE6DRnuN1DG_1kyZXr2j37C8VhyA0,2100
 migrations/0018_purge_orphan_kbslugs.py,sha256=3x5OsMb-JnP9y8_-ztYugk1RiXbOuthTFB-8I1XX3bk,2264
 migrations/0019_upgrade_to_paragraphs_v3.py,sha256=Jf1ljYQoLj1QExz9-tDIxI7QrwPhixIHxvQJvHOl6WA,2506
+migrations/0020_drain_nodes_from_cluster.py,sha256=NNC6FXnaVciuIdkqBJz0I1ZJLu0QHHp_0DDYhnT70cE,3268
 migrations/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/__init__.py,sha256=_abCmDJ_0ku483Os4UAjPX7Nywm39cQgAV_DiyjsKeQ,891
 nucliadb/health.py,sha256=zPwd3CAFJf9owhbadtyGLvHekOjX9ykvxLYWYxnD5eo,3733
 nucliadb/learning_proxy.py,sha256=6r_fFgE662yEFgNpgGNxc3KTfFiR78yiEN95Qir6ctI,11626
 nucliadb/metrics_exporter.py,sha256=PummIqtRLdpcONPIpRKBj_jGYnX7B9XZ2IO048bu2pM,4806
 nucliadb/openapi.py,sha256=wDiw0dVEvTpJvbatkJ0JZLkKm9RItZT5PWRHjqRfqTA,2272
 nucliadb/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/common/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/locking.py,sha256=M9ODhLZUfCyrtx3qaCE7282L2Nkga1mcFUsXhh0cV50,5022
 nucliadb/common/cluster/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/cluster/base.py,sha256=z_JD-xNVPB6-6O_u8YMpyOPP3fRmimwq7LbA3EGqDnE,4971
 nucliadb/common/cluster/exceptions.py,sha256=V3c_fgH00GyJ-a5CaGLhwTuhwhUNR9YAGvS5jaRuc_Y,1495
 nucliadb/common/cluster/grpc_node_dummy.py,sha256=10OWSt-k2198cvaQtm12gjdsjyfjEY0laXcVcaz7gyc,3790
 nucliadb/common/cluster/index_node.py,sha256=WafWLzU1l7EHj1VyG0w6qi2BW_Izc8rFze6ZWbYvT9g,3429
-nucliadb/common/cluster/manager.py,sha256=PP3FsOumvanZ27FOvvOk5COg9BJo8Y4G_Xfie1e44J4,21672
+nucliadb/common/cluster/manager.py,sha256=VnBVZk6bYxstfKDLlgwsKZVpfLw_QNVlPDcAoh1njbw,22097
 nucliadb/common/cluster/rebalance.py,sha256=o2LEvVUUHA30QW7ei4HtbXxL1RraMrrZoUB3qSYl8WI,8593
-nucliadb/common/cluster/rollover.py,sha256=Jswv3p16X5nV8rmgHSSTDgAXKDos1RfumtILkMYP3xs,19773
-nucliadb/common/cluster/settings.py,sha256=snENrNo9voc1TZ6uyBnuSHGoS2Ocga_Kn-W33nOlO-c,2713
+nucliadb/common/cluster/rollover.py,sha256=FRMZduNsOhvdFfWUHimN2wgTI988elwZvh91NNmcT0g,20221
+nucliadb/common/cluster/settings.py,sha256=cLi99xKvwxJbCJoTjO2I0gyLRcfvroz8FF7wAiH-sUo,2992
 nucliadb/common/cluster/utils.py,sha256=5Y4YMfjBzDRDaPAsFDAzpAm9hCp2yCkvfJOEQOPZH_w,5747
 nucliadb/common/cluster/discovery/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/cluster/discovery/base.py,sha256=P0JwzRYqOKxOzV_K_glwPizDGFGBY-l8G7TeTId9LIA,6553
 nucliadb/common/cluster/discovery/k8s.py,sha256=pvuyIYuWWDpRz7Bv8D_LOKFMz0w8sucpJvDshmRNpe0,12518
 nucliadb/common/cluster/discovery/manual.py,sha256=7wdcyfrR8oii2hP3AzOTAaUAGwkQu7eOj9Xl7Q49IUQ,1957
 nucliadb/common/cluster/discovery/single.py,sha256=2BhcencPKQQIfVitmTPJZm3TkBHyY9ZMcr-Clh8k2tM,1737
 nucliadb/common/cluster/discovery/types.py,sha256=vs-K790rofjZ4FWYaMkgjkZZqMvIvd_0eSw3shuiLwA,1139
@@ -319,15 +320,15 @@
 nucliadb/tests/unit/test_learning_proxy.py,sha256=e3-wL_gsv0nQoChfvHR6NfDqSBzesnoq5MeGaHjzyNM,7892
 nucliadb/tests/unit/test_metrics_exporter.py,sha256=t__hVxV0Fo0duKtnJQl7BjyOXtP7QcD0pzHD9936z4o,2642
 nucliadb/tests/unit/test_openapi.py,sha256=ivwIs7UcTDfGyWD85VtzcmurPyU-ez9hvEmSCfFexrs,1341
 nucliadb/tests/unit/test_purge.py,sha256=wxCRrBVAIs4tN1hQwUfbsIhkUV-r9CKE_wgmIyWF_kA,3649
 nucliadb/tests/unit/common/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/tests/unit/common/test_context.py,sha256=GmZlJtXsX4TTNLb49q_SnH0jADgBMSrGKgrc5zOyYH8,1268
 nucliadb/tests/unit/common/cluster/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/tests/unit/common/cluster/test_cluster.py,sha256=phVNLjFuBoem3wWhPASvKEl2LDIROXsJ1Bdq3Uc_5qs,11955
+nucliadb/tests/unit/common/cluster/test_cluster.py,sha256=lO3IXRhXBsVQ7swHhPxKOCusnRsDyksIOSuvWOgDMM0,12240
 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py,sha256=N6aLQI3ZUwLdwLsMJ2hhnIAyGYTODLWYjJILQClaxLs,5387
 nucliadb/tests/unit/common/cluster/test_rollover.py,sha256=j0C-tKH9jwRThiN2DGmyRmskhag4C9pVZ7-0uATUQFI,9465
 nucliadb/tests/unit/common/cluster/discovery/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py,sha256=8rZ5yWiEXgLrMnWH4iX8Zrbw1upVqyM1EMFM2G0yOLo,5627
 nucliadb/tests/unit/common/cluster/standalone/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/tests/unit/common/cluster/standalone/test_service.py,sha256=sg0wWlBZNtLo9pA3rIIv6BAbkRcXsgDV0JreCgjnTHo,3761
 nucliadb/tests/unit/common/cluster/standalone/test_utils.py,sha256=2UHgo366zBqgfm-o7GEzdG9PwzorCmfxxI9styaxo2c,2136
@@ -443,13 +444,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-3.1.0.post496.dist-info/METADATA,sha256=l7F4Im4TStGwtOfIk0HddUE2dYUhDqchoZ5cdmqu5ac,4399
-nucliadb-3.1.0.post496.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-3.1.0.post496.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-3.1.0.post496.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-3.1.0.post496.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-3.1.0.post496.dist-info/RECORD,,
+nucliadb-3.1.0.post497.dist-info/METADATA,sha256=JzoFBLBy2TR224KsYNO1m8yCUUdonXSbThjhehz1Ylc,4399
+nucliadb-3.1.0.post497.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-3.1.0.post497.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-3.1.0.post497.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-3.1.0.post497.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-3.1.0.post497.dist-info/RECORD,,
```

