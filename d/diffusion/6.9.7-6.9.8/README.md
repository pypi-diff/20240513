# Comparing `tmp/diffusion-6.9.7-1-py3-none-any.whl.zip` & `tmp/diffusion-6.9.8-1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,115 +1,115 @@
-Zip file size: 180348 bytes, number of entries: 113
--rw-r--r--  2.0 unx      248 b- defN 24-Apr-03 13:12 diffusion/__init__.py
--rw-r--r--  2.0 unx      739 b- defN 24-Apr-03 13:12 diffusion/exceptions.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 13:12 diffusion/py.typed
--rw-r--r--  2.0 unx     3781 b- defN 24-Apr-03 13:12 diffusion/datatypes/__init__.py
--rw-r--r--  2.0 unx      494 b- defN 24-Apr-03 13:12 diffusion/datatypes/exceptions.py
--rw-r--r--  2.0 unx      652 b- defN 24-Apr-03 13:12 diffusion/datatypes/complex/__init__.py
--rw-r--r--  2.0 unx     2053 b- defN 24-Apr-03 13:12 diffusion/datatypes/complex/jsondatatype.py
--rw-r--r--  2.0 unx      214 b- defN 24-Apr-03 13:12 diffusion/datatypes/complex/recorddatatype.py
--rw-r--r--  2.0 unx      204 b- defN 24-Apr-03 13:12 diffusion/datatypes/complex/routingdatatype.py
--rw-r--r--  2.0 unx      204 b- defN 24-Apr-03 13:12 diffusion/datatypes/complex/unknowndatatype.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 13:12 diffusion/datatypes/foundation/__init__.py
--rw-r--r--  2.0 unx     7795 b- defN 24-Apr-03 13:12 diffusion/datatypes/foundation/abstract.py
--rw-r--r--  2.0 unx     1850 b- defN 24-Apr-03 13:12 diffusion/datatypes/foundation/datatype.py
--rw-r--r--  2.0 unx     1088 b- defN 24-Apr-03 13:12 diffusion/datatypes/primitives/__init__.py
--rw-r--r--  2.0 unx     2095 b- defN 24-Apr-03 13:12 diffusion/datatypes/primitives/binarydatatype.py
--rw-r--r--  2.0 unx      366 b- defN 24-Apr-03 13:12 diffusion/datatypes/primitives/doubledatatype.py
--rw-r--r--  2.0 unx      988 b- defN 24-Apr-03 13:12 diffusion/datatypes/primitives/int64datatype.py
--rw-r--r--  2.0 unx     1602 b- defN 24-Apr-03 13:12 diffusion/datatypes/primitives/primitivedatatype.py
--rw-r--r--  2.0 unx      234 b- defN 24-Apr-03 13:12 diffusion/datatypes/primitives/stringdatatype.py
--rw-r--r--  2.0 unx    11467 b- defN 24-Apr-03 13:12 diffusion/datatypes/timeseries/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 13:12 diffusion/datatypes/timeseries/py.typed
--rw-r--r--  2.0 unx    19412 b- defN 24-Apr-03 13:12 diffusion/datatypes/timeseries/time_series_event.py
--rw-r--r--  2.0 unx     2997 b- defN 24-Apr-03 13:12 diffusion/datatypes/timeseries/time_series_event_metadata.py
--rw-r--r--  2.0 unx     1645 b- defN 24-Apr-03 13:12 diffusion/datatypes/timeseries/types.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 13:12 diffusion/features/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 13:12 diffusion/features/control/__init__.py
--rw-r--r--  2.0 unx     8750 b- defN 24-Apr-03 13:12 diffusion/features/control/metrics/__init__.py
--rw-r--r--  2.0 unx     1138 b- defN 24-Apr-03 13:12 diffusion/features/control/metrics/collector.py
--rw-r--r--  2.0 unx     5218 b- defN 24-Apr-03 13:12 diffusion/features/control/metrics/session_metrics.py
--rw-r--r--  2.0 unx     5158 b- defN 24-Apr-03 13:12 diffusion/features/control/metrics/topic_metrics.py
--rw-r--r--  2.0 unx     9508 b- defN 24-Apr-03 13:12 diffusion/features/control/session_trees/__init__.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-03 13:12 diffusion/features/control/session_trees/branch_mapping.py
--rw-r--r--  2.0 unx     3409 b- defN 24-Apr-03 13:12 diffusion/features/control/session_trees/branch_mapping_table.py
--rw-r--r--  2.0 unx     1031 b- defN 24-Apr-03 13:12 diffusion/features/control/session_trees/invalid_branch_mapping_exception.py
--rw-r--r--  2.0 unx    17686 b- defN 24-Apr-03 13:12 diffusion/features/timeseries/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 13:12 diffusion/features/timeseries/query/__init__.py
--rw-r--r--  2.0 unx     6760 b- defN 24-Apr-03 13:12 diffusion/features/timeseries/query/query_result.py
--rw-r--r--  2.0 unx    49729 b- defN 24-Apr-03 13:12 diffusion/features/timeseries/query/range_query.py
--rw-r--r--  2.0 unx      710 b- defN 24-Apr-03 13:12 diffusion/features/timeseries/query/range_query_parameters.py
--rw-r--r--  2.0 unx    12515 b- defN 24-Apr-03 13:12 diffusion/features/topics/__init__.py
--rw-r--r--  2.0 unx     8127 b- defN 24-Apr-03 13:12 diffusion/features/topics/selectors.py
--rw-r--r--  2.0 unx     2731 b- defN 24-Apr-03 13:12 diffusion/features/topics/streams.py
--rw-r--r--  2.0 unx      424 b- defN 24-Apr-03 13:12 diffusion/features/topics/details/__init__.py
--rw-r--r--  2.0 unx    43807 b- defN 24-Apr-03 13:12 diffusion/features/topics/details/topic_specification.py
--rw-r--r--  2.0 unx     4557 b- defN 24-Apr-03 13:12 diffusion/features/topics/update/__init__.py
--rw-r--r--  2.0 unx     4573 b- defN 24-Apr-03 13:12 diffusion/features/topics/update/constraint_factory.py
--rw-r--r--  2.0 unx    13423 b- defN 24-Apr-03 13:12 diffusion/features/topics/update/constraints.py
--rw-r--r--  2.0 unx     4096 b- defN 24-Apr-03 13:12 diffusion/handlers/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 13:12 diffusion/internal/__init__.py
--rw-r--r--  2.0 unx      677 b- defN 24-Apr-03 13:12 diffusion/internal/components.py
--rw-r--r--  2.0 unx     1522 b- defN 24-Apr-03 13:12 diffusion/internal/encoder.py
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-03 13:12 diffusion/internal/exceptions.py
--rw-r--r--  2.0 unx    12064 b- defN 24-Apr-03 13:12 diffusion/internal/utils.py
--rw-r--r--  2.0 unx      452 b- defN 24-Apr-03 13:12 diffusion/internal/encoded_data/__init__.py
--rw-r--r--  2.0 unx     4234 b- defN 24-Apr-03 13:12 diffusion/internal/encoded_data/abstract.py
--rw-r--r--  2.0 unx      494 b- defN 24-Apr-03 13:12 diffusion/internal/encoded_data/exceptions.py
--rw-r--r--  2.0 unx     1928 b- defN 24-Apr-03 13:12 diffusion/internal/encoded_data/generics.py
--rw-r--r--  2.0 unx     4912 b- defN 24-Apr-03 13:12 diffusion/internal/encoded_data/scalars.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 13:12 diffusion/internal/generated/__init__.py
--rw-r--r--  2.0 unx    10827 b- defN 24-Apr-03 13:12 diffusion/internal/generated/services.py
--rw-r--r--  2.0 unx     7186 b- defN 24-Apr-03 13:12 diffusion/internal/protocol/__init__.py
--rw-r--r--  2.0 unx     9658 b- defN 24-Apr-03 13:12 diffusion/internal/protocol/conversations.py
--rw-r--r--  2.0 unx     2518 b- defN 24-Apr-03 13:12 diffusion/internal/protocol/exceptions.py
--rw-r--r--  2.0 unx     8325 b- defN 24-Apr-03 13:12 diffusion/internal/protocol/message_types.py
--rw-r--r--  2.0 unx    11585 b- defN 24-Apr-03 13:12 diffusion/internal/protocol/properties.py
--rw-r--r--  2.0 unx     1501 b- defN 24-Apr-03 13:12 diffusion/internal/serialisers/__init__.py
--rw-r--r--  2.0 unx     2619 b- defN 24-Apr-03 13:12 diffusion/internal/serialisers/attrs.py
--rw-r--r--  2.0 unx    18499 b- defN 24-Apr-03 13:12 diffusion/internal/serialisers/base.py
--rw-r--r--  2.0 unx     7541 b- defN 24-Apr-03 13:12 diffusion/internal/serialisers/compound.py
--rw-r--r--  2.0 unx    13422 b- defN 24-Apr-03 13:12 diffusion/internal/serialisers/generic_model.py
--rw-r--r--  2.0 unx      786 b- defN 24-Apr-03 13:12 diffusion/internal/serialisers/primitives.py
--rw-r--r--  2.0 unx     1712 b- defN 24-Apr-03 13:12 diffusion/internal/serialisers/pydantic.py
--rw-r--r--  2.0 unx    42379 b- defN 24-Apr-03 13:12 diffusion/internal/serialisers/spec.py
--rw-r--r--  2.0 unx     4071 b- defN 24-Apr-03 13:12 diffusion/internal/serialisers/timeseries.py
--rw-r--r--  2.0 unx      688 b- defN 24-Apr-03 13:12 diffusion/internal/services/__init__.py
--rw-r--r--  2.0 unx    13677 b- defN 24-Apr-03 13:12 diffusion/internal/services/abstract.py
--rw-r--r--  2.0 unx      406 b- defN 24-Apr-03 13:12 diffusion/internal/services/exceptions.py
--rw-r--r--  2.0 unx     2001 b- defN 24-Apr-03 13:12 diffusion/internal/services/locator.py
--rw-r--r--  2.0 unx     6822 b- defN 24-Apr-03 13:12 diffusion/internal/services/messaging.py
--rw-r--r--  2.0 unx     1769 b- defN 24-Apr-03 13:12 diffusion/internal/services/session.py
--rw-r--r--  2.0 unx     5667 b- defN 24-Apr-03 13:12 diffusion/internal/services/topics.py
--rw-r--r--  2.0 unx     6646 b- defN 24-Apr-03 13:12 diffusion/internal/session/__init__.py
--rw-r--r--  2.0 unx     8506 b- defN 24-Apr-03 13:12 diffusion/internal/session/connection.py
--rw-r--r--  2.0 unx     1678 b- defN 24-Apr-03 13:12 diffusion/internal/session/credentials.py
--rw-r--r--  2.0 unx     4290 b- defN 24-Apr-03 13:12 diffusion/internal/session/error_reason.py
--rw-r--r--  2.0 unx     8161 b- defN 24-Apr-03 13:12 diffusion/internal/session/exception_handler.py
--rw-r--r--  2.0 unx      424 b- defN 24-Apr-03 13:12 diffusion/internal/session/locks/__init__.py
--rw-r--r--  2.0 unx     1360 b- defN 24-Apr-03 13:12 diffusion/internal/session/locks/session_lock_acquisition.py
--rw-r--r--  2.0 unx      805 b- defN 24-Apr-03 13:12 diffusion/internal/session/locks/session_lock_request.py
--rw-r--r--  2.0 unx      710 b- defN 24-Apr-03 13:12 diffusion/internal/session/locks/session_lock_request_cancellation.py
--rw-r--r--  2.0 unx      424 b- defN 24-Apr-03 13:12 diffusion/internal/timeseries/__init__.py
--rw-r--r--  2.0 unx      424 b- defN 24-Apr-03 13:12 diffusion/internal/timeseries/query/__init__.py
--rw-r--r--  2.0 unx     2363 b- defN 24-Apr-03 13:12 diffusion/internal/timeseries/query/range_query.py
--rw-r--r--  2.0 unx    27383 b- defN 24-Apr-03 13:12 diffusion/internal/timeseries/query/range_query_parameters.py
--rw-r--r--  2.0 unx     3556 b- defN 24-Apr-03 13:12 diffusion/internal/timeseries/query/range_query_request.py
--rw-r--r--  2.0 unx    10765 b- defN 24-Apr-03 13:12 diffusion/internal/timeseries/query/range_query_result.py
--rw-r--r--  2.0 unx     7618 b- defN 24-Apr-03 13:12 diffusion/internal/topics/__init__.py
--rw-r--r--  2.0 unx      311 b- defN 24-Apr-03 13:12 diffusion/internal/topics/constraints.py
--rw-r--r--  2.0 unx     2192 b- defN 24-Apr-03 13:12 diffusion/internal/validation/__init__.py
--rw-r--r--  2.0 unx     1923 b- defN 24-Apr-03 13:12 diffusion/internal/validation/pydantic.py
--rw-r--r--  2.0 unx    10373 b- defN 24-Apr-03 13:12 diffusion/messaging/__init__.py
--rw-r--r--  2.0 unx    13265 b- defN 24-Apr-03 13:12 diffusion/session/__init__.py
--rw-r--r--  2.0 unx     5509 b- defN 24-Apr-03 13:12 diffusion/session/exceptions.py
--rw-r--r--  2.0 unx     2166 b- defN 24-Apr-03 13:12 diffusion/session/retry_strategy.py
--rw-r--r--  2.0 unx     1223 b- defN 24-Apr-03 13:12 diffusion/session/session_container_factory.py
--rw-r--r--  2.0 unx    12135 b- defN 24-Apr-03 13:12 diffusion/session/session_factory.py
--rw-r--r--  2.0 unx      424 b- defN 24-Apr-03 13:12 diffusion/session/locks/__init__.py
--rw-r--r--  2.0 unx      929 b- defN 24-Apr-03 13:12 diffusion/session/locks/session_lock_acquisition.py
--rw-r--r--  2.0 unx    14937 b- defN 24-Apr-03 13:12 diffusion/session/locks/session_locks.py
--rw-r--r--  2.0 unx     1718 b- defN 24-Apr-03 13:12 diffusion-6.9.7.dist-info/METADATA
--rw-r--r--  2.0 unx      101 b- defN 24-Apr-03 13:12 diffusion-6.9.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Apr-03 13:12 diffusion-6.9.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    11174 b- defN 24-Apr-03 13:12 diffusion-6.9.7.dist-info/RECORD
-113 files, 628764 bytes uncompressed, 162096 bytes compressed:  74.2%
+Zip file size: 180361 bytes, number of entries: 113
+-rw-rw-rw-  2.0 unx      248 b- defN 24-May-13 12:01 diffusion/__init__.py
+-rw-rw-rw-  2.0 unx      739 b- defN 24-May-13 12:01 diffusion/exceptions.py
+-rw-rw-rw-  2.0 unx        0 b- defN 24-May-13 12:01 diffusion/py.typed
+-rw-rw-rw-  2.0 unx     3781 b- defN 24-May-13 12:01 diffusion/datatypes/__init__.py
+-rw-rw-rw-  2.0 unx      494 b- defN 24-May-13 12:01 diffusion/datatypes/exceptions.py
+-rw-rw-rw-  2.0 unx      652 b- defN 24-May-13 12:01 diffusion/datatypes/complex/__init__.py
+-rw-rw-rw-  2.0 unx     2053 b- defN 24-May-13 12:01 diffusion/datatypes/complex/jsondatatype.py
+-rw-rw-rw-  2.0 unx      214 b- defN 24-May-13 12:01 diffusion/datatypes/complex/recorddatatype.py
+-rw-rw-rw-  2.0 unx      204 b- defN 24-May-13 12:01 diffusion/datatypes/complex/routingdatatype.py
+-rw-rw-rw-  2.0 unx      204 b- defN 24-May-13 12:01 diffusion/datatypes/complex/unknowndatatype.py
+-rw-rw-rw-  2.0 unx        0 b- defN 24-May-13 12:01 diffusion/datatypes/foundation/__init__.py
+-rw-rw-rw-  2.0 unx     7795 b- defN 24-May-13 12:01 diffusion/datatypes/foundation/abstract.py
+-rw-rw-rw-  2.0 unx     1850 b- defN 24-May-13 12:01 diffusion/datatypes/foundation/datatype.py
+-rw-rw-rw-  2.0 unx     1088 b- defN 24-May-13 12:01 diffusion/datatypes/primitives/__init__.py
+-rw-rw-rw-  2.0 unx     2095 b- defN 24-May-13 12:01 diffusion/datatypes/primitives/binarydatatype.py
+-rw-rw-rw-  2.0 unx      366 b- defN 24-May-13 12:01 diffusion/datatypes/primitives/doubledatatype.py
+-rw-rw-rw-  2.0 unx      988 b- defN 24-May-13 12:01 diffusion/datatypes/primitives/int64datatype.py
+-rw-rw-rw-  2.0 unx     1602 b- defN 24-May-13 12:01 diffusion/datatypes/primitives/primitivedatatype.py
+-rw-rw-rw-  2.0 unx      234 b- defN 24-May-13 12:01 diffusion/datatypes/primitives/stringdatatype.py
+-rw-rw-rw-  2.0 unx    11467 b- defN 24-May-13 12:01 diffusion/datatypes/timeseries/__init__.py
+-rw-rw-rw-  2.0 unx        0 b- defN 24-May-13 12:01 diffusion/datatypes/timeseries/py.typed
+-rw-rw-rw-  2.0 unx    19412 b- defN 24-May-13 12:01 diffusion/datatypes/timeseries/time_series_event.py
+-rw-rw-rw-  2.0 unx     2997 b- defN 24-May-13 12:01 diffusion/datatypes/timeseries/time_series_event_metadata.py
+-rw-rw-rw-  2.0 unx     1645 b- defN 24-May-13 12:01 diffusion/datatypes/timeseries/types.py
+-rw-rw-rw-  2.0 unx        0 b- defN 24-May-13 12:01 diffusion/features/__init__.py
+-rw-rw-rw-  2.0 unx        0 b- defN 24-May-13 12:01 diffusion/features/control/__init__.py
+-rw-rw-rw-  2.0 unx     8750 b- defN 24-May-13 12:01 diffusion/features/control/metrics/__init__.py
+-rw-rw-rw-  2.0 unx     1138 b- defN 24-May-13 12:01 diffusion/features/control/metrics/collector.py
+-rw-rw-rw-  2.0 unx     5218 b- defN 24-May-13 12:01 diffusion/features/control/metrics/session_metrics.py
+-rw-rw-rw-  2.0 unx     5158 b- defN 24-May-13 12:01 diffusion/features/control/metrics/topic_metrics.py
+-rw-rw-rw-  2.0 unx     9508 b- defN 24-May-13 12:01 diffusion/features/control/session_trees/__init__.py
+-rw-rw-rw-  2.0 unx     1334 b- defN 24-May-13 12:01 diffusion/features/control/session_trees/branch_mapping.py
+-rw-rw-rw-  2.0 unx     3409 b- defN 24-May-13 12:01 diffusion/features/control/session_trees/branch_mapping_table.py
+-rw-rw-rw-  2.0 unx     1031 b- defN 24-May-13 12:01 diffusion/features/control/session_trees/invalid_branch_mapping_exception.py
+-rw-rw-rw-  2.0 unx    17686 b- defN 24-May-13 12:01 diffusion/features/timeseries/__init__.py
+-rw-rw-rw-  2.0 unx        0 b- defN 24-May-13 12:01 diffusion/features/timeseries/query/__init__.py
+-rw-rw-rw-  2.0 unx     6760 b- defN 24-May-13 12:01 diffusion/features/timeseries/query/query_result.py
+-rw-rw-rw-  2.0 unx    49729 b- defN 24-May-13 12:01 diffusion/features/timeseries/query/range_query.py
+-rw-rw-rw-  2.0 unx      710 b- defN 24-May-13 12:01 diffusion/features/timeseries/query/range_query_parameters.py
+-rw-rw-rw-  2.0 unx    12515 b- defN 24-May-13 12:01 diffusion/features/topics/__init__.py
+-rw-rw-rw-  2.0 unx     8127 b- defN 24-May-13 12:01 diffusion/features/topics/selectors.py
+-rw-rw-rw-  2.0 unx     2731 b- defN 24-May-13 12:01 diffusion/features/topics/streams.py
+-rw-rw-rw-  2.0 unx      424 b- defN 24-May-13 12:01 diffusion/features/topics/details/__init__.py
+-rw-rw-rw-  2.0 unx    43807 b- defN 24-May-13 12:01 diffusion/features/topics/details/topic_specification.py
+-rw-rw-rw-  2.0 unx     4557 b- defN 24-May-13 12:01 diffusion/features/topics/update/__init__.py
+-rw-rw-rw-  2.0 unx     4573 b- defN 24-May-13 12:01 diffusion/features/topics/update/constraint_factory.py
+-rw-rw-rw-  2.0 unx    13423 b- defN 24-May-13 12:01 diffusion/features/topics/update/constraints.py
+-rw-rw-rw-  2.0 unx     4096 b- defN 24-May-13 12:01 diffusion/handlers/__init__.py
+-rw-rw-rw-  2.0 unx        0 b- defN 24-May-13 12:01 diffusion/internal/__init__.py
+-rw-rw-rw-  2.0 unx      677 b- defN 24-May-13 12:01 diffusion/internal/components.py
+-rw-rw-rw-  2.0 unx     1522 b- defN 24-May-13 12:01 diffusion/internal/encoder.py
+-rw-rw-rw-  2.0 unx      507 b- defN 24-May-13 12:01 diffusion/internal/exceptions.py
+-rw-rw-rw-  2.0 unx    12064 b- defN 24-May-13 12:01 diffusion/internal/utils.py
+-rw-rw-rw-  2.0 unx      452 b- defN 24-May-13 12:01 diffusion/internal/encoded_data/__init__.py
+-rw-rw-rw-  2.0 unx     4234 b- defN 24-May-13 12:01 diffusion/internal/encoded_data/abstract.py
+-rw-rw-rw-  2.0 unx      494 b- defN 24-May-13 12:01 diffusion/internal/encoded_data/exceptions.py
+-rw-rw-rw-  2.0 unx     1928 b- defN 24-May-13 12:01 diffusion/internal/encoded_data/generics.py
+-rw-rw-rw-  2.0 unx     4912 b- defN 24-May-13 12:01 diffusion/internal/encoded_data/scalars.py
+-rw-rw-rw-  2.0 unx        0 b- defN 24-May-13 12:01 diffusion/internal/generated/__init__.py
+-rw-rw-rw-  2.0 unx    10827 b- defN 24-May-13 12:01 diffusion/internal/generated/services.py
+-rw-rw-rw-  2.0 unx     7186 b- defN 24-May-13 12:01 diffusion/internal/protocol/__init__.py
+-rw-rw-rw-  2.0 unx     9658 b- defN 24-May-13 12:01 diffusion/internal/protocol/conversations.py
+-rw-rw-rw-  2.0 unx     2518 b- defN 24-May-13 12:01 diffusion/internal/protocol/exceptions.py
+-rw-rw-rw-  2.0 unx     8325 b- defN 24-May-13 12:01 diffusion/internal/protocol/message_types.py
+-rw-rw-rw-  2.0 unx    11585 b- defN 24-May-13 12:01 diffusion/internal/protocol/properties.py
+-rw-rw-rw-  2.0 unx     1501 b- defN 24-May-13 12:01 diffusion/internal/serialisers/__init__.py
+-rw-rw-rw-  2.0 unx     2619 b- defN 24-May-13 12:01 diffusion/internal/serialisers/attrs.py
+-rw-rw-rw-  2.0 unx    18499 b- defN 24-May-13 12:01 diffusion/internal/serialisers/base.py
+-rw-rw-rw-  2.0 unx     7541 b- defN 24-May-13 12:01 diffusion/internal/serialisers/compound.py
+-rw-rw-rw-  2.0 unx    13422 b- defN 24-May-13 12:01 diffusion/internal/serialisers/generic_model.py
+-rw-rw-rw-  2.0 unx      786 b- defN 24-May-13 12:01 diffusion/internal/serialisers/primitives.py
+-rw-rw-rw-  2.0 unx     1712 b- defN 24-May-13 12:01 diffusion/internal/serialisers/pydantic.py
+-rw-rw-rw-  2.0 unx    42379 b- defN 24-May-13 12:01 diffusion/internal/serialisers/spec.py
+-rw-rw-rw-  2.0 unx     4071 b- defN 24-May-13 12:01 diffusion/internal/serialisers/timeseries.py
+-rw-rw-rw-  2.0 unx      688 b- defN 24-May-13 12:01 diffusion/internal/services/__init__.py
+-rw-rw-rw-  2.0 unx    13677 b- defN 24-May-13 12:01 diffusion/internal/services/abstract.py
+-rw-rw-rw-  2.0 unx      406 b- defN 24-May-13 12:01 diffusion/internal/services/exceptions.py
+-rw-rw-rw-  2.0 unx     2001 b- defN 24-May-13 12:01 diffusion/internal/services/locator.py
+-rw-rw-rw-  2.0 unx     6822 b- defN 24-May-13 12:01 diffusion/internal/services/messaging.py
+-rw-rw-rw-  2.0 unx     1769 b- defN 24-May-13 12:01 diffusion/internal/services/session.py
+-rw-rw-rw-  2.0 unx     5667 b- defN 24-May-13 12:01 diffusion/internal/services/topics.py
+-rw-rw-rw-  2.0 unx     6646 b- defN 24-May-13 12:01 diffusion/internal/session/__init__.py
+-rw-rw-rw-  2.0 unx     8506 b- defN 24-May-13 12:01 diffusion/internal/session/connection.py
+-rw-rw-rw-  2.0 unx     1678 b- defN 24-May-13 12:01 diffusion/internal/session/credentials.py
+-rw-rw-rw-  2.0 unx     4290 b- defN 24-May-13 12:01 diffusion/internal/session/error_reason.py
+-rw-rw-rw-  2.0 unx     8161 b- defN 24-May-13 12:01 diffusion/internal/session/exception_handler.py
+-rw-rw-rw-  2.0 unx      424 b- defN 24-May-13 12:01 diffusion/internal/session/locks/__init__.py
+-rw-rw-rw-  2.0 unx     1360 b- defN 24-May-13 12:01 diffusion/internal/session/locks/session_lock_acquisition.py
+-rw-rw-rw-  2.0 unx      805 b- defN 24-May-13 12:01 diffusion/internal/session/locks/session_lock_request.py
+-rw-rw-rw-  2.0 unx      710 b- defN 24-May-13 12:01 diffusion/internal/session/locks/session_lock_request_cancellation.py
+-rw-rw-rw-  2.0 unx      424 b- defN 24-May-13 12:01 diffusion/internal/timeseries/__init__.py
+-rw-rw-rw-  2.0 unx      424 b- defN 24-May-13 12:01 diffusion/internal/timeseries/query/__init__.py
+-rw-rw-rw-  2.0 unx     2363 b- defN 24-May-13 12:01 diffusion/internal/timeseries/query/range_query.py
+-rw-rw-rw-  2.0 unx    27383 b- defN 24-May-13 12:01 diffusion/internal/timeseries/query/range_query_parameters.py
+-rw-rw-rw-  2.0 unx     3556 b- defN 24-May-13 12:01 diffusion/internal/timeseries/query/range_query_request.py
+-rw-rw-rw-  2.0 unx    10765 b- defN 24-May-13 12:01 diffusion/internal/timeseries/query/range_query_result.py
+-rw-rw-rw-  2.0 unx     7618 b- defN 24-May-13 12:01 diffusion/internal/topics/__init__.py
+-rw-rw-rw-  2.0 unx      311 b- defN 24-May-13 12:01 diffusion/internal/topics/constraints.py
+-rw-rw-rw-  2.0 unx     2192 b- defN 24-May-13 12:01 diffusion/internal/validation/__init__.py
+-rw-rw-rw-  2.0 unx     1923 b- defN 24-May-13 12:01 diffusion/internal/validation/pydantic.py
+-rw-rw-rw-  2.0 unx    10373 b- defN 24-May-13 12:01 diffusion/messaging/__init__.py
+-rw-rw-rw-  2.0 unx    13265 b- defN 24-May-13 12:01 diffusion/session/__init__.py
+-rw-rw-rw-  2.0 unx     5509 b- defN 24-May-13 12:01 diffusion/session/exceptions.py
+-rw-rw-rw-  2.0 unx     2166 b- defN 24-May-13 12:01 diffusion/session/retry_strategy.py
+-rw-rw-rw-  2.0 unx     1223 b- defN 24-May-13 12:01 diffusion/session/session_container_factory.py
+-rw-rw-rw-  2.0 unx    12135 b- defN 24-May-13 12:01 diffusion/session/session_factory.py
+-rw-rw-rw-  2.0 unx      424 b- defN 24-May-13 12:01 diffusion/session/locks/__init__.py
+-rw-rw-rw-  2.0 unx      929 b- defN 24-May-13 12:01 diffusion/session/locks/session_lock_acquisition.py
+-rw-rw-rw-  2.0 unx    14937 b- defN 24-May-13 12:01 diffusion/session/locks/session_locks.py
+-rw-rw-rw-  2.0 unx     1780 b- defN 24-May-13 12:01 diffusion-6.9.8.dist-info/METADATA
+-rw-rw-rw-  2.0 unx      101 b- defN 24-May-13 12:01 diffusion-6.9.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       10 b- defN 24-May-13 12:01 diffusion-6.9.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    11174 b- defN 24-May-13 12:01 diffusion-6.9.8.dist-info/RECORD
+113 files, 628826 bytes uncompressed, 162109 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -321,20 +321,20 @@
 
 Filename: diffusion/session/locks/session_lock_acquisition.py
 Comment: 
 
 Filename: diffusion/session/locks/session_locks.py
 Comment: 
 
-Filename: diffusion-6.9.7.dist-info/METADATA
+Filename: diffusion-6.9.8.dist-info/METADATA
 Comment: 
 
-Filename: diffusion-6.9.7.dist-info/WHEEL
+Filename: diffusion-6.9.8.dist-info/WHEEL
 Comment: 
 
-Filename: diffusion-6.9.7.dist-info/top_level.txt
+Filename: diffusion-6.9.8.dist-info/top_level.txt
 Comment: 
 
-Filename: diffusion-6.9.7.dist-info/RECORD
+Filename: diffusion-6.9.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `diffusion-6.9.7.dist-info/METADATA` & `diffusion-6.9.8.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-Metadata-Version: 2.1
-Name: diffusion
-Version: 6.9.7
-Summary: Python SDK for Diffusion.
-Home-page: 
-https: //www.diffusiondata.com/
-License: Proprietary
-Keywords: diffusion,cloud,websockets,data
-Classifier: License :: Other/Proprietary License
-Classifier: Environment :: Other Environment
-Classifier: Development Status :: 4 - Beta
-Description-Content-Type: text/markdown
-Requires-Dist: attrs ==21.*,>=21.4.0
-Requires-Dist: cbor2 ==5.*,>=5.1.2
-Requires-Dist: stringcase ==1.*,>=1.2.0
-Requires-Dist: structlog ==21.*,>=21.5.0
-Requires-Dist: typing-extensions ==4.*,>=4.0.1
-Requires-Dist: pydantic ==1.*,>=1.9.0
-Requires-Dist: diffusion-core ==0.0.62
-Requires-Dist: aiohttp ==3.*,>=3.6.2 ; python_version < "3.12"
-Requires-Dist: aiohttp ==3.*,>=3.9.0 ; python_version >= "3.12"
-
-# Python SDK for Diffusion
-
-**Pre-release version; not ready for production.**
-
-The Diffusion Python library allows Python applications to interact with a Diffusion server.
-
-## Supported Python Versions
-
-The Diffusion Python SDK officially supports the following:
-
-Supported Interpreters:
-
-* CPython 3.7.9 or later
-* CPython 3.8.6 or later
-* CPython 3.9.0 or later
-
-Supported Platforms:
-
-* MacOS 10.13-11.5
-* Windows Intel 64-bit
-* Any Linux supported by the [ManyLinux 2010/2014](https://github.com/pypa/manylinux) binary wheel standard.
-
-## Current Capabilities
-
-- Session:
-  - Establish a session
-  - Send user ping
-  - Receive system ping
-- Messaging:
-  - Register request handler
-  - Send request to path
-  - Send request to session
-  - Send request to filter
-  - Register filter message stream
-- Topics:
-  - Topic subscriptions
-  - Topic creation
-  - Topic creation with initial topic value
-  - Topic removal
-  - Topic stream handlers
+Metadata-Version: 2.1
+Name: diffusion
+Version: 6.9.8
+Summary: Python SDK for Diffusion.
+Home-page: 
+https: //www.diffusiondata.com/
+License: Proprietary
+Keywords: diffusion,cloud,websockets,data
+Classifier: License :: Other/Proprietary License
+Classifier: Environment :: Other Environment
+Classifier: Development Status :: 4 - Beta
+Description-Content-Type: text/markdown
+Requires-Dist: attrs ==21.*,>=21.4.0
+Requires-Dist: cbor2 ==5.*,>=5.1.2
+Requires-Dist: stringcase ==1.*,>=1.2.0
+Requires-Dist: structlog ==21.*,>=21.5.0
+Requires-Dist: typing-extensions ==4.*,>=4.0.1
+Requires-Dist: pydantic ==1.*,>=1.9.0
+Requires-Dist: diffusion-core ==0.0.62
+Requires-Dist: aiohttp ==3.*,>=3.6.2 ; python_version < "3.12"
+Requires-Dist: aiohttp ==3.*,>=3.9.0 ; python_version >= "3.12"
+
+# Python SDK for Diffusion
+
+**Pre-release version; not ready for production.**
+
+The Diffusion Python library allows Python applications to interact with a Diffusion server.
+
+## Supported Python Versions
+
+The Diffusion Python SDK officially supports the following:
+
+Supported Interpreters:
+
+* CPython 3.7.9 or later
+* CPython 3.8.6 or later
+* CPython 3.9.0 or later
+
+Supported Platforms:
+
+* MacOS 10.13-11.5
+* Windows Intel 64-bit
+* Any Linux supported by the [ManyLinux 2010/2014](https://github.com/pypa/manylinux) binary wheel standard.
+
+## Current Capabilities
+
+- Session:
+  - Establish a session
+  - Send user ping
+  - Receive system ping
+- Messaging:
+  - Register request handler
+  - Send request to path
+  - Send request to session
+  - Send request to filter
+  - Register filter message stream
+- Topics:
+  - Topic subscriptions
+  - Topic creation
+  - Topic creation with initial topic value
+  - Topic removal
+  - Topic stream handlers
```

## Comparing `diffusion-6.9.7.dist-info/RECORD` & `diffusion-6.9.8.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -103,11 +103,11 @@
 diffusion/session/exceptions.py,sha256=3yIucpyScgEz3xSrj-SXz_YNKxb2pJRAjOJ5DwuU5cM,5509
 diffusion/session/retry_strategy.py,sha256=ksor0KPILAkMJBf9tI31IAd5LMHvcSN7MxRaIsu1noE,2166
 diffusion/session/session_container_factory.py,sha256=1a2x2F8FdxZuYCsL9uzzApAKmzfLuDH35i0nPbB972U,1223
 diffusion/session/session_factory.py,sha256=SIVItr2UCN7_4e4-awYLX_g9Wd6GiFlbWsDOXOGPjEs,12135
 diffusion/session/locks/__init__.py,sha256=-uW_l93bOAVnG1-KXw2utpQAhK6Gvss9cOCdJtFAyRs,424
 diffusion/session/locks/session_lock_acquisition.py,sha256=TjOz21iosDckTJH1AhZ5IOYuONKDBiks57qRJhae9hQ,929
 diffusion/session/locks/session_locks.py,sha256=gu8NtcHWRkditfTrZ5ESLF0z2ZPqYAgo5J1toER795U,14937
-diffusion-6.9.7.dist-info/METADATA,sha256=AFgc2y1299q4f4sBQRG75BAEyRbYBzOzQorY213GVlQ,1718
-diffusion-6.9.7.dist-info/WHEEL,sha256=ExAwMQyqPPAklMrxzDqhEpq-U2yADelmMQC3M8EDYNk,101
-diffusion-6.9.7.dist-info/top_level.txt,sha256=7Q6zKfH0egqajYyKZcvu9BaNkgK3lP6IuD3_eQzyME0,10
-diffusion-6.9.7.dist-info/RECORD,,
+diffusion-6.9.8.dist-info/METADATA,sha256=_h6fjTTctHTyloubxVCMZ1Zh_kCrqZoA5GPek0q4ZhQ,1780
+diffusion-6.9.8.dist-info/WHEEL,sha256=ExAwMQyqPPAklMrxzDqhEpq-U2yADelmMQC3M8EDYNk,101
+diffusion-6.9.8.dist-info/top_level.txt,sha256=7Q6zKfH0egqajYyKZcvu9BaNkgK3lP6IuD3_eQzyME0,10
+diffusion-6.9.8.dist-info/RECORD,,
```

